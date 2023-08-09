# Comparing `tmp/inviz-0.3.0.tar.gz` & `tmp/inviz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.3.0.tar", last modified: Wed Aug  9 00:53:53 2023, max compression
+gzip compressed data, was "inviz-0.3.1.tar", last modified: Wed Aug  9 04:09:11 2023, max compression
```

## Comparing `inviz-0.3.0.tar` & `inviz-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 00:53:53.641550 inviz-0.3.0/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.3.0/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.3.0/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2172 2023-08-09 00:53:53.641550 inviz-0.3.0/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.3.0/README.md
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-09 00:53:53.641550 inviz-0.3.0/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1281 2023-08-09 00:49:10.000000 inviz-0.3.0/setup.py
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 00:53:53.641550 inviz-0.3.0/src/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 00:53:53.641550 inviz-0.3.0/src/cosmo/
--rw-r--r--   0 jswen     (1000) jswen     (1000)       20 2023-08-05 07:38:29.000000 inviz-0.3.0/src/cosmo/__init__.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2652 2023-08-09 00:30:13.000000 inviz-0.3.0/src/cosmo/cosmo.py
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 00:53:53.641550 inviz-0.3.0/src/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2172 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      243 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)      132 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/top_level.txt
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 04:09:11.518816 inviz-0.3.1/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.3.1/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.3.1/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2172 2023-08-09 04:09:11.518816 inviz-0.3.1/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.3.1/README.md
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-09 04:09:11.518816 inviz-0.3.1/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1281 2023-08-09 04:07:35.000000 inviz-0.3.1/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 04:09:11.518816 inviz-0.3.1/src/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       20 2023-08-05 07:38:29.000000 inviz-0.3.1/src/__init__.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 04:09:11.518816 inviz-0.3.1/src/cosmo/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       20 2023-08-05 07:38:29.000000 inviz-0.3.1/src/cosmo/__init__.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2652 2023-08-09 01:01:29.000000 inviz-0.3.1/src/cosmo/cosmo.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 04:09:11.518816 inviz-0.3.1/src/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2172 2023-08-09 04:09:11.000000 inviz-0.3.1/src/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      272 2023-08-09 04:09:11.000000 inviz-0.3.1/src/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-09 04:09:11.000000 inviz-0.3.1/src/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      132 2023-08-09 04:09:11.000000 inviz-0.3.1/src/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-09 04:09:11.000000 inviz-0.3.1/src/inviz.egg-info/top_level.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)    11936 2023-08-09 01:01:29.000000 inviz-0.3.1/src/inviz.py
```

### Comparing `inviz-0.3.0/LICENSE` & `inviz-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.3.0/PKG-INFO` & `inviz-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.3.0
+Version: 0.3.1
 Summary: An interactive visualizer to help explore high-dimensional likelihoods and their observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.3.0/README.md` & `inviz-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.3.0/setup.py` & `inviz-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.3.0",
+    version = "0.3.1",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore high-dimensional likelihoods and their observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     packages=setuptools.find_packages(where='src'),
```

### Comparing `inviz-0.3.0/src/cosmo/cosmo.py` & `inviz-0.3.1/src/cosmo/cosmo.py`

 * *Files identical despite different names*

### Comparing `inviz-0.3.0/src/inviz.egg-info/PKG-INFO` & `inviz-0.3.1/src/inviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.3.0
+Version: 0.3.1
 Summary: An interactive visualizer to help explore high-dimensional likelihoods and their observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

