# Comparing `tmp/s3kv-0.1.2.tar.gz` & `tmp/s3kv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/s3kv-0.1.2.tar", last modified: Wed Aug  9 04:26:20 2023, max compression
+gzip compressed data, was "dist/s3kv-0.1.3.tar", last modified: Wed Aug  9 04:29:37 2023, max compression
```

## Comparing `s3kv-0.1.2.tar` & `s3kv-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 balajibal   (501) staff       (20)        0 2023-08-09 04:26:20.277199 s3kv-0.1.2/
--rw-r--r--   0 balajibal   (501) staff       (20)     3914 2023-08-09 04:26:20.276970 s3kv-0.1.2/PKG-INFO
--rw-r--r--   0 balajibal   (501) staff       (20)     2756 2023-08-05 19:40:19.000000 s3kv-0.1.2/README.md
-drwxr-xr-x   0 balajibal   (501) staff       (20)        0 2023-08-09 04:26:20.276005 s3kv-0.1.2/s3kv/
--rw-r--r--   0 balajibal   (501) staff       (20)        0 2023-08-09 04:26:15.000000 s3kv-0.1.2/s3kv/__init__.py
-drwxr-xr-x   0 balajibal   (501) staff       (20)        0 2023-08-09 04:26:20.276728 s3kv-0.1.2/s3kv.egg-info/
--rw-r--r--   0 balajibal   (501) staff       (20)     3914 2023-08-09 04:26:20.000000 s3kv-0.1.2/s3kv.egg-info/PKG-INFO
--rw-r--r--   0 balajibal   (501) staff       (20)      174 2023-08-09 04:26:20.000000 s3kv-0.1.2/s3kv.egg-info/SOURCES.txt
--rw-r--r--   0 balajibal   (501) staff       (20)        1 2023-08-09 04:26:20.000000 s3kv-0.1.2/s3kv.egg-info/dependency_links.txt
--rw-r--r--   0 balajibal   (501) staff       (20)       20 2023-08-09 04:26:20.000000 s3kv-0.1.2/s3kv.egg-info/requires.txt
--rw-r--r--   0 balajibal   (501) staff       (20)        5 2023-08-09 04:26:20.000000 s3kv-0.1.2/s3kv.egg-info/top_level.txt
--rw-r--r--   0 balajibal   (501) staff       (20)       38 2023-08-09 04:26:20.277262 s3kv-0.1.2/setup.cfg
--rw-r--r--   0 balajibal   (501) staff       (20)      922 2023-08-09 04:25:34.000000 s3kv-0.1.2/setup.py
+drwxr-xr-x   0 balajibal   (501) staff       (20)        0 2023-08-09 04:29:37.348045 s3kv-0.1.3/
+-rw-r--r--   0 balajibal   (501) staff       (20)     3812 2023-08-09 04:29:37.347828 s3kv-0.1.3/PKG-INFO
+-rw-r--r--   0 balajibal   (501) staff       (20)     2670 2023-08-09 04:29:20.000000 s3kv-0.1.3/README.md
+drwxr-xr-x   0 balajibal   (501) staff       (20)        0 2023-08-09 04:29:37.346843 s3kv-0.1.3/s3kv/
+-rw-r--r--   0 balajibal   (501) staff       (20)        0 2023-08-09 04:26:15.000000 s3kv-0.1.3/s3kv/__init__.py
+drwxr-xr-x   0 balajibal   (501) staff       (20)        0 2023-08-09 04:29:37.347588 s3kv-0.1.3/s3kv.egg-info/
+-rw-r--r--   0 balajibal   (501) staff       (20)     3812 2023-08-09 04:29:37.000000 s3kv-0.1.3/s3kv.egg-info/PKG-INFO
+-rw-r--r--   0 balajibal   (501) staff       (20)      174 2023-08-09 04:29:37.000000 s3kv-0.1.3/s3kv.egg-info/SOURCES.txt
+-rw-r--r--   0 balajibal   (501) staff       (20)        1 2023-08-09 04:29:37.000000 s3kv-0.1.3/s3kv.egg-info/dependency_links.txt
+-rw-r--r--   0 balajibal   (501) staff       (20)       20 2023-08-09 04:29:37.000000 s3kv-0.1.3/s3kv.egg-info/requires.txt
+-rw-r--r--   0 balajibal   (501) staff       (20)        5 2023-08-09 04:29:37.000000 s3kv-0.1.3/s3kv.egg-info/top_level.txt
+-rw-r--r--   0 balajibal   (501) staff       (20)       38 2023-08-09 04:29:37.348103 s3kv-0.1.3/setup.cfg
+-rw-r--r--   0 balajibal   (501) staff       (20)      922 2023-08-09 04:29:32.000000 s3kv-0.1.3/setup.py
```

### Comparing `s3kv-0.1.2/PKG-INFO` & `s3kv-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: s3kv
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for interacting with S3 key-value store
 Home-page: https://github.com/BalLab/s3kv
 Author: Balaji Bal
 License: UNKNOWN
-Description: Based on the provided Python code and the comments, here's a README-like summary:
-        
-        # S3KV - Simple Key-Value Store using AWS S3 and Elasticsearch
+Description: # S3KV - Simple Key-Value Store using AWS S3 and Elasticsearch
         
         ## Introduction
-        S3KV is a Python class that provides a simple key-value store using AWS S3 as the data storage and Elasticsearch for metadata indexing. It allows storing and retrieving JSON-formatted data with optional metadata for easy search and retrieval.
+        S3KV is a Python library that provides a simple key-value store backed by S3 Object Storage and Elasticsearch for metadata indexing. It allows storing and retrieving JSON-formatted data with optional metadata for easy search and retrieval.
         
         ## Initialization
         To create an S3KV object, initialize it with the required parameters:
         - `bucket_name`: The name of the S3 bucket to use for storing the data.
         - `aws_access_key_id` and `aws_secret_access_key`: Optional AWS credentials for S3 access.
         - `elasticsearch_host`: Optional Elasticsearch host URL if metadata indexing is needed.
```

### Comparing `s3kv-0.1.2/README.md` & `s3kv-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-Based on the provided Python code and the comments, here's a README-like summary:
-
 # S3KV - Simple Key-Value Store using AWS S3 and Elasticsearch
 
 ## Introduction
-S3KV is a Python class that provides a simple key-value store using AWS S3 as the data storage and Elasticsearch for metadata indexing. It allows storing and retrieving JSON-formatted data with optional metadata for easy search and retrieval.
+S3KV is a Python library that provides a simple key-value store backed by S3 Object Storage and Elasticsearch for metadata indexing. It allows storing and retrieving JSON-formatted data with optional metadata for easy search and retrieval.
 
 ## Initialization
 To create an S3KV object, initialize it with the required parameters:
 - `bucket_name`: The name of the S3 bucket to use for storing the data.
 - `aws_access_key_id` and `aws_secret_access_key`: Optional AWS credentials for S3 access.
 - `elasticsearch_host`: Optional Elasticsearch host URL if metadata indexing is needed.
```

### Comparing `s3kv-0.1.2/s3kv.egg-info/PKG-INFO` & `s3kv-0.1.3/s3kv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: s3kv
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python library for interacting with S3 key-value store
 Home-page: https://github.com/BalLab/s3kv
 Author: Balaji Bal
 License: UNKNOWN
-Description: Based on the provided Python code and the comments, here's a README-like summary:
-        
-        # S3KV - Simple Key-Value Store using AWS S3 and Elasticsearch
+Description: # S3KV - Simple Key-Value Store using AWS S3 and Elasticsearch
         
         ## Introduction
-        S3KV is a Python class that provides a simple key-value store using AWS S3 as the data storage and Elasticsearch for metadata indexing. It allows storing and retrieving JSON-formatted data with optional metadata for easy search and retrieval.
+        S3KV is a Python library that provides a simple key-value store backed by S3 Object Storage and Elasticsearch for metadata indexing. It allows storing and retrieving JSON-formatted data with optional metadata for easy search and retrieval.
         
         ## Initialization
         To create an S3KV object, initialize it with the required parameters:
         - `bucket_name`: The name of the S3 bucket to use for storing the data.
         - `aws_access_key_id` and `aws_secret_access_key`: Optional AWS credentials for S3 access.
         - `elasticsearch_host`: Optional Elasticsearch host URL if metadata indexing is needed.
```

### Comparing `s3kv-0.1.2/setup.py` & `s3kv-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='s3kv',
-    version='0.1.2',
+    version='0.1.3',
     author='Balaji Bal',
     description='A Python library for interacting with S3 key-value store',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/BalLab/s3kv',
     packages=['s3kv'],
     install_requires=[
```

