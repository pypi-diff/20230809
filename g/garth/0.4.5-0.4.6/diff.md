# Comparing `tmp/garth-0.4.5.tar.gz` & `tmp/garth-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.4.5.tar", last modified: Sun Aug  6 16:34:07 2023, max compression
+gzip compressed data, was "garth-0.4.6.tar", last modified: Wed Aug  9 04:47:42 2023, max compression
```

## Comparing `garth-0.4.5.tar` & `garth-0.4.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.5/LICENSE
--rw-r--r--   0        0        0    13307 2023-08-06 16:08:54.789312 garth-0.4.5/README.md
--rw-r--r--   0        0        0      701 2023-08-06 16:32:45.846510 garth-0.4.5/garth/__init__.py
--rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.5/garth/auth_tokens.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.4.5/garth/exc.py
--rw-r--r--   0        0        0     5342 2023-08-06 15:02:02.369881 garth-0.4.5/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.5/garth/py.typed
--rw-r--r--   0        0        0     4629 2023-08-06 15:02:02.370079 garth-0.4.5/garth/sso.py
--rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.5/garth/stats/__init__.py
--rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.5/garth/stats/_base.py
--rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.5/garth/stats/hrv.py
--rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.5/garth/stats/intensity_minutes.py
--rw-r--r--   0        0        0     3523 2023-08-01 01:10:51.104099 garth-0.4.5/garth/stats/sleep.py
--rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.5/garth/stats/steps.py
--rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.5/garth/stats/stress.py
--rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.5/garth/utils.py
--rw-r--r--   0        0        0       22 2023-08-06 16:33:36.780244 garth-0.4.5/garth/version.py
--rw-r--r--   0        0        0     1221 2023-08-06 16:34:07.337987 garth-0.4.5/pyproject.toml
--rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.5/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.5/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.5/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    50890 2023-08-04 23:53:42.180823 garth-0.4.5/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    54154 2023-08-04 23:59:00.720080 garth-0.4.5/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0    71602 2023-08-04 23:53:07.635030 garth-0.4.5/tests/cassettes/test_login_success_mfa.yaml
--rw-r--r--   0        0        0     8025 2023-08-06 15:02:02.370447 garth-0.4.5/tests/cassettes/test_refresh_oauth2_token.yaml
--rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.5/tests/cassettes/test_username.yaml
--rw-r--r--   0        0        0     3687 2023-08-06 15:02:02.370638 garth-0.4.5/tests/conftest.py
--rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.5/tests/stats/cassettes/test_daily_hrv.yaml
--rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.5/tests/stats/cassettes/test_daily_hrv_no_results.yaml
--rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.5/tests/stats/cassettes/test_daily_hrv_paginate.yaml
--rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.5/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
--rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.5/tests/stats/cassettes/test_daily_intensity_minutes.yaml
--rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.5/tests/stats/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.5/tests/stats/cassettes/test_daily_steps.yaml
--rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.5/tests/stats/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.5/tests/stats/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.5/tests/stats/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.5/tests/stats/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.5/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
--rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.5/tests/stats/cassettes/test_weekly_steps.yaml
--rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.5/tests/stats/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.5/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.5/tests/stats/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.5/tests/stats/test_hrv.py
--rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.5/tests/stats/test_intensity_minutes.py
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.5/tests/stats/test_sleep.py
--rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.5/tests/stats/test_steps.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.5/tests/stats/test_stress.py
--rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.5/tests/test_auth_tokens.py
--rw-r--r--   0        0        0     4139 2023-08-06 15:02:02.370821 garth-0.4.5/tests/test_http.py
--rw-r--r--   0        0        0     2684 2023-08-04 23:59:13.586158 garth-0.4.5/tests/test_sso.py
--rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.5/tests/test_utils.py
--rw-r--r--   0        0        0    13759 1970-01-01 00:00:00.000000 garth-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.6/LICENSE
+-rw-r--r--   0        0        0    13307 2023-08-06 16:08:54.789312 garth-0.4.6/README.md
+-rw-r--r--   0        0        0      701 2023-08-09 04:47:33.156063 garth-0.4.6/garth/__init__.py
+-rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.6/garth/auth_tokens.py
+-rw-r--r--   0        0        0      349 2023-08-09 04:47:33.159610 garth-0.4.6/garth/exc.py
+-rw-r--r--   0        0        0     5546 2023-08-09 04:47:33.159734 garth-0.4.6/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.6/garth/py.typed
+-rw-r--r--   0        0        0     4629 2023-08-06 15:02:02.370079 garth-0.4.6/garth/sso.py
+-rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.6/garth/stats/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.6/garth/stats/_base.py
+-rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.6/garth/stats/hrv.py
+-rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.6/garth/stats/intensity_minutes.py
+-rw-r--r--   0        0        0     4678 2023-08-09 04:47:33.163448 garth-0.4.6/garth/stats/sleep.py
+-rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.6/garth/stats/steps.py
+-rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.6/garth/stats/stress.py
+-rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.6/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-08-09 04:47:33.163569 garth-0.4.6/garth/version.py
+-rw-r--r--   0        0        0     1239 2023-08-09 04:47:42.709280 garth-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.6/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.6/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.6/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    50890 2023-08-04 23:53:42.180823 garth-0.4.6/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    54154 2023-08-04 23:59:00.720080 garth-0.4.6/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0    71602 2023-08-04 23:53:07.635030 garth-0.4.6/tests/cassettes/test_login_success_mfa.yaml
+-rw-r--r--   0        0        0     8025 2023-08-06 15:02:02.370447 garth-0.4.6/tests/cassettes/test_refresh_oauth2_token.yaml
+-rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.6/tests/cassettes/test_username.yaml
+-rw-r--r--   0        0        0     3687 2023-08-06 15:02:02.370638 garth-0.4.6/tests/conftest.py
+-rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.6/tests/stats/cassettes/test_daily_hrv.yaml
+-rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.6/tests/stats/cassettes/test_daily_hrv_no_results.yaml
+-rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.6/tests/stats/cassettes/test_daily_hrv_paginate.yaml
+-rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.6/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
+-rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.6/tests/stats/cassettes/test_daily_intensity_minutes.yaml
+-rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.6/tests/stats/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.6/tests/stats/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.6/tests/stats/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.6/tests/stats/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.6/tests/stats/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.6/tests/stats/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.6/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
+-rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.6/tests/stats/cassettes/test_weekly_steps.yaml
+-rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.6/tests/stats/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.6/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.6/tests/stats/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.6/tests/stats/test_hrv.py
+-rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.6/tests/stats/test_intensity_minutes.py
+-rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.6/tests/stats/test_sleep.py
+-rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.6/tests/stats/test_steps.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.6/tests/stats/test_stress.py
+-rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.6/tests/test_auth_tokens.py
+-rw-r--r--   0        0        0     4150 2023-08-09 04:47:33.159878 garth-0.4.6/tests/test_http.py
+-rw-r--r--   0        0        0     2674 2023-08-09 04:47:33.160003 garth-0.4.6/tests/test_sso.py
+-rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.6/tests/test_utils.py
+-rw-r--r--   0        0        0    13759 1970-01-01 00:00:00.000000 garth-0.4.6/PKG-INFO
```

### Comparing `garth-0.4.5/LICENSE` & `garth-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/README.md` & `garth-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/__init__.py` & `garth-0.4.6/garth/__init__.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/auth_tokens.py` & `garth-0.4.6/garth/auth_tokens.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/http.py` & `garth-0.4.6/garth/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import os
 
-from requests import Response, Session
+from requests import HTTPError, Response, Session
 from requests.adapters import HTTPAdapter, Retry
 
 from . import sso
 from .auth_tokens import OAuth1Token, OAuth2Token
+from .exc import GarthHTTPError
 from .utils import asdict
 
 USER_AGENT = {
     "User-Agent": (
         "Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) "
         "AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148"
     ),
@@ -109,15 +110,21 @@
         self.last_resp = self.sess.request(
             method,
             url,
             headers=headers,
             timeout=self.timeout,
             **kwargs,
         )
-        self.last_resp.raise_for_status()
+        try:
+            self.last_resp.raise_for_status()
+        except HTTPError as e:
+            raise GarthHTTPError(
+                msg="Error in request",
+                error=e,
+            )
         return self.last_resp
 
     def get(self, *args, **kwargs) -> Response:
         return self.request("GET", *args, **kwargs)
 
     def post(self, *args, **kwargs) -> Response:
         return self.request("POST", *args, **kwargs)
```

### Comparing `garth-0.4.5/garth/sso.py` & `garth-0.4.6/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/stats/_base.py` & `garth-0.4.6/garth/stats/_base.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/stats/hrv.py` & `garth-0.4.6/garth/stats/hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/stats/intensity_minutes.py` & `garth-0.4.6/garth/stats/intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/stats/steps.py` & `garth-0.4.6/garth/stats/steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/stats/stress.py` & `garth-0.4.6/garth/stats/stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/garth/utils.py` & `garth-0.4.6/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/pyproject.toml` & `garth-0.4.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
 packages = [
     { include = "garth" },
 ]
-version = "0.4.5"
+version = "0.4.6"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -59,13 +59,14 @@
 ]
 linting = [
     "black",
     "ruff",
     "mypy",
     "isort",
     "types-requests",
+    "types-pytz",
 ]
 testing = [
     "coverage",
     "pytest",
     "pytest-vcr",
 ]
```

### Comparing `garth-0.4.5/tests/cassettes/test_client_request.yaml` & `garth-0.4.6/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/cassettes/test_connectapi.yaml` & `garth-0.4.6/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/cassettes/test_exchange.yaml` & `garth-0.4.6/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.4.6/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/cassettes/test_login_success.yaml` & `garth-0.4.6/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/cassettes/test_login_success_mfa.yaml` & `garth-0.4.6/tests/cassettes/test_login_success_mfa.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/cassettes/test_refresh_oauth2_token.yaml` & `garth-0.4.6/tests/cassettes/test_refresh_oauth2_token.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/cassettes/test_username.yaml` & `garth-0.4.6/tests/cassettes/test_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/conftest.py` & `garth-0.4.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_hrv.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_hrv.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_hrv_no_results.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_hrv_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_hrv_paginate.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_hrv_paginate.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_intensity_minutes.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_sleep.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_sleep.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_steps.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_stress.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_daily_stress_pagination.yaml` & `garth-0.4.6/tests/stats/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_sleep_data_get.yaml` & `garth-0.4.6/tests/stats/cassettes/test_sleep_data_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_sleep_data_list.yaml` & `garth-0.4.6/tests/stats/cassettes/test_sleep_data_list.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_weekly_intensity_minutes.yaml` & `garth-0.4.6/tests/stats/cassettes/test_weekly_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_weekly_steps.yaml` & `garth-0.4.6/tests/stats/cassettes/test_weekly_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_weekly_stress.yaml` & `garth-0.4.6/tests/stats/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.4.6/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.4.6/tests/stats/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/test_hrv.py` & `garth-0.4.6/tests/stats/test_hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/test_intensity_minutes.py` & `garth-0.4.6/tests/stats/test_intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/test_sleep.py` & `garth-0.4.6/tests/stats/test_sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/test_steps.py` & `garth-0.4.6/tests/stats/test_steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/stats/test_stress.py` & `garth-0.4.6/tests/stats/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/tests/test_http.py` & `garth-0.4.6/tests/test_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tempfile
 import time
 
 import pytest
-from requests import HTTPError
 
 from garth.auth_tokens import OAuth2Token
+from garth.exc import GarthHTTPError
 from garth.http import Client
 
 
 def test_dump_and_load(authed_client: Client):
     with tempfile.TemporaryDirectory() as tempdir:
         authed_client.dump(tempdir)
 
@@ -83,15 +83,15 @@
 
 
 @pytest.mark.vcr
 def test_client_request(client: Client):
     resp = client.request("GET", "connect", "/")
     assert resp.ok
 
-    with pytest.raises(HTTPError):
+    with pytest.raises(GarthHTTPError):
         client.request("GET", "connectapi", "/")
 
 
 @pytest.mark.vcr
 def test_login_success_mfa(monkeypatch, client: Client):
     def mock_input(_):
         return "327751"
```

### Comparing `garth-0.4.5/tests/test_sso.py` & `garth-0.4.6/tests/test_sso.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import time
 
 import pytest
-from requests import HTTPError
 
 from garth import sso
 from garth.auth_tokens import OAuth1Token, OAuth2Token
-from garth.exc import GarthException
+from garth.exc import GarthException, GarthHTTPError
 from garth.http import Client
 
 
 @pytest.mark.vcr
 def test_login_email_password_fail(client: Client):
-    with pytest.raises(HTTPError):
+    with pytest.raises(GarthHTTPError):
         sso.login("user@example.com", "wrong_p@ssword", client=client)
 
 
 @pytest.mark.vcr
 def test_login_success(client: Client):
     oauth1, oauth2 = sso.login(
         "user@example.com", "correct_password", client=client
```

### Comparing `garth-0.4.5/tests/test_utils.py` & `garth-0.4.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.5/PKG-INFO` & `garth-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.4.5
+Version: 0.4.6
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

