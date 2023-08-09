# Comparing `tmp/thttp-1.2.0.tar.gz` & `tmp/thttp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thttp-1.2.0.tar", last modified: Tue Jan 10 22:02:53 2023, max compression
+gzip compressed data, was "thttp-1.3.0.tar", last modified: Wed Aug  9 01:24:00 2023, max compression
```

## Comparing `thttp-1.2.0.tar` & `thttp-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:02:53.536151 thttp-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-01-10 22:02:53.536151 thttp-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-01-10 22:02:36.000000 thttp-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 22:02:36.000000 thttp-1.2.0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-10 22:02:36.000000 thttp-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-10 22:02:53.536151 thttp-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:02:53.536151 thttp-1.2.0/thttp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-01-10 22:02:53.000000 thttp-1.2.0/thttp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-10 22:02:53.000000 thttp-1.2.0/thttp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 22:02:53.000000 thttp-1.2.0/thttp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 22:02:53.000000 thttp-1.2.0/thttp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-01-10 22:02:36.000000 thttp-1.2.0/thttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:24:00.627649 thttp-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-09 01:23:40.000000 thttp-1.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-08-09 01:24:00.627649 thttp-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-09 01:23:40.000000 thttp-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:23:40.000000 thttp-1.3.0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-09 01:23:40.000000 thttp-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-09 01:24:00.631649 thttp-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:24:00.627649 thttp-1.3.0/thttp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-08-09 01:24:00.000000 thttp-1.3.0/thttp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-09 01:24:00.000000 thttp-1.3.0/thttp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:24:00.000000 thttp-1.3.0/thttp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:24:00.000000 thttp-1.3.0/thttp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-08-09 01:23:40.000000 thttp-1.3.0/thttp.py
```

### Comparing `thttp-1.2.0/PKG-INFO` & `thttp-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: thttp
-Version: 1.2.0
-Summary: An incredibly lightweight wrapper around urllib
-Home-page: https://github.com/sesh/thttp
-Author: Brenton Cleeland
-Author-email: brenton@brntn.me
-Project-URL: Bug Tracker, https://github.com/sesh/thttp/issues
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # thttp
 
 `thttp` is a single file, lightweight, well-tested wrapper around `urllib` that's intended to be copied directly into your project.
 
 It's features include:
 
 - Making GET, POST, PATCH, PUT, HEAD and OPTIONS requests
@@ -26,22 +14,23 @@
 - Sending through a CookieJar object that can be reused between requests
 - Authenticating with HTTP basic auth
 - Specifying a custom timeout for your request
 - Decompressing gzipped content in the response
 - Loading JSON from the response
 - Returning error responses instead of throwing exceptions from `urllib`
 - `pretty()` function for printing responses
+- Ability to upload files using the `{"file": open("file.png", "rb")}` style
 
 Future features:
 
 - Better detection of JSON responses
 - Improve handling of non-utf-8 requests
 - Improve handling of non-utf-8 responses
 
-_Note: this project is not intended to solve all use cases that can be achieved with urllib, requests or other HTTP libraries. The intent is to provide a lightweight tool that simplifies some of the most common use cases for developers._
+_Note: this project is not intended to solve all use cases that can be achieved with urllib, requests, httpx, or other HTTP libraries. The intent is to provide a lightweight tool that simplifies some of the most common use cases for developers._
 
 
 ## Installation
 
 copy `thttp.py` directly into your project:
 
 ```
@@ -95,7 +84,13 @@
 ## Packaging for release
 
 ```
 rm dist/*
 python3 -m build
 python3 -m twine upload dist/*
 ```
+
+
+## License
+
+This code is currently released under the [UNLICENSE](UNLICENSE.md) and considered public domain.
+If more appropriate for your usage you may consider this project released under the [MIT License](LICENSE.md).
```

### Comparing `thttp-1.2.0/README.md` & `thttp-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: thttp
+Version: 1.3.0
+Summary: An incredibly lightweight wrapper around urllib
+Home-page: https://github.com/sesh/thttp
+Author: Brenton Cleeland
+Author-email: brenton@brntn.me
+Project-URL: Bug Tracker, https://github.com/sesh/thttp/issues
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # thttp
 
 `thttp` is a single file, lightweight, well-tested wrapper around `urllib` that's intended to be copied directly into your project.
 
 It's features include:
 
 - Making GET, POST, PATCH, PUT, HEAD and OPTIONS requests
@@ -14,22 +27,23 @@
 - Sending through a CookieJar object that can be reused between requests
 - Authenticating with HTTP basic auth
 - Specifying a custom timeout for your request
 - Decompressing gzipped content in the response
 - Loading JSON from the response
 - Returning error responses instead of throwing exceptions from `urllib`
 - `pretty()` function for printing responses
+- Ability to upload files using the `{"file": open("file.png", "rb")}` style
 
 Future features:
 
 - Better detection of JSON responses
 - Improve handling of non-utf-8 requests
 - Improve handling of non-utf-8 responses
 
-_Note: this project is not intended to solve all use cases that can be achieved with urllib, requests or other HTTP libraries. The intent is to provide a lightweight tool that simplifies some of the most common use cases for developers._
+_Note: this project is not intended to solve all use cases that can be achieved with urllib, requests, httpx, or other HTTP libraries. The intent is to provide a lightweight tool that simplifies some of the most common use cases for developers._
 
 
 ## Installation
 
 copy `thttp.py` directly into your project:
 
 ```
@@ -83,7 +97,13 @@
 ## Packaging for release
 
 ```
 rm dist/*
 python3 -m build
 python3 -m twine upload dist/*
 ```
+
+
+## License
+
+This code is currently released under the [UNLICENSE](UNLICENSE.md) and considered public domain.
+If more appropriate for your usage you may consider this project released under the [MIT License](LICENSE.md).
```

### Comparing `thttp-1.2.0/thttp.egg-info/PKG-INFO` & `thttp-1.3.0/thttp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: thttp
-Version: 1.2.0
+Version: 1.3.0
 Summary: An incredibly lightweight wrapper around urllib
 Home-page: https://github.com/sesh/thttp
 Author: Brenton Cleeland
 Author-email: brenton@brntn.me
 Project-URL: Bug Tracker, https://github.com/sesh/thttp/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # thttp
 
 `thttp` is a single file, lightweight, well-tested wrapper around `urllib` that's intended to be copied directly into your project.
 
 It's features include:
 
@@ -26,22 +27,23 @@
 - Sending through a CookieJar object that can be reused between requests
 - Authenticating with HTTP basic auth
 - Specifying a custom timeout for your request
 - Decompressing gzipped content in the response
 - Loading JSON from the response
 - Returning error responses instead of throwing exceptions from `urllib`
 - `pretty()` function for printing responses
+- Ability to upload files using the `{"file": open("file.png", "rb")}` style
 
 Future features:
 
 - Better detection of JSON responses
 - Improve handling of non-utf-8 requests
 - Improve handling of non-utf-8 responses
 
-_Note: this project is not intended to solve all use cases that can be achieved with urllib, requests or other HTTP libraries. The intent is to provide a lightweight tool that simplifies some of the most common use cases for developers._
+_Note: this project is not intended to solve all use cases that can be achieved with urllib, requests, httpx, or other HTTP libraries. The intent is to provide a lightweight tool that simplifies some of the most common use cases for developers._
 
 
 ## Installation
 
 copy `thttp.py` directly into your project:
 
 ```
@@ -95,7 +97,13 @@
 ## Packaging for release
 
 ```
 rm dist/*
 python3 -m build
 python3 -m twine upload dist/*
 ```
+
+
+## License
+
+This code is currently released under the [UNLICENSE](UNLICENSE.md) and considered public domain.
+If more appropriate for your usage you may consider this project released under the [MIT License](LICENSE.md).
```

### Comparing `thttp-1.2.0/thttp.py` & `thttp-1.3.0/thttp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """
-UNLICENSED
-This is free and unencumbered software released into the public domain.
+You may use this code under the UNLICENSE or MIT License.
+See README.md for details.
 
 https://github.com/sesh/thttp
 """
 
 import gzip
-import ssl
 import json as json_lib
-
+import mimetypes
+import secrets
+import ssl
 from base64 import b64encode
 from collections import namedtuple
-
 from http import HTTPStatus
 from http.cookiejar import CookieJar
 from urllib.error import HTTPError, URLError
 from urllib.parse import urlencode
 from urllib.request import (
-    Request,
-    build_opener,
+    HTTPCookieProcessor,
     HTTPRedirectHandler,
     HTTPSHandler,
-    HTTPCookieProcessor,
+    Request,
+    build_opener,
 )
 
-
 Response = namedtuple("Response", "request content json status url headers cookiejar")
 
 
 class NoRedirect(HTTPRedirectHandler):
     def redirect_request(self, req, fp, code, msg, headers, newurl):
         return None
 
@@ -41,14 +40,15 @@
     headers={},
     method="GET",
     verify=True,
     redirect=True,
     cookiejar=None,
     basic_auth=None,
     timeout=None,
+    files={},  # note: experimental
 ):
     """
     Returns a (named)tuple with the following properties:
         - request
         - content
         - json (dict; or None)
         - headers (dict; all lowercase keys)
@@ -63,34 +63,58 @@
     if params:
         url += "?" + urlencode(params)  # build URL from query parameters
 
     if json and data:
         raise Exception("Cannot provide both json and data parameters")
 
     if method not in ["POST", "PATCH", "PUT"] and (json or data):
-        raise Exception(
-            "Request method must POST, PATCH or PUT if json or data is provided"
-        )
+        raise Exception("Request method must POST, PATCH or PUT if json or data is provided")
+
+    if files and method != "POST":
+        raise Exception("Request method must be POST when uploading files")
 
     if not timeout:
         timeout = 60
 
     if json:  # if we have json, dump it to a string and put it in our data variable
         headers["content-type"] = "application/json"
         data = json_lib.dumps(json).encode("utf-8")
     elif data and not isinstance(data, (str, bytes)):
         data = urlencode(data).encode()
     elif isinstance(data, str):
         data = data.encode()
+    elif files:
+        boundary = secrets.token_hex()
+
+        headers["Content-Type"] = f"multipart/form-data; boundary={boundary}"
+        data = b""
+
+        for key, file in files.items():
+            file_data = file.read()  # okay, we want this to stay as a byte-string
+            if isinstance(file_data, str):
+                file_data = file_data.encode("utf-8")
+            fn = file.name
+
+            mime, _ = mimetypes.guess_type(fn)
+            if not mime:
+                print("Using default mimetype")
+                mime = "application/octet-stream"
+
+            data += b"--" + boundary.encode() + b"\r\n"
+            data += b'Content-Disposition: form-data; name="' + key.encode() + b'"; filename="' + fn.encode() + b'"\r\n'
+            data += b"Content-Type: " + mime.encode() + b"\r\n\r\n"
+            data += file_data + b"\r\n"
+            data += b"--" + boundary.encode() + b"--\r\n"
+
+        data = data
+        headers["Content-Length"] = len(data)
 
     if basic_auth and len(basic_auth) == 2 and "authorization" not in headers:
         username, password = basic_auth
-        headers[
-            "authorization"
-        ] = f'Basic {b64encode(f"{username}:{password}".encode()).decode("ascii")}'
+        headers["authorization"] = f'Basic {b64encode(f"{username}:{password}".encode()).decode("ascii")}'
 
     if not cookiejar:
         cookiejar = CookieJar()
 
     ctx = ssl.create_default_context()
     if not verify:  # ignore ssl errors
         ctx.check_hostname = False
@@ -113,16 +137,15 @@
             headers = {k.lower(): v for k, v in list(resp.info().items())}
 
             if "gzip" in headers.get("content-encoding", ""):
                 content = gzip.decompress(content)
 
             json = (
                 json_lib.loads(content)
-                if "application/json" in headers.get("content-type", "").lower()
-                and content
+                if "application/json" in headers.get("content-type", "").lower() and content
                 else None
             )
     except HTTPError as e:
         status, content, resp_url = (e.code, e.read(), e.geturl())
         headers = {k.lower(): v for k, v in list(e.headers.items())}
 
         if "gzip" in headers.get("content-encoding", ""):
@@ -139,21 +162,15 @@
 
 def pretty(response, headers_only=False):
     RESET = "\033[0m"
     HIGHLIGHT = "\033[34m"
     HTTP_STATUSES = {x.value: x.name for x in HTTPStatus}
 
     # status code
-    print(
-        HIGHLIGHT
-        + str(response.status)
-        + " "
-        + RESET
-        + HTTP_STATUSES.get(response.status, "")
-    )
+    print(HIGHLIGHT + str(response.status) + " " + RESET + HTTP_STATUSES.get(response.status, ""))
 
     # headers
     for k in sorted(response.headers.keys()):
         print(HIGHLIGHT + k + RESET + ": " + response.headers[k])
 
     if headers_only:
         return
@@ -164,17 +181,19 @@
     # response body
     if response.json:
         print(json_lib.dumps(response.json, indent=2))
     else:
         print(response.content.decode())
 
 
-import unittest  # noqa: E402
 import contextlib  # noqa: E402
+import os  # noqa: E402
+import unittest  # noqa: E402
 from io import StringIO  # noqa: E402
+from unittest.mock import patch  # noqa: E402
 
 
 class RequestTestCase(unittest.TestCase):
     def test_cannot_provide_json_and_data(self):
         with self.assertRaises(Exception):
             request(
                 "https://httpbingo.org/post",
@@ -183,64 +202,54 @@
             )
 
     def test_should_fail_if_json_or_data_and_not_p_method(self):
         with self.assertRaises(Exception):
             request("https://httpbingo.org/post", json={"name": "Brenton"})
 
         with self.assertRaises(Exception):
-            request(
-                "https://httpbingo.org/post", json={"name": "Brenton"}, method="HEAD"
-            )
+            request("https://httpbingo.org/post", json={"name": "Brenton"}, method="HEAD")
 
     def test_should_set_content_type_for_json_request(self):
-        response = request(
-            "https://httpbingo.org/post", json={"name": "Brenton"}, method="POST"
-        )
+        response = request("https://httpbingo.org/post", json={"name": "Brenton"}, method="POST")
         self.assertEqual(response.request.headers["Content-type"], "application/json")
 
     def test_should_work(self):
         response = request("https://httpbingo.org/get")
         self.assertEqual(response.status, 200)
 
     def test_should_create_url_from_params(self):
         response = request(
             "https://httpbingo.org/get",
             params={"name": "brenton", "library": "tiny-request"},
         )
-        self.assertEqual(
-            response.url, "https://httpbingo.org/get?name=brenton&library=tiny-request"
-        )
+        self.assertEqual(response.url, "https://httpbingo.org/get?name=brenton&library=tiny-request")
 
     def test_should_return_headers(self):
-        response = request(
-            "https://httpbingo.org/response-headers", params={"Test-Header": "value"}
-        )
+        response = request("https://httpbingo.org/response-headers", params={"Test-Header": "value"})
         self.assertEqual(response.headers["test-header"], "value")
 
     def test_should_populate_json(self):
         response = request("https://httpbingo.org/json")
         self.assertTrue("slideshow" in response.json)
 
     def test_should_return_response_for_404(self):
         response = request("https://httpbingo.org/404")
         self.assertEqual(response.status, 404)
-        self.assertTrue("text/plain" in response.headers["content-type"])
+        self.assertTrue("application/json" in response.headers["content-type"])
 
     def test_should_fail_with_bad_ssl(self):
         with self.assertRaises(URLError):
             request("https://expired.badssl.com/")
 
     def test_should_load_bad_ssl_with_verify_false(self):
         response = request("https://expired.badssl.com/", verify=False)
         self.assertEqual(response.status, 200)
 
     def test_should_form_encode_non_json_post_requests(self):
-        response = request(
-            "https://httpbingo.org/post", data={"name": "test-user"}, method="POST"
-        )
+        response = request("https://httpbingo.org/post", data={"name": "test-user"}, method="POST")
         self.assertEqual(response.json["form"]["name"], ["test-user"])
 
     def test_should_follow_redirect(self):
         response = request(
             "https://httpbingo.org/redirect-to",
             params={"url": "https://example.org/"},
         )
@@ -257,35 +266,27 @@
 
     def test_cookies(self):
         response = request(
             "https://httpbingo.org/cookies/set",
             params={"cookie": "test"},
             redirect=False,
         )
-        response = request(
-            "https://httpbingo.org/cookies", cookiejar=response.cookiejar
-        )
+        response = request("https://httpbingo.org/cookies", cookiejar=response.cookiejar)
         self.assertEqual(response.json["cookie"], "test")
 
     def test_basic_auth(self):
-        response = request(
-            "http://httpbingo.org/basic-auth/user/passwd", basic_auth=("user", "passwd")
-        )
+        response = request("http://httpbingo.org/basic-auth/user/passwd", basic_auth=("user", "passwd"))
         self.assertEqual(response.json["authorized"], True)
 
     def test_should_handle_gzip(self):
-        response = request(
-            "http://httpbingo.org/gzip", headers={"Accept-Encoding": "gzip"}
-        )
+        response = request("http://httpbingo.org/gzip", headers={"Accept-Encoding": "gzip"})
         self.assertEqual(response.json["gzipped"], True)
 
     def test_should_handle_gzip_error(self):
-        response = request(
-            "http://httpbingo.org/status/418", headers={"Accept-Encoding": "gzip"}
-        )
+        response = request("http://httpbingo.org/status/418", headers={"Accept-Encoding": "gzip"})
         self.assertEqual(response.content, b"I'm a teapot!")
 
     def test_should_timeout(self):
         import socket
 
         with self.assertRaises((TimeoutError, socket.timeout)):
             request("http://httpbingo.org/delay/3", timeout=1)
@@ -323,7 +324,33 @@
             pretty(response, headers_only=True)
 
         f.seek(0)
         output = f.read()
 
         self.assertTrue("text/html; charset=utf-8" in output)
         self.assertTrue("<h1>base.html</h1>" not in output)
+
+    def test_thttp_with_mocked_response(self):
+        mocked_response = Response(None, None, {"response": "mocked"}, 200, None, None, None)
+
+        with patch("thttp.request", side_effect=[mocked_response]):
+            response = request("https://example.org")
+            self.assertEqual("mocked", response.json["response"])
+
+    def test_upload_single_file(self):
+        token = os.environ.get("MEDIAPUB_TOKEN")
+        url = os.environ.get("MEDIAPUB_URL")
+
+        if not token or not url:
+            self.skipTest("Skipping media upload test because environment variables are not available")
+
+        for fn in ["test-image.png", "LICENSE.md"]:
+            with open(fn, "rb" if fn.endswith("png") else "r") as f:
+                response = request(
+                    url,
+                    headers={"Authorization": f"Bearer {token}"},
+                    files={"file": f},
+                    method="POST",
+                )
+
+            self.assertEqual(response.status, 201)
+            self.assertTrue("location" in response.headers)
```

