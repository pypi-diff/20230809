# Comparing `tmp/hdx_scraper_geonode-1.5.1.tar.gz` & `tmp/hdx_scraper_geonode-1.5.2.tar.gz`

## Comparing `hdx_scraper_geonode-1.5.1.tar` & `hdx_scraper_geonode-1.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     5290 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/requirements.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/black.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/coveragerc
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/pytest.ini
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/documentation/main.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/documentation/pydoc-markdown.yaml
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/_version.py
--rwxr-xr-x   0        0        0    18251 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/geonodetohdx.py
--rwxr-xr-x   0        0        0     1577 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/hdx_geonode.yaml
--rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/tests/config/project_configuration.yml
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/tests/fixtures/hdx_geonode.yml
--rwxr-xr-x   0        0        0    43552 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/tests/hdx/scraper/geonode/test_geonodetohdx.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/LICENSE
--rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/documentation/main.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/documentation/pydoc-markdown.yaml
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/src/hdx/scraper/geonode/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/src/hdx/scraper/geonode/_version.py
+-rwxr-xr-x   0        0        0    18251 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/src/hdx/scraper/geonode/geonodetohdx.py
+-rwxr-xr-x   0        0        0     1577 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/src/hdx/scraper/geonode/hdx_geonode.yaml
+-rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/tests/config/project_configuration.yml
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/tests/fixtures/hdx_geonode.yml
+-rwxr-xr-x   0        0        0    43608 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/tests/hdx/scraper/geonode/test_geonodetohdx.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/LICENSE
+-rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 hdx_scraper_geonode-1.5.2/PKG-INFO
```

### Comparing `hdx_scraper_geonode-1.5.1/CONTRIBUTING.md` & `hdx_scraper_geonode-1.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/requirements.txt` & `hdx_scraper_geonode-1.5.2/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,52 +2,48 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements.txt --resolver=backtracking pyproject.toml
 #
 annotated-types==0.5.0
     # via pydantic
-anyio==3.7.1
-    # via httpcore
 attrs==23.1.0
     # via
     #   frictionless
     #   jsonlines
     #   jsonschema
 certifi==2023.7.22
-    # via
-    #   httpcore
-    #   requests
+    # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
-chardet==5.1.0
+chardet==5.2.0
     # via frictionless
 charset-normalizer==3.2.0
     # via requests
 ckanapi==4.7
     # via hdx-python-api
 click==8.1.6
     # via typer
 colorama==0.4.6
     # via typer
 coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==41.0.2
+cryptography==41.0.3
     # via pyopenssl
 decorator==5.1.1
     # via
     #   jsonpath-ng
     #   validators
 defopt==6.4.0
     # via hdx-python-api
 distlib==0.3.7
     # via virtualenv
-dnspython==2.4.0
+dnspython==2.4.1
     # via email-validator
 docopt==0.6.2
     # via
     #   ckanapi
     #   num2words
 docutils==0.20.1
     # via defopt
@@ -55,31 +51,26 @@
     # via hdx-python-api
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.12.2
     # via virtualenv
 frictionless==5.15.10
     # via hdx-python-utilities
-h11==0.14.0
-    # via httpcore
-hdx-python-api==6.0.6
+hdx-python-api==6.0.8
     # via hdx-scraper-geonode (pyproject.toml)
-hdx-python-country==3.5.1
+hdx-python-country==3.5.2
     # via hdx-python-api
-hdx-python-utilities==3.6.1
+hdx-python-utilities==3.6.2
     # via hdx-python-country
-httpcore==0.17.3
-    # via dnspython
 humanize==4.7.0
     # via frictionless
 identify==2.5.26
     # via pre-commit
 idna==3.4
     # via
-    #   anyio
     #   email-validator
     #   requests
 ijson==3.2.3
     # via hdx-python-utilities
 inflect==7.0.0
     # via quantulum3
 iniconfig==2.0.0
@@ -118,15 +109,15 @@
     # via quantulum3
 openpyxl==3.1.2
     # via hdx-python-utilities
 packaging==23.1
     # via pytest
 petl==1.7.12
     # via frictionless
-platformdirs==3.9.1
+platformdirs==3.10.0
     # via virtualenv
 pluggy==1.2.0
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
@@ -136,21 +127,21 @@
     # via hdx-scraper-geonode (pyproject.toml)
 pyasn1==0.5.0
     # via
     #   hdx-python-api
     #   ndg-httpsclient
 pycparser==2.21
     # via cffi
-pydantic==2.0.3
+pydantic==2.1.1
     # via
     #   frictionless
     #   inflect
-pydantic-core==2.3.0
+pydantic-core==2.4.0
     # via pydantic
-pygments==2.15.1
+pygments==2.16.1
     # via rich
 pyopenssl==23.2.0
     # via
     #   hdx-python-api
     #   ndg-httpsclient
 pyphonetics==0.5.3
     # via hdx-python-country
@@ -190,15 +181,15 @@
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
@@ -209,19 +200,14 @@
     #   ckanapi
     #   isodate
     #   jsonpath-ng
     #   pockets
     #   python-dateutil
     #   requests-file
     #   sphinxcontrib-napoleon
-sniffio==1.3.0
-    # via
-    #   anyio
-    #   dnspython
-    #   httpcore
 sphinxcontrib-napoleon==0.7
     # via defopt
 stringcase==1.2.0
     # via frictionless
 structlog==23.1.0
     # via libhxl
 tableschema-to-template==0.0.13
@@ -247,15 +233,15 @@
     # via
     #   libhxl
     #   requests
 validators==0.20.0
     # via frictionless
 virtualenv==20.24.2
     # via pre-commit
-wheel==0.41.0
+wheel==0.41.1
     # via libhxl
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
 xlsxwriter==3.1.2
     # via tableschema-to-template
```

### Comparing `hdx_scraper_geonode-1.5.1/.config/pre-commit-config.yaml` & `hdx_scraper_geonode-1.5.2/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/.github/workflows/publish.yaml` & `hdx_scraper_geonode-1.5.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/.github/workflows/run-python-tests.yaml` & `hdx_scraper_geonode-1.5.2/.github/workflows/run-python-tests.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 name: Run tests
 
 on:
   workflow_dispatch: # add run button in github
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

### Comparing `hdx_scraper_geonode-1.5.1/documentation/main.md` & `hdx_scraper_geonode-1.5.2/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/documentation/pydoc-markdown.yaml` & `hdx_scraper_geonode-1.5.2/documentation/pydoc-markdown.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     packages:
       - hdx.scraper.geonode
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Scraper GeoNode
-    theme: readthedocs
+    theme: mkdocs
     repo_url: "https://github.com/OCHA-DAP/hdx-scraper-geonode"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-scraper-geonode
   pages:
     - title: Home
```

### Comparing `hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/geonodetohdx.py` & `hdx_scraper_geonode-1.5.2/src/hdx/scraper/geonode/geonodetohdx.py`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/src/hdx/scraper/geonode/hdx_geonode.yaml` & `hdx_scraper_geonode-1.5.2/src/hdx/scraper/geonode/hdx_geonode.yaml`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/tests/hdx/scraper/geonode/test_geonodetohdx.py` & `hdx_scraper_geonode-1.5.2/tests/hdx/scraper/geonode/test_geonodetohdx.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,44 +230,44 @@
     wfpresources = [
         [
             {
                 "name": "ICA Sudan - Land Degradation shapefile",
                 "url": "http://xxx/geoserver/wfs?format_options=charset:UTF-8&typename=geonode:sdn_ica_landdegradation_geonode_20180201&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "Zipped Shapefile. This layer contains...",
                 "format": "shp",
-                "last_modified": "2018-11-22T00:00:00",
+                "last_modified": "2018-11-22T16:56:00.000000",
                 "resource_type": "api",
                 "url_type": "api",
             },
             {
                 "name": "ICA Sudan - Land Degradation geojson",
                 "url": "http://xxx/geoserver/wfs?srsName=EPSG%3A4326&typename=geonode:sdn_ica_landdegradation_geonode_20180201&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "GeoJSON file. This layer contains...",
                 "format": "geojson",
-                "last_modified": "2018-11-22T00:00:00",
+                "last_modified": "2018-11-22T16:56:00.000000",
                 "resource_type": "api",
                 "url_type": "api",
             },
         ],
         [
             {
                 "name": "ICA Sudan - Most Predominant Livelihood Zones shapefile",
                 "url": "https://ogcserver.gis.wfp.org/geoserver/wfs?format_options=charset:UTF-8&typename=geonode:sdn_ica_predlhz_geonode_20180201&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "Zipped Shapefile. This layer contains...",
                 "format": "shp",
-                "last_modified": "2018-11-22T00:00:00",
+                "last_modified": "2018-11-22T16:18:00.000000",
                 "resource_type": "api",
                 "url_type": "api",
             },
             {
                 "name": "ICA Sudan - Most Predominant Livelihood Zones geojson",
                 "url": "https://ogcserver.gis.wfp.org/geoserver/wfs?srsName=EPSG%3A4326&typename=geonode:sdn_ica_predlhz_geonode_20180201&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "GeoJSON file. This layer contains...",
                 "format": "geojson",
-                "last_modified": "2018-11-22T00:00:00",
+                "last_modified": "2018-11-22T16:18:00.000000",
                 "resource_type": "api",
                 "url_type": "api",
             },
         ],
     ]
 
     wfporganization = {
@@ -378,44 +378,44 @@
     mimuresources = [
         [
             {
                 "name": "Myanmar Town shapefile",
                 "url": "http://yyy/geoserver/wfs?format_options=charset:UTF-8&typename=geonode:mmr_town_2019_july&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "Zipped Shapefile. Towns are urban areas divided into wards.",
                 "format": "shp",
-                "last_modified": "2019-08-05T00:00:00",
+                "last_modified": "2019-08-05T00:00:00.000000",
                 "resource_type": "api",
                 "url_type": "api",
             },
             {
                 "name": "Myanmar Town geojson",
                 "url": "http://yyy/geoserver/wfs?srsName=EPSG%3A4326&typename=geonode:mmr_town_2019_july&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "GeoJSON file. Towns are urban areas divided into wards.",
                 "format": "geojson",
-                "last_modified": "2019-08-05T00:00:00",
+                "last_modified": "2019-08-05T00:00:00.000000",
                 "resource_type": "api",
                 "url_type": "api",
             },
         ],
         [
             {
                 "name": "Myanmar Forest Cover Change shapefile",
                 "url": "http://yyy/geoserver/wfs?format_options=charset:UTF-8&typename=geonode:myan_lvl2_smoothed_dec2015_resamp&outputFormat=SHAPE-ZIP&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "Zipped Shapefile. A Landsat-based classification of Myanmar’s forest cover",
                 "format": "shp",
-                "last_modified": "2019-02-12T00:00:00",
+                "last_modified": "2019-02-12T00:00:00.000000",
                 "resource_type": "api",
                 "url_type": "api",
             },
             {
                 "name": "Myanmar Forest Cover Change geojson",
                 "url": "http://yyy/geoserver/wfs?srsName=EPSG%3A4326&typename=geonode:myan_lvl2_smoothed_dec2015_resamp&outputFormat=json&version=1.0.0&service=WFS&request=GetFeature",
                 "description": "GeoJSON file. A Landsat-based classification of Myanmar’s forest cover",
                 "format": "geojson",
-                "last_modified": "2019-02-12T00:00:00",
+                "last_modified": "2019-02-12T00:00:00.000000",
                 "resource_type": "api",
                 "url_type": "api",
             },
         ],
     ]
 
     mimuorganization = {
```

### Comparing `hdx_scraper_geonode-1.5.1/.gitignore` & `hdx_scraper_geonode-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/LICENSE` & `hdx_scraper_geonode-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/README.md` & `hdx_scraper_geonode-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hdx_scraper_geonode-1.5.1/pyproject.toml` & `hdx_scraper_geonode-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "hdx-python-api >= 6.0.6",
+    "hdx-python-api >= 6.0.8",
     "python-slugify",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

### Comparing `hdx_scraper_geonode-1.5.1/PKG-INFO` & `hdx_scraper_geonode-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-scraper-geonode
-Version: 1.5.1
+Version: 1.5.2
 Summary: HDX Python generic geonode scraper
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-scraper-geonode
 Author-email: Michael Rans <rans@email.com>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,geonode,scraper
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: hdx-python-api>=6.0.6
+Requires-Dist: hdx-python-api>=6.0.8
 Requires-Dist: python-slugify
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
```

