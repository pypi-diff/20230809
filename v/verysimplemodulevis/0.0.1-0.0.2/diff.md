# Comparing `tmp/verysimplemodulevis-0.0.1.tar.gz` & `tmp/verysimplemodulevis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimplemodulevis-0.0.1.tar", last modified: Tue Aug  8 22:19:47 2023, max compression
+gzip compressed data, was "verysimplemodulevis-0.0.2.tar", last modified: Wed Aug  9 02:07:45 2023, max compression
```

## Comparing `verysimplemodulevis-0.0.1.tar` & `verysimplemodulevis-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 22:19:47.413681 verysimplemodulevis-0.0.1/
--rw-rw-rw-   0        0        0     1098 2023-08-08 11:50:36.000000 verysimplemodulevis-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      667 2023-08-08 22:19:47.410683 verysimplemodulevis-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-08 22:19:47.413681 verysimplemodulevis-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-08-08 22:18:00.000000 verysimplemodulevis-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-08 22:19:47.376357 verysimplemodulevis-0.0.1/verysimplemodulevis.egg-info/
--rw-rw-rw-   0        0        0      667 2023-08-08 22:19:46.000000 verysimplemodulevis-0.0.1/verysimplemodulevis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-08-08 22:19:47.000000 verysimplemodulevis-0.0.1/verysimplemodulevis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 22:19:46.000000 verysimplemodulevis-0.0.1/verysimplemodulevis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 22:19:46.000000 verysimplemodulevis-0.0.1/verysimplemodulevis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 02:07:45.678285 verysimplemodulevis-0.0.2/
+-rw-rw-rw-   0        0        0     1098 2023-08-08 11:50:36.000000 verysimplemodulevis-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      667 2023-08-09 02:07:45.674287 verysimplemodulevis-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-09 02:07:45.682282 verysimplemodulevis-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-08-09 01:54:27.000000 verysimplemodulevis-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 02:07:45.672289 verysimplemodulevis-0.0.2/verysimplemodulevis.egg-info/
+-rw-rw-rw-   0        0        0      667 2023-08-09 02:07:45.000000 verysimplemodulevis-0.0.2/verysimplemodulevis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-08-09 02:07:45.000000 verysimplemodulevis-0.0.2/verysimplemodulevis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 02:07:45.000000 verysimplemodulevis-0.0.2/verysimplemodulevis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 02:07:45.000000 verysimplemodulevis-0.0.2/verysimplemodulevis.egg-info/top_level.txt
```

### Comparing `verysimplemodulevis-0.0.1/LICENSE` & `verysimplemodulevis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `verysimplemodulevis-0.0.1/PKG-INFO` & `verysimplemodulevis-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verysimplemodulevis
-Version: 0.0.1
+Version: 0.0.2
 Summary: Meu primeiro projeto em Python
 Author: Victor Macedo
 Author-email: victormacedocarvalho09@gmail.com
 Keywords: python module example
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `verysimplemodulevis-0.0.1/setup.py` & `verysimplemodulevis-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Meu primeiro projeto em Python'
 LONG_DESCRIPTION = 'Esta é a descrição longa do meu projeto.'
 
 # Configurando o setup
 setup(
     name="verysimplemodulevis",
     version=VERSION,
```

### Comparing `verysimplemodulevis-0.0.1/verysimplemodulevis.egg-info/PKG-INFO` & `verysimplemodulevis-0.0.2/verysimplemodulevis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verysimplemodulevis
-Version: 0.0.1
+Version: 0.0.2
 Summary: Meu primeiro projeto em Python
 Author: Victor Macedo
 Author-email: victormacedocarvalho09@gmail.com
 Keywords: python module example
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

