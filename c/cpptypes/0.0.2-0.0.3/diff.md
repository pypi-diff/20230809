# Comparing `tmp/cpptypes-0.0.2.tar.gz` & `tmp/cpptypes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpptypes-0.0.2.tar", last modified: Mon Aug  7 19:23:46 2023, max compression
+gzip compressed data, was "cpptypes-0.0.3.tar", last modified: Wed Aug  9 05:16:23 2023, max compression
```

## Comparing `cpptypes-0.0.2.tar` & `cpptypes-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:23:46.896204 cpptypes-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-07 19:23:18.000000 cpptypes-0.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:23:46.884204 cpptypes-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:23:46.892204 cpptypes-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-07 19:23:18.000000 cpptypes-0.0.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-07 19:23:18.000000 cpptypes-0.0.2/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-07 19:23:18.000000 cpptypes-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-07 19:23:18.000000 cpptypes-0.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-07 19:23:18.000000 cpptypes-0.0.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 19:23:18.000000 cpptypes-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-08-07 19:23:18.000000 cpptypes-0.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-07 19:23:18.000000 cpptypes-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-07 19:23:46.896204 cpptypes-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-08-07 19:23:18.000000 cpptypes-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-07 19:23:18.000000 cpptypes-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-07 19:23:46.896204 cpptypes-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-07 19:23:18.000000 cpptypes-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:23:46.884204 cpptypes-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:23:46.892204 cpptypes-0.0.2/src/cpptypes/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-07 19:23:18.000000 cpptypes-0.0.2/src/cpptypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-07 19:23:18.000000 cpptypes-0.0.2/src/cpptypes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-07 19:23:18.000000 cpptypes-0.0.2/src/cpptypes/create_cpp_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-07 19:23:18.000000 cpptypes-0.0.2/src/cpptypes/create_py_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-08-07 19:23:18.000000 cpptypes-0.0.2/src/cpptypes/parse_cpp_exports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:23:46.896204 cpptypes-0.0.2/src/cpptypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-07 19:23:46.000000 cpptypes-0.0.2/src/cpptypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-07 19:23:46.000000 cpptypes-0.0.2/src/cpptypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:23:46.000000 cpptypes-0.0.2/src/cpptypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 19:23:46.000000 cpptypes-0.0.2/src/cpptypes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:23:46.000000 cpptypes-0.0.2/src/cpptypes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-07 19:23:46.000000 cpptypes-0.0.2/src/cpptypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 19:23:46.000000 cpptypes-0.0.2/src/cpptypes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:23:46.896204 cpptypes-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-07 19:23:18.000000 cpptypes-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-07 19:23:18.000000 cpptypes-0.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-07 19:23:18.000000 cpptypes-0.0.2/tests/test_create_cpp_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-08-07 19:23:18.000000 cpptypes-0.0.2/tests/test_create_py_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-07 19:23:18.000000 cpptypes-0.0.2/tests/test_parse_cpp_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-07 19:23:18.000000 cpptypes-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:16:22.997549 cpptypes-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-09 05:15:54.000000 cpptypes-0.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:16:22.993549 cpptypes-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:16:22.997549 cpptypes-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-09 05:15:54.000000 cpptypes-0.0.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-09 05:15:54.000000 cpptypes-0.0.3/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-09 05:15:54.000000 cpptypes-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-09 05:15:54.000000 cpptypes-0.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-09 05:15:54.000000 cpptypes-0.0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-09 05:15:54.000000 cpptypes-0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-08-09 05:15:54.000000 cpptypes-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-09 05:15:54.000000 cpptypes-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-09 05:16:22.997549 cpptypes-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-08-09 05:15:54.000000 cpptypes-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-09 05:15:54.000000 cpptypes-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-09 05:16:22.997549 cpptypes-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-09 05:15:54.000000 cpptypes-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:16:22.993549 cpptypes-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:16:22.997549 cpptypes-0.0.3/src/cpptypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-09 05:15:54.000000 cpptypes-0.0.3/src/cpptypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-09 05:15:54.000000 cpptypes-0.0.3/src/cpptypes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-09 05:15:54.000000 cpptypes-0.0.3/src/cpptypes/create_cpp_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-08-09 05:15:54.000000 cpptypes-0.0.3/src/cpptypes/create_py_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-08-09 05:15:54.000000 cpptypes-0.0.3/src/cpptypes/parse_cpp_exports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:16:22.997549 cpptypes-0.0.3/src/cpptypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-09 05:16:22.000000 cpptypes-0.0.3/src/cpptypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-09 05:16:22.000000 cpptypes-0.0.3/src/cpptypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 05:16:22.000000 cpptypes-0.0.3/src/cpptypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-09 05:16:22.000000 cpptypes-0.0.3/src/cpptypes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 05:16:22.000000 cpptypes-0.0.3/src/cpptypes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-09 05:16:22.000000 cpptypes-0.0.3/src/cpptypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-09 05:16:22.000000 cpptypes-0.0.3/src/cpptypes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:16:22.997549 cpptypes-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-09 05:15:54.000000 cpptypes-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-09 05:15:54.000000 cpptypes-0.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-09 05:15:54.000000 cpptypes-0.0.3/tests/test_create_cpp_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-08-09 05:15:54.000000 cpptypes-0.0.3/tests/test_create_py_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-09 05:15:54.000000 cpptypes-0.0.3/tests/test_parse_cpp_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-09 05:15:54.000000 cpptypes-0.0.3/tox.ini
```

### Comparing `cpptypes-0.0.2/.coveragerc` & `cpptypes-0.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/.github/workflows/pypi-publish.yml` & `cpptypes-0.0.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/.github/workflows/pypi-test.yml` & `cpptypes-0.0.3/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/.gitignore` & `cpptypes-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/.readthedocs.yml` & `cpptypes-0.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/CONTRIBUTING.md` & `cpptypes-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/LICENSE` & `cpptypes-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/PKG-INFO` & `cpptypes-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpptypes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automatically creates the C++ and Python-side wrappers for ctypes bindings.
 Home-page: https://github.com/biocpy/cpptypes
 Author: Aaron Lun
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/cpptypes
 Platform: any
```

### Comparing `cpptypes-0.0.2/README.md` & `cpptypes-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/setup.cfg` & `cpptypes-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/setup.py` & `cpptypes-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/src/cpptypes/__init__.py` & `cpptypes-0.0.3/src/cpptypes/__init__.py`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/src/cpptypes/__main__.py` & `cpptypes-0.0.3/src/cpptypes/__main__.py`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/src/cpptypes/create_cpp_bindings.py` & `cpptypes-0.0.3/src/cpptypes/create_cpp_bindings.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     # Generating the C++ bindings for each function.
     with open(output_path, "w") as handle:
         handle.write("""/* DO NOT MODIFY: this is automatically generated by the cpptypes */
 
 #include <cstring>
 #include <stdexcept>
+#include <cstdint>
 
 #ifdef _WIN32
 #define PYAPI __declspec(dllexport)
 #else
 #define PYAPI
 #endif
```

### Comparing `cpptypes-0.0.2/src/cpptypes/create_py_bindings.py` & `cpptypes-0.0.3/src/cpptypes/create_py_bindings.py`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/src/cpptypes/parse_cpp_exports.py` & `cpptypes-0.0.3/src/cpptypes/parse_cpp_exports.py`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/src/cpptypes.egg-info/PKG-INFO` & `cpptypes-0.0.3/src/cpptypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpptypes
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automatically creates the C++ and Python-side wrappers for ctypes bindings.
 Home-page: https://github.com/biocpy/cpptypes
 Author: Aaron Lun
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/cpptypes
 Platform: any
```

### Comparing `cpptypes-0.0.2/src/cpptypes.egg-info/SOURCES.txt` & `cpptypes-0.0.3/src/cpptypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/tests/test_create_cpp_bindings.py` & `cpptypes-0.0.3/tests/test_create_cpp_bindings.py`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/tests/test_create_py_bindings.py` & `cpptypes-0.0.3/tests/test_create_py_bindings.py`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/tests/test_parse_cpp_exports.py` & `cpptypes-0.0.3/tests/test_parse_cpp_exports.py`

 * *Files identical despite different names*

### Comparing `cpptypes-0.0.2/tox.ini` & `cpptypes-0.0.3/tox.ini`

 * *Files identical despite different names*

