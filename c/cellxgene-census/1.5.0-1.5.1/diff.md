# Comparing `tmp/cellxgene_census-1.5.0.tar.gz` & `tmp/cellxgene_census-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.5.0.tar", last modified: Sun Aug  6 21:56:55 2023, max compression
+gzip compressed data, was "cellxgene_census-1.5.1.tar", last modified: Tue Aug  8 23:28:13 2023, max compression
```

## Comparing `cellxgene_census-1.5.0.tar` & `cellxgene_census-1.5.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.306281 cellxgene_census-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/src/cellxgene_census/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/src/cellxgene_census/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26112 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/ml/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/_csr_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/_eager_iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.310281 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 21:56:55.000000 cellxgene_census-1.5.0/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    56048 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/ml/test_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/pp/test_hvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/pp/test_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/pp/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 21:56:55.314281 cellxgene_census-1.5.0/tests/experimental/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/experimental/util/test_csr_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-06 21:56:42.000000 cellxgene_census-1.5.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.927824 cellxgene_census-1.5.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.927824 cellxgene_census-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.927824 cellxgene_census-1.5.1/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.927824 cellxgene_census-1.5.1/src/cellxgene_census/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/src/cellxgene_census/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26112 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/ml/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/src/cellxgene_census/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/pp/_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/pp/_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/src/cellxgene_census/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/util/_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/src/cellxgene_census/experimental/util/_eager_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.927824 cellxgene_census-1.5.1/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-08 23:28:13.000000 cellxgene_census-1.5.1/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-08 23:28:13.000000 cellxgene_census-1.5.1/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:28:13.000000 cellxgene_census-1.5.1/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-08 23:28:13.000000 cellxgene_census-1.5.1/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 23:28:13.000000 cellxgene_census-1.5.1/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    56048 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/tests/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/experimental/ml/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/tests/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/experimental/pp/test_hvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/experimental/pp/test_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/experimental/pp/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:28:13.931824 cellxgene_census-1.5.1/tests/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/experimental/util/test_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-08 23:28:01.000000 cellxgene_census-1.5.1/tests/test_util.py
```

### Comparing `cellxgene_census-1.5.0/LICENSE` & `cellxgene_census-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/PKG-INFO` & `cellxgene_census-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.5.0
+Version: 1.5.1
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.5.0/README.md` & `cellxgene_census-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/pyproject.toml` & `cellxgene_census-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies= [
     # NOTE: the tiledbsoma version must be >= to the version used in the Census builder, to
     # ensure that the assets are readable (tiledbsoma supports backward compatible reading).
     # Make sure this version does not fall behind the builder's tiledbsoma version.
-    "tiledbsoma==1.2.7",
+    "tiledbsoma==1.4.0",
     "anndata",
     "numpy>=1.21,<1.25",  # numpy is constrained by numba and the old pip solver
     "requests",
     "typing_extensions",
     "s3fs>=2021.06.1",
     "scipy<1.11",  # work around incompatibility between scipy and pyarrow
     # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
```

### Comparing `cellxgene_census-1.5.0/release_process.md` & `cellxgene_census-1.5.1/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/__init__.py` & `cellxgene_census-1.5.1/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.5.1/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.5.1/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/_open.py` & `cellxgene_census-1.5.1/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.5.1/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.5.1/src/cellxgene_census/_release_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/experimental/ml/pytorch.py` & `cellxgene_census-1.5.1/src/cellxgene_census/experimental/ml/pytorch.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py` & `cellxgene_census-1.5.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_online.py` & `cellxgene_census-1.5.1/src/cellxgene_census/experimental/pp/_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/experimental/pp/_stats.py` & `cellxgene_census-1.5.1/src/cellxgene_census/experimental/pp/_stats.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/_csr_iter.py` & `cellxgene_census-1.5.1/src/cellxgene_census/experimental/util/_csr_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census/experimental/util/_eager_iter.py` & `cellxgene_census-1.5.1/src/cellxgene_census/experimental/util/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.5.1/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.5.0
+Version: 1.5.1
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.5.0/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.5.1/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/README.md` & `cellxgene_census-1.5.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/conftest.py` & `cellxgene_census-1.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/experimental/ml/test_pytorch.py` & `cellxgene_census-1.5.1/tests/experimental/ml/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/experimental/pp/test_hvg.py` & `cellxgene_census-1.5.1/tests/experimental/pp/test_hvg.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/experimental/pp/test_online.py` & `cellxgene_census-1.5.1/tests/experimental/pp/test_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/experimental/pp/test_stats.py` & `cellxgene_census-1.5.1/tests/experimental/pp/test_stats.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/experimental/util/test_csr_iter.py` & `cellxgene_census-1.5.1/tests/experimental/util/test_csr_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/test_acceptance.py` & `cellxgene_census-1.5.1/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/test_directory.py` & `cellxgene_census-1.5.1/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/test_get_anndata.py` & `cellxgene_census-1.5.1/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/test_get_helpers.py` & `cellxgene_census-1.5.1/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/test_open.py` & `cellxgene_census-1.5.1/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.5.0/tests/test_util.py` & `cellxgene_census-1.5.1/tests/test_util.py`

 * *Files identical despite different names*

