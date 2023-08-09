# Comparing `tmp/ryetest-0.1.0.tar.gz` & `tmp/ryetest-0.2.0.tar.gz`

## Comparing `ryetest-0.1.0.tar` & `ryetest-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ryetest-0.1.0/.python-version
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ryetest-0.1.0/cli.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ryetest-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ryetest-0.1.0/requirements.lock
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ryetest-0.1.0/src/ryetest/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 ryetest-0.1.0/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ryetest-0.1.0/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 ryetest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 ryetest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ryetest-0.2.0/.python-version
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ryetest-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 ryetest-0.2.0/requirements.lock
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 ryetest-0.2.0/src/ryetest/__init__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ryetest-0.2.0/src/ryetest/cli.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 ryetest-0.2.0/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ryetest-0.2.0/README.md
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 ryetest-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 ryetest-0.2.0/PKG-INFO
```

### Comparing `ryetest-0.1.0/pyproject.toml` & `ryetest-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ryetest"
-version = "0.1.0"
+version = "0.2.0"
 description = "Add a short description here"
 authors = [{ name = "lijc210", email = "lijc210@163.com" }]
 dependencies = ["requests~=2.31.0", "flask~=2.3.2", "click~=8.1.6"]
 readme = "README.md"
 requires-python = ">= 3.9"
 
 [build-system]
```

