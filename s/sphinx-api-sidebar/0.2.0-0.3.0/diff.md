# Comparing `tmp/sphinx_api_sidebar-0.2.0.tar.gz` & `tmp/sphinx_api_sidebar-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_api_sidebar-0.2.0.tar", last modified: Wed May 17 07:07:14 2023, max compression
+gzip compressed data, was "sphinx_api_sidebar-0.3.0.tar", last modified: Tue Aug  8 23:24:43 2023, max compression
```

## Comparing `sphinx_api_sidebar-0.2.0.tar` & `sphinx_api_sidebar-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-17 07:07:14.069027 sphinx_api_sidebar-0.2.0/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-05-10 08:31:45.000000 sphinx_api_sidebar-0.2.0/LICENSE
--rw-r--r--   0 yihengxiong   (501) staff       (20)        0 2023-05-10 08:31:45.000000 sphinx_api_sidebar-0.2.0/MANIFEST.in
--rw-r--r--   0 yihengxiong   (501) staff       (20)     4241 2023-05-17 07:07:14.068911 sphinx_api_sidebar-0.2.0/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)     2296 2023-05-17 07:05:53.000000 sphinx_api_sidebar-0.2.0/README.md
--rw-r--r--   0 yihengxiong   (501) staff       (20)      441 2023-05-17 07:02:02.000000 sphinx_api_sidebar-0.2.0/pyproject.toml
--rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-17 07:07:14.069076 sphinx_api_sidebar-0.2.0/setup.cfg
--rw-r--r--   0 yihengxiong   (501) staff       (20)      899 2023-05-17 07:02:12.000000 sphinx_api_sidebar-0.2.0/setup.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-17 07:07:14.067469 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar/
--rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-10 08:59:33.000000 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar/__init__.py
--rw-r--r--   0 yihengxiong   (501) staff       (20)     2513 2023-05-17 06:57:51.000000 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar/sphinx_api_sidebar.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-17 07:07:14.068500 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar.egg-info/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     4241 2023-05-17 07:07:14.000000 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar.egg-info/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)      412 2023-05-17 07:07:14.000000 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar.egg-info/SOURCES.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-05-17 07:07:14.000000 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar.egg-info/dependency_links.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       66 2023-05-17 07:07:14.000000 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar.egg-info/entry_points.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       47 2023-05-17 07:07:14.000000 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar.egg-info/requires.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       19 2023-05-17 07:07:14.000000 sphinx_api_sidebar-0.2.0/sphinx_api_sidebar.egg-info/top_level.txt
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-17 07:07:14.068613 sphinx_api_sidebar-0.2.0/tests/
--rw-r--r--   0 yihengxiong   (501) staff       (20)      557 2023-05-10 09:00:08.000000 sphinx_api_sidebar-0.2.0/tests/test_sphinx_api_sidebar.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-08-08 23:24:43.201001 sphinx_api_sidebar-0.3.0/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-05-10 08:31:45.000000 sphinx_api_sidebar-0.3.0/LICENSE
+-rw-r--r--   0 yihengxiong   (501) staff       (20)        0 2023-05-10 08:31:45.000000 sphinx_api_sidebar-0.3.0/MANIFEST.in
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     4683 2023-08-08 23:24:43.200894 sphinx_api_sidebar-0.3.0/PKG-INFO
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     2738 2023-08-08 23:22:35.000000 sphinx_api_sidebar-0.3.0/README.md
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      441 2023-08-08 23:24:26.000000 sphinx_api_sidebar-0.3.0/pyproject.toml
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-08-08 23:24:43.201036 sphinx_api_sidebar-0.3.0/setup.cfg
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      899 2023-08-08 23:24:30.000000 sphinx_api_sidebar-0.3.0/setup.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-08-08 23:24:43.199848 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-10 08:59:33.000000 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar/__init__.py
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     2513 2023-05-17 06:57:51.000000 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar/sphinx_api_sidebar.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-08-08 23:24:43.200594 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar.egg-info/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     4683 2023-08-08 23:24:43.000000 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar.egg-info/PKG-INFO
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      412 2023-08-08 23:24:43.000000 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar.egg-info/SOURCES.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-08-08 23:24:43.000000 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar.egg-info/dependency_links.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       66 2023-08-08 23:24:43.000000 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar.egg-info/entry_points.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       47 2023-08-08 23:24:43.000000 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar.egg-info/requires.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       19 2023-08-08 23:24:43.000000 sphinx_api_sidebar-0.3.0/sphinx_api_sidebar.egg-info/top_level.txt
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-08-08 23:24:43.200731 sphinx_api_sidebar-0.3.0/tests/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      557 2023-05-10 09:00:08.000000 sphinx_api_sidebar-0.3.0/tests/test_sphinx_api_sidebar.py
```

### Comparing `sphinx_api_sidebar-0.2.0/LICENSE` & `sphinx_api_sidebar-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_api_sidebar-0.2.0/PKG-INFO` & `sphinx_api_sidebar-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_api_sidebar
-Version: 0.2.0
+Version: 0.3.0
 Summary: Display any generated static API documentation in a sidebar
 Home-page: https://github.com/Yihengxiong6/sphinx_api_sidebar
 Author: Yiheng Xiong
 Author-email: Yiheng Xiong <georgex8866@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yiheng Xiong
@@ -96,17 +96,40 @@
   },
   # more groups of generated api docs
 ]
 ```
 
 Replace `<your_custom_build_command_*>`, `<generated_api_doc_name_*>`, and `<path_to_generated_api_doc_*>` with the appropriate values for your project.
 
+Here is a real example with javadoc:
+
+```python
+api_docs_generators = [
+  {
+    'command': 'javadoc -d path/to/doc/dir -sourcepath . -subpackages *',
+    'outputs': [
+            {
+                'name': 'Javadoc',
+                'path': 'path/to/doc/dir' # path should be relative to the docs directory
+            },
+        ]
+  },
+]
+```
+
 3. Update your `conf.py` file to include the `api_docs_sidebar.html` template in the html_sidebars configuration:
 
 ```python
 html_sidebars = {
     '**': [
         # ... other sidebars ...
         'sidebar/api_docs_sidebar.html',
     ]
 }
 ```
+
+4. If you haven't, set html static path as follow:
+
+```python
+html_static_path = ['_static']
+```
+
```

### Comparing `sphinx_api_sidebar-0.2.0/README.md` & `sphinx_api_sidebar-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -56,17 +56,40 @@
   },
   # more groups of generated api docs
 ]
 ```
 
 Replace `<your_custom_build_command_*>`, `<generated_api_doc_name_*>`, and `<path_to_generated_api_doc_*>` with the appropriate values for your project.
 
+Here is a real example with javadoc:
+
+```python
+api_docs_generators = [
+  {
+    'command': 'javadoc -d path/to/doc/dir -sourcepath . -subpackages *',
+    'outputs': [
+            {
+                'name': 'Javadoc',
+                'path': 'path/to/doc/dir' # path should be relative to the docs directory
+            },
+        ]
+  },
+]
+```
+
 3. Update your `conf.py` file to include the `api_docs_sidebar.html` template in the html_sidebars configuration:
 
 ```python
 html_sidebars = {
     '**': [
         # ... other sidebars ...
         'sidebar/api_docs_sidebar.html',
     ]
 }
 ```
+
+4. If you haven't, set html static path as follow:
+
+```python
+html_static_path = ['_static']
+```
+
```

### Comparing `sphinx_api_sidebar-0.2.0/setup.py` & `sphinx_api_sidebar-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name="sphinx_api_sidebar",
     description="Display any generated static API documentation in a sidebar",
-    version="0.2.0",
+    version="0.3.0",
     author="Yiheng Xiong",
     author_email="georgex8866@gmail.com",
     url="https://github.com/Yihengxiong6/sphinx_api_sidebar",
     packages=["sphinx_api_sidebar"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `sphinx_api_sidebar-0.2.0/sphinx_api_sidebar/sphinx_api_sidebar.py` & `sphinx_api_sidebar-0.3.0/sphinx_api_sidebar/sphinx_api_sidebar.py`

 * *Files identical despite different names*

### Comparing `sphinx_api_sidebar-0.2.0/sphinx_api_sidebar.egg-info/PKG-INFO` & `sphinx_api_sidebar-0.3.0/sphinx_api_sidebar.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-api-sidebar
-Version: 0.2.0
+Version: 0.3.0
 Summary: Display any generated static API documentation in a sidebar
 Home-page: https://github.com/Yihengxiong6/sphinx_api_sidebar
 Author: Yiheng Xiong
 Author-email: Yiheng Xiong <georgex8866@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yiheng Xiong
@@ -96,17 +96,40 @@
   },
   # more groups of generated api docs
 ]
 ```
 
 Replace `<your_custom_build_command_*>`, `<generated_api_doc_name_*>`, and `<path_to_generated_api_doc_*>` with the appropriate values for your project.
 
+Here is a real example with javadoc:
+
+```python
+api_docs_generators = [
+  {
+    'command': 'javadoc -d path/to/doc/dir -sourcepath . -subpackages *',
+    'outputs': [
+            {
+                'name': 'Javadoc',
+                'path': 'path/to/doc/dir' # path should be relative to the docs directory
+            },
+        ]
+  },
+]
+```
+
 3. Update your `conf.py` file to include the `api_docs_sidebar.html` template in the html_sidebars configuration:
 
 ```python
 html_sidebars = {
     '**': [
         # ... other sidebars ...
         'sidebar/api_docs_sidebar.html',
     ]
 }
 ```
+
+4. If you haven't, set html static path as follow:
+
+```python
+html_static_path = ['_static']
+```
+
```

### Comparing `sphinx_api_sidebar-0.2.0/tests/test_sphinx_api_sidebar.py` & `sphinx_api_sidebar-0.3.0/tests/test_sphinx_api_sidebar.py`

 * *Files identical despite different names*

