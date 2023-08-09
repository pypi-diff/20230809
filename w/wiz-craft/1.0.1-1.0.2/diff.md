# Comparing `tmp/wiz-craft-1.0.1.tar.gz` & `tmp/wiz-craft-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiz-craft-1.0.1.tar", last modified: Sun Aug  6 06:57:28 2023, max compression
+gzip compressed data, was "wiz-craft-1.0.2.tar", last modified: Wed Aug  9 04:42:59 2023, max compression
```

## Comparing `wiz-craft-1.0.1.tar` & `wiz-craft-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 06:57:28.906555 wiz-craft-1.0.1/
--rw-rw-rw-   0        0        0     1089 2023-08-06 03:51:07.000000 wiz-craft-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3345 2023-08-06 06:57:28.905555 wiz-craft-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2566 2023-08-06 04:39:16.000000 wiz-craft-1.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-06 06:57:28.906555 wiz-craft-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1845 2023-08-06 06:57:18.000000 wiz-craft-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 06:57:28.904550 wiz-craft-1.0.1/wiz_craft.egg-info/
--rw-rw-rw-   0        0        0     3345 2023-08-06 06:57:28.000000 wiz-craft-1.0.1/wiz_craft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-08-06 06:57:28.000000 wiz-craft-1.0.1/wiz_craft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 06:57:28.000000 wiz-craft-1.0.1/wiz_craft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-08-06 06:57:28.000000 wiz-craft-1.0.1/wiz_craft.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 06:57:28.000000 wiz-craft-1.0.1/wiz_craft.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 04:42:59.408468 wiz-craft-1.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-08-06 03:51:07.000000 wiz-craft-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4029 2023-08-09 04:42:59.407468 wiz-craft-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3053 2023-08-09 04:03:14.000000 wiz-craft-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-09 04:42:59.408468 wiz-craft-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1772 2023-08-09 04:30:42.000000 wiz-craft-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 04:42:59.406470 wiz-craft-1.0.2/wiz_craft.egg-info/
+-rw-rw-rw-   0        0        0     4029 2023-08-09 04:42:59.000000 wiz-craft-1.0.2/wiz_craft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-08-09 04:42:59.000000 wiz-craft-1.0.2/wiz_craft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 04:42:59.000000 wiz-craft-1.0.2/wiz_craft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-08-09 04:42:59.000000 wiz-craft-1.0.2/wiz_craft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 04:42:59.000000 wiz-craft-1.0.2/wiz_craft.egg-info/top_level.txt
```

### Comparing `wiz-craft-1.0.1/LICENSE` & `wiz-craft-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wiz-craft-1.0.1/setup.py` & `wiz-craft-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from setuptools import setup, find_packages
 
 with open('Readme.md', 'r') as file_handler:
     long_description = file_handler.read()
 
-VERSION = '1.0.1',
 DESCRIPTION = 'A CLI-based dataset preprocessing tool for machine learning tasks. Features include data exploration, ' \
               'null value handling, one-hot encoding, and feature scaling, and download the modified dataset ' \
               'effortlessly. '
 setup(
     name='wiz-craft',
-    version='1.0.1',
+    version='1.0.2',
+    url='https://github.com/Pinak-Datta/wiz-craft',
     author_email='pinakdatta2002@gmail.com',
     author='Pinak Datta',
+    license='OSI Approved :: MIT License',
     description='A CLI-based dataset preprocessing tool for machine learning tasks. Features include data '
                 'exploration, null value handling, one-hot encoding, and feature scaling, and download the modified '
                 'dataset effortlessly.',
     long_description_content_type='text/markdown',
     long_description=long_description,
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'scikit-learn',
         'scipy',
         'pandoc'
     ],
-    keywords=['Dataset preprocessing', 'Data cleaning', 'Machine learning', 'Data analysis', 'Data manipulation',
-              'Data preparation', 'Data engineering', 'CLI tool', 'Command Line Interface', 'Data science',
-              'Feature scaling', 'One-hot encoding', 'Data imputation', 'Null value handling', 'Data exploration',
-              'Data visualization', 'Python library', 'Data transformation', 'Data processing', 'DataWiz', 'Wizcraft',
+    keywords=['Dataset preprocessing', 'Data cleaning', 'Machine learning', 'Data manipulation',
+              'Data preparation', 'Data engineering', 'Feature scaling', 'One-hot encoding', 'Data imputation', 'Null value handling', 'Data exploration',
+              'Data processing', 'wizcraft',
               'wiz-craft', 'WizCraft'
-    ],
+              ],
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: Unix",
```

