# Comparing `tmp/mpzinke-0.0.2.tar.gz` & `tmp/mpzinke-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpzinke-0.0.2.tar", last modified: Fri Aug  4 02:45:23 2023, max compression
+gzip compressed data, was "mpzinke-0.0.3.tar", last modified: Tue Aug  8 23:22:14 2023, max compression
```

## Comparing `mpzinke-0.0.2.tar` & `mpzinke-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:45:23.961906 mpzinke-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 02:44:45.000000 mpzinke-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-04 02:45:23.957906 mpzinke-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-04 02:44:45.000000 mpzinke-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-04 02:45:16.000000 mpzinke-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 02:45:23.961906 mpzinke-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:45:23.953906 mpzinke-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:45:23.957906 mpzinke-0.0.2/src/mpzinke/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:45:23.957906 mpzinke-0.0.2/src/mpzinke/Server/
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-08-04 02:44:45.000000 mpzinke-0.0.2/src/mpzinke/Server/Route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-08-04 02:44:45.000000 mpzinke-0.0.2/src/mpzinke/Server/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-04 02:44:45.000000 mpzinke-0.0.2/src/mpzinke/Server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-04 02:44:45.000000 mpzinke-0.0.2/src/mpzinke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:45:23.957906 mpzinke-0.0.2/src/mpzinke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-04 02:45:23.000000 mpzinke-0.0.2/src/mpzinke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-04 02:45:23.000000 mpzinke-0.0.2/src/mpzinke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:45:23.000000 mpzinke-0.0.2/src/mpzinke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 02:45:23.000000 mpzinke-0.0.2/src/mpzinke.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:22:14.783538 mpzinke-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 23:21:36.000000 mpzinke-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-08 23:22:14.783538 mpzinke-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-08 23:21:36.000000 mpzinke-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-08 23:22:08.000000 mpzinke-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:22:14.783538 mpzinke-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:22:14.783538 mpzinke-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:22:14.783538 mpzinke-0.0.3/src/mpzinke/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:22:14.783538 mpzinke-0.0.3/src/mpzinke/Generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-08 23:21:36.000000 mpzinke-0.0.3/src/mpzinke/Generic/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-08 23:21:36.000000 mpzinke-0.0.3/src/mpzinke/Generic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:22:14.783538 mpzinke-0.0.3/src/mpzinke/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-08-08 23:21:36.000000 mpzinke-0.0.3/src/mpzinke/Server/Route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-08-08 23:21:36.000000 mpzinke-0.0.3/src/mpzinke/Server/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-08 23:21:36.000000 mpzinke-0.0.3/src/mpzinke/Server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-08 23:21:36.000000 mpzinke-0.0.3/src/mpzinke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:22:14.783538 mpzinke-0.0.3/src/mpzinke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-08 23:22:14.000000 mpzinke-0.0.3/src/mpzinke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-08 23:22:14.000000 mpzinke-0.0.3/src/mpzinke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:22:14.000000 mpzinke-0.0.3/src/mpzinke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 23:22:14.000000 mpzinke-0.0.3/src/mpzinke.egg-info/top_level.txt
```

### Comparing `mpzinke-0.0.2/LICENSE` & `mpzinke-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpzinke-0.0.2/PKG-INFO` & `mpzinke-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpzinke
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python libraries for MPZinke.
 Author: Mathew Zinke
 Project-URL: Homepage, https://github.com/MPZinke/Python
 Project-URL: Bug Tracker, https://github.com/MPZinke/Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `mpzinke-0.0.2/pyproject.toml` & `mpzinke-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "Flask>=2.1.3", "Flask-Cors>=3.0.10"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mpzinke"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{name="Mathew Zinke"}]
 description = "Python libraries for MPZinke."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `mpzinke-0.0.2/src/mpzinke/Server/Route.py` & `mpzinke-0.0.3/src/mpzinke/Server/Route.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.0.2/src/mpzinke/Server/Server.py` & `mpzinke-0.0.3/src/mpzinke/Server/Server.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.0.2/src/mpzinke/Server/__init__.py` & `mpzinke-0.0.3/src/mpzinke/Server/__init__.py`

 * *Files identical despite different names*

### Comparing `mpzinke-0.0.2/src/mpzinke/__init__.py` & `mpzinke-0.0.3/src/mpzinke/Generic/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/opt/homebrew/bin/python3
 # -*- coding: utf-8 -*-
 __author__ = "MPZinke"
 
 ########################################################################################################################
 #                                                                                                                      #
 #   created by: MPZinke                                                                                                #
-#   on 2023.07.31                                                                                                      #
+#   on 2023.08.03                                                                                                      #
 #                                                                                                                      #
 #   DESCRIPTION:                                                                                                       #
 #   BUGS:                                                                                                              #
 #   FUTURE:                                                                                                            #
 #                                                                                                                      #
 ########################################################################################################################
 
 
-from .Server import Server
+from .Generic import Generic
```

### Comparing `mpzinke-0.0.2/src/mpzinke.egg-info/PKG-INFO` & `mpzinke-0.0.3/src/mpzinke.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpzinke
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python libraries for MPZinke.
 Author: Mathew Zinke
 Project-URL: Homepage, https://github.com/MPZinke/Python
 Project-URL: Bug Tracker, https://github.com/MPZinke/Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

