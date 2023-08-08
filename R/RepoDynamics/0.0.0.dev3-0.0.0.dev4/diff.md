# Comparing `tmp/RepoDynamics-0.0.0.dev3.tar.gz` & `tmp/RepoDynamics-0.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepoDynamics-0.0.0.dev3.tar", last modified: Tue Aug  8 15:10:12 2023, max compression
+gzip compressed data, was "RepoDynamics-0.0.0.dev4.tar", last modified: Tue Aug  8 21:47:45 2023, max compression
```

## Comparing `RepoDynamics-0.0.0.dev3.tar` & `RepoDynamics-0.0.0.dev4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.071517 RepoDynamics-0.0.0.dev3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.071517 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:10:11.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.071517 RepoDynamics-0.0.0.dev3/src/repodynamics/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/meta_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/cd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/src/repodynamics/files/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/format_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.652122 RepoDynamics-0.0.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 21:47:45.652122 RepoDynamics-0.0.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:47:45.652122 RepoDynamics-0.0.0.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/repodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/cd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/repodynamics/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/format_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/workflow.py
```

### Comparing `RepoDynamics-0.0.0.dev3/pyproject.toml` & `RepoDynamics-0.0.0.dev4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 where = ["src"]
 namespaces = true
 
 
 # ----------------------------------------- Project Metadata -------------------------------------
 #
 [project]
-version = "0.0.0.dev3"
+version = "0.0.0.dev4"
 name = "RepoDynamics"
 #dependencies = [
 #    # https://yaml.readthedocs.io/en/stable/
 #    "ruamel.yaml >= 0.17.32, < 0.18",
 #    # https://tomlkit.readthedocs.io/en/stable/
 #    "tomlkit >= 0.11.8, < 0.12",
 #    "trove-classifiers",
```

### Comparing `RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/SOURCES.txt` & `RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 src/RepoDynamics.egg-info/PKG-INFO
 src/RepoDynamics.egg-info/SOURCES.txt
 src/RepoDynamics.egg-info/dependency_links.txt
 src/RepoDynamics.egg-info/not-zip-safe
 src/RepoDynamics.egg-info/requires.txt
 src/RepoDynamics.egg-info/top_level.txt
 src/repodynamics/__init__.py
+src/repodynamics/__main__.py
+src/repodynamics/ansi.py
 src/repodynamics/cd.py
 src/repodynamics/format_issue.py
 src/repodynamics/metadata.py
 src/repodynamics/workflow.py
 src/repodynamics/actions/__init__.py
 src/repodynamics/actions/__main__.py
 src/repodynamics/actions/context.py
 src/repodynamics/actions/io.py
 src/repodynamics/actions/meta.py
-src/repodynamics/actions/meta_summary.py
 src/repodynamics/files/__init__.py
 src/repodynamics/files/__main__.py
 src/repodynamics/files/pyproject.py
 src/repodynamics/files/readme.py
 src/repodynamics/files/templates.py
```

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/actions/__main__.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/actions/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import argparse
 import importlib
 import sys
 
 from repodynamics.actions import io
+from repodynamics.ansi import SGR
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("action", type=str, help="Name of the action to run.")
-    action_name = parser.parse_args().action.replace('-', '_')
+    action = parser.parse_args().action
+    print()
+    action_name = action.replace('-', '_')
     try:
         action_module = importlib.import_module(f"repodynamics.actions.{action_name}")
         action = getattr(action_module, action_name)
         inputs = io.input(action=action)
         outputs, summary = action(**inputs)
         if outputs:
             io.output(**outputs)
```

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/actions/context.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/actions/context.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/actions/io.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/actions/io.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 from typing import Callable, Optional, get_type_hints
 import os
 import sys
 import json
 
+from repodynamics.ansi import SGR
 
 def input(action: Callable) -> dict:
     """
     Parse inputs from environment variables.
     """
+    print(
+        SGR.format(
+            f"Reading inputs for action '{action.__name__}':",
+            styles=SGR.style("bold", "cyan"),
+        )
+    )
     params = get_type_hints(action)
     args = {}
     if not params:
+        print(
+            SGR.format(
+                f"\tAction requires no inputs.",
+                styles=SGR.style(text_color="green"),
+            )
+        )
         return args
     params.pop("return", None)
     for param, typ in params.items():
         action_name = action.__name__.upper().replace('_', '-')
         param_name = param.upper().replace('_', '-')
         param_env_name = f"RD__{action_name}__{param_name}"
         val = os.environ.get(param_env_name)
@@ -44,15 +57,15 @@
             args[param] = json.loads(val, strict=False)
         else:
             print(f"ERROR: Unknown input type: {typ}")
             sys.exit(1)
     return args
 
 
-def output(**kwargs) -> Optional[dict]:
+def output(**kwargs) -> None:
     with open(os.environ["GITHUB_OUTPUT"], "a") as fh:
         for name, value in kwargs.items():
             print(f"{name.replace('_', '-')}={value}", file=fh)
     return
 
 
 def summary(content: str) -> None:
```

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/cd.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/cd.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/files/__main__.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/files/__main__.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/files/pyproject.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/files/pyproject.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/files/readme.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/files/readme.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/files/templates.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/files/templates.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/format_issue.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/format_issue.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/metadata.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/metadata.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev3/src/repodynamics/workflow.py` & `RepoDynamics-0.0.0.dev4/src/repodynamics/workflow.py`

 * *Files identical despite different names*

