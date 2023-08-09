# Comparing `tmp/robotframework-requestspro-1.2.8.tar.gz` & `tmp/robotframework-requestspro-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-requestspro-1.2.8.tar", last modified: Sat Aug  5 01:19:43 2023, max compression
+gzip compressed data, was "robotframework-requestspro-1.2.9.tar", last modified: Wed Aug  9 02:34:38 2023, max compression
```

## Comparing `robotframework-requestspro-1.2.8.tar` & `robotframework-requestspro-1.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-05 01:19:43.675123 robotframework-requestspro-1.2.8/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/LICENSE
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/MANIFEST.in
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-05 01:19:43.674997 robotframework-requestspro-1.2.8/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/README.md
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/requirements.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-05 01:19:43.675168 robotframework-requestspro-1.2.8/setup.cfg
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/setup.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-05 01:19:43.672626 robotframework-requestspro-1.2.8/src/
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-05 01:19:43.674235 robotframework-requestspro-1.2.8/src/RequestsProLibrary/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     2469 2023-08-05 01:18:46.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/DynamicTestCases.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)    12747 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/RequestsProKeywords.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/__init__.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/compat.py
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-05 00:37:06.000000 robotframework-requestspro-1.2.8/src/RequestsProLibrary/version.py
-drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-05 01:19:43.674815 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/PKG-INFO
--rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/SOURCES.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/dependency_links.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/requires.txt
--rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-05 01:19:43.000000 robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/top_level.txt
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-09 02:34:38.653861 robotframework-requestspro-1.2.9/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1069 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.9/LICENSE
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       34 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.9/MANIFEST.in
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-09 02:34:38.653748 robotframework-requestspro-1.2.9/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       31 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.9/README.md
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       85 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.9/requirements.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       38 2023-08-09 02:34:38.653905 robotframework-requestspro-1.2.9/setup.cfg
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1689 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.9/setup.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-09 02:34:38.651239 robotframework-requestspro-1.2.9/src/
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-09 02:34:38.652998 robotframework-requestspro-1.2.9/src/RequestsProLibrary/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     2469 2023-08-05 01:18:46.000000 robotframework-requestspro-1.2.9/src/RequestsProLibrary/DynamicTestCases.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)    12749 2023-08-09 02:33:15.000000 robotframework-requestspro-1.2.9/src/RequestsProLibrary/RequestsProKeywords.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)     1966 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.9/src/RequestsProLibrary/__init__.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      182 2023-08-04 03:00:29.000000 robotframework-requestspro-1.2.9/src/RequestsProLibrary/compat.py
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       18 2023-08-09 02:34:09.000000 robotframework-requestspro-1.2.9/src/RequestsProLibrary/version.py
+drwxr-xr-x   0 vaanisridhar   (501) staff       (20)        0 2023-08-09 02:34:38.653580 robotframework-requestspro-1.2.9/src/robotframework_requestspro.egg-info/
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      713 2023-08-09 02:34:38.000000 robotframework-requestspro-1.2.9/src/robotframework_requestspro.egg-info/PKG-INFO
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)      515 2023-08-09 02:34:38.000000 robotframework-requestspro-1.2.9/src/robotframework_requestspro.egg-info/SOURCES.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)        1 2023-08-09 02:34:38.000000 robotframework-requestspro-1.2.9/src/robotframework_requestspro.egg-info/dependency_links.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       74 2023-08-09 02:34:38.000000 robotframework-requestspro-1.2.9/src/robotframework_requestspro.egg-info/requires.txt
+-rw-r--r--   0 vaanisridhar   (501) staff       (20)       19 2023-08-09 02:34:38.000000 robotframework-requestspro-1.2.9/src/robotframework_requestspro.egg-info/top_level.txt
```

### Comparing `robotframework-requestspro-1.2.8/LICENSE` & `robotframework-requestspro-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.8/PKG-INFO` & `robotframework-requestspro-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.8
+Version: 1.2.9
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.8/setup.py` & `robotframework-requestspro-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.8/src/RequestsProLibrary/DynamicTestCases.py` & `robotframework-requestspro-1.2.9/src/RequestsProLibrary/DynamicTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.8/src/RequestsProLibrary/RequestsProKeywords.py` & `robotframework-requestspro-1.2.9/src/RequestsProLibrary/RequestsProKeywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from RequestsLibrary import RequestsLibrary
 from urllib3.util import Retry
 from robot.api import logger
 
 
 class RequestsProKeywords(RequestsLibrary):
     ROBOT_LIBRARY_SCOPE = 'Global'
-    DEFAULT_RETRY_METHOD_LIST = list(copy.copy(Retry.DEFAULT_METHOD_WHITELIST))
+    # DEFAULT_RETRY_METHOD_LIST = list(copy.copy(Retry.DEFAULT_METHOD_WHITELIST))
 
     def __init__(self):
         super().__init__()
         for base in RequestsProKeywords.__bases__:
             base.__init__(self)
         self._primers = {}
         self.cookies = None
```

### Comparing `robotframework-requestspro-1.2.8/src/RequestsProLibrary/__init__.py` & `robotframework-requestspro-1.2.9/src/RequestsProLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/PKG-INFO` & `robotframework-requestspro-1.2.9/src/robotframework_requestspro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-requestspro
-Version: 1.2.8
+Version: 1.2.9
 Summary: Robot Framework keyword library wrapper around requests
 Home-page: https://github.com/sridharvpmca/robotframework-requestspro
 Author: Sridhar VP
 Author-email: sridharvpmca@gmail.com
 License: MIT
 Keywords: robotframework testing test automation http client requests
 Platform: any
```

### Comparing `robotframework-requestspro-1.2.8/src/robotframework_requestspro.egg-info/SOURCES.txt` & `robotframework-requestspro-1.2.9/src/robotframework_requestspro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

