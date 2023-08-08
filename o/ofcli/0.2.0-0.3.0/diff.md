# Comparing `tmp/ofcli-0.2.0.tar.gz` & `tmp/ofcli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofcli-0.2.0.tar", last modified: Wed Jul 19 23:12:30 2023, max compression
+gzip compressed data, was "ofcli-0.3.0.tar", last modified: Tue Aug  8 22:36:14 2023, max compression
```

## Comparing `ofcli-0.2.0.tar` & `ofcli-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-19 23:12:30.677336 ofcli-0.2.0/
--rw-r--r--   0 diana     (1000) diana     (1000)     4608 2023-07-19 23:12:30.677336 ofcli-0.2.0/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)     3279 2023-07-17 22:44:14.000000 ofcli-0.2.0/README.md
--rw-r--r--   0 diana     (1000) diana     (1000)      106 2023-06-25 09:29:29.000000 ofcli-0.2.0/pyproject.toml
--rw-r--r--   0 diana     (1000) diana     (1000)     1570 2023-07-19 23:12:30.677336 ofcli-0.2.0/setup.cfg
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-19 23:12:30.677336 ofcli-0.2.0/src/
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-19 23:12:30.677336 ofcli-0.2.0/src/ofcli.egg-info/
--rw-r--r--   0 diana     (1000) diana     (1000)     4608 2023-07-19 23:12:30.000000 ofcli-0.2.0/src/ofcli.egg-info/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)      234 2023-07-19 23:12:30.000000 ofcli-0.2.0/src/ofcli.egg-info/SOURCES.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-19 23:12:30.000000 ofcli-0.2.0/src/ofcli.egg-info/dependency_links.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       46 2023-07-19 23:12:30.000000 ofcli-0.2.0/src/ofcli.egg-info/entry_points.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       50 2023-07-19 23:12:30.000000 ofcli-0.2.0/src/ofcli.egg-info/requires.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-19 23:12:30.000000 ofcli-0.2.0/src/ofcli.egg-info/top_level.txt
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-08-08 22:36:14.926840 ofcli-0.3.0/
+-rw-r--r--   0 diana     (1000) diana     (1000)     4608 2023-08-08 22:36:14.926840 ofcli-0.3.0/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)     3279 2023-07-17 22:44:14.000000 ofcli-0.3.0/README.md
+-rw-r--r--   0 diana     (1000) diana     (1000)      106 2023-06-25 09:29:29.000000 ofcli-0.3.0/pyproject.toml
+-rw-r--r--   0 diana     (1000) diana     (1000)     1570 2023-08-08 22:36:14.926840 ofcli-0.3.0/setup.cfg
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-08-08 22:36:14.923507 ofcli-0.3.0/src/
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-08-08 22:36:14.926840 ofcli-0.3.0/src/ofcli.egg-info/
+-rw-r--r--   0 diana     (1000) diana     (1000)     4608 2023-08-08 22:36:14.000000 ofcli-0.3.0/src/ofcli.egg-info/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)      234 2023-08-08 22:36:14.000000 ofcli-0.3.0/src/ofcli.egg-info/SOURCES.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-08-08 22:36:14.000000 ofcli-0.3.0/src/ofcli.egg-info/dependency_links.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       46 2023-08-08 22:36:14.000000 ofcli-0.3.0/src/ofcli.egg-info/entry_points.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       50 2023-08-08 22:36:14.000000 ofcli-0.3.0/src/ofcli.egg-info/requires.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-08-08 22:36:14.000000 ofcli-0.3.0/src/ofcli.egg-info/top_level.txt
```

### Comparing `ofcli-0.2.0/PKG-INFO` & `ofcli-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofcli
-Version: 0.2.0
+Version: 0.3.0
 Summary: helper CLI tool for OIDC federation exploration
 Home-page: https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ofcli-0.2.0/README.md` & `ofcli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ofcli-0.2.0/setup.cfg` & `ofcli-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ofcli-0.2.0/src/ofcli.egg-info/PKG-INFO` & `ofcli-0.3.0/src/ofcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofcli
-Version: 0.2.0
+Version: 0.3.0
 Summary: helper CLI tool for OIDC federation exploration
 Home-page: https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli/issues
 Classifier: Development Status :: 3 - Alpha
```

