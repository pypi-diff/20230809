# Comparing `tmp/PyLandslide-0.0.5.tar.gz` & `tmp/PyLandslide-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLandslide-0.0.5.tar", last modified: Sat Aug  5 12:36:54 2023, max compression
+gzip compressed data, was "PyLandslide-0.0.7.tar", last modified: Tue Aug  8 17:10:51 2023, max compression
```

## Comparing `PyLandslide-0.0.5.tar` & `PyLandslide-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 12:36:54.837258 PyLandslide-0.0.5/
--rw-rw-rw-   0        0        0    35823 2023-07-24 12:23:37.000000 PyLandslide-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      815 2023-08-05 12:36:54.836246 PyLandslide-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 12:36:54.813291 PyLandslide-0.0.5/PyLandslide/
--rw-rw-rw-   0        0        0      125 2023-07-25 14:20:54.000000 PyLandslide-0.0.5/PyLandslide/__init__.py
--rw-rw-rw-   0        0        0     3134 2023-08-05 12:34:15.000000 PyLandslide-0.0.5/PyLandslide/cli.py
--rw-rw-rw-   0        0        0        0 2023-07-25 14:20:54.000000 PyLandslide-0.0.5/PyLandslide/core.py
--rw-rw-rw-   0        0        0     9923 2023-08-05 12:34:15.000000 PyLandslide-0.0.5/PyLandslide/data_preparation.py
--rw-rw-rw-   0        0        0    11546 2023-08-05 12:34:15.000000 PyLandslide-0.0.5/PyLandslide/sensitivity.py
--rw-rw-rw-   0        0        0     8147 2023-07-29 21:05:23.000000 PyLandslide-0.0.5/PyLandslide/weightrange.py
-drwxrwxrwx   0        0        0        0 2023-08-05 12:36:54.832251 PyLandslide-0.0.5/PyLandslide.egg-info/
--rw-rw-rw-   0        0        0      815 2023-08-05 12:36:51.000000 PyLandslide-0.0.5/PyLandslide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-08-05 12:36:53.000000 PyLandslide-0.0.5/PyLandslide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 12:36:51.000000 PyLandslide-0.0.5/PyLandslide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-05 12:36:52.000000 PyLandslide-0.0.5/PyLandslide.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-08-05 12:36:52.000000 PyLandslide-0.0.5/PyLandslide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-05 12:36:52.000000 PyLandslide-0.0.5/PyLandslide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2023-08-05 12:34:15.000000 PyLandslide-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 12:36:54.838250 PyLandslide-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1163 2023-08-05 12:34:15.000000 PyLandslide-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:10:51.187965 PyLandslide-0.0.7/
+-rw-rw-rw-   0        0        0    35823 2023-08-07 11:17:42.000000 PyLandslide-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3448 2023-08-08 17:10:51.185969 PyLandslide-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-08 17:10:51.165974 PyLandslide-0.0.7/PyLandslide/
+-rw-rw-rw-   0        0        0       54 2023-08-07 17:17:37.000000 PyLandslide-0.0.7/PyLandslide/__init__.py
+-rw-rw-rw-   0        0        0     3980 2023-08-07 22:58:51.000000 PyLandslide-0.0.7/PyLandslide/cli.py
+-rw-rw-rw-   0        0        0    12096 2023-08-08 13:16:00.000000 PyLandslide-0.0.7/PyLandslide/data_preparation.py
+-rw-rw-rw-   0        0        0    14905 2023-08-08 16:00:32.000000 PyLandslide-0.0.7/PyLandslide/sensitivity.py
+-rw-rw-rw-   0        0        0    10112 2023-08-08 16:08:12.000000 PyLandslide-0.0.7/PyLandslide/weightrange.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:10:51.182965 PyLandslide-0.0.7/PyLandslide.egg-info/
+-rw-rw-rw-   0        0        0     3448 2023-08-08 17:10:50.000000 PyLandslide-0.0.7/PyLandslide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-08-08 17:10:51.000000 PyLandslide-0.0.7/PyLandslide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 17:10:50.000000 PyLandslide-0.0.7/PyLandslide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-08 17:10:50.000000 PyLandslide-0.0.7/PyLandslide.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-08-08 17:10:50.000000 PyLandslide-0.0.7/PyLandslide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-08 17:10:50.000000 PyLandslide-0.0.7/PyLandslide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2760 2023-08-08 17:04:05.000000 PyLandslide-0.0.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-08 17:10:51.188974 PyLandslide-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-08-08 17:10:36.000000 PyLandslide-0.0.7/setup.py
```

### Comparing `PyLandslide-0.0.5/LICENSE` & `PyLandslide-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.0.5/PyLandslide/data_preparation.py` & `PyLandslide-0.0.7/PyLandslide/data_preparation.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,38 @@
 import numpy as np
 import logging
 import geopandas as gpd
 from rasterio.warp import reproject, Resampling, calculate_default_transform
 import rasterio
 
 class DataPreparation(object):
+    """
+    This is a data preparation class that includes methods for co-registering raster layers and extracting
+    point data for Machine Learning.
+    """
+
     def __init__(self, json_file=None, folder_name=None, *args, **kwargs):
+        """
+        Initialise a new DataPreparation object.
+
+        Args:
+            json_file: JSON-based document specifying the configuration information for performing data preparation.
+
+            folder_name: Folder containing the raster data.
+        """
         super().__init__(*args, **kwargs)
         self.json_file = json_file
         self.folder_name = folder_name
 
-    def load_data_from_json(self, **kwargs):
-        """Load data from a file
+    def load_data_from_json(self):
+        """
+        Loads the configuration JSON-based document assigned to self.json_file. Extracts the data from the JSON-based
+        document and assign them to self.factors, self.output_directory, self.landslide_locations, and
+        self.nonlandslide_locations.
+
         """
         data = os.path.normpath(os.path.join(os.getcwd(), self.json_file))
         self.json_file_directory = os.path.normpath(os.path.dirname(data))
         
         if isinstance(data, str):
             logging.info('Loading data from file: "{}"'.format(data))
             with open(data, "r") as f:
@@ -40,35 +57,41 @@
         self.landslide_locations = os.path.normpath(os.path.join(self.json_file_directory, loaded_file.pop('landslide_locations')))
 
         if loaded_file.get('nonlandslide_locations') is None:
             raise ValueError('nonlandslide_locations has not been found in the JSON file')
         self.nonlandslide_locations = os.path.normpath(os.path.join(self.json_file_directory, loaded_file.pop('nonlandslide_locations')))
 
     def setup(self):
+        """
+        Calls the load_data_from_json method to extract the information provided in the JSON-based document.
+        """
         self.load_data_from_json()
         print('Setting up WeightRangePreparation based on the file: "{}"'.format(self.json_file))
 
     def factor_data_preperation(self, factors):
+        """
+        Takes a list of dictionaries that include factor names and their associated raster files and returns
+        lists of factor names, datasets, and datasets as arrays.
+        """
         names = []
         sets = []
         sets_arrays = []
         for f in factors:
             names.append(f["name"])
             set_temp = rasterio.open(os.path.normpath(os.path.join(self.json_file_directory, f["file"])))
             sets.append(set_temp)
             sets_arrays.append(set_temp.read(1))
         return names, sets, sets_arrays
 
-    def create_results_dict(self, index_array):
-        results_dic = {}
-        for n in index_array:
-            results_dic[n]=[]
-        return results_dic
-
     def extract(self):
+        """
+        Extracts the factor values at the landslide and non-landslide locations. These locations are obtained from the
+        shapefiles provided in the JSON-based document. The results are saved into features.csv (factor values) and
+        targets.csv (landslide or non-landslide status) in the output directory specified in the JSON-based document.
+        """
         print("Preparing and extracting data...")
         factor_data = self.factor_data_preperation(self.factors)
         self.factor_names = factor_data[0]
         self.factor_sets = factor_data[1]
         self.factor_sets_arrays = factor_data[2]
 
         self.landslide_locations_shp = gpd.read_file(self.landslide_locations)
@@ -122,15 +145,29 @@
         targets_df = pd.DataFrame.from_dict(targets)
         targets_df1 = targets_df.dropna(how='any').reset_index(drop=True)
         targets_df1.index.name = 'id'
         targets_df1.to_csv(os.path.join(self.output_directory,'targets.csv'))
 
         print("Completed.")
 
+    def create_results_dict(self, index_array):
+        """
+        Creates a dictionary for saving the results of the extract() method. This method takes the names indices (in
+        this case factor names) as an argument.
+        """
+        results_dic = {}
+        for n in index_array:
+            results_dic[n]=[]
+        return results_dic
+
     def adjust(self):
+        """
+        Looks into the self.folder_name variable and pre-process the raster files located in it by converting them to uint8
+        to reduce data size. The adjusted files are saved into "folder_name/uint8".
+        """
         dir_list = os.listdir(os.path.join(os.getcwd(), self.folder_name))
         raster_files = []
         outfiles = []
         for f in dir_list:
             if f.endswith('.tif') or f.endswith('.tiff'):
                 raster_files.append(os.path.join(os.getcwd(), self.folder_name, f))
                 outfiles.append(os.path.join(os.getcwd(), self.folder_name, "uint8", f))
@@ -146,14 +183,19 @@
                 profile['nodata'] = 255
                 profile['dtype'] = 'uint8'
                 print(rff)
                 with rasterio.open(outfiles[rx], 'w', **profile) as dst:
                     dst.write(masked_ds, 1)
 
     def align(self):
+        """
+        Co-registers the rasters adjusted with the adjust() method by looking into "folder_name/uint8". The
+        co-registration is performed to ensure that all rasters are aligned, have the same resolution, and same array
+        sizes. The resulting co-registered rasters are saved into "folder_name/alinged_rasters".
+        """
         dir_list = os.listdir(os.path.join(os.getcwd(), self.folder_name))
         raster_files = []
         outfiles = []
         for f in dir_list:
             if f.endswith('.tif') or f.endswith('.tiff'):
                 raster_files.append(os.path.join(os.getcwd(), self.folder_name, "uint8", f))
                 outfiles.append(os.path.join(os.getcwd(), self.folder_name, "alinged_rasters", f))
```

### Comparing `PyLandslide-0.0.5/PyLandslide/weightrange.py` & `PyLandslide-0.0.7/PyLandslide/weightrange.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,36 @@
 import logging
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import confusion_matrix
 logger = logging.getLogger(__name__)
 
 class WeightRangeEstimator(object):
+    """
+    This class includes methods for calculating weight ranges of factors contributing to the occurrence of
+    landslides based on Machine Learning.
+    """
+
     def __init__(self, json_file, *args, **kwargs):
+        """
+        Initialise a new WeightRangeEstimator object.
+
+        Args:
+            json_file: JSON-based document specifying the configuration information for performing weight range
+            calculation.
+        """
         super().__init__(*args, **kwargs)
         self.json_file = json_file
 
-    def load_data_from_json(self, **kwargs):
-        """Load data from a file -
+    def load_data_from_json(self):
+        """
+        Loads the configuration JSON-based document assigned to self.json_file. Extracts the data from the JSON-based
+        document and assign them to self.features_file, self.targets_file, self.max_tree_depth, self.number_trees,
+        self.output_file, self.size_testing_sample, self.number_of_iterations, self.cores, and self.performance_cutoff.
+
         """
         data = os.path.normpath(os.path.join(os.getcwd(), self.json_file))
         self.json_file_directory = os.path.normpath(os.path.dirname(data))
 
         if isinstance(data, str):
             logging.info('Loading data from file: "{}"'.format(data))
             with open(data, "r") as f:
@@ -71,19 +87,30 @@
         if loaded_file.get('performance_cutoff') is None:
             print('performance cutoff has been set to 0.75. If you wish to change this default value, add performance_cutoff to the inputs provided in the JSON file')
             self.performance_cutoff = 0.75
         else:
             self.performance_cutoff = loaded_file.pop('performance_cutoff')
 
     def load_data_from_csv(self, filename, index_column):
+        """
+        Loads a CSV file into a Pandas dataframe. Takes the file name and index column as inputs. This method is used to
+        load the features and targets CSV files for Machine Learning.
+
+        """
         temp = pd.read_csv(filename)
         input_data = temp.set_index(index_column)
         return input_data
 
     def calculate_weight_range(self):
+        """
+        Uses Random Forest Classification Machine Learning Models to estimate weight ranges of the factors contributing
+        to the occurrence of landslides. The data required for this method are provided and loaded from the JSON-based
+        document. The results are written to a CSV file specified in the JSON-based document.
+
+        """
         targets_df = self.load_data_from_csv(self.targets_file, index_column = 'id')
         features_df = self.load_data_from_csv(self.features_file, index_column = 'id')
 
         #Cach target and feature names
         target_names = targets_df.columns
         feature_names = features_df.columns
         all_columns = list(feature_names)
@@ -114,22 +141,32 @@
                 results.at[itera, "testing_overall_accuracy"] = metrics[1]
                 for f, feat in enumerate (feature_names):
                     results.at[itera, feat] = importances[0][f]
 
         results.dropna(how='all').to_csv(self.output_file)
 
     def feature_importance_model(self, targets, features, max_tree_depth, n_estimators, cores):
+        """
+        Trains a Random Forest Classification Model and returns the model and the associated feature importance list.
+        This method takes targets, features,  maximum tree depth, number of trees, and number of processing cores as inputs.
+
+        """
         #create a RandomForestClassifier 
         model = RandomForestClassifier(random_state=1, max_depth=max_tree_depth, n_estimators = n_estimators, n_jobs = cores)
         model.fit(features,targets)
         #calculate relative importance
         importance = model.feature_importances_
         return importance, model
         
     def overall_accuracy(self, mod,X_train,Y_train,X_test,Y_test):
+        """
+        Calculates the Overall Accuracy metric of a Machine Learning model for the testing and training data. This
+        method takes the Machine Learning Model and the training and testing data as inputs.
+
+        """
         Y_predicted_test = mod.predict(X_test)
         Y_predicted_train = mod.predict(X_train)
 
         matrix_test = confusion_matrix(Y_test, Y_predicted_test)
         matrix_train = confusion_matrix(Y_train, Y_predicted_train)
 
         TP_TN_test = 0
@@ -155,9 +192,12 @@
         
         print('overall accuracy in training =', round(overall_accuracy_train,3))
         print('overall accuracy in testing =', round(overall_accuracy_test,3))
 
         return overall_accuracy_train, overall_accuracy_test
 
     def setup(self):
+        """
+        Calls the load_data_from_json method to extract the information provided in the JSON-based document.
+        """
         self.load_data_from_json()
         logger.info('Setting up WeightRangeEstimator based on the file: "{}"'.format(self.json_file))
```

### Comparing `PyLandslide-0.0.5/setup.py` & `PyLandslide-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-with open('README.md') as f:
+with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='PyLandslide',
-    version='0.0.5',
+    version='0.0.7',
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     description='Tools for landslide hazard uncertainty analysis.',
     url='https://github.com/IERRG/PyLandslide',
     author='Mohammed Basheer',
     author_email='mohammedadamabbaker@gmail.com',
     license='GNU',
     install_requires=['click','pandas','numpy','scikit-learn','geopandas','rasterio'],
     packages=find_packages(),
```

