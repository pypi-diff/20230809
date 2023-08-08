# Comparing `tmp/oceanum-0.8.3.tar.gz` & `tmp/oceanum-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.8.3.tar", last modified: Mon Jul 31 20:56:06 2023, max compression
+gzip compressed data, was "oceanum-0.9.0.tar", last modified: Tue Aug  8 22:49:24 2023, max compression
```

## Comparing `oceanum-0.8.3.tar` & `oceanum-0.9.0.tar`

### file list

```diff
@@ -1,69 +1,76 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.498687 oceanum-0.8.3/
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.8.3/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.8.3/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.8.3/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.8.3/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1112 2023-07-31 20:56:06.498687 oceanum-0.8.3/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.8.3/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.462690 oceanum-0.8.3/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.450691 oceanum-0.8.3/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.450691 oceanum-0.8.3/docs/_build/html/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.462690 oceanum-0.8.3/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.450691 oceanum-0.8.3/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.466689 oceanum-0.8.3/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/api.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.450691 oceanum-0.8.3/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.466689 oceanum-0.8.3/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/classes/datamesh/oceanum.datamesh.Query.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.8.3/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.8.3/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.8.3/docs/usage.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.470689 oceanum-0.8.3/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      656 2023-07-31 20:55:59.000000 oceanum-0.8.3/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.8.3/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.482689 oceanum-0.8.3/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.8.3/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.8.3/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    21330 2023-07-30 21:15:42.000000 oceanum-0.8.3/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11333 2023-07-30 20:00:11.000000 oceanum-0.8.3/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      186 2023-07-31 20:33:46.000000 oceanum-0.8.3/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7854 2023-07-31 20:54:29.000000 oceanum-0.8.3/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.8.3/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.474689 oceanum-0.8.3/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1112 2023-07-31 20:56:06.000000 oceanum-0.8.3/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1372 2023-07-31 20:56:06.000000 oceanum-0.8.3/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-31 20:56:06.000000 oceanum-0.8.3/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-07-31 20:56:06.000000 oceanum-0.8.3/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-31 20:56:06.000000 oceanum-0.8.3/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      133 2023-07-31 20:56:06.000000 oceanum-0.8.3/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-07-31 20:56:06.000000 oceanum-0.8.3/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-07-31 20:56:06.498687 oceanum-0.8.3/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1311 2023-07-31 20:54:49.000000 oceanum-0.8.3/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.490688 oceanum-0.8.3/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:56:06.494688 oceanum-0.8.3/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.8.3/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-07-11 23:07:04.000000 oceanum-0.8.3/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.8.3/tests/test_video_compat.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.673147 oceanum-0.9.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.9.0/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.9.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.9.0/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1112 2023-08-08 22:49:24.673147 oceanum-0.9.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.9.0/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.657147 oceanum-0.9.0/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/Makefile
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.649147 oceanum-0.9.0/docs/_build/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.649147 oceanum-0.9.0/docs/_build/html/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.657147 oceanum-0.9.0/docs/_build/html/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2022-12-01 21:44:17.000000 oceanum-0.9.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.9.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.9.0/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.649147 oceanum-0.9.0/docs/_templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.657147 oceanum-0.9.0/docs/_templates/autosummary/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/about.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      741 2023-08-08 22:43:41.000000 oceanum-0.9.0/docs/api.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.649147 oceanum-0.9.0/docs/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.657147 oceanum-0.9.0/docs/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/classes/datamesh/oceanum.datamesh.Connector.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/classes/datamesh/oceanum.datamesh.Query.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.657147 oceanum-0.9.0/docs/classes/storage/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2388 2023-08-08 22:44:06.000000 oceanum-0.9.0/docs/classes/storage/oceanum.storage.FileSystem.rst
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.9.0/docs/conf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.9.0/docs/index.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/make.bat
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-08-08 22:45:18.000000 oceanum-0.9.0/docs/modules.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/oceanum.datamesh.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      384 2023-08-08 22:45:18.000000 oceanum-0.9.0/docs/oceanum.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      240 2023-08-08 22:45:14.000000 oceanum-0.9.0/docs/oceanum.storage.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.9.0/docs/usage.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.657147 oceanum-0.9.0/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      656 2023-08-08 21:53:39.000000 oceanum-0.9.0/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.9.0/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.661147 oceanum-0.9.0/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.9.0/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.9.0/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21330 2023-07-30 21:15:42.000000 oceanum-0.9.0/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11333 2023-07-30 20:00:11.000000 oceanum-0.9.0/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      186 2023-07-31 20:33:46.000000 oceanum-0.9.0/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7854 2023-07-31 20:54:29.000000 oceanum-0.9.0/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.9.0/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.661147 oceanum-0.9.0/oceanum/storage/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       35 2023-08-07 20:38:45.000000 oceanum-0.9.0/oceanum/storage/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9853 2023-08-08 22:37:46.000000 oceanum-0.9.0/oceanum/storage/filesystem.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.661147 oceanum-0.9.0/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1112 2023-08-08 22:49:24.000000 oceanum-0.9.0/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1529 2023-08-08 22:49:24.000000 oceanum-0.9.0/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-08-08 22:49:24.000000 oceanum-0.9.0/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       98 2023-08-08 22:49:24.000000 oceanum-0.9.0/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-08-08 22:49:24.000000 oceanum-0.9.0/oceanum.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      133 2023-08-08 22:49:24.000000 oceanum-0.9.0/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-08-08 22:49:24.000000 oceanum-0.9.0/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-08-08 22:49:24.673147 oceanum-0.9.0/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1400 2023-08-07 21:27:48.000000 oceanum-0.9.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.665147 oceanum-0.9.0/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-08-08 22:49:24.673147 oceanum-0.9.0/tests/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/data/grid_data_1.nc
+-rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/data/ocean_test_1.mp4
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/data/point_data_1.csv
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.9.0/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-07-11 23:07:04.000000 oceanum-0.9.0/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1827 2023-08-08 22:34:41.000000 oceanum-0.9.0/tests/test_storage.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.9.0/tests/test_video_compat.py
```

### Comparing `oceanum-0.8.3/CONTRIBUTING.rst` & `oceanum-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/LICENSE` & `oceanum-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/PKG-INFO` & `oceanum-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.8.3
+Version: 0.9.0
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 Requires-Python: >=3.8
```

### Comparing `oceanum-0.8.3/README.rst` & `oceanum-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/docs/Makefile` & `oceanum-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/docs/api.rst` & `oceanum-0.9.0/docs/api.rst`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,26 @@
    :toctree: classes/datamesh
 
     Connector
     Datasource
     Catalog
     Query
 
+Storage
+---------------------
+.. currentmodule:: oceanum.storage
+
+
+End-user classes
+
+.. autosummary::
+   :toctree: classes/storage
+
+    FileSystem
+
 .. Internal classes
 
 .. .. autosummary::
 ..    :toctree: classes/datamesh
 
 .. 
     automodule:: oceanum.datamesh.connection
```

### Comparing `oceanum-0.8.3/docs/classes/datamesh/oceanum.datamesh.Connector.rst` & `oceanum-0.9.0/docs/classes/datamesh/oceanum.datamesh.Connector.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/docs/conf.py` & `oceanum-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/docs/index.rst` & `oceanum-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/docs/installation.rst` & `oceanum-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/docs/make.bat` & `oceanum-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/docs/oceanum.datamesh.rst` & `oceanum-0.9.0/docs/oceanum.datamesh.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/docs/usage.rst` & `oceanum-0.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/oceanum/__init__.py` & `oceanum-0.9.0/oceanum/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for oceanum."""
 
 __author__ = """Oceanum Developers"""
 __email__ = "developers@oceanum.science"
-__version__ = "0.8.3"
+__version__ = "0.9.0"
 
 
 # Suppress tracebacks in an ipython environment
 try:
     import sys
 
     ipython = get_ipython()
```

### Comparing `oceanum-0.8.3/oceanum/datamesh/catalog.py` & `oceanum-0.9.0/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/oceanum/datamesh/connection.py` & `oceanum-0.9.0/oceanum/datamesh/connection.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/oceanum/datamesh/datasource.py` & `oceanum-0.9.0/oceanum/datamesh/datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/oceanum/datamesh/query.py` & `oceanum-0.9.0/oceanum/datamesh/query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/oceanum/datamesh/zarr.py` & `oceanum-0.9.0/oceanum/datamesh/zarr.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/oceanum.egg-info/PKG-INFO` & `oceanum-0.9.0/oceanum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.8.3
+Version: 0.9.0
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 Requires-Python: >=3.8
```

### Comparing `oceanum-0.8.3/oceanum.egg-info/SOURCES.txt` & `oceanum-0.9.0/oceanum.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/oceanum.datamesh.rst
 docs/oceanum.rst
+docs/oceanum.storage.rst
 docs/usage.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 docs/_templates/autosummary/class.rst
 docs/classes/datamesh/oceanum.datamesh.Catalog.rst
 docs/classes/datamesh/oceanum.datamesh.Connector.rst
 docs/classes/datamesh/oceanum.datamesh.Datasource.rst
 docs/classes/datamesh/oceanum.datamesh.Query.rst
+docs/classes/storage/oceanum.storage.FileSystem.rst
 oceanum/__init__.py
 oceanum/cli.py
 oceanum.egg-info/PKG-INFO
 oceanum.egg-info/SOURCES.txt
 oceanum.egg-info/dependency_links.txt
 oceanum.egg-info/entry_points.txt
 oceanum.egg-info/not-zip-safe
@@ -36,19 +38,22 @@
 oceanum/datamesh/__init__.py
 oceanum/datamesh/catalog.py
 oceanum/datamesh/connection.py
 oceanum/datamesh/datasource.py
 oceanum/datamesh/exceptions.py
 oceanum/datamesh/query.py
 oceanum/datamesh/zarr.py
+oceanum/storage/__init__.py
+oceanum/storage/filesystem.py
 tests/__init__.py
 tests/test_catalog.py
 tests/test_datamesh_connect.py
 tests/test_datamesh_load.py
 tests/test_datamesh_query.py
 tests/test_datamesh_write.py
 tests/test_datasource.py
 tests/test_query.py
+tests/test_storage.py
 tests/test_video_compat.py
 tests/data/grid_data_1.nc
 tests/data/ocean_test_1.mp4
 tests/data/point_data_1.csv
```

### Comparing `oceanum-0.8.3/setup.py` & `oceanum-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     author="Oceanum Developers",
     author_email="developers@oceanum.science",
     description="Library for oceanum.io services",
     entry_points={
         "console_scripts": [
             "oceanum=oceanum.cli:main",
         ],
+        "fsspec.specs": [
+            "oceanum = oceanum.storage:FileSystem",
+        ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme,
     include_package_data=True,
     keywords="oceanum",
     documentation="https://oceanum-python.readthedocs.io",
```

### Comparing `oceanum-0.8.3/tests/data/grid_data_1.nc` & `oceanum-0.9.0/tests/data/grid_data_1.nc`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/data/ocean_test_1.mp4` & `oceanum-0.9.0/tests/data/ocean_test_1.mp4`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/data/point_data_1.csv` & `oceanum-0.9.0/tests/data/point_data_1.csv`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/test_catalog.py` & `oceanum-0.9.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/test_datamesh_connect.py` & `oceanum-0.9.0/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/test_datamesh_load.py` & `oceanum-0.9.0/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/test_datamesh_query.py` & `oceanum-0.9.0/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/test_datamesh_write.py` & `oceanum-0.9.0/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/test_datasource.py` & `oceanum-0.9.0/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/test_query.py` & `oceanum-0.9.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.3/tests/test_video_compat.py` & `oceanum-0.9.0/tests/test_video_compat.py`

 * *Files identical despite different names*

