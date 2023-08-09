# Comparing `tmp/hdx_python_database-1.2.4.tar.gz` & `tmp/hdx_python_database-1.2.5.tar.gz`

## Comparing `hdx_python_database-1.2.4.tar` & `hdx_python_database-1.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     1520 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0     4060 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/documentation/main.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/_version.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/dburi.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/no_timezone.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/postgresql.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/src/hdx/database/with_timezone.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/conftest.py
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/dbtestdate.py
--rwxr-xr-x   0        0        0     3720 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/test_database.py
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/test_dburi.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/tests/hdx/database/test_postgresql.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/LICENSE
--rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/README.md
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 hdx_python_database-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     1520 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0     4060 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/documentation/main.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/src/hdx/database/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/src/hdx/database/_version.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/src/hdx/database/dburi.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/src/hdx/database/no_timezone.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/src/hdx/database/postgresql.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/src/hdx/database/with_timezone.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/tests/hdx/database/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/tests/hdx/database/conftest.py
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/tests/hdx/database/dbtestdate.py
+-rwxr-xr-x   0        0        0     3720 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/tests/hdx/database/test_database.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/tests/hdx/database/test_dburi.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/tests/hdx/database/test_postgresql.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/LICENSE
+-rwxr-xr-x   0        0        0     1249 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/README.md
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 hdx_python_database-1.2.5/PKG-INFO
```

### Comparing `hdx_python_database-1.2.4/CONTRIBUTING.md` & `hdx_python_database-1.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/requirements.txt` & `hdx_python_database-1.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/.config/pre-commit-config.yaml` & `hdx_python_database-1.2.5/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/.github/workflows/publish.yaml` & `hdx_python_database-1.2.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/.github/workflows/run-python-tests.yaml` & `hdx_python_database-1.2.5/.github/workflows/run-python-tests.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # This workflow will install Python dependencies, lint and run tests
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Run tests
 
 on:
+  workflow_dispatch: # add run button in github
   push:
     branches-ignore:
       - gh-pages
+      - 'dependabot/**'
   pull_request:
     branches-ignore:
       - gh-pages
 
 jobs:
   build:
     runs-on: ubuntu-latest
```

### Comparing `hdx_python_database-1.2.4/documentation/main.md` & `hdx_python_database-1.2.5/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/documentation/pydoc-markdown.yaml` & `hdx_python_database-1.2.5/documentation/pydoc-markdown.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     packages:
       - hdx.database
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python Database
-    theme: readthedocs
+    theme: mkdocs
     repo_url: "https://github.com/OCHA-DAP/hdx-python-database"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-database
   pages:
     - title: Home
```

### Comparing `hdx_python_database-1.2.4/src/hdx/database/__init__.py` & `hdx_python_database-1.2.5/src/hdx/database/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/src/hdx/database/dburi.py` & `hdx_python_database-1.2.5/src/hdx/database/dburi.py`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/src/hdx/database/no_timezone.py` & `hdx_python_database-1.2.5/src/hdx/database/no_timezone.py`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/src/hdx/database/postgresql.py` & `hdx_python_database-1.2.5/src/hdx/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/tests/hdx/database/dbtestdate.py` & `hdx_python_database-1.2.5/tests/hdx/database/dbtestdate.py`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/tests/hdx/database/test_database.py` & `hdx_python_database-1.2.5/tests/hdx/database/test_database.py`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/tests/hdx/database/test_dburi.py` & `hdx_python_database-1.2.5/tests/hdx/database/test_dburi.py`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/.gitignore` & `hdx_python_database-1.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/LICENSE` & `hdx_python_database-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/README.md` & `hdx_python_database-1.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-database/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-database?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Downloads](https://img.shields.io/pypi/dm/hdx-python-database.svg)](https://pypistats.org/packages/hdx-python-database)
 
 The HDX Python Database Library provides utilities for connecting to databases in a standard way including
 through an ssh tunnel if needed. It is built on top of SQLAlchemy and simplifies its setup. 
 
 For more information, please read the [documentation](https://hdx-python-database.readthedocs.io/en/latest/).
 
 This library is part of the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) project. If you have
```

### Comparing `hdx_python_database-1.2.4/pyproject.toml` & `hdx_python_database-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx_python_database-1.2.4/PKG-INFO` & `hdx_python_database-1.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-database
-Version: 1.2.4
+Version: 1.2.5
 Summary: HDX Python database utilities
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-database
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,database,postgresql
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,14 +36,15 @@
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-database/actions/workflows/run-python-tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-database/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-database?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![Downloads](https://img.shields.io/pypi/dm/hdx-python-database.svg)](https://pypistats.org/packages/hdx-python-database)
 
 The HDX Python Database Library provides utilities for connecting to databases in a standard way including
 through an ssh tunnel if needed. It is built on top of SQLAlchemy and simplifies its setup. 
 
 For more information, please read the [documentation](https://hdx-python-database.readthedocs.io/en/latest/).
 
 This library is part of the [Humanitarian Data Exchange](https://data.humdata.org/) (HDX) project. If you have
```

