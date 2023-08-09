# Comparing `tmp/torchdatasets-nightly-1691452981.tar.gz` & `tmp/torchdatasets-nightly-1691539373.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchdatasets-nightly-1691452981.tar", last modified: Tue Aug  8 00:03:07 2023, max compression
+gzip compressed data, was "dist/torchdatasets-nightly-1691539373.tar", last modified: Wed Aug  9 00:02:58 2023, max compression
```

## Comparing `torchdatasets-nightly-1691452981.tar` & `torchdatasets-nightly-1691539373.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/cachers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/maps_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/modifiers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/samplers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/torchdata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/torchdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/_dev_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/_name.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/cachers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24308 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-08-08 00:03:01.000000 torchdatasets-nightly-1691452981/torchdatasets/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/torchdatasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/torchdatasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/torchdatasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/torchdatasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/torchdatasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 00:03:06.000000 torchdatasets-nightly-1691452981/torchdatasets_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/cachers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/maps_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/modifiers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/samplers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/torchdata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/torchdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/_dev_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/cachers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24308 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-08-09 00:02:53.000000 torchdatasets-nightly-1691539373/torchdatasets/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/torchdatasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/torchdatasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/torchdatasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/torchdatasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/torchdatasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-09 00:02:58.000000 torchdatasets-nightly-1691539373/torchdatasets_nightly.egg-info/top_level.txt
```

### Comparing `torchdatasets-nightly-1691452981/PKG-INFO` & `torchdatasets-nightly-1691539373/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchdatasets-nightly
-Version: 1691452981
+Version: 1691539373
 Summary: PyTorch based library focused on data processing and input pipelines in general.
 Home-page: https://github.com/szymonmaszke/torchdatasets
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchdatasets
 Project-URL: Documentation, https://szymonmaszke.github.io/torchdatasets/#torchdatasets
```

### Comparing `torchdatasets-nightly-1691452981/README.md` & `torchdatasets-nightly-1691539373/README.md`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/setup.py` & `torchdatasets-nightly-1691539373/setup.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/tests/cachers_test.py` & `torchdatasets-nightly-1691539373/tests/cachers_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/tests/datasets.py` & `torchdatasets-nightly-1691539373/tests/datasets.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/tests/datasets_test.py` & `torchdatasets-nightly-1691539373/tests/datasets_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/tests/maps_test.py` & `torchdatasets-nightly-1691539373/tests/maps_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/tests/modifiers_test.py` & `torchdatasets-nightly-1691539373/tests/modifiers_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/tests/samplers_test.py` & `torchdatasets-nightly-1691539373/tests/samplers_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/tests/torchdata_test.py` & `torchdatasets-nightly-1691539373/tests/torchdata_test.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/tests/utils.py` & `torchdatasets-nightly-1691539373/tests/utils.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/torchdatasets/__init__.py` & `torchdatasets-nightly-1691539373/torchdatasets/__init__.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/torchdatasets/_base.py` & `torchdatasets-nightly-1691539373/torchdatasets/_base.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/torchdatasets/cachers.py` & `torchdatasets-nightly-1691539373/torchdatasets/cachers.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/torchdatasets/datasets.py` & `torchdatasets-nightly-1691539373/torchdatasets/datasets.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/torchdatasets/maps.py` & `torchdatasets-nightly-1691539373/torchdatasets/maps.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/torchdatasets/modifiers.py` & `torchdatasets-nightly-1691539373/torchdatasets/modifiers.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/torchdatasets/samplers.py` & `torchdatasets-nightly-1691539373/torchdatasets/samplers.py`

 * *Files identical despite different names*

### Comparing `torchdatasets-nightly-1691452981/torchdatasets_nightly.egg-info/PKG-INFO` & `torchdatasets-nightly-1691539373/torchdatasets_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchdatasets-nightly
-Version: 1691452981
+Version: 1691539373
 Summary: PyTorch based library focused on data processing and input pipelines in general.
 Home-page: https://github.com/szymonmaszke/torchdatasets
 Author: Szymon Maszke
 Author-email: szymon.maszke@protonmail.com
 License: MIT
 Project-URL: Website, https://szymonmaszke.github.io/torchdatasets
 Project-URL: Documentation, https://szymonmaszke.github.io/torchdatasets/#torchdatasets
```

### Comparing `torchdatasets-nightly-1691452981/torchdatasets_nightly.egg-info/SOURCES.txt` & `torchdatasets-nightly-1691539373/torchdatasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

