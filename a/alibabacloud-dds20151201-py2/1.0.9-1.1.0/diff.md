# Comparing `tmp/alibabacloud_dds20151201_py2-1.0.9.tar.gz` & `tmp/alibabacloud_dds20151201_py2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dds20151201_py2-1.0.9.tar", last modified: Tue Jul 19 10:59:44 2022, max compression
+gzip compressed data, was "dist/alibabacloud_dds20151201_py2-1.1.0.tar", last modified: Wed Aug  9 01:38:30 2023, max compression
```

## Comparing `alibabacloud_dds20151201_py2-1.0.9.tar` & `alibabacloud_dds20151201_py2-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/
--rw-r--r--   0 root         (0) root         (0)      450 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201/
--rw-r--r--   0 root         (0) root         (0)       21 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   183259 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201/client.py
--rw-r--r--   0 root         (0) root         (0)   702647 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2022-07-19 10:59:44.000000 alibabacloud_dds20151201_py2-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:38:30.000000 alibabacloud_dds20151201_py2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      503 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-08-09 01:38:30.000000 alibabacloud_dds20151201_py2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:38:30.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   261929 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201/client.py
+-rw-r--r--   0 root         (0) root         (0)   895350 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:38:30.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-09 01:38:30.000000 alibabacloud_dds20151201_py2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-08-09 01:38:29.000000 alibabacloud_dds20151201_py2-1.1.0/setup.py
```

### Comparing `alibabacloud_dds20151201_py2-1.0.9/LICENSE` & `alibabacloud_dds20151201_py2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dds20151201_py2-1.0.9/PKG-INFO` & `alibabacloud_dds20151201_py2-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dds20151201_py2
-Version: 1.0.9
+Version: 1.1.0
 Summary: Alibaba Cloud Dds (20151201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dds20151201_py2-1.0.9/README-CN.md` & `alibabacloud_dds20151201_py2-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dds20151201_py2-1.0.9/README.md` & `alibabacloud_dds20151201_py2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dds20151201_py2-1.0.9/alibabacloud_dds20151201_py2.egg-info/PKG-INFO` & `alibabacloud_dds20151201_py2-1.1.0/alibabacloud_dds20151201_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dds20151201-py2
-Version: 1.0.9
+Version: 1.1.0
 Summary: Alibaba Cloud Dds (20151201) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dds20151201_py2-1.0.9/setup.py` & `alibabacloud_dds20151201_py2-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dds20151201_py2.
 
-Created on 19/07/2022
+Created on 09/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dds20151201"
 NAME = "alibabacloud_dds20151201_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dds (20151201) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

