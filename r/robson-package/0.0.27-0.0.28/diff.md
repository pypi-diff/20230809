# Comparing `tmp/robson_package-0.0.27.tar.gz` & `tmp/robson_package-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robson_package-0.0.27.tar", last modified: Wed Aug  9 00:49:09 2023, max compression
+gzip compressed data, was "robson_package-0.0.28.tar", last modified: Wed Aug  9 00:56:03 2023, max compression
```

## Comparing `robson_package-0.0.27.tar` & `robson_package-0.0.28.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 00:49:09.752596 robson_package-0.0.27/
--rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.27/LICENSE
--rw-rw-rw-   0        0        0      315 2023-08-09 00:49:09.750592 robson_package-0.0.27/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.27/README.md
-drwxrwxrwx   0        0        0        0 2023-08-09 00:49:09.741592 robson_package-0.0.27/robson_package/
--rw-rw-rw-   0        0        0       33 2023-08-09 00:48:57.000000 robson_package-0.0.27/robson_package/__init__.py
--rw-rw-rw-   0        0        0      519 2023-08-09 00:48:42.000000 robson_package-0.0.27/robson_package/conversor.py
-drwxrwxrwx   0        0        0        0 2023-08-09 00:49:09.748595 robson_package-0.0.27/robson_package.egg-info/
--rw-rw-rw-   0        0        0      315 2023-08-09 00:49:09.000000 robson_package-0.0.27/robson_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-09 00:49:09.000000 robson_package-0.0.27/robson_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 00:49:09.000000 robson_package-0.0.27/robson_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-09 00:49:09.000000 robson_package-0.0.27/robson_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-09 00:49:09.753600 robson_package-0.0.27/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-08-09 00:48:48.000000 robson_package-0.0.27/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:56:03.229197 robson_package-0.0.28/
+-rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.28/LICENSE
+-rw-rw-rw-   0        0        0      315 2023-08-09 00:56:03.229197 robson_package-0.0.28/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.28/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 00:56:03.222173 robson_package-0.0.28/robson_package/
+-rw-rw-rw-   0        0        0      519 2023-08-09 00:55:20.000000 robson_package-0.0.28/robson_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:56:03.227654 robson_package-0.0.28/robson_package.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-08-09 00:56:03.000000 robson_package-0.0.28/robson_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-08-09 00:56:03.000000 robson_package-0.0.28/robson_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 00:56:03.000000 robson_package-0.0.28/robson_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-09 00:56:03.000000 robson_package-0.0.28/robson_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 00:56:03.231460 robson_package-0.0.28/setup.cfg
+-rw-rw-rw-   0        0        0      542 2023-08-09 00:55:33.000000 robson_package-0.0.28/setup.py
```

### Comparing `robson_package-0.0.27/LICENSE` & `robson_package-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `robson_package-0.0.27/robson_package/conversor.py` & `robson_package-0.0.28/robson_package/__init__.py`

 * *Files identical despite different names*

### Comparing `robson_package-0.0.27/setup.py` & `robson_package-0.0.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.27'
+VERSION = '0.0.28'
 DESCRIPTION = 'Meu primeiro pacote em Python'
 LONG_DESCRIPTION = 'Meu primeiro pacote em Python com uma descrição um pouco mais longa'
 
 # Setting up
 setup(
     name="robson_package",
     version=VERSION,
```

