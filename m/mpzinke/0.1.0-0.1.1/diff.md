# Comparing `tmp/mpzinke-0.1.0.tar.gz` & `tmp/mpzinke-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpzinke-0.1.0.tar", last modified: Tue Aug  8 23:45:45 2023, max compression
+gzip compressed data, was "mpzinke-0.1.1.tar", last modified: Wed Aug  9 00:42:38 2023, max compression
```

## Comparing `mpzinke-0.1.0.tar` & `mpzinke-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:45:45.319257 mpzinke-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 23:45:08.000000 mpzinke-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-08 23:45:45.315257 mpzinke-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-08 23:45:08.000000 mpzinke-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-08 23:45:38.000000 mpzinke-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:45:45.319257 mpzinke-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:45:45.315257 mpzinke-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:45:45.315257 mpzinke-0.1.0/src/mpzinke/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:45:45.315257 mpzinke-0.1.0/src/mpzinke/Generic/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/Generic/Generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/Generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/Generic/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:45:45.315257 mpzinke-0.1.0/src/mpzinke/Server/
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/Server/Route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/Server/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/Server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:45:45.315257 mpzinke-0.1.0/src/mpzinke/threading/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/threading/BaseThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/threading/DelayThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/threading/LoopingThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-08 23:45:08.000000 mpzinke-0.1.0/src/mpzinke/threading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:45:45.315257 mpzinke-0.1.0/src/mpzinke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-08 23:45:45.000000 mpzinke-0.1.0/src/mpzinke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-08 23:45:45.000000 mpzinke-0.1.0/src/mpzinke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:45:45.000000 mpzinke-0.1.0/src/mpzinke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 23:45:45.000000 mpzinke-0.1.0/src/mpzinke.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:42:38.256028 mpzinke-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-09 00:41:55.000000 mpzinke-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-09 00:42:38.256028 mpzinke-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-09 00:41:55.000000 mpzinke-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-09 00:42:30.000000 mpzinke-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 00:42:38.256028 mpzinke-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:42:38.252028 mpzinke-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:42:38.256028 mpzinke-0.1.1/src/mpzinke/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:42:38.256028 mpzinke-0.1.1/src/mpzinke/Generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/Generic/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/Generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/Generic/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:42:38.256028 mpzinke-0.1.1/src/mpzinke/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/Server/Route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/Server/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/Server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:42:38.256028 mpzinke-0.1.1/src/mpzinke/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/threading/BaseThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/threading/DelayThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/threading/LoopingThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-09 00:41:55.000000 mpzinke-0.1.1/src/mpzinke/threading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:42:38.256028 mpzinke-0.1.1/src/mpzinke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-09 00:42:38.000000 mpzinke-0.1.1/src/mpzinke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-09 00:42:38.000000 mpzinke-0.1.1/src/mpzinke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:42:38.000000 mpzinke-0.1.1/src/mpzinke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-09 00:42:38.000000 mpzinke-0.1.1/src/mpzinke.egg-info/top_level.txt
```

### Comparing `mpzinke-0.1.0/LICENSE` & `mpzinke-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/PKG-INFO` & `mpzinke-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpzinke
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python libraries for MPZinke.
 Author: Mathew Zinke
 Project-URL: Homepage, https://github.com/MPZinke/Python
 Project-URL: Bug Tracker, https://github.com/MPZinke/Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mpzinke-0.1.0/pyproject.toml` & `mpzinke-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "Flask>=2.1.3", "Flask-Cors>=3.0.10"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mpzinke"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name="Mathew Zinke"}]
 description = "Python libraries for MPZinke."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `mpzinke-0.1.0/src/mpzinke/Generic/__init__.py` & `mpzinke-0.1.1/src/mpzinke/Generic/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke/Generic/__main__.py` & `mpzinke-0.1.1/src/mpzinke/Generic/__main__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke/Server/Route.py` & `mpzinke-0.1.1/src/mpzinke/Server/Route.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke/Server/Server.py` & `mpzinke-0.1.1/src/mpzinke/Server/Server.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 	Methods:
 		- __init__:
 	"""
 	EXCEPTIONS = {401: Unauthorized, 403: Forbidden}
 
 
 	def __init__(self, *, authorization: Optional[callable]=None, handle_error: Optional[callable]=None,
-	  host: str="0.0.0.0", name: str="Flask App", port: int=8080, version: str="1.0.0"
+	  host: str="0.0.0.0", name: str="Flask App", port: int=8080, version: str="1.0.0", **kwargs: dict
 	):
-		self._app = Flask(name)
+		self._app = Flask(name, **kwargs)
 
 		self._cors = CORS(self._app)
 		self._app.config['CORS_HEADERS'] = 'Content-Type'
 		self._app.register_error_handler(Exception, self._handle_error)
 		self._app.after_request(self._after_request)
 
 		self._authorization: callable = authorization
```

### Comparing `mpzinke-0.1.0/src/mpzinke/Server/__init__.py` & `mpzinke-0.1.1/src/mpzinke/Server/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke/__init__.py` & `mpzinke-0.1.1/src/mpzinke/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke/threading/BaseThread.py` & `mpzinke-0.1.1/src/mpzinke/threading/BaseThread.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke/threading/DelayThread.py` & `mpzinke-0.1.1/src/mpzinke/threading/DelayThread.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke/threading/LoopingThread.py` & `mpzinke-0.1.1/src/mpzinke/threading/LoopingThread.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke/threading/__init__.py` & `mpzinke-0.1.1/src/mpzinke/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.0/src/mpzinke.egg-info/PKG-INFO` & `mpzinke-0.1.1/src/mpzinke.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpzinke
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python libraries for MPZinke.
 Author: Mathew Zinke
 Project-URL: Homepage, https://github.com/MPZinke/Python
 Project-URL: Bug Tracker, https://github.com/MPZinke/Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mpzinke-0.1.0/src/mpzinke.egg-info/SOURCES.txt` & `mpzinke-0.1.1/src/mpzinke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

