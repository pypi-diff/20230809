# Comparing `tmp/contiguity-1.0.0.tar.gz` & `tmp/contiguity-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/contiguity-1.0.0.tar", last modified: Wed Jun 28 20:03:50 2023, max compression
+gzip compressed data, was "dist/contiguity-1.0.2.tar", last modified: Wed Aug  9 01:23:35 2023, max compression
```

## Comparing `contiguity-1.0.0.tar` & `contiguity-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 occupymars   (501) staff       (20)        0 2023-06-28 20:03:50.179228 contiguity-1.0.0/
--rw-r--r--   0 occupymars   (501) staff       (20)      423 2023-06-28 20:03:50.178837 contiguity-1.0.0/PKG-INFO
--rw-r--r--   0 occupymars   (501) staff       (20)     5193 2023-06-28 19:59:29.000000 contiguity-1.0.0/README.md
-drwxr-xr-x   0 occupymars   (501) staff       (20)        0 2023-06-28 20:03:50.175768 contiguity-1.0.0/contiguity/
--rw-r--r--   0 occupymars   (501) staff       (20)      239 2023-06-28 06:16:37.000000 contiguity-1.0.0/contiguity/__init__.py
--rw-r--r--   0 occupymars   (501) staff       (20)    12059 2023-06-28 18:14:30.000000 contiguity-1.0.0/contiguity/main.py
-drwxr-xr-x   0 occupymars   (501) staff       (20)        0 2023-06-28 20:03:50.178144 contiguity-1.0.0/contiguity.egg-info/
--rw-r--r--   0 occupymars   (501) staff       (20)      423 2023-06-28 20:03:50.000000 contiguity-1.0.0/contiguity.egg-info/PKG-INFO
--rw-r--r--   0 occupymars   (501) staff       (20)      229 2023-06-28 20:03:50.000000 contiguity-1.0.0/contiguity.egg-info/SOURCES.txt
--rw-r--r--   0 occupymars   (501) staff       (20)        1 2023-06-28 20:03:50.000000 contiguity-1.0.0/contiguity.egg-info/dependency_links.txt
--rw-r--r--   0 occupymars   (501) staff       (20)       30 2023-06-28 20:03:50.000000 contiguity-1.0.0/contiguity.egg-info/requires.txt
--rw-r--r--   0 occupymars   (501) staff       (20)       11 2023-06-28 20:03:50.000000 contiguity-1.0.0/contiguity.egg-info/top_level.txt
--rw-r--r--   0 occupymars   (501) staff       (20)       38 2023-06-28 20:03:50.179428 contiguity-1.0.0/setup.cfg
--rw-r--r--   0 occupymars   (501) staff       (20)      728 2023-06-28 05:51:07.000000 contiguity-1.0.0/setup.py
+drwxr-xr-x   0 occupymars   (501) staff       (20)        0 2023-08-09 01:23:35.390365 contiguity-1.0.2/
+-rw-r--r--   0 occupymars   (501) staff       (20)      423 2023-08-09 01:23:35.390138 contiguity-1.0.2/PKG-INFO
+-rw-r--r--   0 occupymars   (501) staff       (20)     5389 2023-08-09 01:20:30.000000 contiguity-1.0.2/README.md
+drwxr-xr-x   0 occupymars   (501) staff       (20)        0 2023-08-09 01:23:35.387562 contiguity-1.0.2/contiguity/
+-rw-r--r--   0 occupymars   (501) staff       (20)      239 2023-06-28 06:16:37.000000 contiguity-1.0.2/contiguity/__init__.py
+-rw-r--r--   0 occupymars   (501) staff       (20)    12763 2023-08-09 01:17:58.000000 contiguity-1.0.2/contiguity/main.py
+drwxr-xr-x   0 occupymars   (501) staff       (20)        0 2023-08-09 01:23:35.389628 contiguity-1.0.2/contiguity.egg-info/
+-rw-r--r--   0 occupymars   (501) staff       (20)      423 2023-08-09 01:23:35.000000 contiguity-1.0.2/contiguity.egg-info/PKG-INFO
+-rw-r--r--   0 occupymars   (501) staff       (20)      229 2023-08-09 01:23:35.000000 contiguity-1.0.2/contiguity.egg-info/SOURCES.txt
+-rw-r--r--   0 occupymars   (501) staff       (20)        1 2023-08-09 01:23:35.000000 contiguity-1.0.2/contiguity.egg-info/dependency_links.txt
+-rw-r--r--   0 occupymars   (501) staff       (20)       30 2023-08-09 01:23:35.000000 contiguity-1.0.2/contiguity.egg-info/requires.txt
+-rw-r--r--   0 occupymars   (501) staff       (20)       11 2023-08-09 01:23:35.000000 contiguity-1.0.2/contiguity.egg-info/top_level.txt
+-rw-r--r--   0 occupymars   (501) staff       (20)       38 2023-08-09 01:23:35.390455 contiguity-1.0.2/setup.cfg
+-rw-r--r--   0 occupymars   (501) staff       (20)      728 2023-08-09 01:21:29.000000 contiguity-1.0.2/setup.py
```

### Comparing `contiguity-1.0.0/README.md` & `contiguity-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -112,14 +112,22 @@
 verify = client.otp.verify({
     'otp_id': otp_id # you received this when you called client.otp.send(),
     'otp': input # the 6 digits your user inputted.
 })
 ```
 It will return a boolean (true/false). The OTP expires 15 minutes after sending it.
 
+Want to resend an OTP? Use `client.otp.resend()`:
+```py
+resend = client.otp.resend({
+    'otp_id': otp_id # you received this when you called client.otp.send(),
+})
+```
+OTP expiry does not renew.
+
 ## Verify formatting
 Contiguity provides two functions that verify phone number and email formatting, which are:
 
 ```py
 client.verify.number("number")
 ```
 and
```

### Comparing `contiguity-1.0.0/contiguity/main.py` & `contiguity-1.0.2/contiguity/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,67 +12,70 @@
         debug (bool, optional): A flag indicating whether to enable debug mode. Default is False.
     """
     def __init__(self, token, debug=False):
         self.token = token.strip()
         self.debug = debug
         self.baseURL = "https://api.contiguity.co"
         self.orwellBaseURL = "https://orwell.contiguity.co"
+        self.headers = {"Content-Type": "application/json",
+                "Authorization": f"Token {token}"}
 
     @property
     def send(self):
         """
         Returns an instance of the Send class.
         """
-        return Send(self.token, self.baseURL, self.debug)
+        return Send(self.token, self.baseURL, self.headers, self.debug)
 
     @property
     def verify(self):
         """
          Returns an instance of the Verify class.
          """
         return Verify(self.token)
 
     @property
     def email_analytics(self):
         """
          Returns an instance of the EmailAnalytics class.
          """
-        return EmailAnalytics(self.token, self.orwellBaseURL, self.debug)
+        return EmailAnalytics(self.token, self.orwellBaseURL, self.headers, self.debug)
 
     @property
     def quota(self):
         """
          Returns an instance of the Quota class.
          """
-        return Quota(self.token, self.baseURL, self.debug)
+        return Quota(self.token, self.baseURL, self.headers,  self.debug)
 
     @property
     def otp(self):
         """
          Returns an instance of the OTP class.
          """
-        return OTP(self.token, self.baseURL, self.debug)
+        return OTP(self.token, self.baseURL, self.headers, self.debug)
 
     @property
     def template(self):
         """
          Returns an instance of the Template class.
          """
         return Template()
 
 
 class Send:
     """
     Send class for Contiguity.
     """
 
-    def __init__(self, token, baseURL, debug=False):
+    def __init__(self, token, baseURL, headers, debug=False):
         self.token = token
         self.baseURL = baseURL
         self.debug = debug
+        self.headers = headers
 
     def text(self, obj):
         """
         Send a text message.
         Args:
             obj (dict): The object containing the message details.
                 obj['to'] (str): The recipient's phone number.
@@ -98,18 +101,15 @@
 
         text_handler = requests.post(
             f"{self.baseURL}/send/text",
             json={
                 'to': phonenumbers.format_number(parsed_number, phonenumbers.PhoneNumberFormat.E164),
                 'message': obj['message'],
             },
-            headers={
-                "Content-Type": "application/json",
-                "Authorization": f"Token {self.token}",
-            },
+            headers= self.headers
         )
         text_handler_response = text_handler.json()
 
         if text_handler.status_code != 200:
             raise ValueError(
                 f"Contiguity couldn't send your message. Received: {text_handler.status_code} with reason: \"{text_handler_response['message']}\"")
         if self.debug:
@@ -159,18 +159,15 @@
 
         if 'cc' in obj:
             email_payload['cc'] = obj['cc']
 
         email_handler = requests.post(
             f"{self.baseURL}/send/email",
             json=email_payload,
-            headers={
-                "Content-Type": "application/json",
-                "Authorization": f"Token {self.token}",
-            },
+            headers= self.headers
         )
 
         email_handler_response = email_handler.json()
 
         if email_handler.status_code != 200:
             raise ValueError(
                 f"Contiguity couldn't send your email. Received: {email_handler.status_code} with reason: \"{email_handler_response['message']}\"")
@@ -182,86 +179,86 @@
 
 
 class Verify:
     def __init__(self, token):
         self.token = token
 
     def number(self, number):
-        validity = phonenumbers.is_valid_number(phonenumbers.parse(number))
-        return validity
+        try:
+            validity = phonenumbers.is_valid_number(phonenumbers.parse(number))
+            return validity
+        except Exception as e:
+            return False
 
     def email(self, email):
         email_pattern = re.compile(r"^[^\s@]+@[^\s@]+\.[^\s@]+$")
         return bool(email_pattern.match(email))
 
 
 class EmailAnalytics:
-    def __init__(self, token, orwellBaseURL, debug=False):
+    def __init__(self, token, orwellBaseURL, headers,  debug=False):
         self.token = token
         self.orwellBaseURL = orwellBaseURL
         self.debug = debug
+        self.headers = headers
 
     def retrieve(self, id):
         if not self.token:
             raise ValueError("Contiguity requires a token/API key to be provided via contiguity.login('token')")
         if not id:
             raise ValueError("Contiguity Analytics requires an email ID.")
 
         status = requests.get(
             f"{self.orwellBaseURL}/email/status/{id}",
-            headers={
-                "Content-Type": "application/json",
-                "Authorization": f"Token {self.token}",
-            },
+            headers= self.headers
         )
 
         json_data = status.json()
 
         if status.status_code != 200:
             raise ValueError(f"Contiguity Analytics couldn't find an email with ID {id}")
         if self.debug:
             print(f"Contiguity successfully found your email. Data:\n\n{json.dumps(json_data)}")
 
         return json_data
 
 
 class Quota:
-    def __init__(self, token, baseURL, debug=False):
+    def __init__(self, token, baseURL, headers,  debug=False):
         self.token = token
         self.baseURL = baseURL
         self.debug = debug
+        self.headers = headers
 
     def retrieve(self):
         if not self.token:
             raise ValueError("Contiguity requires a token/API key to be provided via contiguity.login('token')")
 
         quota = requests.get(
             f"{self.baseURL}/user/get/quota",
-            headers={
-                "Content-Type": "application/json",
-                "Authorization": f"Token {self.token}",
-            },
+            headers= self.headers
         )
 
         json_data = quota.json()
 
         if quota.status_code != 200:
             raise ValueError(
                 f"Contiguity had an issue finding your quota. Received {quota.status_code} with reason: \"{json_data['message']}\"")
         if self.debug:
             print(f"Contiguity successfully found your quota. Data:\n\n{json.dumps(json_data)}")
 
         return json_data
 
 
 class OTP:
-    def __init__(self, token, baseURL, debug=False):
+    def __init__(self, token, baseURL, headers, debug=False):
         self.token = token
         self.baseURL = baseURL
         self.debug = debug
+        self.headers = headers
 
     def send(self, obj):
         if not self.token:
             raise ValueError("Contiguity requires a token/API key to be provided via contiguity.login('token')")
         if "to" not in obj:
             raise ValueError("Contiguity requires a recipient to be specified.")
         if "language" not in obj:
@@ -272,18 +269,15 @@
         otp_handler = requests.post(
             f"{self.baseURL}/otp/new",
             json={
                 "to": e164,
                 "language": obj["language"],
                 "name": obj.get("name"),
             },
-            headers={
-                "Content-Type": "application/json",
-                "Authorization": f"Token {self.token}",
-            },
+            headers= self.headers
         )
 
         otp_handler_response = otp_handler.json()
 
         if otp_handler.status_code != 200:
             raise ValueError(
                 f"Contiguity couldn't send your OTP. Received: {otp_handler.status_code} with reason: \"{otp_handler_response['message']}\"")
@@ -302,31 +296,53 @@
 
         otp_handler = requests.post(
             f"{self.baseURL}/otp/verify",
             json={
                 "otp": obj["otp"],
                 "otp_id": obj["otp_id"],
             },
-            headers={
-                "Content-Type": "application/json",
-                "Authorization": f"Token {self.token}",
-            },
+            headers= self.headers
         )
 
         otp_handler_response = otp_handler.json()
 
         if otp_handler.status_code != 200:
             raise ValueError(
                 f"Contiguity couldn't verify your OTP. Received: {otp_handler.status_code} with reason: \"{otp_handler_response['message']}\"")
         if self.debug:
             print(
                 f"Contiguity 'verified' your OTP ({obj['otp']}) with boolean verified status: {otp_handler_response['verified']}")
 
         return otp_handler_response["verified"]
 
+    def resend(self, obj):
+        if not self.token:
+            raise ValueError("Contiguity requires a token/API key to be provided via contiguity.login('token')")
+        if "otp_id" not in obj:
+            raise ValueError("Contiguity requires an OTP ID to be specified.")
+
+        otp_handler = requests.post(
+            f"{self.baseURL}/otp/resend",
+            json={
+                "otp_id": obj["otp_id"],
+            },
+            headers= self.headers
+        )
+
+        otp_handler_response = otp_handler.json()
+
+        if otp_handler.status_code != 200:
+            raise ValueError(
+                f"Contiguity couldn't resend your OTP. Received: {otp_handler.status_code} with reason: \"{otp_handler_response['message']}\"")
+        if self.debug:
+            print(
+                f"Contiguity resent your OTP ({obj['otp']}) with boolean resent status: {otp_handler_response['verified']}")
+
+        return otp_handler_response["verified"]
+
 
 class Template:
     def local(self, file):
         try:
             with open(file, "r") as f:
                 file_content = f.read()
                 mini = minify(file_content, minify_js=True, minify_css=True)
```

### Comparing `contiguity-1.0.0/setup.py` & `contiguity-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.2'
 DESCRIPTION = "Contiguity's official Python SDK"
 LONG_DESCRIPTION = "Contiguity's official Python SDK makes using Contiguity easier than ever. See more information at https://github.com/use-contiguity/python"
 
 setup(
     name="contiguity",
     version=VERSION,
     author="Contiguity",
```

