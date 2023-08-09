# Comparing `tmp/pydexcom-0.2.3.tar.gz` & `tmp/pydexcom-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydexcom-0.2.3.tar", last modified: Thu Feb 24 03:40:42 2022, max compression
+gzip compressed data, was "pydexcom-0.3.0a0.tar", last modified: Wed Aug  9 01:08:13 2023, max compression
```

## Comparing `pydexcom-0.2.3.tar` & `pydexcom-0.3.0a0.tar`

### file list

```diff
@@ -1,17 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 03:40:42.352260 pydexcom-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-02-24 03:40:24.000000 pydexcom-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6787 2022-02-24 03:40:42.352260 pydexcom-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6455 2022-02-24 03:40:24.000000 pydexcom-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 03:40:42.352260 pydexcom-0.2.3/pydexcom/
--rw-r--r--   0 runner    (1001) docker     (121)     9983 2022-02-24 03:40:24.000000 pydexcom-0.2.3/pydexcom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-02-24 03:40:24.000000 pydexcom-0.2.3/pydexcom/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-02-24 03:40:24.000000 pydexcom-0.2.3/pydexcom/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 03:40:42.352260 pydexcom-0.2.3/pydexcom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6787 2022-02-24 03:40:42.000000 pydexcom-0.2.3/pydexcom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-02-24 03:40:42.000000 pydexcom-0.2.3/pydexcom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 03:40:42.000000 pydexcom-0.2.3/pydexcom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-24 03:40:42.000000 pydexcom-0.2.3/pydexcom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-24 03:40:42.000000 pydexcom-0.2.3/pydexcom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 03:40:41.000000 pydexcom-0.2.3/pydexcom.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-24 03:40:42.352260 pydexcom-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-02-24 03:40:24.000000 pydexcom-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.539184 pydexcom-0.3.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.531184 pydexcom-0.3.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.535184 pydexcom-0.3.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/.github/workflows/pre-commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.535184 pydexcom-0.3.0a0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/.vscode/pydexcom.code-workspace
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-08-09 01:08:13.539184 pydexcom-0.3.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.535184 pydexcom-0.3.0a0/pydexcom/
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/pydexcom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/pydexcom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/pydexcom/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.535184 pydexcom-0.3.0a0/pydexcom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-08-09 01:08:13.000000 pydexcom-0.3.0a0/pydexcom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-09 01:08:13.000000 pydexcom-0.3.0a0/pydexcom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:08:13.000000 pydexcom-0.3.0a0/pydexcom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-09 01:08:13.000000 pydexcom-0.3.0a0/pydexcom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-09 01:08:13.000000 pydexcom-0.3.0a0/pydexcom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:08:13.539184 pydexcom-0.3.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.535184 pydexcom-0.3.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.531184 pydexcom-0.3.0a0/tests/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.531184 pydexcom-0.3.0a0/tests/cassettes/test_dexcom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.539184 pydexcom-0.3.0a0/tests/cassettes/test_dexcom/TestDexcom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_dexcom/TestDexcom/test_dexcom[p@$$w0rd-u$ern@me].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_dexcom/TestDexcom/test_dexcom[p@$$w0rd-username].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_dexcom/TestDexcom/test_dexcom[password-u$ern@me].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_dexcom/TestDexcom/test_dexcom[password-username].yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.531184 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:08:13.539184 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/dexcom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/test_get_current_glucose_reading.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/test_get_current_glucose_reading_session_expired.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/test_get_glucose_readings[0-0].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/test_get_glucose_readings[0-10].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/test_get_glucose_readings[1-0].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/test_get_glucose_readings[1-10].yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/cassettes/test_glucose_reading/TestGlucoseReading/test_get_latest_glucose_reading.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/test_dexcom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-08-09 01:07:57.000000 pydexcom-0.3.0a0/tests/test_glucose_reading.py
```

### Comparing `pydexcom-0.2.3/LICENSE.txt` & `pydexcom-0.3.0a0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
-Copyright (c) 2020 Gage Benne
+Copyright (c) 2023 Gage Benne
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 The above copyright notice and this permission notice shall be included in all
```

### Comparing `pydexcom-0.2.3/pydexcom/__init__.py` & `pydexcom-0.3.0a0/pydexcom/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,258 +1,302 @@
-"""The pydexcom module for interacting with Dexcom Share API."""
-import datetime
+"""
+.. include:: ../README.md
+"""
+import logging
+import re
+from datetime import datetime
+from typing import Any, Dict, List, Optional
 
 import requests
 
-import re
-
 from .const import (
-    _LOGGER,
-    ACCOUNT_ERROR_ACCOUNT_NOT_FOUND,
-    ACCOUNT_ERROR_PASSWORD_INVALID,
-    ACCOUNT_ERROR_PASSWORD_NULL_EMPTY,
-    ACCOUNT_ERROR_MAX_ATTEMPTS,
-    ACCOUNT_ERROR_UNKNOWN,
-    ACCOUNT_ERROR_USERNAME_NULL_EMPTY,
-    ARGUEMENT_ERROR_MAX_COUNT_INVALID,
-    ARGUEMENT_ERROR_MINUTES_INVALID,
-    ARGUEMENT_ERROR_SERIAL_NUMBER_NULL_EMPTY,
-    DEFAULT_SESSION_ID,
+    DEFAULT_UUID,
     DEXCOM_APPLICATION_ID,
     DEXCOM_AUTHENTICATE_ENDPOINT,
     DEXCOM_BASE_URL,
     DEXCOM_BASE_URL_OUS,
     DEXCOM_GLUCOSE_READINGS_ENDPOINT,
     DEXCOM_LOGIN_ID_ENDPOINT,
-    DEXCOM_TREND_ARROWS,
-    DEXCOM_TREND_DESCRIPTIONS,
     DEXCOM_TREND_DIRECTIONS,
-    DEXCOM_VERIFY_SERIAL_NUMBER_ENDPOINT,
-    MMOL_L_CONVERTION_FACTOR,
-    SESSION_ERROR_SESSION_ID_DEFAULT,
-    SESSION_ERROR_SESSION_ID_NULL,
-    SESSION_ERROR_ACCOUNT_ID_NULL_EMPTY,
-    SESSION_ERROR_ACCOUNT_ID_DEFAULT,
-    SESSION_ERROR_SESSION_NOT_FOUND,
-    SESSION_ERROR_SESSION_NOT_VALID,
+    MAX_MAX_COUNT,
+    MAX_MINUTES,
+    MMOL_L_CONVERSION_FACTOR,
+    REQUEST_TIMEOUT,
+    TREND_ARROWS,
+    TREND_DESCRIPTIONS,
+)
+from .errors import (
+    AccountError,
+    AccountErrorEnum,
+    ArgumentError,
+    ArgumentErrorEnum,
+    DexcomError,
+    SessionError,
+    SessionErrorEnum,
 )
-from .errors import AccountError, ArguementError, SessionError
+
+_LOGGER = logging.getLogger("pydexcom")
 
 
 class GlucoseReading:
     """Class for parsing glucose reading from Dexcom Share API."""
 
-    def __init__(self, json_glucose_reading: dict):
-        """Initialize with JSON glucose reading from Dexcom Share API."""
-        self.value = json_glucose_reading["Value"]
-        self.mg_dl = self.value
-        self.mmol_l = round(self.value * MMOL_L_CONVERTION_FACTOR, 1)
-        self.trend = json_glucose_reading["Trend"]
-        if not isinstance(self.trend, int):
-            self.trend = DEXCOM_TREND_DIRECTIONS.get(self.trend, 0)
-        self.trend_description = DEXCOM_TREND_DESCRIPTIONS[self.trend]
-        self.trend_arrow = DEXCOM_TREND_ARROWS[self.trend]
-        self.time = datetime.datetime.fromtimestamp(
-            int(re.sub("[^0-9]", "", json_glucose_reading["WT"])) / 1000.0
-        )
+    def __init__(self, json_glucose_reading: Dict[str, Any]):
+        """Initialize `GlucoseReading` with JSON glucose reading from Dexcom Share API.
+
+        :param json_glucose_reading: JSON glucose reading from Dexcom Share API
+        """
+        self._json = json_glucose_reading
+        try:
+            self._value = int(json_glucose_reading["Value"])
+            self._trend_direction: str = json_glucose_reading["Trend"]
+            # Dexcom Share API returns `str` direction now, previously `int` trend
+            self._trend: int = DEXCOM_TREND_DIRECTIONS[self._trend_direction]
+            self._datetime = datetime.fromtimestamp(
+                int(re.sub("[^0-9]", "", json_glucose_reading["WT"])) / 1000.0
+            )
+        except (KeyError, TypeError, ValueError):
+            raise ArgumentError(ArgumentErrorEnum.GLUCOSE_READING_INVALID)
+
+    @property
+    def value(self) -> int:
+        """Blood glucose value in mg/dL."""
+        return self._value
+
+    @property
+    def mg_dl(self) -> int:
+        """Blood glucose value in mg/dL."""
+        return self._value
+
+    @property
+    def mmol_l(self) -> float:
+        """Blood glucose value in mmol/L."""
+        return round(self.value * MMOL_L_CONVERSION_FACTOR, 1)
+
+    @property
+    def trend(self) -> int:
+        """Blood glucose trend information
+        (value of `pydexcom.const.DEXCOM_TREND_DIRECTIONS`)."""
+        return self._trend
+
+    @property
+    def trend_direction(self) -> str:
+        """Blood glucose trend direction
+        (key of `pydexcom.const.DEXCOM_TREND_DIRECTIONS`)."""
+        return self._trend_direction
+
+    @property
+    def trend_description(self) -> Optional[str]:
+        """Blood glucose trend information description
+        (`pydexcom.const.TREND_DESCRIPTIONS`).
+        """
+        return TREND_DESCRIPTIONS[self._trend]
+
+    @property
+    def trend_arrow(self) -> str:
+        """Blood glucose trend as unicode arrow (`pydexcom.const.TREND_ARROWS`)."""
+        return TREND_ARROWS[self._trend]
+
+    @property
+    def datetime(self) -> datetime:
+        """Glucose reading recorded time as datetime."""
+        return self._datetime
+
+    @property
+    def json(self) -> Dict[str, Any]:
+        """JSON glucose reading from Dexcom Share API."""
+        return self._json
+
+    def __str__(self) -> str:
+        return str(self._value)
 
 
 class Dexcom:
     """Class for communicating with Dexcom Share API."""
 
     def __init__(self, username: str, password: str, ous: bool = False):
-        """Initialize with JSON glucose reading from Dexcom Share API."""
-        self.base_url = DEXCOM_BASE_URL_OUS if ous else DEXCOM_BASE_URL
-        self.username = username
-        self.password = password
-        self.session_id = None
-        self.account_id = None
-        self.create_session()
+        """
+        Initialize `Dexcom` with Dexcom Share credentials.
 
-    def _request(
+        :param username: username for the Dexcom Share user, *not follower*.
+        :param password: password for the Dexcom Share user.
+        :param ous: whether the Dexcom Share user is outside of the US.
+        """
+        self._base_url = DEXCOM_BASE_URL_OUS if ous else DEXCOM_BASE_URL
+        self._username = username
+        self._password = password
+        self._account_id: Optional[str] = None
+        self._session_id: Optional[str] = None
+        self.__session = requests.Session()
+        self._session()
+
+    def _post(
         self,
-        method: str,
         endpoint: str,
-        params: dict = None,
-        json: dict = {},
-    ) -> dict:
-        """Send request to Dexcom Share API."""
-        try:
-            url = f"{self.base_url}/{endpoint}"
-            _LOGGER.debug(f"{method} request to {endpoint}:")
-            _LOGGER.debug(f"url: {url} params:{params}, json: {json}")
-            r = requests.request(
-                method,
-                url,
-                params=params,
-                json=json,
-            )
-            _LOGGER.debug(f"{method} request response {r.status_code}:")
-            _LOGGER.debug(f"json: {r.json()}")
-            r.raise_for_status()
-            return r.json()
-        except requests.HTTPError:
-            _LOGGER.error(f"json: {r.json()}")
-            if r.status_code == 500:
-                _LOGGER.debug(f'{r.json()["Code"]}: {r.json()["Message"]}')
-                if r.json()["Code"] == "SessionNotValid":
-                    raise SessionError(SESSION_ERROR_SESSION_NOT_VALID)
-                elif r.json()["Code"] == "SessionIdNotFound":
-                    raise SessionError(SESSION_ERROR_SESSION_NOT_FOUND)
-                elif r.json()["Code"] == "SSO_AuthenticateAccountNotFound":
-                    raise AccountError(ACCOUNT_ERROR_ACCOUNT_NOT_FOUND)
-                elif r.json()["Code"] == "AccountPasswordInvalid":
-                    raise AccountError(ACCOUNT_ERROR_PASSWORD_INVALID)
-                elif r.json()["Code"] == "SSO_AuthenticateMaxAttemptsExceeed":
-                    raise AccountError(ACCOUNT_ERROR_MAX_ATTEMPTS)
-                elif r.json()["Code"] == "InvalidArgument":
-                    if "accountName" in r.json()["Message"]:
-                        raise AccountError(ACCOUNT_ERROR_USERNAME_NULL_EMPTY)
-                    if "password" in r.json()["Message"]:
-                        raise AccountError(ACCOUNT_ERROR_PASSWORD_NULL_EMPTY)
-                else:
-                    _LOGGER.error(f'{r.json()["Code"]}: {r.json()["Message"]}')
-            else:
-                _LOGGER.error(f"{r.status_code}: {r.json()}")
-        except Exception:
-            _LOGGER.error(r.status_code)
-            _LOGGER.error("Unknown request error")
-        return None
-
-    def _validate_session_id(self):
-        """Validate session id."""
-        if not self.session_id:
-            _LOGGER.error(SESSION_ERROR_SESSION_ID_NULL)
-            raise SessionError(SESSION_ERROR_SESSION_ID_NULL)
-        if self.session_id == DEFAULT_SESSION_ID:
-            _LOGGER.error(SESSION_ERROR_SESSION_ID_DEFAULT)
-            raise SessionError(SESSION_ERROR_SESSION_ID_DEFAULT)
+        params: Optional[Dict[str, Any]] = None,
+        json: Optional[Dict[str, Any]] = None,
+    ) -> Any:
+        """Send post request to Dexcom Share API.
+
+        :param endpoint: URL of the post request
+        :param params: `dict` to send in the query string of the post request
+        :param json: JSON to send in the body of the post request
+        """
+        response = self.__session.post(
+            f"{self._base_url}/{endpoint}",
+            headers={"Accept-Encoding": "application/json"},
+            params=params,
+            json={} if json is None else json,
+            timeout=REQUEST_TIMEOUT,
+        )
 
-    def _validate_account(self):
-        """Validate credentials."""
-        if not self.username:
-            _LOGGER.error(ACCOUNT_ERROR_USERNAME_NULL_EMPTY)
-            raise AccountError(ACCOUNT_ERROR_USERNAME_NULL_EMPTY)
-        if not self.password:
-            _LOGGER.error(ACCOUNT_ERROR_PASSWORD_NULL_EMPTY)
-            raise AccountError(ACCOUNT_ERROR_PASSWORD_NULL_EMPTY)
+        try:
+            response.raise_for_status()
+            return response.json()
+        except requests.HTTPError as http_error:
+            error = self._handle_response(response)
+            if error:
+                raise error from http_error
+            _LOGGER.error("%s", response.text)
+            raise http_error
 
-    def _validate_account_id(self):
-        """Validate account ID."""
-        if not self.account_id:
-            _LOGGER.error(SESSION_ERROR_ACCOUNT_ID_NULL_EMPTY)
-            raise AccountError(SESSION_ERROR_ACCOUNT_ID_NULL_EMPTY)
-        if self.account_id == DEFAULT_SESSION_ID:
-            _LOGGER.error(SESSION_ERROR_ACCOUNT_ID_DEFAULT)
-            raise AccountError(SESSION_ERROR_ACCOUNT_ID_DEFAULT)
-
-    def create_session(self):
-        """Create Dexcom Share API session by getting session id."""
-        _LOGGER.debug("Get session ID")
-        self._validate_account()
-
-        json = {
-            "accountName": self.username,
-            "password": self.password,
-            "applicationId": DEXCOM_APPLICATION_ID,
-        }
+    def _handle_response(self, response: requests.Response) -> Optional[DexcomError]:
+        error: Optional[DexcomError] = None
         """
-        The Dexcom Share API at DEXCOM_AUTHENTICATE_ENDPOINT
-        returns the account ID if credentials are valid -- whether
-        the username is a classic username or email. Using the
-        account ID the DEXCOM_LOGIN_ID_ENDPOINT is used to fetch
-        a session ID.
+        Parse `requests.Response` for `pydexcom.errors.DexcomError`.
+
+        :param response: `requests.Response` to parse
         """
-        endpoint1 = DEXCOM_AUTHENTICATE_ENDPOINT
-        endpoint2 = DEXCOM_LOGIN_ID_ENDPOINT
+        if response.json():
+            _LOGGER.debug("%s", response.json())
+            code = response.json().get("Code", None)
+            message = response.json().get("Message", None)
+            if code == "SessionIdNotFound":
+                error = SessionError(SessionErrorEnum.NOT_FOUND)
+            elif code == "AccountPasswordInvalid":
+                error = AccountError(AccountErrorEnum.PASSWORD_INVALID)
+            elif code == "SSO_AuthenticateMaxAttemptsExceeed":
+                error = AccountError(AccountErrorEnum.MAX_ATTEMPTS)
+            elif code == "InvalidArgument":
+                if message and "accountName" in message:
+                    error = ArgumentError(ArgumentErrorEnum.USERNAME_INVALID)
+                elif message and "password" in message:
+                    error = ArgumentError(ArgumentErrorEnum.PASSWORD_INVALID)
+                elif message and "UUID" in message:
+                    error = ArgumentError(ArgumentErrorEnum.ACCOUNT_ID_INVALID)
+            elif code and message:
+                _LOGGER.error("%s: %s", code, message)
+        return error
+
+    def _validate_session_id(self) -> None:
+        """Validate session ID."""
+        if any([not isinstance(self._session_id, str), not self._session_id]):
+            raise ArgumentError(ArgumentErrorEnum.SESSION_ID_INVALID)
+        if self._session_id == DEFAULT_UUID:
+            raise ArgumentError(ArgumentErrorEnum.SESSION_ID_DEFAULT)
 
-        self.account_id = self._request("post", endpoint1, json=json)
-        try:
-            self._validate_account_id()
+    def _validate_credentials(self) -> None:
+        """Validate credentials."""
+        if any([not isinstance(self._username, str), not self._username]):
+            raise ArgumentError(ArgumentErrorEnum.USERNAME_INVALID)
+        if any([not isinstance(self._password, str), not self._password]):
+            raise ArgumentError(ArgumentErrorEnum.PASSWORD_INVALID)
 
-            json = {
-                "accountId": self.account_id,
-                "password": self.password,
+    def _validate_account_id(self) -> None:
+        """Validate account ID."""
+        if any([not isinstance(self._account_id, str), not self._account_id]):
+            raise ArgumentError(ArgumentErrorEnum.ACCOUNT_ID_INVALID)
+        if self._account_id == DEFAULT_UUID:
+            raise ArgumentError(ArgumentErrorEnum.ACCOUNT_ID_DEFAULT)
+
+    def _get_account_id(self) -> str:
+        """Retrieve account ID from the authentication endpoint
+        (`pydexcom.const.DEXCOM_AUTHENTICATE_ENDPOINT`)."""
+        return self._post(
+            DEXCOM_AUTHENTICATE_ENDPOINT,
+            json={
+                "accountName": self._username,
+                "password": self._password,
                 "applicationId": DEXCOM_APPLICATION_ID,
-            }
+            },
+        )
 
-            self.session_id = self._request("post", endpoint2, json=json)
-            self._validate_session_id()
-        except SessionError:
-            raise AccountError(ACCOUNT_ERROR_UNKNOWN)
+    def _get_session_id(self) -> str:
+        """Retrieve session ID from the login endpoint
+        (`pydexcom.const.DEXCOM_LOGIN_ID_ENDPOINT`)."""
+        return self._post(
+            DEXCOM_LOGIN_ID_ENDPOINT,
+            json={
+                "accountId": self._account_id,
+                "password": self._password,
+                "applicationId": DEXCOM_APPLICATION_ID,
+            },
+        )
 
-    def verify_serial_number(self, serial_number: str) -> bool:
-        """Verify if transmitter serial number is assigned to user."""
-        self._validate_session_id()
-        if not serial_number:
-            _LOGGER.error(ARGUEMENT_ERROR_SERIAL_NUMBER_NULL_EMPTY)
-            raise ArguementError(ARGUEMENT_ERROR_SERIAL_NUMBER_NULL_EMPTY)
+    def _session(self) -> None:
+        """Create Dexcom Share API session."""
+        self._validate_credentials()
 
-        params = {"sessionId": self.session_id, "serialNumber": serial_number}
-        try:
-            r = self._request(
-                "post", DEXCOM_VERIFY_SERIAL_NUMBER_ENDPOINT, params=params
-            )
-        except SessionError:
-            _LOGGER.debug("Get new session ID")
-            self.create_session()
-            r = self._request(
-                "post", DEXCOM_VERIFY_SERIAL_NUMBER_ENDPOINT, params=params
-            )
-        return r.json() == "AssignedToYou"
+        if self._account_id is None:
+            self._account_id = self._get_account_id()
+            self._validate_account_id()
 
-    def get_glucose_readings(
-        self, minutes: int = 1440, max_count: int = 288
-    ) -> [GlucoseReading]:
-        """Get max_count glucose readings within specified minutes."""
+        self._session_id = self._get_session_id()
         self._validate_session_id()
-        if minutes < 1 or minutes > 1440:
-            _LOGGER.error(ARGUEMENT_ERROR_MINUTES_INVALID)
-            raise ArguementError(ARGUEMENT_ERROR_MINUTES_INVALID)
-        if max_count < 1 or max_count > 288:
-            _LOGGER.error(ARGUEMENT_ERROR_MAX_COUNT_INVALID)
-            raise ArguementError(ARGUEMENT_ERROR_MAX_COUNT_INVALID)
-
-        params = {
-            "sessionId": self.session_id,
-            "minutes": minutes,
-            "maxCount": max_count,
-        }
-        try:
-            json_glucose_readings = self._request(
-                "post", DEXCOM_GLUCOSE_READINGS_ENDPOINT, params=params
-            )
-        except SessionError:
-            self.create_session()
 
-            params = {
-                "sessionId": self.session_id,
+    def _get_glucose_readings(
+        self, minutes: int = MAX_MINUTES, max_count: int = MAX_MAX_COUNT
+    ) -> List[Dict[str, Any]]:
+        """Retrieve glucose readings from the glucose readings endpoint
+        (`pydexcom.const.DEXCOM_GLUCOSE_READINGS_ENDPOINT`)."""
+        if not isinstance(minutes, int) or any([minutes < 0, minutes > MAX_MINUTES]):
+            raise ArgumentError(ArgumentErrorEnum.MINUTES_INVALID)
+        if not isinstance(max_count, int) or any(
+            [max_count < 0, max_count > MAX_MAX_COUNT]
+        ):
+            raise ArgumentError(ArgumentErrorEnum.MAX_COUNT_INVALID)
+
+        return self._post(
+            DEXCOM_GLUCOSE_READINGS_ENDPOINT,
+            params={
+                "sessionId": self._session_id,
                 "minutes": minutes,
                 "maxCount": max_count,
-            }
+            },
+        )
 
-            json_glucose_readings = self._request(
-                "post", DEXCOM_GLUCOSE_READINGS_ENDPOINT, params=params
-            )
+    def get_glucose_readings(
+        self, minutes: int = MAX_MINUTES, max_count: int = MAX_MAX_COUNT
+    ) -> List[GlucoseReading]:
+        """Get `max_count` glucose readings within specified number of `minutes`.
+
+        Catches one instance of a thrown `pydexcom.errors.SessionError` if session ID
+        expired, attempts to get a new session ID and retries.
+
+        :param minutes: Number of minutes to retrieve glucose readings from (1-1440)
+        :param max_count: Maximum number of glucose readings to retrieve (1-288)
+        """
+
+        json_glucose_readings: List[Dict[str, Any]] = []
+
+        try:
+            # Requesting glucose reading with DEFAULT_UUID returns non-JSON empty string
+            self._validate_session_id()
+
+            json_glucose_readings = self._get_glucose_readings(minutes, max_count)
+        except SessionError:
+            # Attempt to update expired session ID
+            self._session()
+
+            json_glucose_readings = self._get_glucose_readings(minutes, max_count)
 
-        glucose_readings = []
-        if not json_glucose_readings:
-            return None
-        for json_glucose_reading in json_glucose_readings:
-            glucose_readings.append(GlucoseReading(json_glucose_reading))
-        if not glucose_readings:
-            return None
-        return glucose_readings
+        return [GlucoseReading(json_reading) for json_reading in json_glucose_readings]
 
-    def get_latest_glucose_reading(self) -> GlucoseReading:
-        """Get latest available glucose reading."""
+    def get_latest_glucose_reading(self) -> Optional[GlucoseReading]:
+        """Get latest available glucose reading, within the last 24 hours."""
         glucose_readings = self.get_glucose_readings(max_count=1)
-        if not glucose_readings:
-            return None
-        return glucose_readings[0]
+        return glucose_readings[0] if glucose_readings else None
 
-    def get_current_glucose_reading(self) -> GlucoseReading:
-        """Get current available glucose reading."""
+    def get_current_glucose_reading(self) -> Optional[GlucoseReading]:
+        """Get current available glucose reading, within the last 10 minutes."""
         glucose_readings = self.get_glucose_readings(minutes=10, max_count=1)
-        if not glucose_readings:
-            return None
-        return glucose_readings[0]
+        return glucose_readings[0] if glucose_readings else None
```

