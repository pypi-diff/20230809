# Comparing `tmp/allin1-0.0.1.tar.gz` & `tmp/allin1-0.0.2.tar.gz`

## Comparing `allin1-0.0.1.tar` & `allin1-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 allin1-0.0.1/MANIFEST.in
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 allin1-0.0.1/README.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/__init__.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/cli.py
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/config.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/demix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/py.typed
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/run.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/spectrogram.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/typings.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/models/__init__.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/models/allinone.py
--rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/models/dinat.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/models/loaders.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/models/utils.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/postprocessing/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/postprocessing/functional.py
--rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/postprocessing/helpers.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 allin1-0.0.1/src/allinone/postprocessing/metrical.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 allin1-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 allin1-0.0.1/LICENSE
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 allin1-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 allin1-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 allin1-0.0.2/MANIFEST.in
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/__init__.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/cli.py
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/config.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/demix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/py.typed
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/run.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/spectrogram.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/typings.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/models/__init__.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/models/allinone.py
+-rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/models/dinat.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/models/loaders.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/models/utils.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/postprocessing/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/postprocessing/functional.py
+-rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/postprocessing/helpers.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 allin1-0.0.2/src/allinone/postprocessing/metrical.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 allin1-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 allin1-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 allin1-0.0.2/README.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 allin1-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 allin1-0.0.2/PKG-INFO
```

### Comparing `allin1-0.0.1/README.md` & `allin1-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Visit [PyTorch](https://pytorch.org/) and install the appropriate version for your system.
 
 ### 2. Install the package
 
 ```shell
 pip install numpy cython  # madmom dependency
-pip install .
+pip install allin1
 ```
 
 ### 3. (Optional) Install FFmpeg for MP3 support
 
 For ubuntu:
 
 ```shell
```

### Comparing `allin1-0.0.1/src/allinone/cli.py` & `allin1-0.0.2/src/allinone/cli.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/config.py` & `allin1-0.0.2/src/allinone/config.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/demix.py` & `allin1-0.0.2/src/allinone/demix.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/run.py` & `allin1-0.0.2/src/allinone/run.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/spectrogram.py` & `allin1-0.0.2/src/allinone/spectrogram.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/typings.py` & `allin1-0.0.2/src/allinone/typings.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/models/allinone.py` & `allin1-0.0.2/src/allinone/models/allinone.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/models/dinat.py` & `allin1-0.0.2/src/allinone/models/dinat.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/models/loaders.py` & `allin1-0.0.2/src/allinone/models/loaders.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/models/utils.py` & `allin1-0.0.2/src/allinone/models/utils.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/postprocessing/functional.py` & `allin1-0.0.2/src/allinone/postprocessing/functional.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/postprocessing/helpers.py` & `allin1-0.0.2/src/allinone/postprocessing/helpers.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/src/allinone/postprocessing/metrical.py` & `allin1-0.0.2/src/allinone/postprocessing/metrical.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/.gitignore` & `allin1-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `allin1-0.0.1/LICENSE` & `allin1-0.0.2/LICENSE`

 * *Files identical despite different names*

