# Comparing `tmp/honeypots-0.8.tar.gz` & `tmp/honeypots-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeypots-0.8.tar", last modified: Tue Apr 13 21:41:51 2021, max compression
+gzip compressed data, was "dist/honeypots-0.9.tar", last modified: Tue Apr 13 21:50:13 2021, max compression
```

## Comparing `honeypots-0.8.tar` & `honeypots-0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        0 2021-04-13 21:41:51.192980 honeypots-0.8/
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     4621 2021-04-13 21:41:51.192980 honeypots-0.8/PKG-INFO
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     3544 2021-04-13 21:39:38.000000 honeypots-0.8/README.rst
-drwxrwxr-x   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        0 2021-04-13 21:41:51.192980 honeypots-0.8/honeypots/
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        0 2021-04-13 21:40:26.000000 honeypots-0.8/honeypots/__init__.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     3242 2021-04-13 21:40:34.000000 honeypots-0.8/honeypots/__main__.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     5720 2021-04-13 21:40:33.000000 honeypots-0.8/honeypots/dns_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6014 2021-04-13 21:40:32.000000 honeypots-0.8/honeypots/ftp_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7955 2021-04-13 21:40:31.000000 honeypots-0.8/honeypots/helper.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6653 2021-04-13 21:40:33.000000 honeypots-0.8/honeypots/http_proxy_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)    10931 2021-04-13 21:40:32.000000 honeypots-0.8/honeypots/http_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)    11855 2021-04-13 21:40:33.000000 honeypots-0.8/honeypots/https_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6861 2021-04-13 21:40:26.000000 honeypots-0.8/honeypots/imap_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     8998 2021-04-13 21:40:32.000000 honeypots-0.8/honeypots/mysql_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7171 2021-04-13 21:40:34.000000 honeypots-0.8/honeypots/pop3_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7266 2021-04-13 21:40:32.000000 honeypots-0.8/honeypots/postgres_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7617 2021-04-13 21:40:33.000000 honeypots-0.8/honeypots/redis_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6859 2021-04-13 21:40:26.000000 honeypots-0.8/honeypots/smb_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7149 2021-04-13 21:40:26.000000 honeypots-0.8/honeypots/smtp_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6948 2021-04-13 21:40:26.000000 honeypots-0.8/honeypots/socks5_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7241 2021-04-13 21:40:35.000000 honeypots-0.8/honeypots/ssh_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6991 2021-04-13 21:40:34.000000 honeypots-0.8/honeypots/telnet_server.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     3943 2021-04-13 20:31:07.000000 honeypots-0.8/honeypots/testing_all.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     3537 2021-04-13 21:40:34.000000 honeypots-0.8/honeypots/testing_dev.py
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     8534 2021-04-13 21:40:31.000000 honeypots-0.8/honeypots/vnc_server.py
-drwxrwxr-x   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        0 2021-04-13 21:41:51.192980 honeypots-0.8/honeypots.egg-info/
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     4621 2021-04-13 21:41:51.000000 honeypots-0.8/honeypots.egg-info/PKG-INFO
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)      745 2021-04-13 21:41:51.000000 honeypots-0.8/honeypots.egg-info/SOURCES.txt
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        1 2021-04-13 21:41:51.000000 honeypots-0.8/honeypots.egg-info/dependency_links.txt
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)       55 2021-04-13 21:41:51.000000 honeypots-0.8/honeypots.egg-info/entry_points.txt
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)      169 2021-04-13 21:41:51.000000 honeypots-0.8/honeypots.egg-info/requires.txt
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)       10 2021-04-13 21:41:51.000000 honeypots-0.8/honeypots.egg-info/top_level.txt
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)       38 2021-04-13 21:41:51.192980 honeypots-0.8/setup.cfg
--rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)      929 2021-04-13 19:23:27.000000 honeypots-0.8/setup.py
+drwxrwxr-x   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        0 2021-04-13 21:50:13.348187 honeypots-0.9/
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     4621 2021-04-13 21:50:13.348187 honeypots-0.9/PKG-INFO
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     3544 2021-04-13 21:39:38.000000 honeypots-0.9/README.rst
+drwxrwxr-x   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        0 2021-04-13 21:50:13.348187 honeypots-0.9/honeypots/
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        0 2021-04-13 21:40:26.000000 honeypots-0.9/honeypots/__init__.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     3479 2021-04-13 21:49:45.000000 honeypots-0.9/honeypots/__main__.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     5720 2021-04-13 21:40:33.000000 honeypots-0.9/honeypots/dns_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6014 2021-04-13 21:40:32.000000 honeypots-0.9/honeypots/ftp_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7955 2021-04-13 21:40:31.000000 honeypots-0.9/honeypots/helper.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6653 2021-04-13 21:40:33.000000 honeypots-0.9/honeypots/http_proxy_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)    10931 2021-04-13 21:40:32.000000 honeypots-0.9/honeypots/http_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)    11855 2021-04-13 21:40:33.000000 honeypots-0.9/honeypots/https_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6861 2021-04-13 21:40:26.000000 honeypots-0.9/honeypots/imap_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     8998 2021-04-13 21:40:32.000000 honeypots-0.9/honeypots/mysql_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7171 2021-04-13 21:40:34.000000 honeypots-0.9/honeypots/pop3_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7266 2021-04-13 21:40:32.000000 honeypots-0.9/honeypots/postgres_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7617 2021-04-13 21:40:33.000000 honeypots-0.9/honeypots/redis_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6859 2021-04-13 21:40:26.000000 honeypots-0.9/honeypots/smb_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7149 2021-04-13 21:40:26.000000 honeypots-0.9/honeypots/smtp_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6948 2021-04-13 21:40:26.000000 honeypots-0.9/honeypots/socks5_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     7241 2021-04-13 21:40:35.000000 honeypots-0.9/honeypots/ssh_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     6991 2021-04-13 21:40:34.000000 honeypots-0.9/honeypots/telnet_server.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     3943 2021-04-13 20:31:07.000000 honeypots-0.9/honeypots/testing_all.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     3537 2021-04-13 21:40:34.000000 honeypots-0.9/honeypots/testing_dev.py
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     8534 2021-04-13 21:40:31.000000 honeypots-0.9/honeypots/vnc_server.py
+drwxrwxr-x   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        0 2021-04-13 21:50:13.348187 honeypots-0.9/honeypots.egg-info/
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)     4621 2021-04-13 21:50:13.000000 honeypots-0.9/honeypots.egg-info/PKG-INFO
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)      745 2021-04-13 21:50:13.000000 honeypots-0.9/honeypots.egg-info/SOURCES.txt
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)        1 2021-04-13 21:50:13.000000 honeypots-0.9/honeypots.egg-info/dependency_links.txt
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)       55 2021-04-13 21:50:13.000000 honeypots-0.9/honeypots.egg-info/entry_points.txt
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)      169 2021-04-13 21:50:13.000000 honeypots-0.9/honeypots.egg-info/requires.txt
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)       10 2021-04-13 21:50:13.000000 honeypots-0.9/honeypots.egg-info/top_level.txt
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)       38 2021-04-13 21:50:13.348187 honeypots-0.9/setup.cfg
+-rw-rw-r--   0 m2u9z1x0v8k3  (1000) m2u9z1x0v8k3  (1000)      929 2021-04-13 21:49:56.000000 honeypots-0.9/setup.py
```

### Comparing `honeypots-0.8/PKG-INFO` & `honeypots-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: honeypots
-Version: 0.8
+Version: 0.9
 Summary: Easy to setup honeypots!
 Home-page: https://github.com/qeeqbox/honeypots
 Author: QeeqBox
 Author-email: gigaqeeq@gmail.com
 License: AGPL-3.0
 Description: .. image:: https://raw.githubusercontent.com/qeeqbox/honeypots/main/readme/honeypots.png
```

### Comparing `honeypots-0.8/README.rst` & `honeypots-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/__main__.py` & `honeypots-0.9/honeypots/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-from honeypots import clean_all
+from honeypots import QDNSServer, QFTPServer, QHTTPProxyServer, QHTTPServer, QHTTPSServer, QIMAPServer, QMysqlServer, QPOP3Server, QPostgresServer, QRedisServer, QSMBServer, QSMTPServer, QSOCKS5Server, QSSHServer, QTelnetServer, QVNCServer, server_arguments, clean_all
 from time import sleep
 from atexit import register
 from argparse import ArgumentParser
 
 all_servers = ['QDNSServer', 'QFTPServer', 'QHTTPProxyServer', 'QHTTPServer', 'QHTTPSServer', 'QIMAPServer', 'QMysqlServer', 'QPOP3Server', 'QPostgresServer', 'QRedisServer', 'QSMBServer', 'QSMTPServer', 'QSOCKS5Server', 'QSSHServer', 'QTelnetServer', 'QVNCServer']
 
 temp_honeypots = []
```

### Comparing `honeypots-0.8/honeypots/dns_server.py` & `honeypots-0.9/honeypots/dns_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/ftp_server.py` & `honeypots-0.9/honeypots/ftp_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/helper.py` & `honeypots-0.9/honeypots/helper.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/http_proxy_server.py` & `honeypots-0.9/honeypots/http_proxy_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/http_server.py` & `honeypots-0.9/honeypots/http_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/https_server.py` & `honeypots-0.9/honeypots/https_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/imap_server.py` & `honeypots-0.9/honeypots/imap_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/mysql_server.py` & `honeypots-0.9/honeypots/mysql_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/pop3_server.py` & `honeypots-0.9/honeypots/pop3_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/postgres_server.py` & `honeypots-0.9/honeypots/postgres_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/redis_server.py` & `honeypots-0.9/honeypots/redis_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/smb_server.py` & `honeypots-0.9/honeypots/smb_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/smtp_server.py` & `honeypots-0.9/honeypots/smtp_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/socks5_server.py` & `honeypots-0.9/honeypots/socks5_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/ssh_server.py` & `honeypots-0.9/honeypots/ssh_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/telnet_server.py` & `honeypots-0.9/honeypots/telnet_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/testing_all.py` & `honeypots-0.9/honeypots/testing_all.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/testing_dev.py` & `honeypots-0.9/honeypots/testing_dev.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots/vnc_server.py` & `honeypots-0.9/honeypots/vnc_server.py`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/honeypots.egg-info/PKG-INFO` & `honeypots-0.9/honeypots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: honeypots
-Version: 0.8
+Version: 0.9
 Summary: Easy to setup honeypots!
 Home-page: https://github.com/qeeqbox/honeypots
 Author: QeeqBox
 Author-email: gigaqeeq@gmail.com
 License: AGPL-3.0
 Description: .. image:: https://raw.githubusercontent.com/qeeqbox/honeypots/main/readme/honeypots.png
```

### Comparing `honeypots-0.8/honeypots.egg-info/SOURCES.txt` & `honeypots-0.9/honeypots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeypots-0.8/setup.py` & `honeypots-0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 setup(
     name='honeypots',
     author='QeeqBox',
     author_email='gigaqeeq@gmail.com',
     description="Easy to setup honeypots!",
     long_description=long_description,
-    version='0.8',
+    version='0.9',
     license="AGPL-3.0",
     url="https://github.com/qeeqbox/honeypots",
     packages=['honeypots'],
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "honeypots = honeypots.__main__:main"
```

