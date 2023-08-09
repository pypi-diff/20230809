# Comparing `tmp/xmltread-0.2.tar.gz` & `tmp/xmltread-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmltread-0.2.tar", last modified: Wed Jul 26 03:19:52 2023, max compression
+gzip compressed data, was "xmltread-0.3.tar", last modified: Wed Aug  9 03:05:16 2023, max compression
```

## Comparing `xmltread-0.2.tar` & `xmltread-0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-26 03:19:52.824470 xmltread-0.2/
--rw-rw-r--   0 pj        (1000) pj        (1000)    35149 2023-07-25 04:53:13.000000 xmltread-0.2/LICENSE
--rw-rw-r--   0 pj        (1000) pj        (1000)    44046 2023-07-26 03:19:52.820470 xmltread-0.2/PKG-INFO
--rw-rw-r--   0 pj        (1000) pj        (1000)     2571 2023-07-25 22:31:44.000000 xmltread-0.2/README.md
--rw-rw-r--   0 pj        (1000) pj        (1000)     1038 2023-07-26 03:19:31.000000 xmltread-0.2/pyproject.toml
--rw-rw-r--   0 pj        (1000) pj        (1000)       38 2023-07-26 03:19:52.824470 xmltread-0.2/setup.cfg
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-26 03:19:52.820470 xmltread-0.2/tests/
--rw-rw-r--   0 pj        (1000) pj        (1000)     4822 2023-07-25 07:11:58.000000 xmltread-0.2/tests/test_orig.py
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-26 03:19:52.820470 xmltread-0.2/xmltread/
--rw-rw-r--   0 pj        (1000) pj        (1000)       24 2023-07-25 05:13:34.000000 xmltread-0.2/xmltread/__init__.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     1616 2023-07-25 23:05:19.000000 xmltread-0.2/xmltread/seeder.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     7861 2023-07-26 03:19:31.000000 xmltread-0.2/xmltread/xmltramp.py
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-26 03:19:52.820470 xmltread-0.2/xmltread.egg-info/
--rw-rw-r--   0 pj        (1000) pj        (1000)    44046 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/PKG-INFO
--rw-rw-r--   0 pj        (1000) pj        (1000)      271 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/SOURCES.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)        1 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/dependency_links.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)       44 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/requires.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)        9 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/top_level.txt
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-08-09 03:05:16.656808 xmltread-0.3/
+-rw-rw-r--   0 pj        (1000) pj        (1000)    35149 2023-07-25 04:53:13.000000 xmltread-0.3/LICENSE
+-rw-rw-r--   0 pj        (1000) pj        (1000)    44046 2023-08-09 03:05:16.656808 xmltread-0.3/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2571 2023-07-25 22:31:44.000000 xmltread-0.3/README.md
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1038 2023-08-09 03:04:48.000000 xmltread-0.3/pyproject.toml
+-rw-rw-r--   0 pj        (1000) pj        (1000)       38 2023-08-09 03:05:16.656808 xmltread-0.3/setup.cfg
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-08-09 03:05:16.656808 xmltread-0.3/tests/
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4822 2023-07-25 07:11:58.000000 xmltread-0.3/tests/test_orig.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)      702 2023-08-09 02:54:40.000000 xmltread-0.3/tests/test_utils.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-08-09 03:05:16.656808 xmltread-0.3/xmltread/
+-rw-rw-r--   0 pj        (1000) pj        (1000)       45 2023-08-03 20:03:51.000000 xmltread-0.3/xmltread/__init__.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1616 2023-07-25 23:05:19.000000 xmltread-0.3/xmltread/seeder.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1192 2023-08-03 22:19:18.000000 xmltread-0.3/xmltread/utils.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     7909 2023-08-03 20:29:53.000000 xmltread-0.3/xmltread/xmltramp.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-08-09 03:05:16.656808 xmltread-0.3/xmltread.egg-info/
+-rw-rw-r--   0 pj        (1000) pj        (1000)    44046 2023-08-09 03:05:16.000000 xmltread-0.3/xmltread.egg-info/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)      309 2023-08-09 03:05:16.000000 xmltread-0.3/xmltread.egg-info/SOURCES.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)        1 2023-08-09 03:05:16.000000 xmltread-0.3/xmltread.egg-info/dependency_links.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       44 2023-08-09 03:05:16.000000 xmltread-0.3/xmltread.egg-info/requires.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)        9 2023-08-09 03:05:16.000000 xmltread-0.3/xmltread.egg-info/top_level.txt
```

### Comparing `xmltread-0.2/LICENSE` & `xmltread-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xmltread-0.2/PKG-INFO` & `xmltread-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmltread
-Version: 0.2
+Version: 0.3
 Summary: Make XML documents more easily accessible
 Author-email: Aaron Swartz <me@aaronsw.com>, Paul Jimenez <pj@place.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `xmltread-0.2/README.md` & `xmltread-0.3/README.md`

 * *Files identical despite different names*

### Comparing `xmltread-0.2/pyproject.toml` & `xmltread-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xmltread"
-version = "0.2"
+version = "0.3"
 requires-python = ">=3.8"
 description = "Make XML documents more easily accessible"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Aaron Swartz", email = "me@aaronsw.com"},
     {name = "Paul Jimenez", email = "pj@place.org"}
```

### Comparing `xmltread-0.2/tests/test_orig.py` & `xmltread-0.3/tests/test_orig.py`

 * *Files identical despite different names*

### Comparing `xmltread-0.2/xmltread/seeder.py` & `xmltread-0.3/xmltread/seeder.py`

 * *Files identical despite different names*

### Comparing `xmltread-0.2/xmltread/xmltramp.py` & `xmltread-0.3/xmltread/xmltramp.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,21 +48,17 @@
 
 
 class Element:
     def __init__(self, name, attrs=None, children=None, prefixes=None):
         if islst(name) and name[0] is None:
             name = name[1]
         if attrs:
-            na = {}
-            for k in attrs:
-                if islst(k) and k[0] is None:
-                    na[k[1]] = attrs[k]
-                else:
-                    na[k] = attrs[k]
-            attrs = na
+            attrs = {
+                (k[1] if islst(k) and k[0] is None else k): v for k, v in attrs.items()
+            }
 
         self._name = name
         self._attrs = attrs or {}
         self._dir = children or []
 
         prefixes = prefixes or {}
         self._prefixes = dict(zip(prefixes.values(), prefixes.keys()))
@@ -235,22 +231,26 @@
             # delete first foo
             for i in range(len(self)):
                 if self[i]._name == n:
                     del self[i]
                 break
 
     def __call__(self, *_pos, **_set):
+        # set kw params
         if _set:
             for k in _set.keys():
                 self._attrs[k] = _set[k]
+        # set k, v pairs of positional params
         if len(_pos) > 1:
             for i in range(0, len(_pos), 2):
                 self._attrs[_pos[i]] = _pos[i + 1]
+        # get the attr specified by the param
         if len(_pos) == 1:
             return self._attrs[_pos[0]]
+        # get all attrs
         if len(_pos) == 0:
             return self._attrs
 
     def __len__(self):
         return len(self._dir)
```

### Comparing `xmltread-0.2/xmltread.egg-info/PKG-INFO` & `xmltread-0.3/xmltread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmltread
-Version: 0.2
+Version: 0.3
 Summary: Make XML documents more easily accessible
 Author-email: Aaron Swartz <me@aaronsw.com>, Paul Jimenez <pj@place.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

