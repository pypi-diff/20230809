# Comparing `tmp/alibabacloud_nis20211216-1.0.0.tar.gz` & `tmp/alibabacloud_nis20211216-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_nis20211216-1.0.0.tar", last modified: Thu Mar  2 08:46:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_nis20211216-1.1.0.tar", last modified: Wed Aug  9 01:40:27 2023, max compression
```

## Comparing `alibabacloud_nis20211216-1.0.0.tar` & `alibabacloud_nis20211216-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216/client.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2023-03-02 08:46:23.000000 alibabacloud_nis20211216-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:40:27.000000 alibabacloud_nis20211216-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-08-09 01:40:27.000000 alibabacloud_nis20211216-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:40:27.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43903 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216/client.py
+-rw-r--r--   0 root         (0) root         (0)    71556 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 01:40:27.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-09 01:40:27.000000 alibabacloud_nis20211216-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-08-09 01:40:26.000000 alibabacloud_nis20211216-1.1.0/setup.py
```

### Comparing `alibabacloud_nis20211216-1.0.0/LICENSE` & `alibabacloud_nis20211216-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216-1.0.0/PKG-INFO` & `alibabacloud_nis20211216-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_nis20211216
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud nis (20211216) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nis20211216-1.0.0/README-CN.md` & `alibabacloud_nis20211216-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216-1.0.0/README.md` & `alibabacloud_nis20211216-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nis20211216-1.0.0/alibabacloud_nis20211216.egg-info/PKG-INFO` & `alibabacloud_nis20211216-1.1.0/alibabacloud_nis20211216.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-nis20211216
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud nis (20211216) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nis20211216-1.0.0/setup.py` & `alibabacloud_nis20211216-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_nis20211216.
 
-Created on 02/03/2023
+Created on 09/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_nis20211216"
 NAME = "alibabacloud_nis20211216" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud nis (20211216) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

