# Comparing `tmp/foursight-3.6.2.tar.gz` & `tmp/foursight-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.6.2.tar", max compression
+gzip compressed data, was "foursight-3.6.3.tar", max compression
```

## Comparing `foursight-3.6.2.tar` & `foursight-3.6.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-3.6.2/LICENSE.txt
--rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-3.6.2/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-3.6.2/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-3.6.2/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    54860 2023-06-21 14:22:50.333640 foursight-3.6.2/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-3.6.2/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    62768 2023-06-21 14:22:50.335968 foursight-3.6.2/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-3.6.2/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-3.6.2/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-3.6.2/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-3.6.2/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-3.6.2/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-3.6.2/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2022-11-16 16:53:13.427051 foursight-3.6.2/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 17:19:30.850214 foursight-3.6.2/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2022-11-16 16:53:13.428402 foursight-3.6.2/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-3.6.2/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 17:19:39.276361 foursight-3.6.2/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-3.6.2/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-19 19:52:24.091978 foursight-3.6.2/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   128352 2023-08-07 20:31:26.074887 foursight-3.6.2/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 17:19:39.282546 foursight-3.6.2/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137844 2023-07-19 18:36:43.844611 foursight-3.6.2/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-3.6.2/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-3.6.2/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1283 2023-08-07 20:31:26.075830 foursight-3.6.2/pyproject.toml
--rw-r--r--   0        0        0     1535 1970-01-01 00:00:00.000000 foursight-3.6.2/setup.py
--rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 foursight-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-3.6.3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-3.6.3/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-3.6.3/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-3.6.3/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54860 2023-06-21 14:22:50.333640 foursight-3.6.3/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-3.6.3/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    62768 2023-06-21 14:22:50.335968 foursight-3.6.3/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-3.6.3/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-3.6.3/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-3.6.3/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-3.6.3/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-3.6.3/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-3.6.3/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2022-11-16 16:53:13.427051 foursight-3.6.3/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 17:19:30.850214 foursight-3.6.3/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2022-11-16 16:53:13.428402 foursight-3.6.3/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-3.6.3/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 17:19:39.276361 foursight-3.6.3/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-3.6.3/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45209 2023-04-19 19:52:24.091978 foursight-3.6.3/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   128352 2023-08-07 20:31:26.074887 foursight-3.6.3/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 17:19:39.282546 foursight-3.6.3/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137844 2023-07-19 18:36:43.844611 foursight-3.6.3/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-3.6.3/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-3.6.3/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1258 2023-08-08 22:32:09.544331 foursight-3.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 foursight-3.6.3/setup.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 foursight-3.6.3/PKG-INFO
```

### Comparing `foursight-3.6.2/LICENSE.txt` & `foursight-3.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/app_utils.py` & `foursight-3.6.3/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/check_schedules.py` & `foursight-3.6.3/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/check_setup.json` & `foursight-3.6.3/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.6.3/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.6.3/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.6.3/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.6.3/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.6.3/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/chalicelib_fourfront/package.py` & `foursight-3.6.3/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.6.2/pyproject.toml` & `foursight-3.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "foursight"
-version = "3.6.2"
+version = "3.6.3"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-#dcicutils = "^7.5.1"
-dcicutils = "7.6.0.1b4"
+dcicutils = "^7.7.0"
 click = "^7.1.2"
 PyJWT = "^2.5.0"
 Jinja2 = "2.10.1"
 MarkupSafe = "1.1.1"
 google-api-python-client = "^1.7.4"
 geocoder = "1.38.1"
 elasticsearch = "^7.13.4"
```

### Comparing `foursight-3.6.2/setup.py` & `foursight-3.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Jinja2==2.10.1',
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'click>=7.1.2,<8.0.0',
- 'dcicutils==7.6.0.1b4',
+ 'dcicutils>=7.7.0,<8.0.0',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
  'foursight-core==4.4.0',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.7.4,<2.0.0',
  'gspread>=3.6.0',
@@ -34,15 +34,15 @@
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight',
-    'version': '3.6.2',
+    'version': '3.6.3',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight-3.6.2/PKG-INFO` & `foursight-3.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.6.2
+Version: 3.6.3
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: dcicutils (==7.6.0.1b4)
+Requires-Dist: dcicutils (>=7.7.0,<8.0.0)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: foursight-core (==4.4.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.7.4,<2.0.0)
 Requires-Dist: gspread (>=3.6.0)
```

