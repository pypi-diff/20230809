# Comparing `tmp/mlbi_at_dku_lib-0.3.0.tar.gz` & `tmp/mlbi_at_dku_lib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.3.0.tar", last modified: Tue Aug  8 15:35:52 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.3.1.tar", last modified: Tue Aug  8 15:42:33 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.3.0.tar` & `mlbi_at_dku_lib-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:35:52.438177 mlbi_at_dku_lib-0.3.0/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.3.0/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.3.0/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-08-08 15:35:52.438177 mlbi_at_dku_lib-0.3.0/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.3.0/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-08-08 15:35:28.000000 mlbi_at_dku_lib-0.3.0/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-08 15:35:52.438177 mlbi_at_dku_lib-0.3.0/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.3.0/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:35:52.374179 mlbi_at_dku_lib-0.3.0/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:35:52.374179 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-12 11:45:27.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:35:52.426178 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14747 2023-07-13 16:58:06.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10966 2023-08-08 15:33:37.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157995 2023-07-14 18:22:21.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36606 2023-07-12 11:49:13.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-11 14:11:49.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:35:52.374179 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-08-08 15:35:52.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      662 2023-08-08 15:35:52.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-08 15:35:52.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-08 15:35:52.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-08 15:35:52.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-08-08 15:35:52.000000 mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:42:33.516802 mlbi_at_dku_lib-0.3.1/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.3.1/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.3.1/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-08-08 15:42:33.516802 mlbi_at_dku_lib-0.3.1/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.3.1/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-08-08 15:42:17.000000 mlbi_at_dku_lib-0.3.1/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-08 15:42:33.516802 mlbi_at_dku_lib-0.3.1/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.3.1/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:42:33.452803 mlbi_at_dku_lib-0.3.1/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:42:33.452803 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-12 11:45:27.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:42:33.508802 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14747 2023-07-13 16:58:06.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10979 2023-08-08 15:42:09.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157995 2023-07-14 18:22:21.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36606 2023-07-12 11:49:13.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-11 14:11:49.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-08 15:42:33.456803 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-08-08 15:42:33.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      662 2023-08-08 15:42:33.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-08 15:42:33.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-08 15:42:33.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-08 15:42:33.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-08-08 15:42:33.000000 mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/top_level.txt
```

### Comparing `mlbi_at_dku_lib-0.3.0/LICENSE` & `mlbi_at_dku_lib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/PKG-INFO` & `mlbi_at_dku_lib-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.3.0/pyproject.toml` & `mlbi_at_dku_lib-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlbi_at_dku_lib"
-version = "0.3.0"
+version = "0.3.1"
 description = "Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/data/GTmap_hg19.csv` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/data/GTmap_hg38.csv` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/data/GTmap_mm10.csv` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/deg.py` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/deg.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/deiso.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time, os, sys, warnings
+import time, os, sys, warnings, collections
 import numpy as np
 import pandas as pd
 from scipy import stats
 
 SKLEARN = True
 try:
     from sklearn.decomposition import PCA
```

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/hicat.py` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/hicat.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.3.0/src/mlbi_at_dku_lib.egg-info/SOURCES.txt` & `mlbi_at_dku_lib-0.3.1/src/mlbi_at_dku_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

