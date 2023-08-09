# Comparing `tmp/pyimporters-mesh-0.4.93.tar.gz` & `tmp/pyimporters-mesh-0.4.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimporters-mesh-0.4.93.tar", last modified: Fri Feb 25 10:01:03 2022, max compression
+gzip compressed data, was "pyimporters-mesh-0.4.97.tar", last modified: Fri Feb 25 14:54:51 2022, max compression
```

## Comparing `pyimporters-mesh-0.4.93.tar` & `pyimporters-mesh-0.4.97.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       97 2021-11-23 15:54:25.417461 pyimporters-mesh-0.4.93/.dockerignore
--rw-r--r--   0        0        0      147 2021-11-23 15:54:25.418461 pyimporters-mesh-0.4.93/.gitignore
--rw-r--r--   0        0        0      448 2021-11-23 15:54:25.419461 pyimporters-mesh-0.4.93/Dockerfile
--rw-r--r--   0        0        0    10495 2022-02-25 09:52:00.175486 pyimporters-mesh-0.4.93/Jenkinsfile
--rw-r--r--   0        0        0      148 2021-11-23 15:54:25.421461 pyimporters-mesh-0.4.93/README.md
--rw-r--r--   0        0        0       61 2022-02-25 10:01:02.084697 pyimporters-mesh-0.4.93/pyimporters_mesh/__init__.py
--rw-r--r--   0        0        0     4020 2021-11-23 15:54:25.422461 pyimporters-mesh-0.4.93/pyimporters_mesh/mesh.py
--rw-r--r--   0        0        0     1979 2022-02-25 09:57:53.992767 pyimporters-mesh-0.4.93/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-23 15:54:25.423461 pyimporters-mesh-0.4.93/tests/__init__.py
--rwxr-xr-x   0        0        0     3280 2021-11-23 15:54:25.425461 pyimporters-mesh-0.4.93/tests/data/small.zip
--rw-r--r--   0        0        0     1065 2021-11-23 15:54:25.425461 pyimporters-mesh-0.4.93/tests/test_mesh.py
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 pyimporters-mesh-0.4.93/setup.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 pyimporters-mesh-0.4.93/PKG-INFO
+-rw-r--r--   0        0        0       97 2021-11-23 15:54:25.417461 pyimporters-mesh-0.4.97/.dockerignore
+-rw-r--r--   0        0        0      147 2021-11-23 15:54:25.418461 pyimporters-mesh-0.4.97/.gitignore
+-rw-r--r--   0        0        0      448 2021-11-23 15:54:25.419461 pyimporters-mesh-0.4.97/Dockerfile
+-rw-r--r--   0        0        0    10495 2022-02-25 09:52:00.175486 pyimporters-mesh-0.4.97/Jenkinsfile
+-rw-r--r--   0        0        0      148 2021-11-23 15:54:25.421461 pyimporters-mesh-0.4.97/README.md
+-rw-r--r--   0        0        0       61 2022-02-25 14:54:49.872586 pyimporters-mesh-0.4.97/pyimporters_mesh/__init__.py
+-rw-r--r--   0        0        0     4020 2021-11-23 15:54:25.422461 pyimporters-mesh-0.4.97/pyimporters_mesh/mesh.py
+-rw-r--r--   0        0        0     1981 2022-02-25 14:52:56.153612 pyimporters-mesh-0.4.97/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-23 15:54:25.423461 pyimporters-mesh-0.4.97/tests/__init__.py
+-rwxr-xr-x   0        0        0     3280 2021-11-23 15:54:25.425461 pyimporters-mesh-0.4.97/tests/data/small.zip
+-rw-r--r--   0        0        0     1065 2021-11-23 15:54:25.425461 pyimporters-mesh-0.4.97/tests/test_mesh.py
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 pyimporters-mesh-0.4.97/setup.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 pyimporters-mesh-0.4.97/PKG-INFO
```

### Comparing `pyimporters-mesh-0.4.93/Jenkinsfile` & `pyimporters-mesh-0.4.97/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyimporters-mesh-0.4.93/pyimporters_mesh/mesh.py` & `pyimporters-mesh-0.4.97/pyimporters_mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `pyimporters-mesh-0.4.93/pyproject.toml` & `pyimporters-mesh-0.4.97/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 [tool.flakehell]
 exclude = ["README.md"]
 format = "colored"
 #format = "junit-xml"
 max_line_length = 120
 show_source = true
 #whitelist = "../../allowlist.txt"
-extended_default_ignore=[]
+extended_default_ignore = []
 
 [tool.flakehell.plugins]
 flake8-bandit = ["+*", "-S322"]
 flake8-bugbear = ["+*"]
 flake8-builtins = ["+*"]
 flake8-comprehensions = ["+*"]
 flake8-darglint = ["+*"]
```

### Comparing `pyimporters-mesh-0.4.93/tests/data/small.zip` & `pyimporters-mesh-0.4.97/tests/data/small.zip`

 * *Files identical despite different names*

### Comparing `pyimporters-mesh-0.4.93/tests/test_mesh.py` & `pyimporters-mesh-0.4.97/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `pyimporters-mesh-0.4.93/setup.py` & `pyimporters-mesh-0.4.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = \
 ['pyimporters_plugins>=0.4.0,<0.5.0', 'collections-extended', 'lxml']
 
 entry_points = \
 {'pyimporters.plugins': ['mesh = pyimporters_mesh.mesh:MeSHKnowledgeParser']}
 
 setup(name='pyimporters-mesh',
-      version='0.4.93',
+      version='0.4.97',
       description='Sherpa knowledge import plugins',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyimporters-mesh-0.4.93/PKG-INFO` & `pyimporters-mesh-0.4.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimporters-mesh
-Version: 0.4.93
+Version: 0.4.97
 Summary: Sherpa knowledge import plugins
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

