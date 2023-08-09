# Comparing `tmp/alibabacloud_nis20211216_py2-1.0.0.tar.gz` & `tmp/alibabacloud_nis20211216_py2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_nis20211216_py2-1.0.0.tar", last modified: Thu Mar  2 08:45:58 2023, max compression
+gzip compressed data, was "dist/alibabacloud_nis20211216_py2-1.1.0.tar", last modified: Wed Aug  9 01:37:53 2023, max compression
```

## Comparing `alibabacloud_nis20211216_py2-1.0.0.tar` & `alibabacloud_nis20211216_py2-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-02 08:45:57.000000 alibabacloud_nis20211216_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-02 08:45:57.000000 alibabacloud_nis20211216_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-02 08:45:57.000000 alibabacloud_nis20211216_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-03-02 08:45:57.000000 alibabacloud_nis20211216_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-02 08:45:57.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-03-02 08:45:57.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216/client.py
--rw-r--r--   0 root         (0) root         (0)    10013 2023-03-02 08:45:57.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-02 08:45:58.000000 alibabacloud_nis20211216_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-03-02 08:45:57.000000 alibabacloud_nis20211216_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20081 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216/client.py
+-rw-r--r--   0 root         (0) root         (0)    71951 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-09 01:37:53.000000 alibabacloud_nis20211216_py2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-08-09 01:37:52.000000 alibabacloud_nis20211216_py2-1.1.0/setup.py
```

### Comparing `alibabacloud_nis20211216_py2-1.0.0/LICENSE` & `alibabacloud_nis20211216_py2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216_py2-1.0.0/PKG-INFO` & `alibabacloud_nis20211216_py2-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_nis20211216_py2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud nis (20211216) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nis20211216_py2-1.0.0/README-CN.md` & `alibabacloud_nis20211216_py2-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216_py2-1.0.0/README.md` & `alibabacloud_nis20211216_py2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216_py2-1.0.0/alibabacloud_nis20211216_py2.egg-info/PKG-INFO` & `alibabacloud_nis20211216_py2-1.1.0/alibabacloud_nis20211216_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-nis20211216-py2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud nis (20211216) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nis20211216_py2-1.0.0/setup.py` & `alibabacloud_nis20211216_py2-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_nis20211216_py2.
 
-Created on 02/03/2023
+Created on 09/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_nis20211216"
 NAME = "alibabacloud_nis20211216_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud nis (20211216) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

