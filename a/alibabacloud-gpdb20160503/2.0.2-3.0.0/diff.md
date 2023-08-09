# Comparing `tmp/alibabacloud_gpdb20160503-2.0.2.tar.gz` & `tmp/alibabacloud_gpdb20160503-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gpdb20160503-2.0.2.tar", last modified: Wed Aug  2 02:10:31 2023, max compression
+gzip compressed data, was "dist/alibabacloud_gpdb20160503-3.0.0.tar", last modified: Wed Aug  9 03:35:05 2023, max compression
```

## Comparing `alibabacloud_gpdb20160503-2.0.2.tar` & `alibabacloud_gpdb20160503-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2355 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)   509950 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/client.py
--rw-r--r--   0 root         (0) root         (0)   743266 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2355 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2637 2023-08-02 02:10:31.000000 alibabacloud_gpdb20160503-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   510954 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503/client.py
+-rw-r--r--   0 root         (0) root         (0)   744292 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-09 03:35:05.000000 alibabacloud_gpdb20160503-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-08-09 03:35:04.000000 alibabacloud_gpdb20160503-3.0.0/setup.py
```

### Comparing `alibabacloud_gpdb20160503-2.0.2/ChangeLog.md` & `alibabacloud_gpdb20160503-3.0.0/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-08-02 Version: 2.0.2
+- Add Cloud Disk Encryption.
+
 2023-07-26 Version: 2.0.1
 - Add Cloud Disk Encryption.
 
 2023-07-10 Version: 2.0.0
 - Add Cloud Disk Encryption.
 
 2023-01-09 Version: 1.1.21
```

### Comparing `alibabacloud_gpdb20160503-2.0.2/LICENSE` & `alibabacloud_gpdb20160503-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.2/PKG-INFO` & `alibabacloud_gpdb20160503-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gpdb20160503
-Version: 2.0.2
+Version: 3.0.0
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503-2.0.2/README-CN.md` & `alibabacloud_gpdb20160503-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.2/README.md` & `alibabacloud_gpdb20160503-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/client.py` & `alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,26 +397,32 @@
             query['Collection'] = request.collection
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         if not UtilClient.is_unset(request.dimension):
             query['Dimension'] = request.dimension
         if not UtilClient.is_unset(request.full_text_retrieval_fields):
             query['FullTextRetrievalFields'] = request.full_text_retrieval_fields
+        if not UtilClient.is_unset(request.hnsw_m):
+            query['HnswM'] = request.hnsw_m
         if not UtilClient.is_unset(request.manager_account):
             query['ManagerAccount'] = request.manager_account
         if not UtilClient.is_unset(request.manager_account_password):
             query['ManagerAccountPassword'] = request.manager_account_password
         if not UtilClient.is_unset(request.metadata):
             query['Metadata'] = request.metadata
+        if not UtilClient.is_unset(request.metrics):
+            query['Metrics'] = request.metrics
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.parser):
             query['Parser'] = request.parser
+        if not UtilClient.is_unset(request.pq_enable):
+            query['PqEnable'] = request.pq_enable
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateCollection',
@@ -445,26 +451,32 @@
             query['Collection'] = request.collection
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         if not UtilClient.is_unset(request.dimension):
             query['Dimension'] = request.dimension
         if not UtilClient.is_unset(request.full_text_retrieval_fields):
             query['FullTextRetrievalFields'] = request.full_text_retrieval_fields
+        if not UtilClient.is_unset(request.hnsw_m):
+            query['HnswM'] = request.hnsw_m
         if not UtilClient.is_unset(request.manager_account):
             query['ManagerAccount'] = request.manager_account
         if not UtilClient.is_unset(request.manager_account_password):
             query['ManagerAccountPassword'] = request.manager_account_password
         if not UtilClient.is_unset(request.metadata):
             query['Metadata'] = request.metadata
+        if not UtilClient.is_unset(request.metrics):
+            query['Metrics'] = request.metrics
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.parser):
             query['Parser'] = request.parser
+        if not UtilClient.is_unset(request.pq_enable):
+            query['PqEnable'] = request.pq_enable
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateCollection',
@@ -1185,24 +1197,28 @@
         query = {}
         if not UtilClient.is_unset(request.collection):
             query['Collection'] = request.collection
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         if not UtilClient.is_unset(request.dimension):
             query['Dimension'] = request.dimension
+        if not UtilClient.is_unset(request.hnsw_m):
+            query['HnswM'] = request.hnsw_m
         if not UtilClient.is_unset(request.manager_account):
             query['ManagerAccount'] = request.manager_account
         if not UtilClient.is_unset(request.manager_account_password):
             query['ManagerAccountPassword'] = request.manager_account_password
         if not UtilClient.is_unset(request.metrics):
             query['Metrics'] = request.metrics
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.pq_enable):
+            query['PqEnable'] = request.pq_enable
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateVectorIndex',
@@ -1229,24 +1245,28 @@
         query = {}
         if not UtilClient.is_unset(request.collection):
             query['Collection'] = request.collection
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         if not UtilClient.is_unset(request.dimension):
             query['Dimension'] = request.dimension
+        if not UtilClient.is_unset(request.hnsw_m):
+            query['HnswM'] = request.hnsw_m
         if not UtilClient.is_unset(request.manager_account):
             query['ManagerAccount'] = request.manager_account
         if not UtilClient.is_unset(request.manager_account_password):
             query['ManagerAccountPassword'] = request.manager_account_password
         if not UtilClient.is_unset(request.metrics):
             query['Metrics'] = request.metrics
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.pq_enable):
+            query['PqEnable'] = request.pq_enable
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateVectorIndex',
```

### Comparing `alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503/models.py` & `alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,32 +421,38 @@
 class CreateCollectionRequest(TeaModel):
     def __init__(
         self,
         collection: str = None,
         dbinstance_id: str = None,
         dimension: int = None,
         full_text_retrieval_fields: str = None,
+        hnsw_m: int = None,
         manager_account: str = None,
         manager_account_password: str = None,
         metadata: str = None,
+        metrics: str = None,
         namespace: str = None,
         owner_id: int = None,
         parser: str = None,
+        pq_enable: int = None,
         region_id: str = None,
     ):
         self.collection = collection
         self.dbinstance_id = dbinstance_id
         self.dimension = dimension
         self.full_text_retrieval_fields = full_text_retrieval_fields
+        self.hnsw_m = hnsw_m
         self.manager_account = manager_account
         self.manager_account_password = manager_account_password
         self.metadata = metadata
+        self.metrics = metrics
         self.namespace = namespace
         self.owner_id = owner_id
         self.parser = parser
+        self.pq_enable = pq_enable
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -458,52 +464,64 @@
             result['Collection'] = self.collection
         if self.dbinstance_id is not None:
             result['DBInstanceId'] = self.dbinstance_id
         if self.dimension is not None:
             result['Dimension'] = self.dimension
         if self.full_text_retrieval_fields is not None:
             result['FullTextRetrievalFields'] = self.full_text_retrieval_fields
+        if self.hnsw_m is not None:
+            result['HnswM'] = self.hnsw_m
         if self.manager_account is not None:
             result['ManagerAccount'] = self.manager_account
         if self.manager_account_password is not None:
             result['ManagerAccountPassword'] = self.manager_account_password
         if self.metadata is not None:
             result['Metadata'] = self.metadata
+        if self.metrics is not None:
+            result['Metrics'] = self.metrics
         if self.namespace is not None:
             result['Namespace'] = self.namespace
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.parser is not None:
             result['Parser'] = self.parser
+        if self.pq_enable is not None:
+            result['PqEnable'] = self.pq_enable
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Collection') is not None:
             self.collection = m.get('Collection')
         if m.get('DBInstanceId') is not None:
             self.dbinstance_id = m.get('DBInstanceId')
         if m.get('Dimension') is not None:
             self.dimension = m.get('Dimension')
         if m.get('FullTextRetrievalFields') is not None:
             self.full_text_retrieval_fields = m.get('FullTextRetrievalFields')
+        if m.get('HnswM') is not None:
+            self.hnsw_m = m.get('HnswM')
         if m.get('ManagerAccount') is not None:
             self.manager_account = m.get('ManagerAccount')
         if m.get('ManagerAccountPassword') is not None:
             self.manager_account_password = m.get('ManagerAccountPassword')
         if m.get('Metadata') is not None:
             self.metadata = m.get('Metadata')
+        if m.get('Metrics') is not None:
+            self.metrics = m.get('Metrics')
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('Parser') is not None:
             self.parser = m.get('Parser')
+        if m.get('PqEnable') is not None:
+            self.pq_enable = m.get('PqEnable')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class CreateCollectionResponseBody(TeaModel):
     def __init__(
@@ -1712,30 +1730,34 @@
 
 class CreateVectorIndexRequest(TeaModel):
     def __init__(
         self,
         collection: str = None,
         dbinstance_id: str = None,
         dimension: int = None,
+        hnsw_m: int = None,
         manager_account: str = None,
         manager_account_password: str = None,
         metrics: str = None,
         namespace: str = None,
         owner_id: int = None,
+        pq_enable: int = None,
         region_id: str = None,
     ):
         self.collection = collection
         self.dbinstance_id = dbinstance_id
         self.dimension = dimension
+        self.hnsw_m = hnsw_m
         self.manager_account = manager_account
         self.manager_account_password = manager_account_password
         # Distance Metrics。
         self.metrics = metrics
         self.namespace = namespace
         self.owner_id = owner_id
+        self.pq_enable = pq_enable
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1745,46 +1767,54 @@
         result = dict()
         if self.collection is not None:
             result['Collection'] = self.collection
         if self.dbinstance_id is not None:
             result['DBInstanceId'] = self.dbinstance_id
         if self.dimension is not None:
             result['Dimension'] = self.dimension
+        if self.hnsw_m is not None:
+            result['HnswM'] = self.hnsw_m
         if self.manager_account is not None:
             result['ManagerAccount'] = self.manager_account
         if self.manager_account_password is not None:
             result['ManagerAccountPassword'] = self.manager_account_password
         if self.metrics is not None:
             result['Metrics'] = self.metrics
         if self.namespace is not None:
             result['Namespace'] = self.namespace
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
+        if self.pq_enable is not None:
+            result['PqEnable'] = self.pq_enable
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Collection') is not None:
             self.collection = m.get('Collection')
         if m.get('DBInstanceId') is not None:
             self.dbinstance_id = m.get('DBInstanceId')
         if m.get('Dimension') is not None:
             self.dimension = m.get('Dimension')
+        if m.get('HnswM') is not None:
+            self.hnsw_m = m.get('HnswM')
         if m.get('ManagerAccount') is not None:
             self.manager_account = m.get('ManagerAccount')
         if m.get('ManagerAccountPassword') is not None:
             self.manager_account_password = m.get('ManagerAccountPassword')
         if m.get('Metrics') is not None:
             self.metrics = m.get('Metrics')
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
+        if m.get('PqEnable') is not None:
+            self.pq_enable = m.get('PqEnable')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class CreateVectorIndexResponseBody(TeaModel):
     def __init__(
@@ -16392,26 +16422,26 @@
 class ModifyAccountDescriptionRequest(TeaModel):
     def __init__(
         self,
         account_description: str = None,
         account_name: str = None,
         dbinstance_id: str = None,
     ):
-        # The description of the account. The description must meet the following requirements:
+        # The new description of the database account.
         # 
         # *   The description must start with a letter.
-        # *   The description can contain letters, digits, underscores (\_), and hyphens (-).
         # *   The description cannot start with `http://` or `https://`.
+        # *   The description can contain letters, underscores (\_), hyphens (-), and digits.
         # *   The description must be 2 to 256 characters in length.
         self.account_description = account_description
         # The name of the database account.
-        # 
-        # > You can call the [DescribeAccounts](~~~~) operation to query the information about database accounts in a cluster, including the database account name.
         self.account_name = account_name
-        # The ID of the instance.
+        # The instance ID.
+        # 
+        # > You can call the [DescribeDBInstances](~~86911~~) operation to query the IDs of all AnalyticDB for PostgreSQL instances within a region.
         self.dbinstance_id = dbinstance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16439,15 +16469,15 @@
 
 
 class ModifyAccountDescriptionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18288,20 +18318,20 @@
 
 
 class QueryCollectionDataResponseBodyMatchesMatch(TeaModel):
     def __init__(
         self,
         id: str = None,
         metadata: Dict[str, str] = None,
-        similarity: float = None,
+        score: float = None,
         values: QueryCollectionDataResponseBodyMatchesMatchValues = None,
     ):
         self.id = id
         self.metadata = metadata
-        self.similarity = similarity
+        self.score = score
         self.values = values
 
     def validate(self):
         if self.values:
             self.values.validate()
 
     def to_map(self):
@@ -18310,28 +18340,28 @@
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.metadata is not None:
             result['Metadata'] = self.metadata
-        if self.similarity is not None:
-            result['Similarity'] = self.similarity
+        if self.score is not None:
+            result['Score'] = self.score
         if self.values is not None:
             result['Values'] = self.values.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('Metadata') is not None:
             self.metadata = m.get('Metadata')
-        if m.get('Similarity') is not None:
-            self.similarity = m.get('Similarity')
+        if m.get('Score') is not None:
+            self.score = m.get('Score')
         if m.get('Values') is not None:
             temp_model = QueryCollectionDataResponseBodyMatchesMatchValues()
             self.values = temp_model.from_map(m['Values'])
         return self
 
 
 class QueryCollectionDataResponseBodyMatches(TeaModel):
```

### Comparing `alibabacloud_gpdb20160503-2.0.2/alibabacloud_gpdb20160503.egg-info/PKG-INFO` & `alibabacloud_gpdb20160503-3.0.0/alibabacloud_gpdb20160503.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gpdb20160503
-Version: 2.0.2
+Version: 3.0.0
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503-2.0.2/setup.py` & `alibabacloud_gpdb20160503-3.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gpdb20160503.
 
-Created on 02/08/2023
+Created on 09/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gpdb20160503"
 NAME = "alibabacloud_gpdb20160503" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python"
```

