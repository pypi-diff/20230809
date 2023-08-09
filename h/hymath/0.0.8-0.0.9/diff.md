# Comparing `tmp/hymath-0.0.8.tar.gz` & `tmp/hymath-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hymath-0.0.8.tar", last modified: Mon Mar  8 04:20:40 2021, max compression
+gzip compressed data, was "hymath-0.0.9.tar", last modified: Wed Aug  9 03:05:10 2023, max compression
```

## Comparing `hymath-0.0.8.tar` & `hymath-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-03-08 04:20:40.243962 hymath-0.0.8/
--rw-rw-rw-   0        0        0      393 2021-03-08 04:20:40.233750 hymath-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-03-08 04:20:40.161424 hymath-0.0.8/hymath/
--rw-rw-rw-   0        0        0        0 2021-02-14 11:53:16.000000 hymath-0.0.8/hymath/__init__.py
--rw-rw-rw-   0        0        0     1255 2021-03-08 03:34:41.000000 hymath-0.0.8/hymath/math.py
--rw-rw-rw-   0        0        0     3049 2021-03-08 04:20:19.000000 hymath-0.0.8/hymath/print.py
-drwxrwxrwx   0        0        0        0 2021-03-08 04:20:40.191108 hymath-0.0.8/hymath.egg-info/
--rw-rw-rw-   0        0        0      393 2021-03-08 04:20:39.000000 hymath-0.0.8/hymath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2021-03-08 04:20:39.000000 hymath-0.0.8/hymath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-08 04:20:39.000000 hymath-0.0.8/hymath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-03-08 04:20:39.000000 hymath-0.0.8/hymath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-03-08 04:20:40.243962 hymath-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      505 2021-03-08 04:20:19.000000 hymath-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:05:10.484372 hymath-0.0.9/
+-rw-rw-rw-   0        0        0      338 2023-08-09 03:05:10.482491 hymath-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-09 03:05:10.461077 hymath-0.0.9/hymath/
+-rw-rw-rw-   0        0        0        0 2023-08-09 02:19:32.000000 hymath-0.0.9/hymath/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-08-09 03:03:49.000000 hymath-0.0.9/hymath/math.py
+-rw-rw-rw-   0        0        0     3049 2023-08-09 02:21:07.000000 hymath-0.0.9/hymath/print.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:05:10.478416 hymath-0.0.9/hymath.egg-info/
+-rw-rw-rw-   0        0        0      338 2023-08-09 03:05:10.000000 hymath-0.0.9/hymath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-08-09 03:05:10.000000 hymath-0.0.9/hymath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 03:05:10.000000 hymath-0.0.9/hymath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-09 03:05:10.000000 hymath-0.0.9/hymath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 03:05:10.484372 hymath-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      688 2023-08-09 02:25:40.000000 hymath-0.0.9/setup.py
```

### Comparing `hymath-0.0.8/hymath/print.py` & `hymath-0.0.9/hymath/print.py`

 * *Files identical despite different names*

