# Comparing `tmp/aifactory-1.8.2.tar.gz` & `tmp/aifactory-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.8.2.tar", last modified: Wed Aug  9 01:58:15 2023, max compression
+gzip compressed data, was "aifactory-1.8.3.tar", last modified: Wed Aug  9 02:14:30 2023, max compression
```

## Comparing `aifactory-1.8.2.tar` & `aifactory-1.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 01:58:15.285806 aifactory-1.8.2/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 01:58:15.285646 aifactory-1.8.2/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 01:58:15.284713 aifactory-1.8.2/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)    14001 2023-08-09 01:55:13.000000 aifactory-1.8.2/aifactory/score.py
--rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/train.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 01:58:15.285355 aifactory-1.8.2/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-09 01:58:15.285857 aifactory-1.8.2/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-08-09 01:36:48.000000 aifactory-1.8.2/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:14:30.366236 aifactory-1.8.3/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:14:30.366096 aifactory-1.8.3/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:14:30.364813 aifactory-1.8.3/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14001 2023-08-09 01:55:13.000000 aifactory-1.8.3/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:14:30.365878 aifactory-1.8.3/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-09 02:14:30.366284 aifactory-1.8.3/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-08-09 02:14:22.000000 aifactory-1.8.3/setup.py
```

### Comparing `aifactory-1.8.2/aifactory/api.py` & `aifactory-1.8.3/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.2/aifactory/demo.py` & `aifactory-1.8.3/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.2/aifactory/grade.py` & `aifactory-1.8.3/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.2/aifactory/make_zip.py` & `aifactory-1.8.3/aifactory/make_zip.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.2/aifactory/score.py` & `aifactory-1.8.3/aifactory/score.py`

 * *Files identical despite different names*

