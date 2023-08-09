# Comparing `tmp/opprint-1.0.2.tar.gz` & `tmp/opprint-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opprint-1.0.2.tar", max compression
+gzip compressed data, was "opprint-1.0.3.tar", max compression
```

## Comparing `opprint-1.0.2.tar` & `opprint-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1073 2022-10-16 22:29:35.497596 opprint-1.0.2/LICENSE
--rw-r--r--   0        0        0      433 2022-10-21 21:54:41.313857 opprint-1.0.2/README.md
--rw-r--r--   0        0        0      566 2022-10-21 22:01:15.520663 opprint-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      807 2022-10-17 23:24:05.157641 opprint-1.0.2/src/opPrint.py
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 opprint-1.0.2/setup.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 opprint-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-10-16 22:29:35.497596 opprint-1.0.3/LICENSE
+-rw-r--r--   0        0        0      433 2023-08-09 04:03:37.284546 opprint-1.0.3/README.md
+-rw-r--r--   0        0        0      566 2023-08-09 04:06:07.866886 opprint-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-08-09 04:03:50.464401 opprint-1.0.3/src/opprint.py
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 opprint-1.0.3/PKG-INFO
```

### Comparing `opprint-1.0.2/LICENSE` & `opprint-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opprint-1.0.2/pyproject.toml` & `opprint-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["poetry-core~=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-name = "opPrint"
-version = "1.0.2"
+name = "opprint"
+version = "1.0.3"
 authors = [
   "rapid537 <rapid537@zoho.com>",
 ]
 description = "Override print formatter"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 homepage = "https://github.com/rapid537/op.git"
 packages = [
-    { include = "opPrint.py", from = "src" }
+    { include = "opprint.py", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 PyYAML = "^6.0"
```

### Comparing `opprint-1.0.2/src/opPrint.py` & `opprint-1.0.3/src/opprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,9 +21,9 @@
             if yml:
                 return print('\n', yaml.dump(label_or_var))
             return print('\n', pprint.pformat(label_or_var))
         if var:
             return print(f'\n{label_or_var}\n', var, '\n')
         return print('\n', label_or_var, '\n')
     except Exception as error:
-        print('\nopPrint internal error...')
+        print('\nopprint internal error...')
         print(error, '\n')
```

### Comparing `opprint-1.0.2/PKG-INFO` & `opprint-1.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: opprint
-Version: 1.0.2
+Version: 1.0.3
 Summary: Override print formatter
 Home-page: https://github.com/rapid537/op.git
 Author: rapid537
 Author-email: rapid537@zoho.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 ## installation ##
 ```
 python3 -m pip install opprint
 ```
 
 ## usage ##
 op(***arg***, ***var***=None, ***format***=False, ***yml***=False)
 ```
-from opPrint import op
+from opprint import op
 greeting = 'hello world!'
 
 # basic
 op(greeting)
 
 # with label
 op('op says...', greeting)
```

