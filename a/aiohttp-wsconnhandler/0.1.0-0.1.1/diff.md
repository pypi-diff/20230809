# Comparing `tmp/aiohttp-wsconnhandler-0.1.0.tar.gz` & `tmp/aiohttp-wsconnhandler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp-wsconnhandler-0.1.0.tar", last modified: Wed Aug  9 02:35:43 2023, max compression
+gzip compressed data, was "aiohttp-wsconnhandler-0.1.1.tar", last modified: Wed Aug  9 04:21:47 2023, max compression
```

## Comparing `aiohttp-wsconnhandler-0.1.0.tar` & `aiohttp-wsconnhandler-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 02:35:43.169915 aiohttp-wsconnhandler-0.1.0/
--rw-r--r--   0 deuser    (1000) deuser    (1000)     1107 2023-08-09 00:32:32.000000 aiohttp-wsconnhandler-0.1.0/LICENSE
--rw-r--r--   0 deuser    (1000) deuser    (1000)     1240 2023-08-09 02:35:43.169915 aiohttp-wsconnhandler-0.1.0/PKG-INFO
--rw-r--r--   0 deuser    (1000) deuser    (1000)      627 2023-08-09 00:48:17.000000 aiohttp-wsconnhandler-0.1.0/README.md
--rw-r--r--   0 deuser    (1000) deuser    (1000)      720 2023-08-09 00:32:18.000000 aiohttp-wsconnhandler-0.1.0/pyproject.toml
--rw-r--r--   0 deuser    (1000) deuser    (1000)       38 2023-08-09 02:35:43.169915 aiohttp-wsconnhandler-0.1.0/setup.cfg
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 02:35:43.169915 aiohttp-wsconnhandler-0.1.0/src/
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 02:35:43.169915 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler/
--rw-r--r--   0 deuser    (1000) deuser    (1000)       55 2023-08-09 00:24:58.000000 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler/__init__.py
--rw-r--r--   0 deuser    (1000) deuser    (1000)     8756 2023-08-09 00:20:44.000000 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler/ws_connection_handler.py
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 02:35:43.169915 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler.egg-info/
--rw-r--r--   0 deuser    (1000) deuser    (1000)     1240 2023-08-09 02:35:43.000000 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler.egg-info/PKG-INFO
--rw-r--r--   0 deuser    (1000) deuser    (1000)      365 2023-08-09 02:35:43.000000 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler.egg-info/SOURCES.txt
--rw-r--r--   0 deuser    (1000) deuser    (1000)        1 2023-08-09 02:35:43.000000 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler.egg-info/dependency_links.txt
--rw-r--r--   0 deuser    (1000) deuser    (1000)        8 2023-08-09 02:35:43.000000 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler.egg-info/requires.txt
--rw-r--r--   0 deuser    (1000) deuser    (1000)       22 2023-08-09 02:35:43.000000 aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler.egg-info/top_level.txt
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:21:47.653217 aiohttp-wsconnhandler-0.1.1/
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     1107 2023-08-09 00:32:32.000000 aiohttp-wsconnhandler-0.1.1/LICENSE
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     1317 2023-08-09 04:21:47.653217 aiohttp-wsconnhandler-0.1.1/PKG-INFO
+-rw-r--r--   0 deuser    (1000) deuser    (1000)      627 2023-08-09 00:48:17.000000 aiohttp-wsconnhandler-0.1.1/README.md
+-rw-r--r--   0 deuser    (1000) deuser    (1000)      787 2023-08-09 03:31:01.000000 aiohttp-wsconnhandler-0.1.1/pyproject.toml
+-rw-r--r--   0 deuser    (1000) deuser    (1000)       38 2023-08-09 04:21:47.653217 aiohttp-wsconnhandler-0.1.1/setup.cfg
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:21:47.649217 aiohttp-wsconnhandler-0.1.1/src/
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:21:47.653217 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler/
+-rw-r--r--   0 deuser    (1000) deuser    (1000)       55 2023-08-09 00:24:58.000000 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler/__init__.py
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     8756 2023-08-09 00:20:44.000000 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler/ws_connection_handler.py
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:21:47.653217 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler.egg-info/
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     1317 2023-08-09 04:21:47.000000 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler.egg-info/PKG-INFO
+-rw-r--r--   0 deuser    (1000) deuser    (1000)      365 2023-08-09 04:21:47.000000 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 deuser    (1000) deuser    (1000)        1 2023-08-09 04:21:47.000000 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 deuser    (1000) deuser    (1000)        8 2023-08-09 04:21:47.000000 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler.egg-info/requires.txt
+-rw-r--r--   0 deuser    (1000) deuser    (1000)       22 2023-08-09 04:21:47.000000 aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler.egg-info/top_level.txt
```

### Comparing `aiohttp-wsconnhandler-0.1.0/LICENSE` & `aiohttp-wsconnhandler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp-wsconnhandler-0.1.0/PKG-INFO` & `aiohttp-wsconnhandler-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: aiohttp-wsconnhandler
-Version: 0.1.0
+Version: 0.1.1
 Summary: A class that provides receive and send queues when handling WebSocket communication with aiohttp.
 Author-email: darkhaniop <darkhaniop@google.com>
 Project-URL: Homepage, https://github.com/gw-tools/aiohttp-wsconnhandler
 Project-URL: Bug Tracker, https://github.com/gw-tools/aiohttp-wsconnhandler/issues
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: aiohttp
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiohttp-wsconnhandler
 
 The package implements the `WSConnectionHandler` class that provides receive and send queues when handling WebSocket communication with aiohttp.
```

### Comparing `aiohttp-wsconnhandler-0.1.0/README.md` & `aiohttp-wsconnhandler-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp-wsconnhandler-0.1.0/pyproject.toml` & `aiohttp-wsconnhandler-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiohttp-wsconnhandler"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="darkhaniop", email="darkhaniop@google.com" },
 ]
 description = "A class that provides receive and send queues when handling WebSocket communication with aiohttp."
 readme = "README.md"
 requires-python = ">=3.7, <4"
 classifiers = [
+    "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Framework :: aiohttp",
 ]
 
 dependencies = [
   "aiohttp",
 ]
 
 [project.urls]
```

### Comparing `aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler/ws_connection_handler.py` & `aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler/ws_connection_handler.py`

 * *Files identical despite different names*

### Comparing `aiohttp-wsconnhandler-0.1.0/src/aiohttp_wsconnhandler.egg-info/PKG-INFO` & `aiohttp-wsconnhandler-0.1.1/src/aiohttp_wsconnhandler.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: aiohttp-wsconnhandler
-Version: 0.1.0
+Version: 0.1.1
 Summary: A class that provides receive and send queues when handling WebSocket communication with aiohttp.
 Author-email: darkhaniop <darkhaniop@google.com>
 Project-URL: Homepage, https://github.com/gw-tools/aiohttp-wsconnhandler
 Project-URL: Bug Tracker, https://github.com/gw-tools/aiohttp-wsconnhandler/issues
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: aiohttp
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiohttp-wsconnhandler
 
 The package implements the `WSConnectionHandler` class that provides receive and send queues when handling WebSocket communication with aiohttp.
```

