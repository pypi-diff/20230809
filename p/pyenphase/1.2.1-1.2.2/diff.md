# Comparing `tmp/pyenphase-1.2.1.tar.gz` & `tmp/pyenphase-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-1.2.1.tar", max compression
+gzip compressed data, was "pyenphase-1.2.2.tar", max compression
```

## Comparing `pyenphase-1.2.1.tar` & `pyenphase-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1067 2023-08-09 01:50:30.834357 pyenphase-1.2.1/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-09 01:50:30.834357 pyenphase-1.2.1/README.md
--rw-r--r--   0        0        0     2376 2023-08-09 01:50:31.734361 pyenphase-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1284 2023-08-09 01:50:31.702360 pyenphase-1.2.1/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     8363 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/auth.py
--rw-r--r--   0        0        0     1367 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/const.py
--rw-r--r--   0        0        0     7547 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1272 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     3279 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/firmware.py
--rw-r--r--   0        0        0      413 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/json.py
--rw-r--r--   0        0        0        0 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2469 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     2673 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     1846 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0     1250 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      873 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1436 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/py.typed
--rw-r--r--   0        0        0     1095 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/ssl.py
--rw-r--r--   0        0        0        0 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/updaters/__init__.py
--rw-r--r--   0        0        0     1451 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/updaters/api_v1_production.py
--rw-r--r--   0        0        0     1598 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/updaters/api_v1_production_inverters.py
--rw-r--r--   0        0        0     1583 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/updaters/base.py
--rw-r--r--   0        0        0     4504 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/updaters/ensemble.py
--rw-r--r--   0        0        0     3216 2023-08-09 01:50:30.834357 pyenphase-1.2.1/src/pyenphase/updaters/production.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-09 01:58:33.808632 pyenphase-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-09 01:58:33.808632 pyenphase-1.2.2/README.md
+-rw-r--r--   0        0        0     2376 2023-08-09 01:58:34.972724 pyenphase-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1284 2023-08-09 01:58:34.936721 pyenphase-1.2.2/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     8363 2023-08-09 01:58:33.808632 pyenphase-1.2.2/src/pyenphase/auth.py
+-rw-r--r--   0        0        0     1367 2023-08-09 01:58:33.808632 pyenphase-1.2.2/src/pyenphase/const.py
+-rw-r--r--   0        0        0     7547 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1272 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     3279 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0      413 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/json.py
+-rw-r--r--   0        0        0        0 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2469 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     2673 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     1846 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0     1250 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      873 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1436 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/py.typed
+-rw-r--r--   0        0        0     1095 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0        0 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/updaters/__init__.py
+-rw-r--r--   0        0        0     1451 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/updaters/api_v1_production.py
+-rw-r--r--   0        0        0     1456 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/updaters/api_v1_production_inverters.py
+-rw-r--r--   0        0        0     1583 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/updaters/base.py
+-rw-r--r--   0        0        0     4504 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/updaters/ensemble.py
+-rw-r--r--   0        0        0     3216 2023-08-09 01:58:33.812632 pyenphase-1.2.2/src/pyenphase/updaters/production.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.2.2/PKG-INFO
```

### Comparing `pyenphase-1.2.1/LICENSE` & `pyenphase-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/README.md` & `pyenphase-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/pyproject.toml` & `pyenphase-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "1.2.1"
+version = "1.2.2"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-1.2.1/src/pyenphase/__init__.py` & `pyenphase-1.2.2/src/pyenphase/__init__.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/auth.py` & `pyenphase-1.2.2/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/const.py` & `pyenphase-1.2.2/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/envoy.py` & `pyenphase-1.2.2/src/pyenphase/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/exceptions.py` & `pyenphase-1.2.2/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/firmware.py` & `pyenphase-1.2.2/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/models/dry_contacts.py` & `pyenphase-1.2.2/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/models/encharge.py` & `pyenphase-1.2.2/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/models/enpower.py` & `pyenphase-1.2.2/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/models/envoy.py` & `pyenphase-1.2.2/src/pyenphase/models/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/models/inverter.py` & `pyenphase-1.2.2/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/models/system_consumption.py` & `pyenphase-1.2.2/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/models/system_production.py` & `pyenphase-1.2.2/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/ssl.py` & `pyenphase-1.2.2/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/updaters/api_v1_production.py` & `pyenphase-1.2.2/src/pyenphase/updaters/api_v1_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/updaters/api_v1_production_inverters.py` & `pyenphase-1.2.2/src/pyenphase/updaters/api_v1_production_inverters.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 class EnvoyApiV1ProductionInvertersUpdater(EnvoyUpdater):
     """Class to handle updates for inverter production data."""
 
     async def probe(
         self, discovered_features: SupportedFeatures
     ) -> SupportedFeatures | None:
         """Probe the Envoy for this updater and return SupportedFeatures."""
-        if SupportedFeatures.INVERTERS in discovered_features:
-            # Already discovered from another updater
-            return None
-
         try:
             await self._json_probe_request(URL_PRODUCTION_INVERTERS)
         except ENDPOINT_PROBE_EXCEPTIONS as e:
             _LOGGER.debug(
                 "Production endpoint not found at %s: %s", URL_PRODUCTION_INVERTERS, e
             )
             return None
```

### Comparing `pyenphase-1.2.1/src/pyenphase/updaters/base.py` & `pyenphase-1.2.2/src/pyenphase/updaters/base.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/updaters/ensemble.py` & `pyenphase-1.2.2/src/pyenphase/updaters/ensemble.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/src/pyenphase/updaters/production.py` & `pyenphase-1.2.2/src/pyenphase/updaters/production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.2.1/PKG-INFO` & `pyenphase-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 1.2.1
+Version: 1.2.2
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
-Metadata-Version: 2.1 Name: pyenphase Version: 1.2.1 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 1.2.2 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

