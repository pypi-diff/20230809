# Comparing `tmp/types-aiobotocore-guardduty-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-guardduty-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-guardduty-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-guardduty-2.5.4.tar", last modified: Wed Aug  9 01:28:52 2023, max compression
```

## Comparing `types-aiobotocore-guardduty-2.5.2.post3.tar` & `types-aiobotocore-guardduty-2.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.851908 types-aiobotocore-guardduty-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:24:48.000000 types-aiobotocore-guardduty-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-08-04 12:37:47.847908 types-aiobotocore-guardduty-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-08-04 12:24:48.000000 types-aiobotocore-guardduty-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:47.851908 types-aiobotocore-guardduty-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 12:24:47.000000 types-aiobotocore-guardduty-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.827907 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-04 12:24:48.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-04 12:24:48.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 12:24:48.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52639 2023-08-04 12:24:50.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-08-04 12:24:48.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-08-04 12:24:50.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-04 12:24:50.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-08-04 12:24:50.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-08-04 12:24:50.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:24:48.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93001 2023-08-04 12:24:52.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92914 2023-08-04 12:24:51.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:24:48.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:47.843908 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-08-04 12:37:47.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:37:47.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:47.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:47.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:47.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:37:47.000000 types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:52.898739 types-aiobotocore-guardduty-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-08-09 01:28:52.894739 types-aiobotocore-guardduty-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:28:52.898739 types-aiobotocore-guardduty-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:52.894739 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52639 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-08-09 01:16:23.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-09 01:16:23.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93001 2023-08-09 01:16:25.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92914 2023-08-09 01:16:24.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-09 01:16:21.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:52.894739 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-08-09 01:28:52.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-09 01:28:52.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:28:52.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:28:52.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-09 01:28:52.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-09 01:28:52.000000 types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/LICENSE` & `types-aiobotocore-guardduty-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/PKG-INFO` & `types-aiobotocore-guardduty-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-guardduty
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GuardDuty 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GuardDuty 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[aiobotocore.GuardDuty 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/README.md` & `types-aiobotocore-guardduty-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GuardDuty 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[aiobotocore.GuardDuty 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/setup.py` & `types-aiobotocore-guardduty-2.5.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-guardduty",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.GuardDuty 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/__init__.py` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/__init__.pyi` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/__main__.py` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GuardDuty 2.5.2\nVersion:         2.5.2.post3\nBuilder"
-        " version: 7.17.2\nDocs:           "
+        "Type annotations for aiobotocore.GuardDuty 2.5.4\nVersion:         2.5.4\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
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

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/client.py` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/client.pyi` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/literals.py` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
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
@@ -305,14 +306,15 @@
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
@@ -391,26 +393,28 @@
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
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/literals.pyi` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
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
@@ -303,14 +304,15 @@
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
@@ -389,26 +391,28 @@
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
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/paginator.py` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/paginator.pyi` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/type_defs.py` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty/type_defs.pyi` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/PKG-INFO` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-guardduty
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.GuardDuty 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GuardDuty 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[aiobotocore.GuardDuty 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-guardduty-2.5.2.post3/types_aiobotocore_guardduty.egg-info/SOURCES.txt` & `types-aiobotocore-guardduty-2.5.4/types_aiobotocore_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

