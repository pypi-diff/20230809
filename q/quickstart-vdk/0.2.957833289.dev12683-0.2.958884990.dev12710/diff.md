# Comparing `tmp/quickstart-vdk-0.2.957833289.dev12683.tar.gz` & `tmp/quickstart-vdk-0.2.958884990.dev12710.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.957833289.dev12683.tar", last modified: Mon Aug  7 08:34:16 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.958884990.dev12710.tar", last modified: Tue Aug  8 04:23:43 2023, max compression
```

## Comparing `quickstart-vdk-0.2.957833289.dev12683.tar` & `quickstart-vdk-0.2.958884990.dev12710.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:34:16.408176 quickstart-vdk-0.2.957833289.dev12683/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-08-07 08:34:16.408176 quickstart-vdk-0.2.957833289.dev12683/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-08-07 08:33:53.000000 quickstart-vdk-0.2.957833289.dev12683/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:34:16.404176 quickstart-vdk-0.2.957833289.dev12683/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-08-07 08:34:16.000000 quickstart-vdk-0.2.957833289.dev12683/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-08-07 08:34:16.000000 quickstart-vdk-0.2.957833289.dev12683/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:34:16.000000 quickstart-vdk-0.2.957833289.dev12683/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-08-07 08:34:16.000000 quickstart-vdk-0.2.957833289.dev12683/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-07 08:34:16.000000 quickstart-vdk-0.2.957833289.dev12683/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 08:34:16.408176 quickstart-vdk-0.2.957833289.dev12683/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-08-07 08:34:03.000000 quickstart-vdk-0.2.957833289.dev12683/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:34:16.408176 quickstart-vdk-0.2.957833289.dev12683/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-08-07 08:33:53.000000 quickstart-vdk-0.2.957833289.dev12683/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:23:43.842147 quickstart-vdk-0.2.958884990.dev12710/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-08-08 04:23:43.842147 quickstart-vdk-0.2.958884990.dev12710/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-08-08 04:20:47.000000 quickstart-vdk-0.2.958884990.dev12710/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:23:43.842147 quickstart-vdk-0.2.958884990.dev12710/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-08-08 04:23:43.000000 quickstart-vdk-0.2.958884990.dev12710/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-08-08 04:23:43.000000 quickstart-vdk-0.2.958884990.dev12710/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 04:23:43.000000 quickstart-vdk-0.2.958884990.dev12710/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-08-08 04:23:43.000000 quickstart-vdk-0.2.958884990.dev12710/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-08 04:23:43.000000 quickstart-vdk-0.2.958884990.dev12710/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 04:23:43.842147 quickstart-vdk-0.2.958884990.dev12710/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-08-08 04:23:32.000000 quickstart-vdk-0.2.958884990.dev12710/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 04:23:43.842147 quickstart-vdk-0.2.958884990.dev12710/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-08-08 04:20:47.000000 quickstart-vdk-0.2.958884990.dev12710/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.957833289.dev12683/PKG-INFO` & `quickstart-vdk-0.2.958884990.dev12710/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.957833289.dev12683
+Version: 0.2.958884990.dev12710
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.957833289.dev12683/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.958884990.dev12710/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.957833289.dev12683
+Version: 0.2.958884990.dev12710
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.957833289.dev12683/setup.py` & `quickstart-vdk-0.2.958884990.dev12710/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.957833289.dev12683"
+__version__ = "0.2.958884990.dev12710"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

