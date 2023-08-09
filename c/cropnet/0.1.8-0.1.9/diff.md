# Comparing `tmp/cropnet-0.1.8.tar.gz` & `tmp/cropnet-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropnet-0.1.8.tar", last modified: Tue Aug  8 22:26:45 2023, max compression
+gzip compressed data, was "cropnet-0.1.9.tar", last modified: Tue Aug  8 23:06:27 2023, max compression
```

## Comparing `cropnet-0.1.8.tar` & `cropnet-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:26:45.773485 cropnet-0.1.8/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-08-08 22:26:45.773485 cropnet-0.1.8/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4071 2023-08-05 18:54:16.000000 cropnet-0.1.8/README.md
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:26:45.773485 cropnet-0.1.8/cropnet/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       54 2023-08-08 22:07:02.000000 cropnet-0.1.8/cropnet/__init__.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     9033 2023-08-08 21:11:09.000000 cropnet-0.1.8/cropnet/data_downloader.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     8217 2023-08-07 07:16:24.000000 cropnet-0.1.8/cropnet/data_retriever.py
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:26:45.773485 cropnet-0.1.8/cropnet/dataset/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-08-08 22:07:02.000000 cropnet-0.1.8/cropnet/dataset/__init__.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     6251 2023-08-05 18:54:16.000000 cropnet-0.1.8/cropnet/dataset/hrrr_computed_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-08-05 18:54:16.000000 cropnet-0.1.8/cropnet/dataset/sentinel2_imagery.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     2433 2023-08-05 18:54:16.000000 cropnet-0.1.8/cropnet/dataset/usda_crop_dataset.py
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:26:45.773485 cropnet-0.1.8/cropnet/utils/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        0 2023-08-05 21:36:09.000000 cropnet-0.1.8/cropnet/utils/__init__.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     8716 2023-08-07 06:31:22.000000 cropnet-0.1.8/cropnet/utils/download_USDA.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)    22738 2023-08-08 22:04:24.000000 cropnet-0.1.8/cropnet/utils/download_sentinel.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     6994 2023-08-07 04:04:10.000000 cropnet-0.1.8/cropnet/utils/download_wrf.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)    37414 2023-08-07 04:04:10.000000 cropnet-0.1.8/cropnet/utils/extract_wrf_data.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     2016 2023-08-05 21:40:46.000000 cropnet-0.1.8/cropnet/utils/geo_utils.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     3057 2023-08-07 05:10:49.000000 cropnet-0.1.8/cropnet/utils/path_utils.py
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 22:26:45.773485 cropnet-0.1.8/cropnet.egg-info/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-08-08 22:26:45.000000 cropnet-0.1.8/cropnet.egg-info/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      599 2023-08-08 22:26:45.000000 cropnet-0.1.8/cropnet.egg-info/SOURCES.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-08-08 22:26:45.000000 cropnet-0.1.8/cropnet.egg-info/dependency_links.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      250 2023-08-08 22:26:45.000000 cropnet-0.1.8/cropnet.egg-info/requires.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-08-08 22:26:45.000000 cropnet-0.1.8/cropnet.egg-info/top_level.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-08-08 22:26:45.773485 cropnet-0.1.8/setup.cfg
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1510 2023-08-08 22:26:42.000000 cropnet-0.1.8/setup.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 23:06:27.283748 cropnet-0.1.9/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     5164 2023-08-08 23:06:27.283748 cropnet-0.1.9/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4479 2023-08-08 23:03:09.000000 cropnet-0.1.9/README.md
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 23:06:27.279748 cropnet-0.1.9/cropnet/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       54 2023-08-08 22:07:02.000000 cropnet-0.1.9/cropnet/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     9033 2023-08-08 21:11:09.000000 cropnet-0.1.9/cropnet/data_downloader.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     8217 2023-08-07 07:16:24.000000 cropnet-0.1.9/cropnet/data_retriever.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 23:06:27.279748 cropnet-0.1.9/cropnet/dataset/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-08-08 22:07:02.000000 cropnet-0.1.9/cropnet/dataset/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     6251 2023-08-05 18:54:16.000000 cropnet-0.1.9/cropnet/dataset/hrrr_computed_dataset.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-08-05 18:54:16.000000 cropnet-0.1.9/cropnet/dataset/sentinel2_imagery.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     2433 2023-08-05 18:54:16.000000 cropnet-0.1.9/cropnet/dataset/usda_crop_dataset.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 23:06:27.283748 cropnet-0.1.9/cropnet/utils/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        0 2023-08-05 21:36:09.000000 cropnet-0.1.9/cropnet/utils/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     8716 2023-08-07 06:31:22.000000 cropnet-0.1.9/cropnet/utils/download_USDA.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)    22738 2023-08-08 22:04:24.000000 cropnet-0.1.9/cropnet/utils/download_sentinel.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     6994 2023-08-07 04:04:10.000000 cropnet-0.1.9/cropnet/utils/download_wrf.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)    37414 2023-08-07 04:04:10.000000 cropnet-0.1.9/cropnet/utils/extract_wrf_data.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     2016 2023-08-05 21:40:46.000000 cropnet-0.1.9/cropnet/utils/geo_utils.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     3057 2023-08-07 05:10:49.000000 cropnet-0.1.9/cropnet/utils/path_utils.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 23:06:27.283748 cropnet-0.1.9/cropnet/utils/supplementary/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        0 2023-08-05 21:36:09.000000 cropnet-0.1.9/cropnet/utils/supplementary/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4802 2023-08-07 04:04:10.000000 cropnet-0.1.9/cropnet/utils/supplementary/geo_grid_recent.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-08-08 23:06:27.279748 cropnet-0.1.9/cropnet.egg-info/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     5164 2023-08-08 23:06:27.000000 cropnet-0.1.9/cropnet.egg-info/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      686 2023-08-08 23:06:27.000000 cropnet-0.1.9/cropnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-08-08 23:06:27.000000 cropnet-0.1.9/cropnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      250 2023-08-08 23:06:27.000000 cropnet-0.1.9/cropnet.egg-info/requires.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-08-08 23:06:27.000000 cropnet-0.1.9/cropnet.egg-info/top_level.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-08-08 23:06:27.283748 cropnet-0.1.9/setup.cfg
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1541 2023-08-08 23:06:19.000000 cropnet-0.1.9/setup.py
```

### Comparing `cropnet-0.1.8/PKG-INFO` & `cropnet-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
@@ -70,10 +70,25 @@
 
 ```python
 pip install cropnet
 ```
 
 
 
+Note that if your Python version is older than 3.10.0, you may need to run the following commend before installation to make sure `cartopy` is successfully installed:
+
+```shell
+sudo apt install python3-dev libproj-dev proj-data proj-bin libgeos-dev
+# If using Python 3.x, consider installing python3.x-dev
+sudo apt install python3.10-dev
+
+# install required package for Heribe
+pip install ecmwflibs
+```
+
+
+
+
+
 ## License
 
 CropNet has a [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/) license.
```

### Comparing `cropnet-0.1.8/README.md` & `cropnet-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -52,10 +52,25 @@
 
 ```python
 pip install cropnet
 ```
 
 
 
+Note that if your Python version is older than 3.10.0, you may need to run the following commend before installation to make sure `cartopy` is successfully installed:
+
+```shell
+sudo apt install python3-dev libproj-dev proj-data proj-bin libgeos-dev
+# If using Python 3.x, consider installing python3.x-dev
+sudo apt install python3.10-dev
+
+# install required package for Heribe
+pip install ecmwflibs
+```
+
+
+
+
+
 ## License
 
 CropNet has a [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/) license.
```

### Comparing `cropnet-0.1.8/cropnet/data_downloader.py` & `cropnet-0.1.9/cropnet/data_downloader.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/data_retriever.py` & `cropnet-0.1.9/cropnet/data_retriever.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/dataset/hrrr_computed_dataset.py` & `cropnet-0.1.9/cropnet/dataset/hrrr_computed_dataset.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/dataset/sentinel2_imagery.py` & `cropnet-0.1.9/cropnet/dataset/sentinel2_imagery.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/dataset/usda_crop_dataset.py` & `cropnet-0.1.9/cropnet/dataset/usda_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/utils/download_USDA.py` & `cropnet-0.1.9/cropnet/utils/download_USDA.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/utils/download_sentinel.py` & `cropnet-0.1.9/cropnet/utils/download_sentinel.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/utils/download_wrf.py` & `cropnet-0.1.9/cropnet/utils/download_wrf.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/utils/extract_wrf_data.py` & `cropnet-0.1.9/cropnet/utils/extract_wrf_data.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/utils/geo_utils.py` & `cropnet-0.1.9/cropnet/utils/geo_utils.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet/utils/path_utils.py` & `cropnet-0.1.9/cropnet/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.8/cropnet.egg-info/PKG-INFO` & `cropnet-0.1.9/cropnet.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
@@ -70,10 +70,25 @@
 
 ```python
 pip install cropnet
 ```
 
 
 
+Note that if your Python version is older than 3.10.0, you may need to run the following commend before installation to make sure `cartopy` is successfully installed:
+
+```shell
+sudo apt install python3-dev libproj-dev proj-data proj-bin libgeos-dev
+# If using Python 3.x, consider installing python3.x-dev
+sudo apt install python3.10-dev
+
+# install required package for Heribe
+pip install ecmwflibs
+```
+
+
+
+
+
 ## License
 
 CropNet has a [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/) license.
```

### Comparing `cropnet-0.1.8/cropnet.egg-info/SOURCES.txt` & `cropnet-0.1.9/cropnet.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 cropnet/dataset/usda_crop_dataset.py
 cropnet/utils/__init__.py
 cropnet/utils/download_USDA.py
 cropnet/utils/download_sentinel.py
 cropnet/utils/download_wrf.py
 cropnet/utils/extract_wrf_data.py
 cropnet/utils/geo_utils.py
-cropnet/utils/path_utils.py
+cropnet/utils/path_utils.py
+cropnet/utils/supplementary/__init__.py
+cropnet/utils/supplementary/geo_grid_recent.py
```

### Comparing `cropnet-0.1.8/setup.py` & `cropnet-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 # read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cropnet',
-    version='0.1.8',
+    version='0.1.9',
     description='A Python package for the CropNet dataset',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Anonymous AI4Science',
     author_email='anonymous.ai4science@gmail.com',
     license='Free for non-commercial use',
-    packages=['cropnet', 'cropnet.dataset', 'cropnet.utils'],
+    packages=['cropnet', 'cropnet.dataset', 'cropnet.utils', 'cropnet.utils.supplementary'],
     install_requires=[
         'torch >= 1.13.0',
         'torchvision >= 0.14.0',
         'numpy >= 1.24.4',
         'pandas >= 2.0.3',
         'h5py >= 3.9.0',
         'Pillow >= 10.0.0',
```

