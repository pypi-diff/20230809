# Comparing `tmp/micropub-0.1.2.tar.gz` & `tmp/micropub-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropub-0.1.2.tar", max compression
+gzip compressed data, was "micropub-0.1.3.tar", max compression
```

## Comparing `micropub-0.1.2.tar` & `micropub-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3473 2023-07-20 05:38:30.720873 micropub-0.1.2/micropub/__init__.py
--rw-r--r--   0        0        0     2737 2023-02-13 00:57:16.634666 micropub-0.1.2/micropub/__main__.py
--rw-r--r--   0        0        0      993 2023-08-02 03:47:39.376928 micropub-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 micropub-0.1.2/setup.py
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 micropub-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3473 2023-08-08 23:56:50.474640 micropub-0.1.3/micropub/__init__.py
+-rw-r--r--   0        0        0     2737 2023-08-07 01:15:29.273139 micropub-0.1.3/micropub/__main__.py
+-rw-r--r--   0        0        0     1010 2023-08-08 23:57:17.995061 micropub-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 micropub-0.1.3/setup.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 micropub-0.1.3/PKG-INFO
```

### Comparing `micropub-0.1.2/micropub/__init__.py` & `micropub-0.1.3/micropub/__init__.py`

 * *Files identical despite different names*

### Comparing `micropub-0.1.2/micropub/__main__.py` & `micropub-0.1.3/micropub/__main__.py`

 * *Files identical despite different names*

### Comparing `micropub-0.1.2/pyproject.toml` & `micropub-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropub"
-version = "0.1.2"
+version = "0.1.3"
 description = "utilities to help implement Micropub servers and clients"
 keywords = ["IndieWeb", "Micropub"]
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "0BSD"
 
 [tool.poetry.scripts]
 micropub = "micropub.__main__:main"
@@ -12,14 +12,15 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 requests = "^2.28.2"
 txtint = ">=0.0"
 microformats = ">=0.0"
 indieauth = ">=0.0"
 requests-toolbelt = "^1.0"
+tqdm = "^4.65.2"
 
 [tool.poetry.group.dev.dependencies]
 nuitka = "^1.2.6"
 zstandard = "^0.19.0"
 ordered-set = "^4.1.0"
 gmpg = {path="../gmpg", develop=true}
 txtint = {path="../txtint", develop=true}
```

### Comparing `micropub-0.1.2/setup.py` & `micropub-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['indieauth>=0.0',
  'microformats>=0.0',
  'requests-toolbelt>=1.0,<2.0',
  'requests>=2.28.2,<3.0.0',
+ 'tqdm>=4.65.2,<5.0.0',
  'txtint>=0.0']
 
 entry_points = \
 {'console_scripts': ['micropub = micropub.__main__:main']}
 
 setup_kwargs = {
     'name': 'micropub',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'utilities to help implement Micropub servers and clients',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `micropub-0.1.2/PKG-INFO` & `micropub-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: micropub
-Version: 0.1.2
+Version: 0.1.3
 Summary: utilities to help implement Micropub servers and clients
 License: 0BSD
 Keywords: IndieWeb,Micropub
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: indieauth (>=0.0)
 Requires-Dist: microformats (>=0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0,<2.0)
+Requires-Dist: tqdm (>=4.65.2,<5.0.0)
 Requires-Dist: txtint (>=0.0)
```

