# Comparing `tmp/cropnet-0.1.6.tar.gz` & `tmp/cropnet-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropnet-0.1.6.tar", last modified: Sun Jun 18 22:28:11 2023, max compression
+gzip compressed data, was "cropnet-0.1.7.tar", last modified: Tue Aug  8 22:11:13 2023, max compression
```

## Comparing `cropnet-0.1.6.tar` & `cropnet-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,28 @@
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 22:28:11.759532 cropnet-0.1.6/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-06-18 22:28:11.759532 cropnet-0.1.6/PKG-INFO
--rw-r--r--   0 fudong    (1000) fudong    (1000)     4071 2023-06-18 21:41:32.000000 cropnet-0.1.6/README.md
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 22:28:11.755532 cropnet-0.1.6/cropnet/
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 22:28:11.759532 cropnet-0.1.6/cropnet/dataset/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-18 22:27:38.000000 cropnet-0.1.6/cropnet/dataset/__init__.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     6251 2023-06-18 21:33:51.000000 cropnet-0.1.6/cropnet/dataset/hrrr_computed_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-06-17 22:36:51.000000 cropnet-0.1.6/cropnet/dataset/sentinel2_imagery.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     2433 2023-06-18 21:33:51.000000 cropnet-0.1.6/cropnet/dataset/usda_crop_dataset.py
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 22:28:11.755532 cropnet-0.1.6/cropnet.egg-info/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-06-18 22:28:11.000000 cropnet-0.1.6/cropnet.egg-info/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      315 2023-06-18 22:28:11.000000 cropnet-0.1.6/cropnet.egg-info/SOURCES.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-18 22:28:11.000000 cropnet-0.1.6/cropnet.egg-info/dependency_links.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       77 2023-06-18 22:28:11.000000 cropnet-0.1.6/cropnet.egg-info/requires.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-18 22:28:11.000000 cropnet-0.1.6/cropnet.egg-info/top_level.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-18 22:28:11.759532 cropnet-0.1.6/setup.cfg
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1215 2023-06-18 22:27:38.000000 cropnet-0.1.6/setup.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:11:13.486788 cropnet-0.1.7/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4706 2023-08-08 22:11:13.486788 cropnet-0.1.7/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4071 2023-08-05 18:54:16.000000 cropnet-0.1.7/README.md
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:11:13.486788 cropnet-0.1.7/cropnet/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       54 2023-08-08 22:07:02.000000 cropnet-0.1.7/cropnet/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     9033 2023-08-08 21:11:09.000000 cropnet-0.1.7/cropnet/data_downloader.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     8217 2023-08-07 07:16:24.000000 cropnet-0.1.7/cropnet/data_retriever.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:11:13.486788 cropnet-0.1.7/cropnet/dataset/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-08-08 22:07:02.000000 cropnet-0.1.7/cropnet/dataset/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     6251 2023-08-05 18:54:16.000000 cropnet-0.1.7/cropnet/dataset/hrrr_computed_dataset.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-08-05 18:54:16.000000 cropnet-0.1.7/cropnet/dataset/sentinel2_imagery.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     2433 2023-08-05 18:54:16.000000 cropnet-0.1.7/cropnet/dataset/usda_crop_dataset.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:11:13.486788 cropnet-0.1.7/cropnet/utils/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        0 2023-08-05 21:36:09.000000 cropnet-0.1.7/cropnet/utils/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     8716 2023-08-07 06:31:22.000000 cropnet-0.1.7/cropnet/utils/download_USDA.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)    22738 2023-08-08 22:04:24.000000 cropnet-0.1.7/cropnet/utils/download_sentinel.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     6994 2023-08-07 04:04:10.000000 cropnet-0.1.7/cropnet/utils/download_wrf.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)    37414 2023-08-07 04:04:10.000000 cropnet-0.1.7/cropnet/utils/extract_wrf_data.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     2016 2023-08-05 21:40:46.000000 cropnet-0.1.7/cropnet/utils/geo_utils.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     3057 2023-08-07 05:10:49.000000 cropnet-0.1.7/cropnet/utils/path_utils.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:11:13.486788 cropnet-0.1.7/cropnet.egg-info/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4706 2023-08-08 22:11:13.000000 cropnet-0.1.7/cropnet.egg-info/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      599 2023-08-08 22:11:13.000000 cropnet-0.1.7/cropnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-08-08 22:11:13.000000 cropnet-0.1.7/cropnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      250 2023-08-08 22:11:13.000000 cropnet-0.1.7/cropnet.egg-info/requires.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-08-08 22:11:13.000000 cropnet-0.1.7/cropnet.egg-info/top_level.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-08-08 22:11:13.486788 cropnet-0.1.7/setup.cfg
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1461 2023-08-08 22:10:58.000000 cropnet-0.1.7/setup.py
```

### Comparing `cropnet-0.1.6/PKG-INFO` & `cropnet-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # CropNet
```

### Comparing `cropnet-0.1.6/README.md` & `cropnet-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.6/cropnet/dataset/hrrr_computed_dataset.py` & `cropnet-0.1.7/cropnet/dataset/hrrr_computed_dataset.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.6/cropnet/dataset/sentinel2_imagery.py` & `cropnet-0.1.7/cropnet/dataset/sentinel2_imagery.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.6/cropnet/dataset/usda_crop_dataset.py` & `cropnet-0.1.7/cropnet/dataset/usda_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.6/cropnet.egg-info/PKG-INFO` & `cropnet-0.1.7/cropnet.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # CropNet
```

### Comparing `cropnet-0.1.6/setup.py` & `cropnet-0.1.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,39 +3,44 @@
 
 # read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cropnet',
-    version='0.1.6',
+    version='0.1.7',
     description='A Python package for the CropNet dataset',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Anonymous AI4Science',
     author_email='anonymous.ai4science@gmail.com',
     license='Free for non-commercial use',
-    packages=['cropnet.dataset'],
+    packages=['cropnet', 'cropnet.dataset', 'cropnet.utils'],
     install_requires=[
-        'torch >= 1.11.0',
-        'numpy',
-        'torchvision',
-        'numpy',
-        'pandas',
-        'h5py',
-        'Pillow',
-        'einops',
-        'scikit-learn',
+        'torch >= 1.13.0',
+        'torchvision >= 0.14.0',
+        'numpy >= 1.24.4',
+        'pandas >= 2.0.3',
+        'h5py >= 3.9.0',
+        'Pillow >= 10.0.0',
+        'einops >= 0.6.1',
+        'scikit-learn >= 1.3.0',
+        'matplotlib >= 3.7.2',
+        'oauthlib >= 3.2.2',
+        'requests-oauthlib >= 1.3.1',
+        'geopandas >= 0.13.2',
+        'shapely >= 2.0.1',
+        'tqdm >= 4.65.0',
+        'herbie-data >= 2023.3.0',
     ],
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'License :: Free for non-commercial use',
         'Operating System :: MacOS',
         'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
 )
```

