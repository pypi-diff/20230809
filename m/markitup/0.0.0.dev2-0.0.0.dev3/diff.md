# Comparing `tmp/markitup-0.0.0.dev2.tar.gz` & `tmp/markitup-0.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markitup-0.0.0.dev2.tar", last modified: Mon Aug  7 16:59:19 2023, max compression
+gzip compressed data, was "markitup-0.0.0.dev3.tar", last modified: Tue Aug  8 15:43:39 2023, max compression
```

## Comparing `markitup-0.0.0.dev2.tar` & `markitup-0.0.0.dev3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:19.505415 markitup-0.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 16:59:19.505415 markitup-0.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-07 16:59:10.000000 markitup-0.0.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 16:59:19.505415 markitup-0.0.0.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:19.505415 markitup-0.0.0.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:19.505415 markitup-0.0.0.dev2/src/markitup/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 16:59:10.000000 markitup-0.0.0.dev2/src/markitup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18843 2023-08-07 16:59:10.000000 markitup-0.0.0.dev2/src/markitup/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-07 16:59:10.000000 markitup-0.0.0.dev2/src/markitup/md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 16:59:19.505415 markitup-0.0.0.dev2/src/markitup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-07 16:59:19.000000 markitup-0.0.0.dev2/src/markitup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-07 16:59:19.000000 markitup-0.0.0.dev2/src/markitup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:59:19.000000 markitup-0.0.0.dev2/src/markitup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 16:59:19.000000 markitup-0.0.0.dev2/src/markitup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 16:59:19.000000 markitup-0.0.0.dev2/src/markitup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:43:39.204669 markitup-0.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 15:43:39.204669 markitup-0.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-08 15:43:29.000000 markitup-0.0.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:43:39.204669 markitup-0.0.0.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:43:39.200669 markitup-0.0.0.dev3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:43:39.204669 markitup-0.0.0.dev3/src/markitup/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 15:43:29.000000 markitup-0.0.0.dev3/src/markitup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19185 2023-08-08 15:43:29.000000 markitup-0.0.0.dev3/src/markitup/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-08 15:43:29.000000 markitup-0.0.0.dev3/src/markitup/md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:43:39.204669 markitup-0.0.0.dev3/src/markitup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 15:43:39.000000 markitup-0.0.0.dev3/src/markitup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-08 15:43:39.000000 markitup-0.0.0.dev3/src/markitup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:43:39.000000 markitup-0.0.0.dev3/src/markitup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:43:38.000000 markitup-0.0.0.dev3/src/markitup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 15:43:39.000000 markitup-0.0.0.dev3/src/markitup.egg-info/top_level.txt
```

### Comparing `markitup-0.0.0.dev2/pyproject.toml` & `markitup-0.0.0.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 where = ["src"]
 namespaces = true
 
 
 # ----------------------------------------- Project Metadata -------------------------------------
 #
 [project]
-version = "0.0.0.dev2"
+version = "0.0.0.dev3"
 name = "markitup"
 requires-python = ">=3.9"
```

### Comparing `markitup-0.0.0.dev2/src/markitup/html.py` & `markitup-0.0.0.dev3/src/markitup/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,17 +526,20 @@
         type: Literal["disc", "circle", "square"] = "disc",
         tag_seperator: Optional[str] = "\n",
         content_indent: Optional[str] = "\t",
         **attrs,
     ):
         attrs["type"] = type
         if isinstance(content, str):
-            content = [LI(content=content)]
+            content = [LI(content=content, tag_seperator=tag_seperator, content_indent=content_indent)]
         elif isinstance(content, Sequence):
-            content = [LI(content=li) for li in content]
+            content = [
+                LI(content=content, tag_seperator=tag_seperator, content_indent=content_indent)
+                for li in content
+            ]
         super().__init__(
             tag=f"ul",
             attrs=attrs,
             content=content,
             tag_seperator=tag_seperator,
             content_indent=content_indent,
         )
@@ -568,17 +571,20 @@
         content_indent: Optional[str] = "\t",
         **attrs,
     ):
         attrs["type"] = type
         attrs["start"] = start
         attrs["reversed"] = reversed
         if isinstance(content, str):
-            content = [LI(content=content)]
+            content = [LI(content=content, tag_seperator=tag_seperator, content_indent=content_indent)]
         elif isinstance(content, Sequence):
-            content = [LI(content=li) for li in content]
+            content = [
+                LI(content=content, tag_seperator=tag_seperator, content_indent=content_indent)
+                for li in content
+            ]
         super().__init__(
             tag=f"ol",
             attrs=attrs,
             content=content,
             tag_seperator=tag_seperator,
             content_indent=content_indent,
         )
```

