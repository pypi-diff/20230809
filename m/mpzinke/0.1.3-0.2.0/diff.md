# Comparing `tmp/mpzinke-0.1.3.tar.gz` & `tmp/mpzinke-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpzinke-0.1.3.tar", last modified: Wed Aug  9 00:59:52 2023, max compression
+gzip compressed data, was "mpzinke-0.2.0.tar", last modified: Wed Aug  9 01:31:52 2023, max compression
```

## Comparing `mpzinke-0.1.3.tar` & `mpzinke-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:59:52.380952 mpzinke-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-09 00:59:03.000000 mpzinke-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-09 00:59:52.380952 mpzinke-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-09 00:59:03.000000 mpzinke-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-09 00:59:42.000000 mpzinke-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 00:59:52.380952 mpzinke-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:59:52.376952 mpzinke-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:59:52.380952 mpzinke-0.1.3/src/mpzinke/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:59:52.380952 mpzinke-0.1.3/src/mpzinke/Generic/
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/Generic/Generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/Generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/Generic/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:59:52.380952 mpzinke-0.1.3/src/mpzinke/Server/
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/Server/Route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/Server/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/Server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:59:52.380952 mpzinke-0.1.3/src/mpzinke/threading/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/threading/BaseThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/threading/DelayThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/threading/LoopingThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-09 00:59:03.000000 mpzinke-0.1.3/src/mpzinke/threading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:59:52.380952 mpzinke-0.1.3/src/mpzinke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-09 00:59:52.000000 mpzinke-0.1.3/src/mpzinke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-09 00:59:52.000000 mpzinke-0.1.3/src/mpzinke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:59:52.000000 mpzinke-0.1.3/src/mpzinke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-09 00:59:52.000000 mpzinke-0.1.3/src/mpzinke.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:31:52.353932 mpzinke-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-09 01:31:16.000000 mpzinke-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-09 01:31:52.353932 mpzinke-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-09 01:31:16.000000 mpzinke-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-09 01:31:45.000000 mpzinke-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:31:52.353932 mpzinke-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:31:52.349932 mpzinke-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:31:52.349932 mpzinke-0.2.0/src/mpzinke/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:31:52.349932 mpzinke-0.2.0/src/mpzinke/Generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/Generic/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/Generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/Generic/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:31:52.349932 mpzinke-0.2.0/src/mpzinke/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/Server/Route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/Server/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/Server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:31:52.353932 mpzinke-0.2.0/src/mpzinke/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/threading/BaseThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/threading/DelayThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/threading/LoopingThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-09 01:31:16.000000 mpzinke-0.2.0/src/mpzinke/threading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:31:52.349932 mpzinke-0.2.0/src/mpzinke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-09 01:31:52.000000 mpzinke-0.2.0/src/mpzinke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-09 01:31:52.000000 mpzinke-0.2.0/src/mpzinke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:31:52.000000 mpzinke-0.2.0/src/mpzinke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-09 01:31:52.000000 mpzinke-0.2.0/src/mpzinke.egg-info/top_level.txt
```

### Comparing `mpzinke-0.1.3/LICENSE` & `mpzinke-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/PKG-INFO` & `mpzinke-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpzinke
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python libraries for MPZinke.
 Author: Mathew Zinke
 Project-URL: Homepage, https://github.com/MPZinke/Python
 Project-URL: Bug Tracker, https://github.com/MPZinke/Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mpzinke-0.1.3/pyproject.toml` & `mpzinke-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "Flask>=2.1.3", "Flask-Cors>=3.0.10"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mpzinke"
-version = "0.1.3"
+version = "0.2.0"
 authors = [{name="Mathew Zinke"}]
 description = "Python libraries for MPZinke."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `mpzinke-0.1.3/src/mpzinke/Generic/Generic.py` & `mpzinke-0.2.0/src/mpzinke/Generic/Generic.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke/Generic/__init__.py` & `mpzinke-0.2.0/src/mpzinke/Generic/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke/Generic/__main__.py` & `mpzinke-0.2.0/src/mpzinke/Generic/__main__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke/Server/Route.py` & `mpzinke-0.2.0/src/mpzinke/Server/Route.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 		for type, value in self._additional_args.items():
 			if(type in (params := self._methods[request.method].__annotations__).values()):
 				kwargs[list(params.keys())[list(params.values()).index(type)]] = value
 
 		return self._methods[request.method](**kwargs)
 
 
+	def __iter__(self) -> Dict[str, str]:
+		yield from {f"{method} {self._url}": callback.__doc__ for method, callback in self._methods.items()}.items()
+
+
 	# ————————————————————————————————————————— ROUTES::CALLBACK  VALIDATION ————————————————————————————————————————— #
 
 	@staticmethod
 	def compare_function_params(func1: Dict[str, type], func2: Dict[str, type]) -> Dict[str, type]:
 		"""
 		SUMMARY: Compares the args and types of two functions.
 		PARAMS:  Takes the args and types of function 1 and the args and types of function 2.
```

### Comparing `mpzinke-0.1.3/src/mpzinke/Server/Server.py` & `mpzinke-0.2.0/src/mpzinke/Server/Server.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 		"""
 		SUMMARY: Adds routes to server & class, and starts the server instance.
 		DETAILS: Sets routes using hardcoded routes, functions & HTTP request methods. Calls the Flask::run method.
 		"""
 		self._app.run(host=self._host, port=self._port)
 
 
+	def __iter__(self) -> list[str]:
+		yield from {endpoint: doc_string for route in self._routes for endpoint, doc_string in dict(route).items()}.items()
+
+
 	# ——————————————————————————————————————————————— REQUEST HANDLING ——————————————————————————————————————————————— #
 
 	def _after_request(self, response):
 		"""
 		FROM: https://stackoverflow.com/a/30717205
 		"""
 		response.headers["Version"] = self._version
@@ -98,14 +102,18 @@
 		return jsonify(error=str(error), traceback=exception_traceback), 500
 
 
 	# ————————————————————————————————————————————————————— AUTH ————————————————————————————————————————————————————— #
 
 	@staticmethod
 	def bearer_auth(*authorization_args: list) -> callable:
+		"""
+		SUMMARY: Function used for no authorization. Can be called statically or dynamically.
+		PARAMS:  Takes either the bearer token or the object calling it and the bearer token.
+		"""
 		use_message = "Use either statically with `Server.bearer_auth(auth: str)`" \
 		  + " or dynamically with `<server_object>.bearer_auth(auth: str)`"
 		if(len(authorization_args) == 0):
 			raise TypeError(f"An authorization string must be passed to `bearer_auth`\n{use_message}")
 
 		if(len(authorization_args) > 2):
 			raise TypeError(f"Too many arguments passed\n{use_message}")
@@ -130,14 +138,17 @@
 				raise Forbidden()
 
 		return check_auth
 
 
 	@staticmethod
 	def no_auth(*_: list) -> True:
+		"""
+		Function used for no authorization. Can be called statically or dynamically.
+		"""
 		return True
 
 
 	# ———————————————————————————————————————————————————— ROUTES ———————————————————————————————————————————————————— #
 	# ———————————————————————————————————————————————————————————————————————————————————————————————————————————————— #
 
 	def route(self, url: URL, GET: callable=None, *, additional_args: Dict[type, any]=None,
```

### Comparing `mpzinke-0.1.3/src/mpzinke/Server/__init__.py` & `mpzinke-0.2.0/src/mpzinke/Server/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke/__init__.py` & `mpzinke-0.2.0/src/mpzinke/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke/threading/BaseThread.py` & `mpzinke-0.2.0/src/mpzinke/threading/BaseThread.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke/threading/DelayThread.py` & `mpzinke-0.2.0/src/mpzinke/threading/DelayThread.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke/threading/LoopingThread.py` & `mpzinke-0.2.0/src/mpzinke/threading/LoopingThread.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke/threading/__init__.py` & `mpzinke-0.2.0/src/mpzinke/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.1.3/src/mpzinke.egg-info/PKG-INFO` & `mpzinke-0.2.0/src/mpzinke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpzinke
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python libraries for MPZinke.
 Author: Mathew Zinke
 Project-URL: Homepage, https://github.com/MPZinke/Python
 Project-URL: Bug Tracker, https://github.com/MPZinke/Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mpzinke-0.1.3/src/mpzinke.egg-info/SOURCES.txt` & `mpzinke-0.2.0/src/mpzinke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

