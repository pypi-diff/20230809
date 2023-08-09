# Comparing `tmp/robson_package-0.0.25.tar.gz` & `tmp/robson_package-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robson_package-0.0.25.tar", last modified: Wed Aug  9 00:34:52 2023, max compression
+gzip compressed data, was "robson_package-0.0.26.tar", last modified: Wed Aug  9 00:45:33 2023, max compression
```

## Comparing `robson_package-0.0.25.tar` & `robson_package-0.0.26.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 00:34:52.703584 robson_package-0.0.25/
--rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.25/LICENSE
--rw-rw-rw-   0        0        0      315 2023-08-09 00:34:52.702579 robson_package-0.0.25/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.25/README.md
-drwxrwxrwx   0        0        0        0 2023-08-09 00:34:52.693584 robson_package-0.0.25/robson_package/
--rw-rw-rw-   0        0        0       21 2023-08-09 00:22:10.000000 robson_package-0.0.25/robson_package/__init__.py
--rw-rw-rw-   0        0        0      515 2023-08-08 11:56:48.000000 robson_package-0.0.25/robson_package/robson_package.py
-drwxrwxrwx   0        0        0        0 2023-08-09 00:34:52.700581 robson_package-0.0.25/robson_package.egg-info/
--rw-rw-rw-   0        0        0      315 2023-08-09 00:34:52.000000 robson_package-0.0.25/robson_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-08-09 00:34:52.000000 robson_package-0.0.25/robson_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 00:34:52.000000 robson_package-0.0.25/robson_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-09 00:34:52.000000 robson_package-0.0.25/robson_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-09 00:34:52.704582 robson_package-0.0.25/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-08-09 00:34:50.000000 robson_package-0.0.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:45:33.536118 robson_package-0.0.26/
+-rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.26/LICENSE
+-rw-rw-rw-   0        0        0      315 2023-08-09 00:45:33.535123 robson_package-0.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.26/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 00:45:33.525116 robson_package-0.0.26/robson_package/
+-rw-rw-rw-   0        0        0       16 2023-08-09 00:44:58.000000 robson_package-0.0.26/robson_package/__init__.py
+-rw-rw-rw-   0        0        0      515 2023-08-08 11:56:48.000000 robson_package-0.0.26/robson_package/conversor.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:45:33.533119 robson_package-0.0.26/robson_package.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-08-09 00:45:33.000000 robson_package-0.0.26/robson_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-09 00:45:33.000000 robson_package-0.0.26/robson_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 00:45:33.000000 robson_package-0.0.26/robson_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-09 00:45:33.000000 robson_package-0.0.26/robson_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 00:45:33.536118 robson_package-0.0.26/setup.cfg
+-rw-rw-rw-   0        0        0      542 2023-08-09 00:44:25.000000 robson_package-0.0.26/setup.py
```

### Comparing `robson_package-0.0.25/LICENSE` & `robson_package-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `robson_package-0.0.25/robson_package/robson_package.py` & `robson_package-0.0.26/robson_package/conversor.py`

 * *Files identical despite different names*

### Comparing `robson_package-0.0.25/setup.py` & `robson_package-0.0.26/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
-VERSION = '0.0.25'
+VERSION = '0.0.26'
 DESCRIPTION = 'Meu primeiro pacote em Python'
-LONG_DESCRIPTION = 'Meu primeiro pacote em Python com uma descrição im pouco mais longa'
+LONG_DESCRIPTION = 'Meu primeiro pacote em Python com uma descrição um pouco mais longa'
 
 # Setting up
 setup(
     name="robson_package",
     version=VERSION,
     author="Robson-tech",
     author_email="robson.junior@ufpi.edu.br",
```

