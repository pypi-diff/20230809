# Comparing `tmp/pygrb_lc-0.1.7.tar.gz` & `tmp/pygrb_lc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.1.7.tar", last modified: Mon Jul 31 11:06:02 2023, max compression
+gzip compressed data, was "pygrb_lc-0.1.8.tar", last modified: Tue Aug  8 23:17:54 2023, max compression
```

## Comparing `pygrb_lc-0.1.7.tar` & `pygrb_lc-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:06:02.951846 pygrb_lc-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-31 11:06:02.951846 pygrb_lc-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-31 11:06:02.951846 pygrb_lc-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:06:02.947846 pygrb_lc-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:06:02.951846 pygrb_lc-0.1.7/src/pygrb_lc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/blind_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/furie.py
--rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/src/pygrb_lc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:06:02.951846 pygrb_lc-0.1.7/src/pygrb_lc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-31 11:06:02.000000 pygrb_lc-0.1.7/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-31 11:06:02.000000 pygrb_lc-0.1.7/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:06:02.000000 pygrb_lc-0.1.7/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 11:06:02.000000 pygrb_lc-0.1.7/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:06:02.951846 pygrb_lc-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/tests/test_light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-31 11:05:51.000000 pygrb_lc-0.1.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:17:54.458654 pygrb_lc-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-08-08 23:17:54.458654 pygrb_lc-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-08 23:17:54.458654 pygrb_lc-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:17:54.450653 pygrb_lc-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:17:54.454654 pygrb_lc-0.1.8/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:17:54.454654 pygrb_lc-0.1.8/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-08-08 23:17:54.000000 pygrb_lc-0.1.8/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-08 23:17:54.000000 pygrb_lc-0.1.8/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:17:54.000000 pygrb_lc-0.1.8/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 23:17:54.000000 pygrb_lc-0.1.8/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:17:54.458654 pygrb_lc-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-08 23:17:45.000000 pygrb_lc-0.1.8/tests/test_utils.py
```

### Comparing `pygrb_lc-0.1.7/LICENSE` & `pygrb_lc-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/PKG-INFO` & `pygrb_lc-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb_lc
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.1.7/README.md` & `pygrb_lc-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/setup.cfg` & `pygrb_lc-0.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygrb_lc
-version = 0.1.7
+version = 0.1.8
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jorezzz/pygrb_lc
 project_urls =
```

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.1.8/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc/catalogs.py` & `pygrb_lc-0.1.8/src/pygrb_lc/catalogs.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,22 +27,22 @@
         '''
         closest = self.find_closest(event_time)
         if abs(closest[self.event_column] - event_time).total_seconds() <= precision:
             return closest
         else:
             return None
 
-    def crossmatch(self, other, precision: int = 5):
+    def crossmatch(self, other, precision = 5):
         '''
         Args:
             other (Catalog): instance of other catalog to match with
-            precision (int, optional): precision of crossmatching in seconds
+            precision (int, str, optional): precision of crossmatching in seconds, if str then column with name precision in seconds
         '''
         for i,event in self.iterrows():
-            idx = other.find_event(event[self.event_column], precision)
+            idx = other.find_event(event[self.event_column], precision if type(precision) is int else event[precision])
             if idx is not None:
                 for column in other.param_columns:
                     column_new = column if column not in self.param_columns else column + '_other'
                     self.loc[self.index==i,[column_new]] = other.loc[other.index==idx.name,column].values
         return self
     
     def save(self, path):
```

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc/config.py` & `pygrb_lc-0.1.8/src/pygrb_lc/config.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.1.8/src/pygrb_lc/crossmatching.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc/furie.py` & `pygrb_lc-0.1.8/src/pygrb_lc/furie.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.1.8/src/pygrb_lc/light_curves.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc/time.py` & `pygrb_lc-0.1.8/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc/utils.py` & `pygrb_lc-0.1.8/src/pygrb_lc/utils.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.7/src/pygrb_lc.egg-info/PKG-INFO` & `pygrb_lc-0.1.8/src/pygrb_lc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb-lc
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.1.7/tests/test_utils.py` & `pygrb_lc-0.1.8/tests/test_utils.py`

 * *Files identical despite different names*

