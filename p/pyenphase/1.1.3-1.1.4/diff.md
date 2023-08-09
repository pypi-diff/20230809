# Comparing `tmp/pyenphase-1.1.3.tar.gz` & `tmp/pyenphase-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-1.1.3.tar", max compression
+gzip compressed data, was "pyenphase-1.1.4.tar", max compression
```

## Comparing `pyenphase-1.1.3.tar` & `pyenphase-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-08-08 21:28:43.047738 pyenphase-1.1.3/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-08 21:28:43.047738 pyenphase-1.1.3/README.md
--rw-r--r--   0        0        0     2376 2023-08-08 21:28:44.007747 pyenphase-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1242 2023-08-08 21:28:43.975746 pyenphase-1.1.3/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     8363 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/auth.py
--rw-r--r--   0        0        0      976 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/const.py
--rw-r--r--   0        0        0    16186 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1272 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     3279 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/firmware.py
--rw-r--r--   0        0        0        0 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2451 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     2673 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     1846 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0     1086 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      873 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1436 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/py.typed
--rw-r--r--   0        0        0     1095 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-08 23:54:47.042256 pyenphase-1.1.4/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-08 23:54:47.042256 pyenphase-1.1.4/README.md
+-rw-r--r--   0        0        0     2376 2023-08-08 23:54:48.062266 pyenphase-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1242 2023-08-08 23:54:48.030266 pyenphase-1.1.4/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     8363 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      976 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/const.py
+-rw-r--r--   0        0        0    16186 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1272 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     3279 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0        0 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2469 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     2673 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     1846 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0     1086 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      873 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1436 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/py.typed
+-rw-r--r--   0        0        0     1095 2023-08-08 23:54:47.046256 pyenphase-1.1.4/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.1.4/PKG-INFO
```

### Comparing `pyenphase-1.1.3/LICENSE` & `pyenphase-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/README.md` & `pyenphase-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/pyproject.toml` & `pyenphase-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "1.1.3"
+version = "1.1.4"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-1.1.3/src/pyenphase/__init__.py` & `pyenphase-1.1.4/src/pyenphase/__init__.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/auth.py` & `pyenphase-1.1.4/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/const.py` & `pyenphase-1.1.4/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/envoy.py` & `pyenphase-1.1.4/src/pyenphase/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/exceptions.py` & `pyenphase-1.1.4/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/firmware.py` & `pyenphase-1.1.4/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/models/dry_contacts.py` & `pyenphase-1.1.4/src/pyenphase/models/dry_contacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     status: str
 
     @classmethod
     def from_api(cls, relay: dict[str, Any]) -> EnvoyDryContactStatus:
         """Initialize from the API."""
         return cls(
             id=relay["id"],
-            status=relay["status"],
+            status=DryContactStatus(relay["status"]),
         )
 
 
 @dataclass(slots=True)
 class EnvoyDryContactSettings:
     """Model for the Enpower dry contact relay settings."""
```

### Comparing `pyenphase-1.1.3/src/pyenphase/models/encharge.py` & `pyenphase-1.1.4/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/models/enpower.py` & `pyenphase-1.1.4/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/models/envoy.py` & `pyenphase-1.1.4/src/pyenphase/models/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/models/inverter.py` & `pyenphase-1.1.4/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/models/system_consumption.py` & `pyenphase-1.1.4/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/models/system_production.py` & `pyenphase-1.1.4/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/src/pyenphase/ssl.py` & `pyenphase-1.1.4/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.3/PKG-INFO` & `pyenphase-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 1.1.3
+Version: 1.1.4
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
-Metadata-Version: 2.1 Name: pyenphase Version: 1.1.3 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 1.1.4 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

