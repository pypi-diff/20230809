# Comparing `tmp/quickemail-0.2.8-py3-none-any.whl.zip` & `tmp/quickemail-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8766 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    29106 b- defN 23-Jul-27 06:15 quickemail.py
--rw-rw-rw-  2.0 fat     3139 b- defN 23-Jul-27 06:48 quickemail-0.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 06:48 quickemail-0.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-27 06:48 quickemail-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      381 b- defN 23-Jul-27 06:48 quickemail-0.2.8.dist-info/RECORD
-5 files, 32729 bytes uncompressed, 8058 bytes compressed:  75.4%
+Zip file size: 8909 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    29565 b- defN 23-Aug-09 05:29 quickemail.py
+-rw-rw-rw-  2.0 fat     3181 b- defN 23-Aug-09 05:30 quickemail-0.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-09 05:30 quickemail-0.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-09 05:30 quickemail-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      381 b- defN 23-Aug-09 05:30 quickemail-0.2.9.dist-info/RECORD
+5 files, 33230 bytes uncompressed, 8201 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: quickemail.py
 Comment: 
 
-Filename: quickemail-0.2.8.dist-info/METADATA
+Filename: quickemail-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: quickemail-0.2.8.dist-info/WHEEL
+Filename: quickemail-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: quickemail-0.2.8.dist-info/top_level.txt
+Filename: quickemail-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: quickemail-0.2.8.dist-info/RECORD
+Filename: quickemail-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quickemail.py

```diff
@@ -32,14 +32,17 @@
 
         发信人、收信人为必须参数：
         quicksend.mail_from = 'AA高丽A<a@test.com>'    # 发信人地址，格式为:   FullName<email address>
         quicksend.mail_to = '一二三<123@test.com>,ABC<abc@test.com>'    # 格式同上，多地址使用逗号","分隔
 
         抄送人，可省略：
         quicksend.mail_cc = '一二三<123@test.com>,中语言C<abc@test.com>,AA高丽A<a@test.com>'
+        
+        邮件时间定义，可省略：
+        quicksend.mail_date = 1691544067
 
         邮件主题、内容，支持使用HTML： 
         quicksend.mail_subject = 'mY subject还有中文!'
         quicksend.mail_content = '<font color=red>red content一段中文</font>'
         quicksend.is_html = True
 
         添加附件，可省略：
@@ -67,15 +70,15 @@
             
         result = quicksend.send(msg)
         if result:
             print(result)
 
 """
 
-__version__ = '0.2.4'
+__version__ = '0.2.9'
 
 __author__ = 'clayboy <clayboy@foxmail.com>'
 
 
 class QuickEmail:
     _content_type = {
         'acp': 'audio/x-mei-aac',
@@ -418,14 +421,15 @@
         self._mail_to = ''
         self._mail_cc = None
         self._mail_bcc = None
         self._mail_subject = ''
         self._mail_content = ''
         self._mail_attach = None
         self._is_html = True
+        self._date = formatdate(localtime=True)
         self._time_out = 20
         self._helo = "QuickEmail"
         self._content_from = None
         self._content_to = None
         self._content_cc = None
         self._msg = None
 
@@ -475,14 +479,19 @@
         self._mail_attach = filelist
 
     def set_is_html(self, b):
         self._is_html = b
 
     def set_time_out(self, t):
         self._time_out = t
+        
+    def set_mail_date(self, t):
+        if not isinstance(t, int):
+            raise TypeError("need Int timestamp.")
+        self._date = formatdate(timeval=t, localtime=True)
 
     def set_tls(self, b):
         self._tls = b
 
     def set_ssl(self, b):
         self._ssl = b
 
@@ -555,14 +564,22 @@
         return self._mail_bcc
 
     @mail_bcc.setter
     def mail_bcc(self, s):
         self._mail_bcc = s
 
     @property
+    def mail_date(self):
+        return self._date
+
+    @mail_date.setter
+    def mail_date(self, t):
+        self.set_mail_date(t)
+
+    @property
     def content_from(self):
         return self._content_from
 
     @content_from.setter
     def content_from(self, s):
         self._content_from = s
 
@@ -705,15 +722,15 @@
             if self.content_cc:
                 msg['CC'] = self._mailto_rebuild(self.content_cc)
             else:
                 msg['CC'] = self._mailto_rebuild(self.mail_cc)
 
         msg['Message-ID'] = '<QuickEmail.{}.{}@{}>'.format(time.time(), random.randint(1, 1000), self._get_fromdomain())
 
-        msg['Date'] = formatdate(localtime=True)
+        msg['Date'] = self._date
 
         msg_html_content = MIMEText(self.mail_content, html_plain, _charset='utf-8')
         msg.attach(msg_html_content)
 
         if self.mail_attach is not None:
             for attach_file in self.mail_attach:
                 file_name = os.path.basename(attach_file)
@@ -830,15 +847,14 @@
 
         send_err = ''
         try:
             if self.ssl:
                 smtp_handle = smtplib.SMTP_SSL(host=self.host, port=self.port, timeout=self.time_out)
             else:
                 smtp_handle = smtplib.SMTP(host=self.host, port=self.port, timeout=self.time_out)
-            # smtp_handle.connect(self.host, self.port)
             smtp_handle.set_debuglevel = self._debuglevel
             smtp_handle.ehlo(self._helo)
             if self.tls:
                 smtp_handle.starttls()
             smtp_handle.login(self.auth_user, self.user_pass)
             smtp_handle.sendmail(smtpfrom, smtpto.split(','), msgdata)
             smtp_handle.quit()
@@ -870,20 +886,21 @@
     quicksend.debug = True
     quicksend.tls = True
     quicksend.auth_user = 'abc'
     quicksend.user_pass = 'test'
     quicksend.mail_from = '<a@test.com>'
     quicksend.mail_to = '一二三 <123@test.com>,abc@test.com,<a@test.com>'
     quicksend.mail_cc = '张三<b@test.com>'
+    quicksend.mail_date = 1691544067
     quicksend.mail_subject = 'mY subject还有中文!'
     quicksend.mail_content = '<font color=red>red content一段中文</font>'
     quicksend.mail_attach = ['C:\\Users\\Administrator\\Pictures\\163.com.png']
     quicksend.is_html = True
     quicksend.content_from = '假发件人<a@a.com>'
     quicksend.content_cc = 'e@test.com'
 
     # msg = quicksend.creatmsg()
     # print(msg)
     print(quicksend.auth_user, quicksend.user_pass)
-    do_send = quicksend.send()
+    do_send = quicksend.authsend()
     if not do_send:
         print(do_send)
```

## Comparing `quickemail-0.2.8.dist-info/METADATA` & `quickemail-0.2.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickemail
-Version: 0.2.8
+Version: 0.2.9
 Summary: Quick send email use python3.
 Home-page: http://clayboy.cn
 Author: Clayboy
 Author-email: clayboy@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -33,19 +33,22 @@
         quicksend.helo = 'QuickEmail'                 # HELO主机名不能使用有空格的字符串，可以省略
         quicksend.tls = True / quicksend.ssl = True   # 开启startTLS或者SSL，SSL端口一般为465
         认证用户名和密码，authsend()必须的参数：
         quicksend.mail_user = 'a'                     # 认证用户名
         quicksend.user_pass = 'test'                  # 认证用户的密码
     
         发信人、收信人为必须参数：
-        quicksend.mail_from = 'AA高丽A<a@test.com>'    # 发信人地址，格式为:   FullName<email address>
+        quicksend.mail_from = 'AA高A<a@test.com>'    # 发信人地址，格式为:   FullName<email address>
         quicksend.mail_to = '一二三<123@test.com>,ABC<abc@test.com>'    # 格式同上，多地址使用逗号","分隔
     
         抄送人，可省略：
-        quicksend.mail_cc = '一二三<123@test.com>,中语言C<abc@test.com>,AA高丽A<a@test.com>'
+        quicksend.mail_cc = '一二三<123@test.com>'
+        
+        邮件时间定义，可省略：
+        quicksend.mail_date = 1691544067
     
         邮件主题、内容，支持使用HTML： 
         quicksend.mail_subject = 'mY subject还有中文!'
         quicksend.mail_content = '<font color=red>red content一段中文</font>'
         quicksend.is_html = True
     
         添加附件，可省略：
```

