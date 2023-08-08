# Comparing `tmp/RepoDynamics-0.0.0.dev5.tar.gz` & `tmp/RepoDynamics-0.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepoDynamics-0.0.0.dev5.tar", last modified: Tue Aug  8 22:53:29 2023, max compression
+gzip compressed data, was "RepoDynamics-0.0.0.dev6.tar", last modified: Tue Aug  8 23:09:18 2023, max compression
```

## Comparing `RepoDynamics-0.0.0.dev5.tar` & `RepoDynamics-0.0.0.dev6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.860682 RepoDynamics-0.0.0.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/src/repodynamics/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/cd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/src/repodynamics/files/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/format_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:09:18.212876 RepoDynamics-0.0.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 23:09:18.212876 RepoDynamics-0.0.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:09:18.212876 RepoDynamics-0.0.0.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:09:18.208876 RepoDynamics-0.0.0.dev6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:09:18.212876 RepoDynamics-0.0.0.dev6/src/RepoDynamics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 23:09:18.000000 RepoDynamics-0.0.0.dev6/src/RepoDynamics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-08 23:09:18.000000 RepoDynamics-0.0.0.dev6/src/RepoDynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:09:18.000000 RepoDynamics-0.0.0.dev6/src/RepoDynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:09:17.000000 RepoDynamics-0.0.0.dev6/src/RepoDynamics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 23:09:18.000000 RepoDynamics-0.0.0.dev6/src/RepoDynamics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 23:09:18.000000 RepoDynamics-0.0.0.dev6/src/RepoDynamics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:09:18.212876 RepoDynamics-0.0.0.dev6/src/repodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:09:18.212876 RepoDynamics-0.0.0.dev6/src/repodynamics/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/actions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/actions/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/actions/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/actions/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/cd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:09:18.212876 RepoDynamics-0.0.0.dev6/src/repodynamics/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/files/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/files/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/files/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/format_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 23:09:10.000000 RepoDynamics-0.0.0.dev6/src/repodynamics/workflow.py
```

### Comparing `RepoDynamics-0.0.0.dev5/pyproject.toml` & `RepoDynamics-0.0.0.dev6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 where = ["src"]
 namespaces = true
 
 
 # ----------------------------------------- Project Metadata -------------------------------------
 #
 [project]
-version = "0.0.0.dev5"
+version = "0.0.0.dev6"
 name = "RepoDynamics"
 #dependencies = [
 #    # https://yaml.readthedocs.io/en/stable/
 #    "ruamel.yaml >= 0.17.32, < 0.18",
 #    # https://tomlkit.readthedocs.io/en/stable/
 #    "tomlkit >= 0.11.8, < 0.12",
 #    "trove-classifiers",
```

### Comparing `RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/SOURCES.txt` & `RepoDynamics-0.0.0.dev6/src/RepoDynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/__main__.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/__main__.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/actions/__main__.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/actions/__main__.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/actions/context.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/actions/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,10 +12,10 @@
         content_indent=""
     )
     payload_details = html.details(
         content=md.code_block(json.dumps(dict(sorted(payload_data.items())), indent=4), "json"),
         summary="🖥 Event Payload",
         content_indent=""
     )
-    return None, f"{context_details}\n{payload_details}"
+    return None, f"<h3>Workflow Context</h3>{context_details}\n{payload_details}"
```

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/actions/io.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/actions/io.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/actions/meta.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/actions/meta.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/ansi.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/ansi.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/cd.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/cd.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/files/__main__.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/files/__main__.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/files/pyproject.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/files/pyproject.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/files/readme.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/files/readme.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/files/templates.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/files/templates.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/format_issue.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/format_issue.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/metadata.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/metadata.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev5/src/repodynamics/workflow.py` & `RepoDynamics-0.0.0.dev6/src/repodynamics/workflow.py`

 * *Files identical despite different names*

