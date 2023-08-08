# Comparing `tmp/snitch-protos-0.0.58.tar.gz` & `tmp/snitch-protos-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.58.tar", last modified: Tue Aug  8 21:46:16 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.59.tar", last modified: Tue Aug  8 22:30:23 2023, max compression
```

## Comparing `snitch-protos-0.0.58.tar` & `snitch-protos-0.0.59.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 21:45:47.000000 snitch-protos-0.0.58/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:45:47.000000 snitch-protos-0.0.58/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    35734 2023-08-08 21:45:47.000000 snitch-protos-0.0.58/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-08 21:45:47.000000 snitch-protos-0.0.58/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:30:23.165775 snitch-protos-0.0.59/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 22:30:23.165775 snitch-protos-0.0.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 22:29:47.000000 snitch-protos-0.0.59/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 22:30:23.165775 snitch-protos-0.0.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-08 22:30:22.000000 snitch-protos-0.0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:30:23.165775 snitch-protos-0.0.59/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:29:47.000000 snitch-protos-0.0.59/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:30:23.165775 snitch-protos-0.0.59/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    35735 2023-08-08 22:29:47.000000 snitch-protos-0.0.59/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:30:23.165775 snitch-protos-0.0.59/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-08 22:29:47.000000 snitch-protos-0.0.59/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:30:23.165775 snitch-protos-0.0.59/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 22:30:23.000000 snitch-protos-0.0.59/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 22:30:23.000000 snitch-protos-0.0.59/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:30:23.000000 snitch-protos-0.0.59/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 22:30:23.000000 snitch-protos-0.0.59/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.58/PKG-INFO` & `snitch-protos-0.0.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.58
+Version: 0.0.59
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.58/setup.py` & `snitch-protos-0.0.59/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.58',
+    version='0.0.59',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.58/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.59/snitch_protos/protos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         10002, optional=True, group="X_wasm_function"
     )
     """WASM function name to execute (set by snitch-server)"""
 
 
 @dataclass(eq=False, repr=False)
 class LiveInfo(betterproto.Message):
-    audience: List["Audience"] = betterproto.message_field(1)
+    audiences: List["Audience"] = betterproto.message_field(1)
     """If empty, client has not announced any audiences"""
 
     client: "ClientInfo" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class PipelineInfo(betterproto.Message):
```

### Comparing `snitch-protos-0.0.58/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.59/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.58/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.59/snitch_protos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.58
+Version: 0.0.59
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

