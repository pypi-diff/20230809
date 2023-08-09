# Comparing `tmp/testApiGroup-1.0.0.7.tar.gz` & `tmp/testApiGroup-1.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testApiGroup-1.0.0.7.tar", last modified: Mon Jul 31 06:50:43 2023, max compression
+gzip compressed data, was "testApiGroup-1.0.0.8.tar", last modified: Mon Jul 31 06:57:57 2023, max compression
```

## Comparing `testApiGroup-1.0.0.7.tar` & `testApiGroup-1.0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:50:43.273041 testApiGroup-1.0.0.7/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:50:43.272174 testApiGroup-1.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 06:50:43.273041 testApiGroup-1.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      281 2023-07-31 06:50:42.000000 testApiGroup-1.0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:50:43.257042 testApiGroup-1.0.0.7/testApiGroup/
--rw-rw-rw-   0        0        0     1122 2023-07-31 06:50:42.000000 testApiGroup-1.0.0.7/testApiGroup/testApiGroup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:50:43.269041 testApiGroup-1.0.0.7/testApiGroup.egg-info/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 06:50:43.000000 testApiGroup-1.0.0.7/testApiGroup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 06:57:57.704057 testApiGroup-1.0.0.8/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:57:57.704057 testApiGroup-1.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:57:57.705058 testApiGroup-1.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      281 2023-07-31 06:57:57.000000 testApiGroup-1.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:57:57.691057 testApiGroup-1.0.0.8/testApiGroup/
+-rw-rw-rw-   0        0        0     1122 2023-07-31 06:57:57.000000 testApiGroup-1.0.0.8/testApiGroup/testApiGroup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:57:57.702058 testApiGroup-1.0.0.8/testApiGroup.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:57:57.000000 testApiGroup-1.0.0.8/testApiGroup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-31 06:57:57.000000 testApiGroup-1.0.0.8/testApiGroup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:57:57.000000 testApiGroup-1.0.0.8/testApiGroup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 06:57:57.000000 testApiGroup-1.0.0.8/testApiGroup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 06:57:57.000000 testApiGroup-1.0.0.8/testApiGroup.egg-info/top_level.txt
```

### Comparing `testApiGroup-1.0.0.7/testApiGroup/testApiGroup.py` & `testApiGroup-1.0.0.8/testApiGroup/testApiGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import requests
 import logging
 
 
-class testApiGroup:
+class TestApiGroup:
     def __init__(self):
         self.headers = {'Content-Type': 'application/json'}
         self.url = 'http://localhost:8080'
         logging.basicConfig(
             level=logging.DEBUG,  # 设置日志级别为DEBUG
             format='%(asctime)s - %(levelname)s - %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S'
```

