# Comparing `tmp/hdx_python_country-3.5.1.tar.gz` & `tmp/hdx_python_country-3.5.2.tar.gz`

## Comparing `hdx_python_country-3.5.1.tar` & `hdx_python_country-3.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/documentation/.readthedocs.yaml
--rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/documentation/main.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0    67466 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/_version.py
--rwxr-xr-x   0        0        0    12372 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/adminlevel.py
--rwxr-xr-x   0        0        0    32382 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/country.py
--rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/currency.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/names.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/src/hdx/location/phonetics.py
--rwxr-xr-x   0        0        0    22035 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/fixtures/adminlevel.yaml
--rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/fixtures/secondary_historic_rates.csv
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/fixtures/secondary_rates.json
--rwxr-xr-x   0        0        0    65717 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/Countries_UZB_Deleted.csv
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/__init__.py
--rwxr-xr-x   0        0        0     4457 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/test_adminlevel.py
--rwxr-xr-x   0        0        0    30396 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/test_country.py
--rwxr-xr-x   0        0        0     9462 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/tests/hdx/location/test_currency.py
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/.gitignore
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/LICENSE
--rwxr-xr-x   0        0        0     2306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/README.md
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/pyproject.toml
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 hdx_python_country-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     3966 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/documentation/main.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0    67466 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/src/hdx/location/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/src/hdx/location/_version.py
+-rwxr-xr-x   0        0        0    12372 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/src/hdx/location/adminlevel.py
+-rwxr-xr-x   0        0        0    32382 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/src/hdx/location/country.py
+-rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/src/hdx/location/currency.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/src/hdx/location/names.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/src/hdx/location/phonetics.py
+-rwxr-xr-x   0        0        0    22035 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/tests/fixtures/adminlevel.yaml
+-rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/tests/fixtures/secondary_historic_rates.csv
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/tests/fixtures/secondary_rates.json
+-rwxr-xr-x   0        0        0    65717 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/tests/hdx/location/Countries_UZB_Deleted.csv
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/tests/hdx/location/__init__.py
+-rwxr-xr-x   0        0        0     4457 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/tests/hdx/location/test_adminlevel.py
+-rwxr-xr-x   0        0        0    30396 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/tests/hdx/location/test_country.py
+-rwxr-xr-x   0        0        0     9462 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/tests/hdx/location/test_currency.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/.gitignore
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/LICENSE
+-rwxr-xr-x   0        0        0     2306 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/README.md
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 hdx_python_country-3.5.2/PKG-INFO
```

### Comparing `hdx_python_country-3.5.1/CONTRIBUTING.md` & `hdx_python_country-3.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/requirements.txt` & `hdx_python_country-3.5.2/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements.txt --resolver=backtracking pyproject.toml
 #
+annotated-types==0.5.0
+    # via pydantic
 attrs==23.1.0
     # via
     #   frictionless
     #   jsonlines
     #   jsonschema
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
 cfgv==3.3.1
     # via pre-commit
-chardet==5.1.0
+chardet==5.2.0
     # via frictionless
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via typer
 colorama==0.4.6
     # via typer
 coverage[toml]==7.2.7
     # via pytest-cov
 decorator==5.1.1
     # via
     #   jsonpath-ng
     #   validators
-distlib==0.3.6
+distlib==0.3.7
     # via virtualenv
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.12.2
     # via virtualenv
-frictionless==5.13.1
+frictionless==5.15.10
     # via hdx-python-utilities
-hdx-python-utilities==3.6.1
+hdx-python-utilities==3.6.2
     # via hdx-python-country (pyproject.toml)
-humanize==4.6.0
+humanize==4.7.0
     # via frictionless
-identify==2.5.24
+identify==2.5.26
     # via pre-commit
 idna==3.4
     # via requests
-ijson==3.2.2
+ijson==3.2.3
     # via hdx-python-utilities
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
 jinja2==3.1.2
     # via frictionless
@@ -55,15 +57,15 @@
     # via hdx-python-utilities
 jsonpath-ng==1.5.3
     # via libhxl
 jsonschema==4.17.3
     # via
     #   frictionless
     #   tableschema-to-template
-libhxl==5.0.1
+libhxl==5.0.2
     # via hdx-python-country (pyproject.toml)
 loguru==0.7.0
     # via hdx-python-utilities
 markdown-it-py==3.0.0
     # via rich
 marko==2.0.0
     # via frictionless
@@ -75,27 +77,29 @@
     # via pre-commit
 openpyxl==3.1.2
     # via hdx-python-utilities
 packaging==23.1
     # via pytest
 petl==1.7.12
     # via frictionless
-platformdirs==3.8.0
+platformdirs==3.10.0
     # via virtualenv
 pluggy==1.2.0
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
 pre-commit==3.3.3
     # via hdx-python-country (pyproject.toml)
-pydantic==1.10.9
+pydantic==2.1.1
     # via frictionless
-pygments==2.15.1
+pydantic-core==2.4.0
+    # via pydantic
+pygments==2.16.1
     # via rich
 pyphonetics==0.5.3
     # via hdx-python-country (pyproject.toml)
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.4.0
     # via
@@ -109,15 +113,15 @@
     #   frictionless
     #   hdx-python-utilities
     #   libhxl
 python-io-wrapper==0.3.1
     # via libhxl
 python-slugify==8.0.1
     # via frictionless
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
 ratelimit==2.2.1
     # via hdx-python-utilities
 requests==2.31.0
@@ -125,15 +129,15 @@
     #   frictionless
     #   libhxl
     #   requests-file
 requests-file==1.5.1
     # via hdx-python-utilities
 rfc3986==2.0.0
     # via frictionless
-rich==13.4.2
+rich==13.5.2
     # via typer
 ruamel-yaml==0.17.32
     # via hdx-python-utilities
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 shellingham==1.5.0.post1
     # via typer
@@ -153,32 +157,33 @@
     # via hdx-python-utilities
 tabulate==0.9.0
     # via frictionless
 text-unidecode==1.3
     # via python-slugify
 typer[all]==0.9.0
     # via frictionless
-typing-extensions==4.6.3
+typing-extensions==4.7.1
     # via
     #   frictionless
     #   pydantic
+    #   pydantic-core
     #   typer
 unidecode==1.3.6
     # via
     #   libhxl
     #   pyphonetics
-urllib3==2.0.3
+urllib3==2.0.4
     # via
     #   libhxl
     #   requests
 validators==0.20.0
     # via frictionless
-virtualenv==20.23.1
+virtualenv==20.24.2
     # via pre-commit
-wheel==0.40.0
+wheel==0.41.1
     # via libhxl
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
 xlsxwriter==3.1.2
     # via tableschema-to-template
```

### Comparing `hdx_python_country-3.5.1/.config/pre-commit-config.yaml` & `hdx_python_country-3.5.2/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/.github/workflows/publish.yaml` & `hdx_python_country-3.5.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/.github/workflows/run-python-tests.yaml` & `hdx_python_country-3.5.2/.github/workflows/run-python-tests.yaml`

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

### Comparing `hdx_python_country-3.5.1/documentation/main.md` & `hdx_python_country-3.5.2/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/documentation/pydoc-markdown.yaml` & `hdx_python_country-3.5.2/documentation/pydoc-markdown.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     packages:
       - hdx.location
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python Country
-    theme: readthedocs
+    theme: mkdocs
     repo_url: "https://github.com/OCHA-DAP/hdx-python-country"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-country
   pages:
     - title: Home
```

### Comparing `hdx_python_country-3.5.1/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv` & `hdx_python_country-3.5.2/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/src/hdx/location/adminlevel.py` & `hdx_python_country-3.5.2/src/hdx/location/adminlevel.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/src/hdx/location/country.py` & `hdx_python_country-3.5.2/src/hdx/location/country.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/src/hdx/location/currency.py` & `hdx_python_country-3.5.2/src/hdx/location/currency.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/src/hdx/location/names.py` & `hdx_python_country-3.5.2/src/hdx/location/names.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/src/hdx/location/phonetics.py` & `hdx_python_country-3.5.2/src/hdx/location/phonetics.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/tests/fixtures/adminlevel.yaml` & `hdx_python_country-3.5.2/tests/fixtures/adminlevel.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/tests/fixtures/secondary_historic_rates.csv` & `hdx_python_country-3.5.2/tests/fixtures/secondary_historic_rates.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/tests/fixtures/secondary_rates.json` & `hdx_python_country-3.5.2/tests/fixtures/secondary_rates.json`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/tests/hdx/location/Countries_UZB_Deleted.csv` & `hdx_python_country-3.5.2/tests/hdx/location/Countries_UZB_Deleted.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/tests/hdx/location/test_adminlevel.py` & `hdx_python_country-3.5.2/tests/hdx/location/test_adminlevel.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/tests/hdx/location/test_country.py` & `hdx_python_country-3.5.2/tests/hdx/location/test_country.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/tests/hdx/location/test_currency.py` & `hdx_python_country-3.5.2/tests/hdx/location/test_currency.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/.gitignore` & `hdx_python_country-3.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/LICENSE` & `hdx_python_country-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/README.md` & `hdx_python_country-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.5.1/pyproject.toml` & `hdx_python_country-3.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "hdx-python-utilities>=3.6.1",
+    "hdx-python-utilities>=3.6.2",
     "libhxl",
     "pyphonetics",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
```

### Comparing `hdx_python_country-3.5.1/PKG-INFO` & `hdx_python_country-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-country
-Version: 3.5.1
+Version: 3.5.2
 Summary: HDX Python country code and exchange rate (fx) utilities
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-country
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,country,country code,currencies,currency,exchange rate,foreign exchange,fx,iso 3166,iso2,iso3,location,region
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: hdx-python-utilities>=3.6.1
+Requires-Dist: hdx-python-utilities>=3.6.2
 Requires-Dist: libhxl
 Requires-Dist: pyphonetics
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
```

