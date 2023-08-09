# Comparing `tmp/reactpy_django-3.3.0.tar.gz` & `tmp/reactpy_django-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_django-3.3.0.tar", last modified: Sat Aug  5 07:52:46 2023, max compression
+gzip compressed data, was "reactpy_django-3.3.1.tar", last modified: Wed Aug  9 00:51:29 2023, max compression
```

## Comparing `reactpy_django-3.3.0.tar` & `reactpy_django-3.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.351398 reactpy_django-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.351398 reactpy_django-3.3.0/src/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/http/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/http/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/0004_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.351398 reactpy_django-3.3.0/src/reactpy_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/static/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django/static/reactpy_django/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.351398 reactpy_django-3.3.0/src/reactpy_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/templates/reactpy/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/templates/reactpy/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/templatetags/reactpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/websocket/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-05 07:52:16.000000 reactpy_django-3.3.0/src/reactpy_django/websocket/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:52:46.355398 reactpy_django-3.3.0/src/reactpy_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:52:39.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-05 07:52:46.000000 reactpy_django-3.3.0/src/reactpy_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.517692 reactpy_django-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-09 00:51:29.517692 reactpy_django-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-09 00:51:29.517692 reactpy_django-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.505692 reactpy_django-3.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.513692 reactpy_django-3.3.1/src/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.513692 reactpy_django-3.3.1/src/reactpy_django/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/http/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/http/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.513692 reactpy_django-3.3.1/src/reactpy_django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/migrations/0004_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.505692 reactpy_django-3.3.1/src/reactpy_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.513692 reactpy_django-3.3.1/src/reactpy_django/static/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-08-09 00:51:29.000000 reactpy_django-3.3.1/src/reactpy_django/static/reactpy_django/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.505692 reactpy_django-3.3.1/src/reactpy_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.513692 reactpy_django-3.3.1/src/reactpy_django/templates/reactpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/templates/reactpy/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.513692 reactpy_django-3.3.1/src/reactpy_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/templatetags/reactpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.517692 reactpy_django-3.3.1/src/reactpy_django/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/websocket/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-09 00:50:44.000000 reactpy_django-3.3.1/src/reactpy_django/websocket/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:51:29.513692 reactpy_django-3.3.1/src/reactpy_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-08-09 00:51:29.000000 reactpy_django-3.3.1/src/reactpy_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-09 00:51:29.000000 reactpy_django-3.3.1/src/reactpy_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:51:29.000000 reactpy_django-3.3.1/src/reactpy_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:51:20.000000 reactpy_django-3.3.1/src/reactpy_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-09 00:51:29.000000 reactpy_django-3.3.1/src/reactpy_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-09 00:51:29.000000 reactpy_django-3.3.1/src/reactpy_django.egg-info/top_level.txt
```

### Comparing `reactpy_django-3.3.0/LICENSE` & `reactpy_django-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/PKG-INFO` & `reactpy_django-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy_django
-Version: 3.3.0
+Version: 3.3.1
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reactpy_django Version: 3.3.0 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy_django Version: 3.3.1 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
```

### Comparing `reactpy_django-3.3.0/README.md` & `reactpy_django-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/setup.py` & `reactpy_django-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/checks.py` & `reactpy_django-3.3.1/src/reactpy_django/checks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 
 from django.contrib.staticfiles.finders import find
 from django.core.checks import Error, Tags, Warning, register
+from django.template import loader
 
 
 @register(Tags.compatibility)
 def reactpy_warnings(app_configs, **kwargs):
     from django.conf import settings
     from django.urls import reverse
 
@@ -44,15 +45,15 @@
             )
         )
 
     # Warn if REACTPY_BACKHAUL_THREAD is set to True on Linux with Daphne
     if (
         sys.argv
         and sys.argv[0].endswith("daphne")
-        and getattr(settings, "REACTPY_BACKHAUL_THREAD", True)
+        and getattr(settings, "REACTPY_BACKHAUL_THREAD", False)
         and sys.platform == "linux"
     ):
         warnings.append(
             Warning(
                 "REACTPY_BACKHAUL_THREAD is enabled but you running with Daphne on Linux. "
                 "This configuration is known to be unstable.",
                 hint="Set settings.py:REACTPY_BACKHAUL_THREAD to False or use a different webserver.",
@@ -72,19 +73,55 @@
 
     # Check if any components failed to be registered
     if REACTPY_FAILED_COMPONENTS:
         warnings.append(
             Warning(
                 "ReactPy failed to register the following components:\n\t+ "
                 + "\n\t+ ".join(REACTPY_FAILED_COMPONENTS),
-                hint="Check if these paths are valid, or if an exception is being raised during import.",
+                hint="Check if these paths are valid, or if an exception is being "
+                "raised during import.",
                 id="reactpy_django.W005",
             )
         )
 
+    # Check if the reactpy/component.html template exists
+    try:
+        loader.get_template("reactpy/component.html")
+    except Exception:
+        warnings.append(
+            Warning(
+                "ReactPy HTML templates could not be found!",
+                hint="Check your settings.py:TEMPLATES configuration and make sure "
+                "ReactPy-Django is installed properly.",
+                id="reactpy_django.W006",
+            )
+        )
+
+    # Check if REACTPY_WEBSOCKET_URL doesn't end with a slash
+    REACTPY_WEBSOCKET_URL = getattr(settings, "REACTPY_WEBSOCKET_URL", "")
+    if isinstance(REACTPY_WEBSOCKET_URL, str):
+        if not REACTPY_WEBSOCKET_URL or not REACTPY_WEBSOCKET_URL.endswith("/"):
+            warnings.append(
+                Warning(
+                    "REACTPY_WEBSOCKET_URL did not end with a forward slash.",
+                    hint="Change your URL to be written in the following format: 'example_url/'",
+                    id="reactpy_django.W007",
+                )
+            )
+
+        # Check if REACTPY_WEBSOCKET_URL doesn't start with an alphanumeric character
+        if not REACTPY_WEBSOCKET_URL or not REACTPY_WEBSOCKET_URL[0].isalnum():
+            warnings.append(
+                Warning(
+                    "REACTPY_WEBSOCKET_URL did not start with an alphanumeric character.",
+                    hint="Change your URL to be written in the following format: 'example_url/'",
+                    id="reactpy_django.W008",
+                )
+            )
+
     return warnings
 
 
 @register(Tags.compatibility)
 def reactpy_errors(app_configs, **kwargs):
     from django.conf import settings
```

### Comparing `reactpy_django-3.3.0/src/reactpy_django/components.py` & `reactpy_django-3.3.1/src/reactpy_django/components.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/config.py` & `reactpy_django-3.3.1/src/reactpy_django/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     settings,
     "REACTPY_AUTH_BACKEND",
     None,
 )
 REACTPY_BACKHAUL_THREAD: bool = getattr(
     settings,
     "REACTPY_BACKHAUL_THREAD",
-    True,
+    False,
 )
```

### Comparing `reactpy_django-3.3.0/src/reactpy_django/database.py` & `reactpy_django-3.3.1/src/reactpy_django/database.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/decorators.py` & `reactpy_django-3.3.1/src/reactpy_django/decorators.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/hooks.py` & `reactpy_django-3.3.1/src/reactpy_django/hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     Query,
     QueryOptions,
     _Params,
     _Result,
 )
 from reactpy_django.utils import generate_obj_name
 
-
 _logger = logging.getLogger(__name__)
 _REFETCH_CALLBACKS: DefaultDict[
     Callable[..., Any], set[Callable[[], None]]
 ] = DefaultDict(set)
 
 
 def use_location() -> Location:
```

### Comparing `reactpy_django-3.3.0/src/reactpy_django/http/views.py` & `reactpy_django-3.3.1/src/reactpy_django/http/views.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/migrations/0001_initial.py` & `reactpy_django-3.3.1/src/reactpy_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py` & `reactpy_django-3.3.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/migrations/0004_config.py` & `reactpy_django-3.3.1/src/reactpy_django/migrations/0004_config.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/models.py` & `reactpy_django-3.3.1/src/reactpy_django/models.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/static/reactpy_django/client.js` & `reactpy_django-3.3.1/src/reactpy_django/static/reactpy_django/client.js`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/templates/reactpy/component.html` & `reactpy_django-3.3.1/src/reactpy_django/templates/reactpy/component.html`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/templatetags/reactpy.py` & `reactpy_django-3.3.1/src/reactpy_django/templatetags/reactpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from reactpy_django.types import ComponentParamData
 from reactpy_django.utils import (
     _register_component,
     check_component_args,
     func_has_args,
 )
 
-
 REACTPY_WEB_MODULES_URL = reverse("reactpy:web_modules", args=["x"])[:-1][1:]
 register = template.Library()
 _logger = getLogger(__name__)
 
 
 @register.inclusion_tag("reactpy/component.html")
 def component(dotted_path: str, *args, **kwargs):
```

### Comparing `reactpy_django-3.3.0/src/reactpy_django/types.py` & `reactpy_django-3.3.1/src/reactpy_django/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from django.db.models.base import Model
 from django.db.models.query import QuerySet
 from django.views.generic import View
 from reactpy.types import Connection as _Connection
 from typing_extensions import ParamSpec
 
-
 __all__ = [
     "_Result",
     "_Params",
     "_Data",
     "ComponentWebsocket",
     "Query",
     "Mutation",
```

### Comparing `reactpy_django-3.3.0/src/reactpy_django/utils.py` & `reactpy_django-3.3.1/src/reactpy_django/utils.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django/websocket/consumer.py` & `reactpy_django-3.3.1/src/reactpy_django/websocket/consumer.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.3.0/src/reactpy_django.egg-info/PKG-INFO` & `reactpy_django-3.3.1/src/reactpy_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-django
-Version: 3.3.0
+Version: 3.3.1
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reactpy-django Version: 3.3.0 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy-django Version: 3.3.1 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
```

### Comparing `reactpy_django-3.3.0/src/reactpy_django.egg-info/SOURCES.txt` & `reactpy_django-3.3.1/src/reactpy_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

