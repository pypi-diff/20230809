# Comparing `tmp/circuitree-0.4.1.tar.gz` & `tmp/circuitree-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.4.1.tar", max compression
+gzip compressed data, was "circuitree-0.5.0.tar", max compression
```

## Comparing `circuitree-0.4.1.tar` & `circuitree-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.4.1/LICENSE
--rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.4.1/README.md
--rwxr-xr-x   0        0        0      117 2023-06-23 05:39:39.142840 circuitree-0.4.1/circuitree/__init__.py
--rwxr-xr-x   0        0        0    18064 2023-07-19 18:42:14.554281 circuitree-0.4.1/circuitree/circuitree.py
--rw-r--r--   0        0        0     1230 2023-07-19 21:27:11.130891 circuitree-0.4.1/circuitree/metrics.py
--rwxr-xr-x   0        0        0    17267 2023-07-18 22:26:33.157080 circuitree-0.4.1/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.4.1/circuitree/modularity.py
--rw-r--r--   0        0        0     9971 2023-07-19 23:52:50.067895 circuitree-0.4.1/circuitree/parallel.py
--rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.4.1/circuitree/regret.py
--rw-r--r--   0        0        0     1442 2023-06-23 05:30:14.382829 circuitree-0.4.1/circuitree/utils.py
--rw-r--r--   0        0        0    10391 2023-06-28 20:54:12.669759 circuitree-0.4.1/circuitree/viz.py
--rw-r--r--   0        0        0     1813 2023-07-19 23:56:21.017826 circuitree-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 circuitree-0.4.1/setup.py
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 circuitree-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 23:12:20.534641 circuitree-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1011 2023-08-08 23:12:20.534641 circuitree-0.5.0/README.md
+-rwxr-xr-x   0        0        0      117 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    18064 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/circuitree.py
+-rw-r--r--   0        0        0     1230 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/metrics.py
+-rwxr-xr-x   0        0        0    17267 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/modularity.py
+-rw-r--r--   0        0        0     9971 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/parallel.py
+-rw-r--r--   0        0        0      267 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/regret.py
+-rw-r--r--   0        0        0     1442 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/utils.py
+-rw-r--r--   0        0        0    10391 2023-08-08 23:12:20.534641 circuitree-0.5.0/circuitree/viz.py
+-rw-r--r--   0        0        0     1785 2023-08-08 23:58:23.053541 circuitree-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 circuitree-0.5.0/setup.py
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 circuitree-0.5.0/PKG-INFO
```

### Comparing `circuitree-0.4.1/LICENSE` & `circuitree-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/README.md` & `circuitree-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/circuitree/circuitree.py` & `circuitree-0.5.0/circuitree/circuitree.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/circuitree/metrics.py` & `circuitree-0.5.0/circuitree/metrics.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/circuitree/models.py` & `circuitree-0.5.0/circuitree/models.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/circuitree/modularity.py` & `circuitree-0.5.0/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/circuitree/parallel.py` & `circuitree-0.5.0/circuitree/parallel.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/circuitree/utils.py` & `circuitree-0.5.0/circuitree/utils.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/circuitree/viz.py` & `circuitree-0.5.0/circuitree/viz.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.4.1/pyproject.toml` & `circuitree-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuitree"
-version = "0.4.1"
+version = "0.5.0"
 description = "Genetic circuit design using Monte Carlo tree search"
 authors = ["pranav-bhamidipati <pbhamidi@usc.edu>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -60,8 +60,7 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [virtualenvs]
 in-project = true
-prefer-active-python = true
```

### Comparing `circuitree-0.4.1/setup.py` & `circuitree-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
               'pandas>=2.0.0,<3.0.0',
               'tables>=3.8.0,<4.0.0',
               'pyarrow>=12.0.0,<13.0.0',
               'h5py>=3.8.0,<4.0.0']}
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'Genetic circuit design using Monte Carlo tree search',
     'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `circuitree-0.4.1/PKG-INFO` & `circuitree-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.4.1
+Version: 0.5.0
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

