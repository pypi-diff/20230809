# Comparing `tmp/multiparlog-1.0.0.tar.gz` & `tmp/multiparlog-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiparlog-1.0.0.tar", last modified: Fri Oct  7 20:00:21 2022, max compression
+gzip compressed data, was "multiparlog-1.0.3.tar", last modified: Tue Aug  8 22:23:24 2023, max compression
```

## Comparing `multiparlog-1.0.0.tar` & `multiparlog-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2022-10-07 20:00:21.013240 multiparlog-1.0.0/
--rw-r--r--   0 rkotulla  (1000) users      (100)        0 2022-07-12 21:52:53.000000 multiparlog-1.0.0/LICENSE
--rw-r--r--   0 rkotulla  (1000) users      (100)      594 2022-10-07 20:00:21.013240 multiparlog-1.0.0/PKG-INFO
--rw-r--r--   0 rkotulla  (1000) users      (100)       44 2022-07-12 21:56:21.000000 multiparlog-1.0.0/README.md
--rw-r--r--   0 rkotulla  (1000) users      (100)      954 2022-10-07 19:58:17.000000 multiparlog-1.0.0/pyproject.toml
--rw-r--r--   0 rkotulla  (1000) users      (100)       38 2022-10-07 20:00:21.013240 multiparlog-1.0.0/setup.cfg
--rw-r--r--   0 rkotulla  (1000) users      (100)      659 2022-10-07 19:59:38.000000 multiparlog-1.0.0/setup.py
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2022-10-07 20:00:21.009240 multiparlog-1.0.0/src/
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2022-10-07 20:00:21.009240 multiparlog-1.0.0/src/multiparlog/
--rw-r--r--   0 rkotulla  (1000) users      (100)       56 2022-07-14 23:13:26.000000 multiparlog-1.0.0/src/multiparlog/__init__.py
--rwxr-xr-x   0 rkotulla  (1000) users      (100)    15521 2022-10-07 15:34:04.000000 multiparlog-1.0.0/src/multiparlog/mplogging.py
-drwxr-xr-x   0 rkotulla  (1000) users      (100)        0 2022-10-07 20:00:21.009240 multiparlog-1.0.0/src/multiparlog.egg-info/
--rw-r--r--   0 rkotulla  (1000) users      (100)      594 2022-10-07 20:00:21.000000 multiparlog-1.0.0/src/multiparlog.egg-info/PKG-INFO
--rw-r--r--   0 rkotulla  (1000) users      (100)      254 2022-10-07 20:00:21.000000 multiparlog-1.0.0/src/multiparlog.egg-info/SOURCES.txt
--rw-r--r--   0 rkotulla  (1000) users      (100)        1 2022-10-07 20:00:21.000000 multiparlog-1.0.0/src/multiparlog.egg-info/dependency_links.txt
--rw-r--r--   0 rkotulla  (1000) users      (100)       12 2022-10-07 20:00:21.000000 multiparlog-1.0.0/src/multiparlog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:23:24.524070 multiparlog-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:23:21.000000 multiparlog-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-08 22:23:24.524070 multiparlog-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 22:23:21.000000 multiparlog-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-08 22:23:23.000000 multiparlog-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 22:23:24.524070 multiparlog-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-08 22:23:23.000000 multiparlog-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:23:24.520070 multiparlog-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:23:24.524070 multiparlog-1.0.3/src/multiparlog/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-08 22:23:21.000000 multiparlog-1.0.3/src/multiparlog/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15521 2023-08-08 22:23:21.000000 multiparlog-1.0.3/src/multiparlog/mplogging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:23:24.524070 multiparlog-1.0.3/src/multiparlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-08 22:23:24.000000 multiparlog-1.0.3/src/multiparlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-08 22:23:24.000000 multiparlog-1.0.3/src/multiparlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:23:24.000000 multiparlog-1.0.3/src/multiparlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 22:23:24.000000 multiparlog-1.0.3/src/multiparlog.egg-info/top_level.txt
```

### Comparing `multiparlog-1.0.0/PKG-INFO` & `multiparlog-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiparlog
-Version: 1.0.0
+Version: 1.0.3
 Summary: A flexible multi-processing safe logging tool
 Author-email: Ralf Kotulla <ralf.kotulla@gmail.com>
 Project-URL: Homepage, https://github.com/rkotulla/multiparallel_logging
 Project-URL: Bug Tracker, https://github.com/rkotulla/multiparallel_logging/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multiparlog-1.0.0/pyproject.toml` & `multiparlog-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multiparlog"
-version = "1.0.0"
+version = "1.0.3"
 authors = [
   { name="Ralf Kotulla", email="ralf.kotulla@gmail.com" },
 ]
 description = "A flexible multi-processing safe logging tool"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
@@ -14,28 +14,30 @@
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/rkotulla/multiparallel_logging"
 "Bug Tracker" = "https://github.com/rkotulla/multiparallel_logging/issues"
 
-[tool.bumpver]
-current_version = "1.0.0"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message = "bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = false
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = [
-    'current_version = "{version}"',
-]
-"setup.py" = [
-    "{version}",
-    "{pep440_version}",
-]
-"README.md" = [
-    "{version}",
-    "{pep440_version}",
-]
 
+#
+#[tool.bumpver]
+#current_version = "1.0.0"
+#version_pattern = "MAJOR.MINOR.PATCH"
+#commit_message = "bump version {old_version} -> {new_version}"
+#commit = true
+#tag = true
+#push = false
+#
+#[tool.bumpver.file_patterns]
+#"pyproject.toml" = [
+#    'current_version = "{version}"',
+#]
+#"setup.py" = [
+#    "{version}",
+#    "{pep440_version}",
+#]
+#"README.md" = [
+#    "{version}",
+#    "{pep440_version}",
+#]
+#
```

### Comparing `multiparlog-1.0.0/setup.py` & `multiparlog-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,14 @@
     name = "multiparlog",
     package_dir = {'': 'src'},
     packages = ['multiparlog'],
     # packages = find_namespace_packages(include=['src.multiparlog.*']),
     # entry_points = {
     #     "console_scripts": []
     #     },
-    version = "1.0.0",
+    version = "1.0.3",
     # description = "A flexible multi-processing safe logging tool",
     # # long_description = long_descr,
     # author = "Ralf Kotulla",
     # author_email = "ralf.kotulla@gmail.com",
     # url = "https://github.com/rkotulla/multiparallel_logging",
     )
```

### Comparing `multiparlog-1.0.0/src/multiparlog/mplogging.py` & `multiparlog-1.0.3/src/multiparlog/mplogging.py`

 * *Files identical despite different names*

### Comparing `multiparlog-1.0.0/src/multiparlog.egg-info/PKG-INFO` & `multiparlog-1.0.3/src/multiparlog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiparlog
-Version: 1.0.0
+Version: 1.0.3
 Summary: A flexible multi-processing safe logging tool
 Author-email: Ralf Kotulla <ralf.kotulla@gmail.com>
 Project-URL: Homepage, https://github.com/rkotulla/multiparallel_logging
 Project-URL: Bug Tracker, https://github.com/rkotulla/multiparallel_logging/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

