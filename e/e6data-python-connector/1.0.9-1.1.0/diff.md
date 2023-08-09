# Comparing `tmp/e6data-python-connector-1.0.9.tar.gz` & `tmp/e6data-python-connector-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e6data-python-connector-1.0.9.tar", last modified: Wed Jun  7 06:14:32 2023, max compression
+gzip compressed data, was "e6data-python-connector-1.1.0.tar", last modified: Wed Aug  9 05:39:27 2023, max compression
```

## Comparing `e6data-python-connector-1.0.9.tar` & `e6data-python-connector-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-07 06:14:32.505863 e6data-python-connector-1.0.9/
--rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/LICENSE
--rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/MANIFEST.in
--rw-r--r--   0 vishalanand   (501) staff       (20)     7548 2023-06-07 06:14:32.506001 e6data-python-connector-1.0.9/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)     5380 2023-06-07 06:14:30.000000 e6data-python-connector-1.0.9/README.md
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-07 06:14:32.485676 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/
--rw-r--r--   0 vishalanand   (501) staff       (20)     7548 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)      632 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/entry_points.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       66 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/requires.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        6 2023-06-07 06:14:32.000000 e6data-python-connector-1.0.9/e6data_python_connector.egg-info/top_level.txt
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-07 06:14:32.499096 e6data-python-connector-1.0.9/e6xdb/
--rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/common.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/datainputstream.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/date_time_utils.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    17760 2023-06-06 12:43:44.000000 e6data-python-connector-1.0.9/e6xdb/e6x.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/exceptions.py
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-06-07 06:14:32.504535 e6data-python-connector-1.0.9/e6xdb/server/
--rw-r--r--   0 vishalanand   (501) staff       (20)   206971 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.9/e6xdb/server/QueryEngineService.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/server/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/server/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-05-30 06:20:46.000000 e6data-python-connector-1.0.9/e6xdb/server/ttypes.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/sqlalchemy_e6x.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/e6xdb/typeId.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.9/pyproject.toml
--rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-06-07 06:14:32.508451 e6data-python-connector-1.0.9/setup.cfg
--rw-r--r--   0 vishalanand   (501) staff       (20)     1925 2023-06-07 06:14:30.000000 e6data-python-connector-1.0.9/setup.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-08-09 05:39:26.998173 e6data-python-connector-1.1.0/
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/LICENSE
+-rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/MANIFEST.in
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7778 2023-08-09 05:39:26.998376 e6data-python-connector-1.1.0/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)     5586 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/README.md
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-08-09 05:39:26.905907 e6data-python-connector-1.1.0/e6data_python_connector/
+-rw-r--r--   0 vishalanand   (501) staff       (20)       99 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6data_python_connector/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    19629 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6data_python_connector/e6xgrpc.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-08-09 05:39:26.938878 e6data-python-connector-1.1.0/e6data_python_connector/server/
+-rw-r--r--   0 vishalanand   (501) staff       (20)   206971 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6data_python_connector/server/QueryEngineService.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6data_python_connector/server/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6data_python_connector/server/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    16035 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6data_python_connector/server/e6x_engine_pb2.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    46671 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6data_python_connector/server/e6x_engine_pb2_grpc.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6data_python_connector/server/ttypes.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-08-09 05:39:26.927334 e6data-python-connector-1.1.0/e6data_python_connector.egg-info/
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7778 2023-08-09 05:39:26.000000 e6data-python-connector-1.1.0/e6data_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)      878 2023-08-09 05:39:26.000000 e6data-python-connector-1.1.0/e6data_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-08-09 05:39:26.000000 e6data-python-connector-1.1.0/e6data_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-08-09 05:39:26.000000 e6data-python-connector-1.1.0/e6data_python_connector.egg-info/entry_points.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)      102 2023-08-09 05:39:26.000000 e6data-python-connector-1.1.0/e6data_python_connector.egg-info/requires.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       30 2023-08-09 05:39:26.000000 e6data-python-connector-1.1.0/e6data_python_connector.egg-info/top_level.txt
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-08-09 05:39:26.997089 e6data-python-connector-1.1.0/e6xdb/
+-rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/e6xdb/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-08-08 09:43:15.000000 e6data-python-connector-1.1.0/e6xdb/common.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/e6xdb/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/e6xdb/datainputstream.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/e6xdb/date_time_utils.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    17693 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/e6xdb/e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/e6xdb/exceptions.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/e6xdb/sqlalchemy_e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/e6xdb/typeId.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.1.0/pyproject.toml
+-rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-08-09 05:39:27.001742 e6data-python-connector-1.1.0/setup.cfg
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1983 2023-08-09 05:38:58.000000 e6data-python-connector-1.1.0/setup.py
```

### Comparing `e6data-python-connector-1.0.9/LICENSE` & `e6data-python-connector-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/PKG-INFO` & `e6data-python-connector-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.9
+Version: 1.1.0
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Description: # e6data Python Connector
         
-        ![version](https://img.shields.io/badge/version-1.0.9-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.1.0-blue.svg)
         
         ## Introduction
         
         The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
         
         To install the Python package, use the command below:
         ```shell
@@ -25,39 +25,40 @@
         * Access Token generated in the e6data console.
         
         ### Create a Connection
         
         Use your e6data Email ID as the username and your access token as the password.
         
         ```python
-        import e6xdb.e6x as edb
+        from e6data_python_connector import Connection
         
         username = '<username>'  # Your e6data Email ID.
         password = '<password>'  # Access Token generated in the e6data console.
         
         host = '<host>'  # IP address or hostname of the cluster to be used.
         database = '<database>'  # # Database to perform the query on.
         port = 9000  # Port of the e6data engine.
+        catalog_name = '<catalog_name>'
         
-        conn = edb.connect(
+        conn = Connection(
             host=host,
             port=port,
             username=username,
             database=database,
             password=password
         )
         ```
         
         ### Perform a Queries & Get Results
         
         ```python
         
         query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the query.
         
-        cursor = conn.cursor()
+        cursor = conn.cursor(catalog_name=catalog_name)
         query_id = cursor.execute(query)  # The execute function returns a unique query ID, which can be use to abort the query.
         all_records = cursor.fetchall()
         for row in all_records:
            print(row)
         ```
         
         To fetch all the records:
@@ -95,23 +96,23 @@
         query_id = '<query_id>'  # query id from execute function response.
         cursor.cancel(query_id)
         ```
         
         Switch database in an existing connection:
         ```python
         database = '<new_database_name>'  # Replace with the new database.
-        cursor = conn.cursor(database)
+        cursor = conn.cursor(database, catalog_name)
         ```
         
         ### Get Query Time Metrics
         ```python
         import json
         query = 'SELECT * FROM <TABLE_NAME>'
         
-        cursor = conn.cursor()
+        cursor = conn.cursor(catalog_name)
         query_id = cursor.execute(query)  # execute function returns query id, can be use for aborting th query.
         all_records = cursor.fetchall()
         
         query_planner = json.loads(cursor.explain_analyse())
         
         execution_time = query_planner.get("total_query_time")  # In milliseconds
         queue_time = query_planner.get("executionQueueingTime")  # In milliseconds
@@ -163,23 +164,25 @@
         
         host = '<host>'  # IP address or hostname of the cluster to be used.
         database = '<database>'  # # Database to perform the query on.
         port = 9000  # Port of the e6data engine.
         
         sql_query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the actual query.
         
+        catalog_name = '<catalog_name>'  # Replace with the actual catalog name.
+        
         conn = edb.connect(
             host=host,
             port=port,
             username=username,
             database=database,
             password=password
         )
         
-        cursor = conn.cursor(db_name=database)
+        cursor = conn.cursor(db_name=database, catalog_name=catalog_name)
         query_id = cursor.execute(sql_query)
         all_records = cursor.fetchall()
         planner_result = json.loads(cursor.explain_analyse())
         execution_time = planner_result.get("total_query_time") / 1000  # Converting into seconds.
         row_count = planner_result.get('row_count_out')
         columns = [col[0] for col in cursor.description]  # Get the column names and merge them with the results.
         results = []
```

### Comparing `e6data-python-connector-1.0.9/README.md` & `e6data-python-connector-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # e6data Python Connector
 
-![version](https://img.shields.io/badge/version-1.0.9-blue.svg)
+![version](https://img.shields.io/badge/version-1.1.0-blue.svg)
 
 ## Introduction
 
 The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
 
 To install the Python package, use the command below:
 ```shell
@@ -17,39 +17,40 @@
 * Access Token generated in the e6data console.
 
 ### Create a Connection
 
 Use your e6data Email ID as the username and your access token as the password.
 
 ```python
-import e6xdb.e6x as edb
+from e6data_python_connector import Connection
 
 username = '<username>'  # Your e6data Email ID.
 password = '<password>'  # Access Token generated in the e6data console.
 
 host = '<host>'  # IP address or hostname of the cluster to be used.
 database = '<database>'  # # Database to perform the query on.
 port = 9000  # Port of the e6data engine.
+catalog_name = '<catalog_name>'
 
-conn = edb.connect(
+conn = Connection(
     host=host,
     port=port,
     username=username,
     database=database,
     password=password
 )
 ```
 
 ### Perform a Queries & Get Results
 
 ```python
 
 query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the query.
 
-cursor = conn.cursor()
+cursor = conn.cursor(catalog_name=catalog_name)
 query_id = cursor.execute(query)  # The execute function returns a unique query ID, which can be use to abort the query.
 all_records = cursor.fetchall()
 for row in all_records:
    print(row)
 ```
 
 To fetch all the records:
@@ -87,23 +88,23 @@
 query_id = '<query_id>'  # query id from execute function response.
 cursor.cancel(query_id)
 ```
 
 Switch database in an existing connection:
 ```python
 database = '<new_database_name>'  # Replace with the new database.
-cursor = conn.cursor(database)
+cursor = conn.cursor(database, catalog_name)
 ```
 
 ### Get Query Time Metrics
 ```python
 import json
 query = 'SELECT * FROM <TABLE_NAME>'
 
-cursor = conn.cursor()
+cursor = conn.cursor(catalog_name)
 query_id = cursor.execute(query)  # execute function returns query id, can be use for aborting th query.
 all_records = cursor.fetchall()
 
 query_planner = json.loads(cursor.explain_analyse())
 
 execution_time = query_planner.get("total_query_time")  # In milliseconds
 queue_time = query_planner.get("executionQueueingTime")  # In milliseconds
@@ -155,23 +156,25 @@
 
 host = '<host>'  # IP address or hostname of the cluster to be used.
 database = '<database>'  # # Database to perform the query on.
 port = 9000  # Port of the e6data engine.
 
 sql_query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the actual query.
 
+catalog_name = '<catalog_name>'  # Replace with the actual catalog name.
+
 conn = edb.connect(
     host=host,
     port=port,
     username=username,
     database=database,
     password=password
 )
 
-cursor = conn.cursor(db_name=database)
+cursor = conn.cursor(db_name=database, catalog_name=catalog_name)
 query_id = cursor.execute(sql_query)
 all_records = cursor.fetchall()
 planner_result = json.loads(cursor.explain_analyse())
 execution_time = planner_result.get("total_query_time") / 1000  # Converting into seconds.
 row_count = planner_result.get('row_count_out')
 columns = [col[0] for col in cursor.description]  # Get the column names and merge them with the results.
 results = []
```

### Comparing `e6data-python-connector-1.0.9/e6data_python_connector.egg-info/PKG-INFO` & `e6data-python-connector-1.1.0/e6data_python_connector.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.9
+Version: 1.1.0
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Description: # e6data Python Connector
         
-        ![version](https://img.shields.io/badge/version-1.0.9-blue.svg)
+        ![version](https://img.shields.io/badge/version-1.1.0-blue.svg)
         
         ## Introduction
         
         The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
         
         To install the Python package, use the command below:
         ```shell
@@ -25,39 +25,40 @@
         * Access Token generated in the e6data console.
         
         ### Create a Connection
         
         Use your e6data Email ID as the username and your access token as the password.
         
         ```python
-        import e6xdb.e6x as edb
+        from e6data_python_connector import Connection
         
         username = '<username>'  # Your e6data Email ID.
         password = '<password>'  # Access Token generated in the e6data console.
         
         host = '<host>'  # IP address or hostname of the cluster to be used.
         database = '<database>'  # # Database to perform the query on.
         port = 9000  # Port of the e6data engine.
+        catalog_name = '<catalog_name>'
         
-        conn = edb.connect(
+        conn = Connection(
             host=host,
             port=port,
             username=username,
             database=database,
             password=password
         )
         ```
         
         ### Perform a Queries & Get Results
         
         ```python
         
         query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the query.
         
-        cursor = conn.cursor()
+        cursor = conn.cursor(catalog_name=catalog_name)
         query_id = cursor.execute(query)  # The execute function returns a unique query ID, which can be use to abort the query.
         all_records = cursor.fetchall()
         for row in all_records:
            print(row)
         ```
         
         To fetch all the records:
@@ -95,23 +96,23 @@
         query_id = '<query_id>'  # query id from execute function response.
         cursor.cancel(query_id)
         ```
         
         Switch database in an existing connection:
         ```python
         database = '<new_database_name>'  # Replace with the new database.
-        cursor = conn.cursor(database)
+        cursor = conn.cursor(database, catalog_name)
         ```
         
         ### Get Query Time Metrics
         ```python
         import json
         query = 'SELECT * FROM <TABLE_NAME>'
         
-        cursor = conn.cursor()
+        cursor = conn.cursor(catalog_name)
         query_id = cursor.execute(query)  # execute function returns query id, can be use for aborting th query.
         all_records = cursor.fetchall()
         
         query_planner = json.loads(cursor.explain_analyse())
         
         execution_time = query_planner.get("total_query_time")  # In milliseconds
         queue_time = query_planner.get("executionQueueingTime")  # In milliseconds
@@ -163,23 +164,25 @@
         
         host = '<host>'  # IP address or hostname of the cluster to be used.
         database = '<database>'  # # Database to perform the query on.
         port = 9000  # Port of the e6data engine.
         
         sql_query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the actual query.
         
+        catalog_name = '<catalog_name>'  # Replace with the actual catalog name.
+        
         conn = edb.connect(
             host=host,
             port=port,
             username=username,
             database=database,
             password=password
         )
         
-        cursor = conn.cursor(db_name=database)
+        cursor = conn.cursor(db_name=database, catalog_name=catalog_name)
         query_id = cursor.execute(sql_query)
         all_records = cursor.fetchall()
         planner_result = json.loads(cursor.explain_analyse())
         execution_time = planner_result.get("total_query_time") / 1000  # Converting into seconds.
         row_count = planner_result.get('row_count_out')
         columns = [col[0] for col in cursor.description]  # Get the column names and merge them with the results.
         results = []
```

### Comparing `e6data-python-connector-1.0.9/e6xdb/common.py` & `e6data-python-connector-1.1.0/e6xdb/common.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/e6xdb/constants.py` & `e6data-python-connector-1.1.0/e6xdb/constants.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/e6xdb/datainputstream.py` & `e6data-python-connector-1.1.0/e6xdb/datainputstream.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/e6xdb/date_time_utils.py` & `e6data-python-connector-1.1.0/e6xdb/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/e6xdb/e6x.py` & `e6data-python-connector-1.1.0/e6xdb/e6x.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import logging
 import re
 import sys
 from decimal import Decimal
 from io import BytesIO
 from ssl import CERT_NONE, CERT_OPTIONAL, CERT_REQUIRED
 
-from e6xdb.server import QueryEngineService
+from e6data_python_connector.server import QueryEngineService
 from thrift.protocol import TBinaryProtocol, TMultiplexedProtocol
 from thrift.transport import TSocket
 from thrift.transport import TTransport
 
 from e6xdb.common import DBAPITypeObject, ParamEscaper, DBAPICursor
 from e6xdb.constants import *
 from e6xdb.datainputstream import DataInputStream, get_query_columns_info, read_rows_from_batch, read_values_from_array
@@ -116,17 +116,14 @@
         self.__password = password
         self._database = database
         self._session_id = None
 
         # service_name = 'E6x'  # E6x  QueryExecutor
         service_name = 'QueryEngine'  # E6x  QueryExecutor
 
-        if scheme != "e6data":
-            raise ValueError("scheme is not e6data")
-
         if not self.__username or not self.__password:
             raise ValueError("username or password cannot be empty.")
         if port is None:
             port = 9000
         self._transport = TSocket.TSocket(host, port)
         self._transport = TTransport.TBufferedTransport(self._transport)
```

### Comparing `e6data-python-connector-1.0.9/e6xdb/server/QueryEngineService.py` & `e6data-python-connector-1.1.0/e6data_python_connector/server/QueryEngineService.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/e6xdb/server/ttypes.py` & `e6data-python-connector-1.1.0/e6data_python_connector/server/ttypes.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/e6xdb/sqlalchemy_e6x.py` & `e6data-python-connector-1.1.0/e6xdb/sqlalchemy_e6x.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/e6xdb/typeId.py` & `e6data-python-connector-1.1.0/e6xdb/typeId.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.9/setup.py` & `e6data-python-connector-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import os
 
 import setuptools
 
 envstring = lambda var: os.environ.get(var) or ""
 
-VERSION = [1, 0, 9]
+VERSION = [1, 1, 0]
 
 
 def get_long_desc():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     return long_description
 
@@ -40,14 +40,16 @@
     install_requires=[
         'sqlalchemy>=1.0.0',
         'future',
         'python-dateutil',
         'pycryptodome',
         'pytz',
         'thrift',
+        'grpcio>=1.56.2',
+        'grpcio-tools>=1.56.2',
     ],
     classifiers=[
         "Operating System :: POSIX :: Linux",
         "License :: OSI Approved :: Apache Software License",
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

