# Comparing `tmp/types-aiobotocore-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-2.5.2.post1.tar", last modified: Fri Aug  4 14:07:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-2.5.4.tar", last modified: Wed Aug  9 01:28:23 2023, max compression
```

## Comparing `types-aiobotocore-2.5.2.post1.tar` & `types-aiobotocore-2.5.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 14:07:59.496649 types-aiobotocore-2.5.2.post1/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 14:07:26.000000 types-aiobotocore-2.5.2.post1/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    81023 2023-08-04 14:07:59.496649 types-aiobotocore-2.5.2.post1/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    69437 2023-08-04 14:07:26.000000 types-aiobotocore-2.5.2.post1/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 14:07:59.496649 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/
--rw-r--r--   0 vlad      (1000) vlad      (1000)       17 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1627 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/args.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      175 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/awsrequest.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1357 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      300 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/config.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      399 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/configprovider.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5731 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/credentials.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      477 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/discovery.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1467 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/endpoint.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      394 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/eventstream.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      595 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/handlers.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      261 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/hooks.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      643 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/httpchecksum.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      968 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/httpsession.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      732 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/paginate.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      745 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/parsers.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 14:07:26.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)      541 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/regions.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1389 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/response.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/retryhandler.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   214191 2023-08-04 14:07:29.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/session.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2182 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/signers.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/tokens.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2147 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/utils.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      581 2023-08-04 14:07:25.000000 types-aiobotocore-2.5.2.post1/aiobotocore-stubs/waiter.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 14:07:59.496649 types-aiobotocore-2.5.2.post1/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)    50147 2023-08-04 14:07:26.000000 types-aiobotocore-2.5.2.post1/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 14:07:59.496649 types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    81023 2023-08-04 14:07:59.000000 types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1045 2023-08-04 14:07:59.000000 types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 14:07:59.000000 types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 14:07:59.000000 types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)    37185 2023-08-04 14:07:59.000000 types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       18 2023-08-04 14:07:59.000000 types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:23.538419 types-aiobotocore-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-09 01:09:18.000000 types-aiobotocore-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    81017 2023-08-09 01:28:23.538419 types-aiobotocore-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    69437 2023-08-09 01:09:18.000000 types-aiobotocore-2.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:23.526419 types-aiobotocore-2.5.4/aiobotocore-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/args.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/awsrequest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/configprovider.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/eventstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/httpchecksum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/httpsession.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/paginate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/parsers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:09:18.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/regions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/retryhandler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   214191 2023-08-09 01:09:22.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/signers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/tokens.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-09 01:09:17.000000 types-aiobotocore-2.5.4/aiobotocore-stubs/waiter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:28:23.538419 types-aiobotocore-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    50141 2023-08-09 01:09:18.000000 types-aiobotocore-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:28:23.538419 types-aiobotocore-2.5.4/types_aiobotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    81017 2023-08-09 01:28:23.000000 types-aiobotocore-2.5.4/types_aiobotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-09 01:28:23.000000 types-aiobotocore-2.5.4/types_aiobotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:28:23.000000 types-aiobotocore-2.5.4/types_aiobotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:28:23.000000 types-aiobotocore-2.5.4/types_aiobotocore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)    37185 2023-08-09 01:28:23.000000 types-aiobotocore-2.5.4/types_aiobotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-09 01:28:23.000000 types-aiobotocore-2.5.4/types_aiobotocore.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-2.5.2.post1/LICENSE` & `types-aiobotocore-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/PKG-INFO` & `types-aiobotocore-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore 2.5.4 generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -394,15 +394,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore.svg?color=blue)](https://pypi.org/project/types-aiobotocore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore)](https://pepy.tech/project/types-aiobotocore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore 2.5.2](https://github.com/aio-libs/aiobotocore) compatible with
+[aiobotocore 2.5.4](https://github.com/aio-libs/aiobotocore) compatible with
 [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-2.5.2.post1/README.md` & `types-aiobotocore-2.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore.svg?color=blue)](https://pypi.org/project/types-aiobotocore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore)](https://pepy.tech/project/types-aiobotocore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore 2.5.2](https://github.com/aio-libs/aiobotocore) compatible with
+[aiobotocore 2.5.4](https://github.com/aio-libs/aiobotocore) compatible with
 [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/args.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/args.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/client.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/credentials.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/credentials.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/endpoint.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/handlers.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/handlers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/httpchecksum.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/httpchecksum.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/httpsession.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/paginate.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/paginate.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/parsers.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/regions.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/regions.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/response.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/retryhandler.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/retryhandler.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/session.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/signers.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/signers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/tokens.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/tokens.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/utils.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/aiobotocore-stubs/waiter.pyi` & `types-aiobotocore-2.5.4/aiobotocore-stubs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/setup.py` & `types-aiobotocore-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore",
-    version="2.5.2.post1",
+    version="2.5.4",
     packages=["aiobotocore-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.17.2",
+    description="Type annotations for aiobotocore 2.5.4 generated with mypy-boto3-builder 7.17.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -412,15 +412,15 @@
             "types-aiobotocore-dynamodb>=2.5.0, <2.6.0",
             "types-aiobotocore-ec2>=2.5.0, <2.6.0",
             "types-aiobotocore-lambda>=2.5.0, <2.6.0",
             "types-aiobotocore-rds>=2.5.0, <2.6.0",
             "types-aiobotocore-s3>=2.5.0, <2.6.0",
             "types-aiobotocore-sqs>=2.5.0, <2.6.0",
         ],
-        "aiobotocore": ["aiobotocore==2.5.2", "botocore==1.31.19"],
+        "aiobotocore": ["aiobotocore==2.5.4", "botocore==1.31.17"],
         "accessanalyzer": ["types-aiobotocore-accessanalyzer>=2.5.0, <2.6.0"],
         "account": ["types-aiobotocore-account>=2.5.0, <2.6.0"],
         "acm": ["types-aiobotocore-acm>=2.5.0, <2.6.0"],
         "acm-pca": ["types-aiobotocore-acm-pca>=2.5.0, <2.6.0"],
         "alexaforbusiness": ["types-aiobotocore-alexaforbusiness>=2.5.0, <2.6.0"],
         "amp": ["types-aiobotocore-amp>=2.5.0, <2.6.0"],
         "amplify": ["types-aiobotocore-amplify>=2.5.0, <2.6.0"],
```

### Comparing `types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/PKG-INFO` & `types-aiobotocore-2.5.4/types_aiobotocore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.17.2
+Version: 2.5.4
+Summary: Type annotations for aiobotocore 2.5.4 generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -394,15 +394,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore.svg?color=blue)](https://pypi.org/project/types-aiobotocore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore)](https://pepy.tech/project/types-aiobotocore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore 2.5.2](https://github.com/aio-libs/aiobotocore) compatible with
+[aiobotocore 2.5.4](https://github.com/aio-libs/aiobotocore) compatible with
 [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/SOURCES.txt` & `types-aiobotocore-2.5.4/types_aiobotocore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.5.2.post1/types_aiobotocore.egg-info/requires.txt` & `types-aiobotocore-2.5.4/types_aiobotocore.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 [acm]
 types-aiobotocore-acm<2.6.0,>=2.5.0
 
 [acm-pca]
 types-aiobotocore-acm-pca<2.6.0,>=2.5.0
 
 [aiobotocore]
-aiobotocore==2.5.2
-botocore==1.31.19
+aiobotocore==2.5.4
+botocore==1.31.17
 
 [alexaforbusiness]
 types-aiobotocore-alexaforbusiness<2.6.0,>=2.5.0
 
 [all]
 types-aiobotocore-accessanalyzer<2.6.0,>=2.5.0
 types-aiobotocore-account<2.6.0,>=2.5.0
```

