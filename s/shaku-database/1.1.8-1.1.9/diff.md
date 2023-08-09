# Comparing `tmp/shaku-database-1.1.8.tar.gz` & `tmp/shaku-database-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.8.tar", last modified: Tue Aug  1 01:27:23 2023, max compression
+gzip compressed data, was "shaku-database-1.1.9.tar", last modified: Wed Aug  9 02:47:35 2023, max compression
```

## Comparing `shaku-database-1.1.8.tar` & `shaku-database-1.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.388624 shaku-database-1.1.8/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.8/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-08-01 01:27:23.388401 shaku-database-1.1.8/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.8/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386004 shaku-database-1.1.8/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.8/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386366 shaku-database-1.1.8/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.8/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.8/database/bigquery/bq_sql_parser.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.8/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386616 shaku-database-1.1.8/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.8/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.8/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386864 shaku-database-1.1.8/database/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.8/database/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.8/database/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.386997 shaku-database-1.1.8/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.387227 shaku-database-1.1.8/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.387484 shaku-database-1.1.8/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    17515 2023-08-01 01:26:48.000000 shaku-database-1.1.8/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-08-01 01:27:23.388667 shaku-database-1.1.8/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-08-01 01:26:50.000000 shaku-database-1.1.8/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-01 01:27:23.388177 shaku-database-1.1.8/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-08-01 01:27:23.000000 shaku-database-1.1.8/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.529456 shaku-database-1.1.9/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.9/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-08-09 02:47:35.529255 shaku-database-1.1.9/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.9/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.526065 shaku-database-1.1.9/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.9/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.526576 shaku-database-1.1.9/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.9/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.9/database/bigquery/bq_sql_parser.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     2099 2023-08-09 02:46:26.000000 shaku-database-1.1.9/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.526919 shaku-database-1.1.9/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.9/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.9/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.527277 shaku-database-1.1.9/database/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.9/database/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.9/database/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.527514 shaku-database-1.1.9/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.9/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.527756 shaku-database-1.1.9/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.9/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.9/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.528138 shaku-database-1.1.9/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.9/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    17515 2023-08-01 01:26:48.000000 shaku-database-1.1.9/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-08-09 02:47:35.529502 shaku-database-1.1.9/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-08-09 02:46:37.000000 shaku-database-1.1.9/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-08-09 02:47:35.529055 shaku-database-1.1.9/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-08-09 02:47:35.000000 shaku-database-1.1.9/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-08-09 02:47:35.000000 shaku-database-1.1.9/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-08-09 02:47:35.000000 shaku-database-1.1.9/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-08-09 02:47:35.000000 shaku-database-1.1.9/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-08-09 02:47:35.000000 shaku-database-1.1.9/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.8/LICENSE` & `shaku-database-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.8/PKG-INFO` & `shaku-database-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.8
+Version: 1.1.9
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.8/README.md` & `shaku-database-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.8/database/bigquery/bq_sql_parser.py` & `shaku-database-1.1.9/database/bigquery/bq_sql_parser.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.8/database/bigquery/util.py` & `shaku-database-1.1.9/database/bigquery/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from google.cloud import bigquery
-
 from google.cloud.exceptions import NotFound
 
 
 def save_data_to_bq(insert_df, dataset_id, table_id):
     try:
         client = bigquery.Client()
         # 資料表參數
@@ -47,7 +46,19 @@
     else:
         schema = [bigquery.SchemaField(col, t, mode="REQUIRED") for col, t in zip(columns, types)]
     table = bigquery.Table(table_name, schema=schema)
     table = client.create_table(table)  # Make an API request.
     print(
         "Created table {}.{}.{}".format(table.project, table.dataset_id, table.table_id)
     )
+
+
+def get_table_info(dataset, table_name):
+    client = bigquery.Client()
+    # table_id = 'your-project.your_dataset.your_table'
+    full_table_id = f'{dataset}.{table_name}'
+    table = client.get_table(full_table_id)
+    # print("Table schema: {}".format(table.schema))
+    # print("Table description: {}".format(table.description))
+    # print("Table has {} rows".format(table.num_rows))
+    return table.schema
+
```

### Comparing `shaku-database-1.1.8/database/cloud_sql/crud.py` & `shaku-database-1.1.9/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.8/database/cloud_storage/util.py` & `shaku-database-1.1.9/database/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.8/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.9/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.8/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.9/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.8/setup.py` & `shaku-database-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 EX_INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else ""
                        for s in requirements.split("\n")}
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 setup(
     name="shaku-database",
-    version="1.1.8",
+    version="1.1.9",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.8/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.9/shaku_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.8
+Version: 1.1.9
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.8/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.9/shaku_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.8/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.9/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

