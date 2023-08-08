# Comparing `tmp/WormholeSort-1.0.0.tar.gz` & `tmp/WormholeSort-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WormholeSort-1.0.0.tar", last modified: Tue Aug  8 22:27:14 2023, max compression
+gzip compressed data, was "WormholeSort-1.0.1.tar", last modified: Tue Aug  8 22:34:36 2023, max compression
```

## Comparing `WormholeSort-1.0.0.tar` & `WormholeSort-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 22:27:14.000317 WormholeSort-1.0.0/
--rw-rw-rw-   0        0        0     1640 2023-08-08 22:27:13.998984 WormholeSort-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-08-08 22:20:11.000000 WormholeSort-1.0.0/README.md
--rw-rw-rw-   0        0        0      662 2023-08-08 22:24:37.000000 WormholeSort-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-08 22:27:14.000372 WormholeSort-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-08 22:27:13.993371 WormholeSort-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-08 22:27:13.998323 WormholeSort-1.0.0/src/WormholeSort.egg-info/
--rw-rw-rw-   0        0        0     1640 2023-08-08 22:27:13.000000 WormholeSort-1.0.0/src/WormholeSort.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-08-08 22:27:13.000000 WormholeSort-1.0.0/src/WormholeSort.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 22:27:13.000000 WormholeSort-1.0.0/src/WormholeSort.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-08-08 22:27:13.000000 WormholeSort-1.0.0/src/WormholeSort.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-08-08 22:08:26.000000 WormholeSort-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     1150 2023-08-08 22:05:58.000000 WormholeSort-1.0.0/src/wormholeSort.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:34:36.855970 WormholeSort-1.0.1/
+-rw-rw-rw-   0        0        0     1640 2023-08-08 22:34:36.854966 WormholeSort-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2023-08-08 22:20:11.000000 WormholeSort-1.0.1/README.md
+-rw-rw-rw-   0        0        0      662 2023-08-08 22:34:17.000000 WormholeSort-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 22:34:36.855970 WormholeSort-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 22:34:36.849950 WormholeSort-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 22:34:36.854966 WormholeSort-1.0.1/src/WormholeSort.egg-info/
+-rw-rw-rw-   0        0        0     1640 2023-08-08 22:34:36.000000 WormholeSort-1.0.1/src/WormholeSort.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-08-08 22:34:36.000000 WormholeSort-1.0.1/src/WormholeSort.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 22:34:36.000000 WormholeSort-1.0.1/src/WormholeSort.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-08-08 22:34:36.000000 WormholeSort-1.0.1/src/WormholeSort.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1150 2023-08-08 22:05:58.000000 WormholeSort-1.0.1/src/WormholeSort.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 22:08:26.000000 WormholeSort-1.0.1/src/__init__.py
```

### Comparing `WormholeSort-1.0.0/PKG-INFO` & `WormholeSort-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WormholeSort
-Version: 1.0.0
+Version: 1.0.1
 Summary: An alternative sorting method that sorts the indices rather than list elements.
 Author-email: arda-guler <ardaguler09@gmail.com>
 Project-URL: Homepage, https://github.com/arda-guler/WormholeSort
 Project-URL: Bug Tracker, https://github.com/arda-guler/WormholeSort/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `WormholeSort-1.0.0/README.md` & `WormholeSort-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `WormholeSort-1.0.0/pyproject.toml` & `WormholeSort-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WormholeSort"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="arda-guler", email="ardaguler09@gmail.com" },
 ]
 description = "An alternative sorting method that sorts the indices rather than list elements."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `WormholeSort-1.0.0/src/WormholeSort.egg-info/PKG-INFO` & `WormholeSort-1.0.1/src/WormholeSort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WormholeSort
-Version: 1.0.0
+Version: 1.0.1
 Summary: An alternative sorting method that sorts the indices rather than list elements.
 Author-email: arda-guler <ardaguler09@gmail.com>
 Project-URL: Homepage, https://github.com/arda-guler/WormholeSort
 Project-URL: Bug Tracker, https://github.com/arda-guler/WormholeSort/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `WormholeSort-1.0.0/src/wormholeSort.py` & `WormholeSort-1.0.1/src/WormholeSort.py`

 * *Files identical despite different names*

