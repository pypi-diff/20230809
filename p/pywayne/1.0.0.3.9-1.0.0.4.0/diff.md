# Comparing `tmp/pywayne-1.0.0.3.9.tar.gz` & `tmp/pywayne-1.0.0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.3.9.tar", last modified: Mon May 15 07:59:08 2023, max compression
+gzip compressed data, was "pywayne-1.0.0.4.0.tar", last modified: Wed Aug  9 03:16:41 2023, max compression
```

## Comparing `pywayne-1.0.0.3.9.tar` & `pywayne-1.0.0.4.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-05-15 07:59:08.559360 pywayne-1.0.0.3.9/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)      951 2023-05-15 07:59:08.559225 pywayne-1.0.0.3.9/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      528 2023-02-10 11:37:25.000000 pywayne-1.0.0.3.9/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-05-15 07:59:08.558157 pywayne-1.0.0.3.9/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      173 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-02-04 02:47:36.000000 pywayne-1.0.0.3.9/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16676 2023-05-15 07:58:38.000000 pywayne-1.0.0.3.9/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7353 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)     6904 2022-11-16 06:56:46.000000 pywayne-1.0.0.3.9/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-05-15 07:59:08.559014 pywayne-1.0.0.3.9/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)      951 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      305 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      133 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2023-05-15 07:59:08.000000 pywayne-1.0.0.3.9/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2023-05-15 07:59:08.559414 pywayne-1.0.0.3.9/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1409 2023-05-15 07:58:46.000000 pywayne-1.0.0.3.9/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-08-09 03:16:41.903039 pywayne-1.0.0.4.0/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2022-11-16 06:56:46.000000 pywayne-1.0.0.4.0/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)      951 2023-08-09 03:16:41.902907 pywayne-1.0.0.4.0/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      528 2023-02-10 11:37:25.000000 pywayne-1.0.0.4.0/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-08-09 03:16:41.901557 pywayne-1.0.0.4.0/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-08-08 11:53:30.000000 pywayne-1.0.0.4.0/pywayne/__init__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-08-09 03:16:41.902475 pywayne-1.0.0.4.0/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-08-09 03:13:09.000000 pywayne-1.0.0.4.0/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     1898 2023-08-09 03:13:23.000000 pywayne-1.0.0.4.0/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-08-09 03:16:41.902708 pywayne-1.0.0.4.0/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-08-09 03:13:03.000000 pywayne-1.0.0.4.0/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      219 2023-08-09 03:12:58.000000 pywayne-1.0.0.4.0/pywayne/calibration/spatial_temporal.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-02-04 02:47:36.000000 pywayne-1.0.0.4.0/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16676 2023-05-15 07:58:38.000000 pywayne-1.0.0.4.0/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7353 2022-11-16 06:56:46.000000 pywayne-1.0.0.4.0/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2022-11-16 06:56:46.000000 pywayne-1.0.0.4.0/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2022-11-16 06:56:46.000000 pywayne-1.0.0.4.0/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6904 2022-11-16 06:56:46.000000 pywayne-1.0.0.4.0/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2023-08-09 03:16:41.902212 pywayne-1.0.0.4.0/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)      951 2023-08-09 03:16:41.000000 pywayne-1.0.0.4.0/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      424 2023-08-09 03:16:41.000000 pywayne-1.0.0.4.0/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2023-08-09 03:16:41.000000 pywayne-1.0.0.4.0/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      133 2023-08-09 03:16:41.000000 pywayne-1.0.0.4.0/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2023-08-09 03:16:41.000000 pywayne-1.0.0.4.0/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2023-08-09 03:16:41.903081 pywayne-1.0.0.4.0/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1409 2023-08-09 03:15:52.000000 pywayne-1.0.0.4.0/setup.py
```

### Comparing `pywayne-1.0.0.3.9/LICENSE` & `pywayne-1.0.0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.9/PKG-INFO` & `pywayne-1.0.0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.3.9
+Version: 1.0.0.4.0
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.3.9/README.md` & `pywayne-1.0.0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.9/pywayne/data_structure.py` & `pywayne-1.0.0.4.0/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.9/pywayne/dsp.py` & `pywayne-1.0.0.4.0/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.9/pywayne/gui.py` & `pywayne-1.0.0.4.0/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.9/pywayne/math.py` & `pywayne-1.0.0.4.0/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.9/pywayne/plot.py` & `pywayne-1.0.0.4.0/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.9/pywayne/tools.py` & `pywayne-1.0.0.4.0/pywayne/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.3.9/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.4.0/pywayne.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.3.9
+Version: 1.0.0.4.0
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.3.9/setup.py` & `pywayne-1.0.0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return [line for line in lineiter if line and not line.startswith("#") and not line.startswith("~")]
 
 
 install_reqs = parse_requirements('requirements.txt')
 
 setuptools.setup(
     name="pywayne",
-    version="1.0.0.3.9",
+    version="1.0.0.4.0",
     author="Wayne",
     author_email="wang121ye@hotmail.com",
     description="Some useful tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wangyendt/wangye_algorithm_lib",
     classifiers=[
```

