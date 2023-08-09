# Comparing `tmp/types-aiobotocore-accessanalyzer-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-accessanalyzer-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-accessanalyzer-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-accessanalyzer-2.5.4.tar", last modified: Wed Aug  9 01:28:17 2023, max compression
```

## Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3.tar` & `types-aiobotocore-accessanalyzer-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.487096 types-aiobotocore-accessanalyzer-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-08-04 12:37:13.479096 types-aiobotocore-accessanalyzer-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:13.487096 types-aiobotocore-accessanalyzer-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 12:17:47.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.479096 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26596 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26551 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42741 2023-08-04 12:17:49.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42662 2023-08-04 12:17:49.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:17:48.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.479096 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-08-04 12:37:13.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:37:13.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:13.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:13.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:13.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:37:13.000000 types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:17.570351 types-aiobotocore-accessanalyzer-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-08-09 01:28:17.570351 types-aiobotocore-accessanalyzer-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:28:17.570351 types-aiobotocore-accessanalyzer-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:17.566352 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26596 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26551 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42741 2023-08-09 01:09:25.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42662 2023-08-09 01:09:25.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-09 01:09:24.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:17.570351 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-08-09 01:28:17.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-09 01:28:17.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:28:17.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:28:17.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-09 01:28:17.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-09 01:28:17.000000 types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/LICENSE` & `types-aiobotocore-accessanalyzer-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/PKG-INFO` & `types-aiobotocore-accessanalyzer-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-accessanalyzer
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AccessAnalyzer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AccessAnalyzer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-accessanalyzer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-accessanalyzer)](https://pepy.tech/project/types-aiobotocore-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AccessAnalyzer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[aiobotocore.AccessAnalyzer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/README.md` & `types-aiobotocore-accessanalyzer-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-accessanalyzer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-accessanalyzer)](https://pepy.tech/project/types-aiobotocore-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AccessAnalyzer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[aiobotocore.AccessAnalyzer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/setup.py` & `types-aiobotocore-accessanalyzer-2.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-accessanalyzer",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_accessanalyzer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AccessAnalyzer 2.5.2 service generated with"
+        "Type annotations for aiobotocore.AccessAnalyzer 2.5.4 service generated with"
         " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/__init__.py` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/__init__.pyi` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/__main__.py` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AccessAnalyzer 2.5.2\nVersion:        "
-        " 2.5.2.post3\nBuilder version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.AccessAnalyzer 2.5.4\nVersion:         2.5.4\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post3")
+    print("2.5.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/client.py` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/client.pyi` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/literals.py` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -244,14 +245,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -330,26 +332,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -520,14 +524,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/literals.pyi` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -242,14 +243,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -328,26 +330,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -518,14 +522,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/paginator.py` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/paginator.pyi` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/type_defs.py` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer/type_defs.pyi` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/PKG-INFO` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-accessanalyzer
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.AccessAnalyzer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.AccessAnalyzer 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-accessanalyzer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-accessanalyzer)](https://pepy.tech/project/types-aiobotocore-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AccessAnalyzer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[aiobotocore.AccessAnalyzer 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-accessanalyzer-2.5.2.post3/types_aiobotocore_accessanalyzer.egg-info/SOURCES.txt` & `types-aiobotocore-accessanalyzer-2.5.4/types_aiobotocore_accessanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

