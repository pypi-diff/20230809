# Comparing `tmp/aeppl-nightly-0.1.5.dev20230807.tar.gz` & `tmp/aeppl-nightly-0.1.5.dev20230808.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-nightly-0.1.5.dev20230807.tar", last modified: Mon Aug  7 00:34:08 2023, max compression
+gzip compressed data, was "aeppl-nightly-0.1.5.dev20230808.tar", last modified: Tue Aug  8 00:32:12 2023, max compression
```

## Comparing `aeppl-nightly-0.1.5.dev20230807.tar` & `aeppl-nightly-0.1.5.dev20230808.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:08.341378 aeppl-nightly-0.1.5.dev20230807/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-07 00:34:08.341378 aeppl-nightly-0.1.5.dev20230807/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:08.341378 aeppl-nightly-0.1.5.dev20230807/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-07 00:34:08.341378 aeppl-nightly-0.1.5.dev20230807/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:08.337378 aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-07 00:34:08.000000 aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-07 00:34:08.000000 aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:34:08.000000 aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 00:34:08.000000 aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-07 00:34:08.000000 aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 00:34:08.000000 aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-07 00:34:08.341378 aeppl-nightly-0.1.5.dev20230807/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 00:34:08.341378 aeppl-nightly-0.1.5.dev20230807/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-08-07 00:33:54.000000 aeppl-nightly-0.1.5.dev20230807/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:32:12.697361 aeppl-nightly-0.1.5.dev20230808/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-08 00:32:12.697361 aeppl-nightly-0.1.5.dev20230808/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:32:12.697361 aeppl-nightly-0.1.5.dev20230808/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-08 00:32:12.697361 aeppl-nightly-0.1.5.dev20230808/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:32:12.693361 aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-08 00:32:12.000000 aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-08 00:32:12.000000 aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 00:32:12.000000 aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 00:32:12.000000 aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-08 00:32:12.000000 aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 00:32:12.000000 aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-08 00:32:12.697361 aeppl-nightly-0.1.5.dev20230808/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:32:12.697361 aeppl-nightly-0.1.5.dev20230808/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-08-08 00:32:02.000000 aeppl-nightly-0.1.5.dev20230808/versioneer.py
```

### Comparing `aeppl-nightly-0.1.5.dev20230807/LICENSE` & `aeppl-nightly-0.1.5.dev20230808/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/PKG-INFO` & `aeppl-nightly-0.1.5.dev20230808/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.5.dev20230807
+Version: 0.1.5.dev20230808
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.5.dev20230807/README.md` & `aeppl-nightly-0.1.5.dev20230808/README.md`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/abstract.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/censoring.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/convolutions.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/cumsum.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/dists.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/joint_logprob.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/logprob.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/mixture.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/printing.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/rewriting.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/scan.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/tensor.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/transforms.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl/utils.py` & `aeppl-nightly-0.1.5.dev20230808/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/PKG-INFO` & `aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.5.dev20230807
+Version: 0.1.5.dev20230808
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.5.dev20230807/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl-nightly-0.1.5.dev20230808/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/setup.cfg` & `aeppl-nightly-0.1.5.dev20230808/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/setup.py` & `aeppl-nightly-0.1.5.dev20230808/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_abstract.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_censoring.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_composite_logprob.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_convolutions.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_cumsum.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_dist.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_joint_logprob.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_logprob.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_mixture.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_printing.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_rewriting.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_scan.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_tensor.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_transforms.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/tests/test_utils.py` & `aeppl-nightly-0.1.5.dev20230808/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.5.dev20230807/versioneer.py` & `aeppl-nightly-0.1.5.dev20230808/versioneer.py`

 * *Files identical despite different names*

