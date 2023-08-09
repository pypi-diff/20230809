# Comparing `tmp/robson_package-0.0.21.tar.gz` & `tmp/robson_package-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robson_package-0.0.21.tar", last modified: Wed Aug  9 00:00:34 2023, max compression
+gzip compressed data, was "robson_package-0.0.22.tar", last modified: Wed Aug  9 00:15:01 2023, max compression
```

## Comparing `robson_package-0.0.21.tar` & `robson_package-0.0.22.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 00:00:34.921765 robson_package-0.0.21/
--rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.21/LICENSE
--rw-rw-rw-   0        0        0      260 2023-08-09 00:00:34.921765 robson_package-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.21/README.md
-drwxrwxrwx   0        0        0        0 2023-08-09 00:00:34.917753 robson_package-0.0.21/robson_package.egg-info/
--rw-rw-rw-   0        0        0      260 2023-08-09 00:00:34.000000 robson_package-0.0.21/robson_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-08-09 00:00:34.000000 robson_package-0.0.21/robson_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 00:00:34.000000 robson_package-0.0.21/robson_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-08-09 00:00:34.000000 robson_package-0.0.21/robson_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-09 00:00:34.921765 robson_package-0.0.21/setup.cfg
--rw-rw-rw-   0        0        0      482 2023-08-08 23:56:04.000000 robson_package-0.0.21/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-09 00:00:34.921765 robson_package-0.0.21/src/
--rw-rw-rw-   0        0        0      185 2023-08-08 23:45:03.000000 robson_package-0.0.21/src/__init__.py
--rw-rw-rw-   0        0        0      515 2023-08-08 11:56:48.000000 robson_package-0.0.21/src/robson_package.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:15:01.336452 robson_package-0.0.22/
+-rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.22/LICENSE
+-rw-rw-rw-   0        0        0      301 2023-08-09 00:15:01.336452 robson_package-0.0.22/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.22/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 00:15:01.331315 robson_package-0.0.22/robson_package.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-08-09 00:15:01.000000 robson_package-0.0.22/robson_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-08-09 00:15:01.000000 robson_package-0.0.22/robson_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 00:15:01.000000 robson_package-0.0.22/robson_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-08-09 00:15:01.000000 robson_package-0.0.22/robson_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 00:15:01.336452 robson_package-0.0.22/setup.cfg
+-rw-rw-rw-   0        0        0      534 2023-08-09 00:14:57.000000 robson_package-0.0.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:15:01.334296 robson_package-0.0.22/src/
+-rw-rw-rw-   0        0        0       21 2023-08-09 00:01:57.000000 robson_package-0.0.22/src/__init__.py
+-rw-rw-rw-   0        0        0      515 2023-08-08 11:56:48.000000 robson_package-0.0.22/src/robson_package.py
```

### Comparing `robson_package-0.0.21/LICENSE` & `robson_package-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `robson_package-0.0.21/src/robson_package.py` & `robson_package-0.0.22/src/robson_package.py`

 * *Files identical despite different names*

