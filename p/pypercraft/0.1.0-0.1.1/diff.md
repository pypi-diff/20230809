# Comparing `tmp/pypercraft-0.1.0.tar.gz` & `tmp/pypercraft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypercraft-0.1.0.tar", last modified: Tue Aug  8 00:10:15 2023, max compression
+gzip compressed data, was "pypercraft-0.1.1.tar", last modified: Tue Aug  8 23:51:25 2023, max compression
```

## Comparing `pypercraft-0.1.0.tar` & `pypercraft-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alkhalifas   (501) staff       (20)        0 2023-08-08 00:10:15.376394 pypercraft-0.1.0/
--rw-r--r--   0 alkhalifas   (501) staff       (20)     1072 2023-08-01 12:16:31.000000 pypercraft-0.1.0/LICENSE
--rw-r--r--   0 alkhalifas   (501) staff       (20)      179 2023-08-08 00:10:15.375652 pypercraft-0.1.0/PKG-INFO
--rw-r--r--   0 alkhalifas   (501) staff       (20)      326 2023-08-07 02:42:12.000000 pypercraft-0.1.0/README.md
-drwxr-xr-x   0 alkhalifas   (501) staff       (20)        0 2023-08-08 00:10:15.353245 pypercraft-0.1.0/api/
--rw-r--r--   0 alkhalifas   (501) staff       (20)        0 2023-08-01 12:16:31.000000 pypercraft-0.1.0/api/__init__.py
--rw-r--r--   0 alkhalifas   (501) staff       (20)     1614 2023-08-07 01:37:27.000000 pypercraft-0.1.0/api/api.py
-drwxr-xr-x   0 alkhalifas   (501) staff       (20)        0 2023-08-08 00:10:15.356295 pypercraft-0.1.0/pypercraft/
--rw-r--r--   0 alkhalifas   (501) staff       (20)        0 2023-08-01 12:16:31.000000 pypercraft-0.1.0/pypercraft/__init__.py
--rw-r--r--   0 alkhalifas   (501) staff       (20)     1988 2023-08-07 02:29:37.000000 pypercraft-0.1.0/pypercraft/prompts.py
--rw-r--r--   0 alkhalifas   (501) staff       (20)     5334 2023-08-07 01:21:28.000000 pypercraft-0.1.0/pypercraft/pypercraft.py
-drwxr-xr-x   0 alkhalifas   (501) staff       (20)        0 2023-08-08 00:10:15.369414 pypercraft-0.1.0/pypercraft.egg-info/
--rw-r--r--   0 alkhalifas   (501) staff       (20)      179 2023-08-08 00:10:15.000000 pypercraft-0.1.0/pypercraft.egg-info/PKG-INFO
--rw-r--r--   0 alkhalifas   (501) staff       (20)      353 2023-08-08 00:10:15.000000 pypercraft-0.1.0/pypercraft.egg-info/SOURCES.txt
--rw-r--r--   0 alkhalifas   (501) staff       (20)        1 2023-08-08 00:10:15.000000 pypercraft-0.1.0/pypercraft.egg-info/dependency_links.txt
--rw-r--r--   0 alkhalifas   (501) staff       (20)      134 2023-08-08 00:10:15.000000 pypercraft-0.1.0/pypercraft.egg-info/requires.txt
--rw-r--r--   0 alkhalifas   (501) staff       (20)       21 2023-08-08 00:10:15.000000 pypercraft-0.1.0/pypercraft.egg-info/top_level.txt
--rw-r--r--   0 alkhalifas   (501) staff       (20)       38 2023-08-08 00:10:15.377183 pypercraft-0.1.0/setup.cfg
--rw-r--r--   0 alkhalifas   (501) staff       (20)      514 2023-08-08 00:10:00.000000 pypercraft-0.1.0/setup.py
-drwxr-xr-x   0 alkhalifas   (501) staff       (20)        0 2023-08-08 00:10:15.374448 pypercraft-0.1.0/tests/
--rw-r--r--   0 alkhalifas   (501) staff       (20)        0 2023-08-01 12:16:31.000000 pypercraft-0.1.0/tests/__init__.py
--rw-r--r--   0 alkhalifas   (501) staff       (20)     1691 2023-08-07 01:48:43.000000 pypercraft-0.1.0/tests/test_api.py
--rw-r--r--   0 alkhalifas   (501) staff       (20)     4000 2023-08-07 01:27:04.000000 pypercraft-0.1.0/tests/test_pypercraft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:51:25.261965 pypercraft-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 23:51:13.000000 pypercraft-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-08 23:51:25.257965 pypercraft-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-08 23:51:13.000000 pypercraft-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:51:25.253965 pypercraft-0.1.1/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:51:13.000000 pypercraft-0.1.1/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-08 23:51:13.000000 pypercraft-0.1.1/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:51:25.257965 pypercraft-0.1.1/pypercraft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:51:13.000000 pypercraft-0.1.1/pypercraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-08 23:51:13.000000 pypercraft-0.1.1/pypercraft/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-08-08 23:51:13.000000 pypercraft-0.1.1/pypercraft/pypercraft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:51:25.257965 pypercraft-0.1.1/pypercraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-08 23:51:25.000000 pypercraft-0.1.1/pypercraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-08 23:51:25.000000 pypercraft-0.1.1/pypercraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:51:25.000000 pypercraft-0.1.1/pypercraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-08 23:51:25.000000 pypercraft-0.1.1/pypercraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 23:51:25.000000 pypercraft-0.1.1/pypercraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:51:25.261965 pypercraft-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-08 23:51:13.000000 pypercraft-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:51:25.257965 pypercraft-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:51:13.000000 pypercraft-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-08 23:51:13.000000 pypercraft-0.1.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-08-08 23:51:13.000000 pypercraft-0.1.1/tests/test_pypercraft.py
```

### Comparing `pypercraft-0.1.0/LICENSE` & `pypercraft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypercraft-0.1.0/api/api.py` & `pypercraft-0.1.1/api/api.py`

 * *Files identical despite different names*

### Comparing `pypercraft-0.1.0/pypercraft/prompts.py` & `pypercraft-0.1.1/pypercraft/prompts.py`

 * *Files identical despite different names*

### Comparing `pypercraft-0.1.0/pypercraft/pypercraft.py` & `pypercraft-0.1.1/pypercraft/pypercraft.py`

 * *Files identical despite different names*

### Comparing `pypercraft-0.1.0/tests/test_api.py` & `pypercraft-0.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pypercraft-0.1.0/tests/test_pypercraft.py` & `pypercraft-0.1.1/tests/test_pypercraft.py`

 * *Files identical despite different names*

