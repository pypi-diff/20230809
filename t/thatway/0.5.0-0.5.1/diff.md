# Comparing `tmp/thatway-0.5.0.tar.gz` & `tmp/thatway-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thatway-0.5.0.tar", last modified: Tue Aug  8 18:26:10 2023, max compression
+gzip compressed data, was "thatway-0.5.1.tar", last modified: Tue Aug  8 18:35:28 2023, max compression
```

## Comparing `thatway-0.5.0.tar` & `thatway-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:26:10.037705 thatway-0.5.0/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1071 2023-08-07 18:07:13.000000 thatway-0.5.0/LICENSE
--rw-r--r--   0 jlorieau   (501) staff       (20)     6382 2023-08-08 18:26:10.037453 thatway-0.5.0/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     6008 2023-08-08 18:25:02.000000 thatway-0.5.0/README.rst
--rw-r--r--   0 jlorieau   (501) staff       (20)      819 2023-08-08 15:51:25.000000 thatway-0.5.0/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-08-08 18:26:10.037799 thatway-0.5.0/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:26:10.034547 thatway-0.5.0/tests/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6629 2023-08-08 18:20:16.000000 thatway-0.5.0/tests/test_base.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:26:10.035353 thatway-0.5.0/thatway/
--rw-r--r--   0 jlorieau   (501) staff       (20)      123 2023-08-08 18:25:38.000000 thatway-0.5.0/thatway/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    13169 2023-08-08 18:20:09.000000 thatway-0.5.0/thatway/base.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:26:10.037096 thatway-0.5.0/thatway.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6382 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)      242 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       57 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        8 2023-08-08 18:26:10.000000 thatway-0.5.0/thatway.egg-info/top_level.txt
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:35:28.502418 thatway-0.5.1/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1071 2023-08-07 18:07:13.000000 thatway-0.5.1/LICENSE
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6441 2023-08-08 18:35:28.502148 thatway-0.5.1/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6008 2023-08-08 18:25:02.000000 thatway-0.5.1/README.rst
+-rw-r--r--   0 jlorieau   (501) staff       (20)      884 2023-08-08 18:34:55.000000 thatway-0.5.1/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-08-08 18:35:28.502505 thatway-0.5.1/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:35:28.498714 thatway-0.5.1/tests/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6629 2023-08-08 18:20:16.000000 thatway-0.5.1/tests/test_base.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:35:28.499746 thatway-0.5.1/thatway/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      123 2023-08-08 18:34:58.000000 thatway-0.5.1/thatway/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    13169 2023-08-08 18:20:09.000000 thatway-0.5.1/thatway/base.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-08-08 18:35:28.501763 thatway-0.5.1/thatway.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6441 2023-08-08 18:35:28.000000 thatway-0.5.1/thatway.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)      242 2023-08-08 18:35:28.000000 thatway-0.5.1/thatway.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-08-08 18:35:28.000000 thatway-0.5.1/thatway.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       57 2023-08-08 18:35:28.000000 thatway-0.5.1/thatway.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        8 2023-08-08 18:35:28.000000 thatway-0.5.1/thatway.egg-info/top_level.txt
```

### Comparing `thatway-0.5.0/LICENSE` & `thatway-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thatway-0.5.0/PKG-INFO` & `thatway-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: thatway
-Version: 0.5.0
+Version: 0.5.1
 Author: Justin Lorieau
+Project-URL: Homepage, https://github.com/jlorieau/thatway
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `thatway-0.5.0/README.rst` & `thatway-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `thatway-0.5.0/pyproject.toml` & `thatway-0.5.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -27,9 +27,12 @@
 dev = [  # For development
     "pytest>=7.4",  # Testing framework
     "twine>=4.0",  # Manage package uploads
     "build",  # Manage package builds
     "black[d]",  # Code formatter
     ]
 
+[project.urls]
+Homepage = "https://github.com/jlorieau/thatway"
+
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --doctest-glob='*.rst'"
```

### Comparing `thatway-0.5.0/tests/test_base.py` & `thatway-0.5.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `thatway-0.5.0/thatway/base.py` & `thatway-0.5.1/thatway/base.py`

 * *Files identical despite different names*

### Comparing `thatway-0.5.0/thatway.egg-info/PKG-INFO` & `thatway-0.5.1/thatway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: thatway
-Version: 0.5.0
+Version: 0.5.1
 Author: Justin Lorieau
+Project-URL: Homepage, https://github.com/jlorieau/thatway
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

