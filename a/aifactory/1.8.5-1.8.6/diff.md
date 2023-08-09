# Comparing `tmp/aifactory-1.8.5.tar.gz` & `tmp/aifactory-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.8.5.tar", last modified: Wed Aug  9 02:24:52 2023, max compression
+gzip compressed data, was "aifactory-1.8.6.tar", last modified: Wed Aug  9 02:29:55 2023, max compression
```

## Comparing `aifactory-1.8.5.tar` & `aifactory-1.8.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:24:52.349472 aifactory-1.8.5/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:24:52.349238 aifactory-1.8.5/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:24:52.347259 aifactory-1.8.5/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.5/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.5/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.5/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.5/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.5/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)    14026 2023-08-09 02:24:02.000000 aifactory-1.8.5/aifactory/score.py
--rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.5/aifactory/train.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:24:52.348826 aifactory-1.8.5/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:24:52.000000 aifactory-1.8.5/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-09 02:24:52.000000 aifactory-1.8.5/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-09 02:24:52.000000 aifactory-1.8.5/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-09 02:24:52.000000 aifactory-1.8.5/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-09 02:24:52.000000 aifactory-1.8.5/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-09 02:24:52.349541 aifactory-1.8.5/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-08-09 02:24:31.000000 aifactory-1.8.5/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:29:55.358217 aifactory-1.8.6/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:29:55.358086 aifactory-1.8.6/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:29:55.356260 aifactory-1.8.6/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.6/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.6/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.6/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.6/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.6/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14026 2023-08-09 02:24:02.000000 aifactory-1.8.6/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.6/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:29:55.357854 aifactory-1.8.6/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:29:55.000000 aifactory-1.8.6/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-09 02:29:55.000000 aifactory-1.8.6/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-09 02:29:55.000000 aifactory-1.8.6/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-09 02:29:55.000000 aifactory-1.8.6/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-09 02:29:55.000000 aifactory-1.8.6/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-09 02:29:55.358269 aifactory-1.8.6/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-08-09 02:29:35.000000 aifactory-1.8.6/setup.py
```

### Comparing `aifactory-1.8.5/aifactory/api.py` & `aifactory-1.8.6/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.5/aifactory/demo.py` & `aifactory-1.8.6/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.5/aifactory/grade.py` & `aifactory-1.8.6/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.5/aifactory/make_zip.py` & `aifactory-1.8.6/aifactory/make_zip.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.5/aifactory/score.py` & `aifactory-1.8.6/aifactory/score.py`

 * *Files identical despite different names*

