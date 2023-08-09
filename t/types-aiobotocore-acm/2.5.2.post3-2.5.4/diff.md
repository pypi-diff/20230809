# Comparing `tmp/types-aiobotocore-acm-2.5.2.post3.tar.gz` & `tmp/types-aiobotocore-acm-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-acm-2.5.2.post3.tar", last modified: Fri Aug  4 12:37:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-acm-2.5.4.tar", last modified: Wed Aug  9 01:28:17 2023, max compression
```

## Comparing `types-aiobotocore-acm-2.5.2.post3.tar` & `types-aiobotocore-acm-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.471096 types-aiobotocore-acm-2.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-08-04 12:37:13.463096 types-aiobotocore-acm-2.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:37:13.471096 types-aiobotocore-acm-2.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.459095 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 12:17:50.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-04 12:17:51.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:37:13.463096 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-08-04 12:37:13.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:37:13.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:13.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:37:13.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:37:13.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:37:13.000000 types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:17.574352 types-aiobotocore-acm-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-08-09 01:28:17.574352 types-aiobotocore-acm-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:28:17.578352 types-aiobotocore-acm-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:17.570351 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14895 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-08-09 01:09:28.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-09 01:09:27.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:17.574352 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-08-09 01:28:17.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-09 01:28:17.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:28:17.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:28:17.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-09 01:28:17.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-09 01:28:17.000000 types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-acm-2.5.2.post3/LICENSE` & `types-aiobotocore-acm-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/PKG-INFO` & `types-aiobotocore-acm-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ACM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[aiobotocore.ACM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-acm-2.5.2.post3/README.md` & `types-aiobotocore-acm-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[aiobotocore.ACM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-acm-2.5.2.post3/setup.py` & `types-aiobotocore-acm-2.5.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-acm",
-    version="2.5.2.post3",
+    version="2.5.4",
     packages=["types_aiobotocore_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.ACM 2.5.4 service generated with mypy-boto3-builder"
         " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/__init__.py` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/__init__.pyi` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/__main__.py` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ACM 2.5.2\nVersion:         2.5.2.post3\nBuilder version:"
+        "Type annotations for aiobotocore.ACM 2.5.4\nVersion:         2.5.4\nBuilder version:"
         " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
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

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/client.py` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/client.pyi` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/literals.py` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/literals.py`

 * *Files 1% similar despite different names*

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
@@ -510,14 +514,15 @@
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

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/literals.pyi` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
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
@@ -240,14 +241,15 @@
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
@@ -326,26 +328,28 @@
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
@@ -508,14 +512,15 @@
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

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/paginator.py` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/paginator.pyi` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/type_defs.py` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/type_defs.pyi` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/waiter.py` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm/waiter.pyi` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/PKG-INFO` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-acm
-Version: 2.5.2.post3
-Summary: Type annotations for aiobotocore.ACM 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore.ACM 2.5.4 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-acm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-acm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-acm)](https://pepy.tech/project/types-aiobotocore-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ACM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[aiobotocore.ACM 2.5.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-acm-2.5.2.post3/types_aiobotocore_acm.egg-info/SOURCES.txt` & `types-aiobotocore-acm-2.5.4/types_aiobotocore_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

