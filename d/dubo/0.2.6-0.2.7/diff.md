# Comparing `tmp/dubo-0.2.6.tar.gz` & `tmp/dubo-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dubo-0.2.6.tar", max compression
+gzip compressed data, was "dubo-0.2.7.tar", max compression
```

## Comparing `dubo-0.2.6.tar` & `dubo-0.2.7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1092 2023-01-05 00:01:04.309003 dubo-0.2.6/LICENSE
--rw-r--r--   0        0        0      171 2023-01-05 05:56:58.393399 dubo-0.2.6/README.md
--rw-r--r--   0        0        0      235 2023-08-08 00:25:26.678841 dubo-0.2.6/dubo/__init__.py
--rw-r--r--   0        0        0      119 2023-08-08 00:25:26.679080 dubo-0.2.6/dubo/__version__.py
--rw-r--r--   0        0        0     5814 2023-08-08 00:25:26.679329 dubo-0.2.6/dubo/ask_dubo.py
--rw-r--r--   0        0        0      474 2023-08-07 22:44:27.019712 dubo-0.2.6/dubo/config.py
--rw-r--r--   0        0        0      592 2023-08-08 00:25:26.679535 dubo-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 dubo-0.2.6/setup.py
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 dubo-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-01-05 00:01:04.309003 dubo-0.2.7/LICENSE
+-rw-r--r--   0        0        0      171 2023-01-05 05:56:58.393399 dubo-0.2.7/README.md
+-rw-r--r--   0        0        0      251 2023-08-08 03:04:33.815436 dubo-0.2.7/dubo/__init__.py
+-rw-r--r--   0        0        0      119 2023-08-08 23:41:15.716405 dubo-0.2.7/dubo/__version__.py
+-rw-r--r--   0        0        0    11106 2023-08-09 00:57:26.774578 dubo-0.2.7/dubo/ask_dubo.py
+-rw-r--r--   0        0        0      739 2023-08-08 23:37:47.216596 dubo-0.2.7/dubo/config.py
+-rw-r--r--   0        0        0      375 2023-08-08 02:51:55.171195 dubo-0.2.7/dubo/entities.py
+-rw-r--r--   0        0        0      665 2023-08-09 00:42:16.302609 dubo-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      869 1970-01-01 00:00:00.000000 dubo-0.2.7/setup.py
+-rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 dubo-0.2.7/PKG-INFO
```

### Comparing `dubo-0.2.6/LICENSE` & `dubo-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dubo-0.2.6/pyproject.toml` & `dubo-0.2.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [tool.poetry]
 name = "dubo"
-version = "0.2.6"
+version = "0.2.7"
 description = "Analytics made simple"
 authors = ["Andrew Duberstein <ajduberstein@gmail.com>", "Andrew Duberstein <duber@mercator.tech>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.0.0"
 altair = "^5.0.1"
 pydeck = "^0.8.0"
+python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 black = "^22.12.0"
 pylint = "^2.15.9"
 jupyterlite = {version = "^0.1.0b17", allow-prereleases = true}
 jupyterlab-server = "^2.18.0"
+vcrpy = "^5.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[flake8]
+max-line-length = 88
```

### Comparing `dubo-0.2.6/setup.py` & `dubo-0.2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 packages = \
 ['dubo']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['altair>=5.0.1,<6.0.0', 'pandas>=1.0.0,<2.0.0', 'pydeck>=0.8.0,<0.9.0']
+['altair>=5.0.1,<6.0.0',
+ 'pandas>=1.0.0,<2.0.0',
+ 'pydeck>=0.8.0,<0.9.0',
+ 'python-dotenv>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'dubo',
-    'version': '0.2.6',
+    'version': '0.2.7',
     'description': 'Analytics made simple',
     'long_description': 'dubo\n====\n\ndubo is a client for running LLMs against DataFrames and other 2D data.\n\nIt is currently in an alpha release and not yet ready for use in production pipelines.\n',
     'author': 'Andrew Duberstein',
     'author_email': 'ajduberstein@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dubo-0.2.6/PKG-INFO` & `dubo-0.2.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dubo
-Version: 0.2.6
+Version: 0.2.7
 Summary: Analytics made simple
 License: MIT
 Author: Andrew Duberstein
 Author-email: ajduberstein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: altair (>=5.0.1,<6.0.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
 Requires-Dist: pydeck (>=0.8.0,<0.9.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 dubo
 ====
 
 dubo is a client for running LLMs against DataFrames and other 2D data.
```

