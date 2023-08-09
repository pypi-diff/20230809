# Comparing `tmp/pyenphase-1.1.4.tar.gz` & `tmp/pyenphase-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-1.1.4.tar", max compression
+gzip compressed data, was "pyenphase-1.2.0.tar", max compression
```

## Comparing `pyenphase-1.1.4.tar` & `pyenphase-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
--rw-r--r--   0        0        0     1067 2023-08-08 23:54:47.042256 pyenphase-1.1.4/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-08 23:54:47.042256 pyenphase-1.1.4/README.md
--rw-r--r--   0        0        0     2376 2023-08-08 23:54:48.062266 pyenphase-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1242 2023-08-08 23:54:48.030266 pyenphase-1.1.4/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     8363 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/auth.py
--rw-r--r--   0        0        0      976 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/const.py
--rw-r--r--   0        0        0    16186 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1272 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     3279 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/firmware.py
--rw-r--r--   0        0        0        0 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2469 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     2673 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     1846 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0     1086 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      873 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1436 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/py.typed
--rw-r--r--   0        0        0     1095 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-09 00:57:29.169963 pyenphase-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-09 00:57:29.169963 pyenphase-1.2.0/README.md
+-rw-r--r--   0        0        0     2376 2023-08-09 00:57:30.210017 pyenphase-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1284 2023-08-09 00:57:30.170015 pyenphase-1.2.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     8363 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0     1367 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0     7547 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1272 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     3279 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0      413 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/json.py
+-rw-r--r--   0        0        0        0 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2469 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     2673 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     1846 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0     1250 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      873 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1436 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0     1095 2023-08-09 00:57:29.169963 pyenphase-1.2.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0        0 2023-08-09 00:57:29.173963 pyenphase-1.2.0/src/pyenphase/updaters/__init__.py
+-rw-r--r--   0        0        0     1451 2023-08-09 00:57:29.173963 pyenphase-1.2.0/src/pyenphase/updaters/api_v1_production.py
+-rw-r--r--   0        0        0     1598 2023-08-09 00:57:29.173963 pyenphase-1.2.0/src/pyenphase/updaters/api_v1_production_inverters.py
+-rw-r--r--   0        0        0     1583 2023-08-09 00:57:29.173963 pyenphase-1.2.0/src/pyenphase/updaters/base.py
+-rw-r--r--   0        0        0     4504 2023-08-09 00:57:29.173963 pyenphase-1.2.0/src/pyenphase/updaters/ensemble.py
+-rw-r--r--   0        0        0     3216 2023-08-09 00:57:29.173963 pyenphase-1.2.0/src/pyenphase/updaters/production.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.2.0/PKG-INFO
```

### Comparing `pyenphase-1.1.4/LICENSE` & `pyenphase-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/README.md` & `pyenphase-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/pyproject.toml` & `pyenphase-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "1.1.4"
+version = "1.2.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-1.1.4/src/pyenphase/__init__.py` & `pyenphase-1.2.0/src/pyenphase/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Python wrapper for Enphase Envoy API."""
 
 from .auth import EnvoyTokenAuth
-from .envoy import AUTH_TOKEN_MIN_VERSION, Envoy
+from .envoy import AUTH_TOKEN_MIN_VERSION, Envoy, register_updater
 from .exceptions import (
     EnvoyAuthenticationError,
     EnvoyAuthenticationRequired,
     EnvoyCommunicationError,
     EnvoyError,
     EnvoyFirmwareCheckError,
     EnvoyFirmwareFatalCheckError,
@@ -17,14 +17,15 @@
 from .models.envoy import EnvoyData
 from .models.inverter import EnvoyInverter
 from .models.system_consumption import EnvoySystemConsumption
 from .models.system_production import EnvoySystemProduction
 
 __all__ = (
     AUTH_TOKEN_MIN_VERSION,
+    "register_updater",
     "Envoy",
     "EnvoyData",
     "EnvoyTokenAuth",
     "EnvoyError",
     "EnvoyCommunicationError",
     "EnvoyFirmwareCheckError",
     "EnvoyFirmwareFatalCheckError",
```

### Comparing `pyenphase-1.1.4/src/pyenphase/auth.py` & `pyenphase-1.2.0/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/const.py` & `pyenphase-1.2.0/src/pyenphase/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,16 @@
+import enum
+
 import httpx
+from awesomeversion import AwesomeVersion
+
+# Versions
+LEGACY_ENVOY_VERSION = AwesomeVersion("3.9.0")
+ENSEMBLE_MIN_VERSION = AwesomeVersion("5.0.0")
+AUTH_TOKEN_MIN_VERSION = AwesomeVersion("7.0.0")
 
 # System Production
 URL_PRODUCTION_INVERTERS = "/api/v1/production/inverters"
 URL_PRODUCTION_V1 = "/api/v1/production"
 URL_PRODUCTION_JSON = "/production.json"
 URL_PRODUCTION = "/production"
 
@@ -27,7 +35,17 @@
 LOCAL_TIMEOUT = httpx.Timeout(
     # The envoy can be slow to respond but fast to connect to we
     # need to set a long timeout for the read and a short timeout
     # for the connect
     timeout=10.0,
     read=60.0,
 )
+
+
+class SupportedFeatures(enum.IntFlag):
+    INVERTERS = 1
+    METERING = 2
+    TOTAL_CONSUMPTION = 4
+    NET_CONSUMPTION = 8
+    ENCHARGE = 16
+    ENPOWER = 32
+    PRODUCTION = 64
```

### Comparing `pyenphase-1.1.4/src/pyenphase/exceptions.py` & `pyenphase-1.2.0/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/firmware.py` & `pyenphase-1.2.0/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/models/dry_contacts.py` & `pyenphase-1.2.0/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/models/encharge.py` & `pyenphase-1.2.0/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/models/enpower.py` & `pyenphase-1.2.0/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/models/envoy.py` & `pyenphase-1.2.0/src/pyenphase/models/envoy.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,8 +21,11 @@
     system_consumption: EnvoySystemConsumption | None = None
     system_production: EnvoySystemProduction | None = None
     dry_contact_status: dict[str, EnvoyDryContactStatus] = field(default_factory=dict)
     dry_contact_settings: dict[str, EnvoyDryContactSettings] = field(
         default_factory=dict
     )
     inverters: dict[str, EnvoyInverter] = field(default_factory=dict)
-    raw: dict[str, dict[str, Any]] = field(default_factory=dict)
+    # Raw data is exposed so we can __eq__ the data to see if
+    # anything has changed and consumers of the library can
+    # avoid dispatching data if nothing has changed.
+    raw: dict[str, Any] = field(default_factory=dict)
```

### Comparing `pyenphase-1.1.4/src/pyenphase/models/inverter.py` & `pyenphase-1.2.0/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/models/system_consumption.py` & `pyenphase-1.2.0/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/models/system_production.py` & `pyenphase-1.2.0/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/src/pyenphase/ssl.py` & `pyenphase-1.2.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.4/PKG-INFO` & `pyenphase-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 1.1.4
+Version: 1.2.0
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 1.1.4 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 1.2.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

