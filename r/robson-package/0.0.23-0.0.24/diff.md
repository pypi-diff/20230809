# Comparing `tmp/robson_package-0.0.23.tar.gz` & `tmp/robson_package-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robson_package-0.0.23.tar", last modified: Wed Aug  9 00:20:10 2023, max compression
+gzip compressed data, was "robson_package-0.0.24.tar", last modified: Wed Aug  9 00:24:09 2023, max compression
```

## Comparing `robson_package-0.0.23.tar` & `robson_package-0.0.24.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 00:20:10.480569 robson_package-0.0.23/
--rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.23/LICENSE
--rw-rw-rw-   0        0        0      315 2023-08-09 00:20:10.480569 robson_package-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.23/README.md
-drwxrwxrwx   0        0        0        0 2023-08-09 00:20:10.479560 robson_package-0.0.23/robson_package.egg-info/
--rw-rw-rw-   0        0        0      315 2023-08-09 00:20:10.000000 robson_package-0.0.23/robson_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-08-09 00:20:10.000000 robson_package-0.0.23/robson_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 00:20:10.000000 robson_package-0.0.23/robson_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-09 00:20:10.000000 robson_package-0.0.23/robson_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-09 00:20:10.480569 robson_package-0.0.23/setup.cfg
--rw-rw-rw-   0        0        0      554 2023-08-09 00:20:02.000000 robson_package-0.0.23/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-09 00:20:10.480569 robson_package-0.0.23/src/
--rw-rw-rw-   0        0        0       21 2023-08-09 00:01:57.000000 robson_package-0.0.23/src/__init__.py
--rw-rw-rw-   0        0        0      515 2023-08-08 11:56:48.000000 robson_package-0.0.23/src/robson_package.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:24:09.654796 robson_package-0.0.24/
+-rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.24/LICENSE
+-rw-rw-rw-   0        0        0      315 2023-08-09 00:24:09.653775 robson_package-0.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.24/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 00:24:09.649181 robson_package-0.0.24/robson_package.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-08-09 00:24:09.000000 robson_package-0.0.24/robson_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-08-09 00:24:09.000000 robson_package-0.0.24/robson_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 00:24:09.000000 robson_package-0.0.24/robson_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-09 00:24:09.000000 robson_package-0.0.24/robson_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 00:24:09.654796 robson_package-0.0.24/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-08-09 00:23:51.000000 robson_package-0.0.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:24:09.651878 robson_package-0.0.24/src/
+-rw-rw-rw-   0        0        0       21 2023-08-09 00:22:10.000000 robson_package-0.0.24/src/__init__.py
+-rw-rw-rw-   0        0        0      515 2023-08-08 11:56:48.000000 robson_package-0.0.24/src/robson_package.py
```

### Comparing `robson_package-0.0.23/LICENSE` & `robson_package-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `robson_package-0.0.23/setup.py` & `robson_package-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.23'
+VERSION = '0.0.24'
 DESCRIPTION = 'Meu primeiro pacote em Python'
 LONG_DESCRIPTION = 'Meu primeiro pacote em Python com uma descrição im pouco mais longa'
 
 # Setting up
 setup(
     name="robson_package",
     version=VERSION,
```

### Comparing `robson_package-0.0.23/src/robson_package.py` & `robson_package-0.0.24/src/robson_package.py`

 * *Files identical despite different names*

