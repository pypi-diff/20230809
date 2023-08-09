# Comparing `tmp/chalk-harness-1.2.3.tar.gz` & `tmp/chalk-harness-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalk-harness-1.2.3.tar", last modified: Mon Aug  7 22:43:24 2023, max compression
+gzip compressed data, was "chalk-harness-1.2.4.tar", last modified: Tue Aug  8 21:32:57 2023, max compression
```

## Comparing `chalk-harness-1.2.3.tar` & `chalk-harness-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/chalk_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-07 22:43:23.000000 chalk-harness-1.2.3/chalk_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-07 22:43:24.000000 chalk-harness-1.2.3/chalk_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:43:23.000000 chalk-harness-1.2.3/chalk_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 22:43:23.000000 chalk-harness-1.2.3/chalk_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 22:43:23.000000 chalk-harness-1.2.3/chalk_harness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/chalkharness/
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/chalkharness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/chalkharness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:24.063546 chalk-harness-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/tests/SanityTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:43:02.000000 chalk-harness-1.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:32:57.200918 chalk-harness-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 21:32:57.200918 chalk-harness-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:32:57.200918 chalk-harness-1.2.4/chalk_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 21:32:57.000000 chalk-harness-1.2.4/chalk_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-08 21:32:57.000000 chalk-harness-1.2.4/chalk_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:32:57.000000 chalk-harness-1.2.4/chalk_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 21:32:57.000000 chalk-harness-1.2.4/chalk_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 21:32:57.000000 chalk-harness-1.2.4/chalk_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:32:57.200918 chalk-harness-1.2.4/chalkharness/
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/chalkharness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/chalkharness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:32:57.200918 chalk-harness-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:32:57.200918 chalk-harness-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/tests/SanityTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:32:43.000000 chalk-harness-1.2.4/tests/__init__.py
```

### Comparing `chalk-harness-1.2.3/README.md` & `chalk-harness-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.3/chalkharness/__init__.py` & `chalk-harness-1.2.4/chalkharness/__init__.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.3/setup.py` & `chalk-harness-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.2.3/tests/SanityTestCase.py` & `chalk-harness-1.2.4/tests/SanityTestCase.py`

 * *Files identical despite different names*

