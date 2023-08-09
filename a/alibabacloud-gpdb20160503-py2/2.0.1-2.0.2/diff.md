# Comparing `tmp/alibabacloud_gpdb20160503_py2-2.0.1.tar.gz` & `tmp/alibabacloud_gpdb20160503_py2-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gpdb20160503_py2-2.0.1.tar", last modified: Wed Jul 26 06:50:39 2023, max compression
+gzip compressed data, was "dist/alibabacloud_gpdb20160503_py2-2.0.2.tar", last modified: Wed Aug  2 02:10:33 2023, max compression
```

## Comparing `alibabacloud_gpdb20160503_py2-2.0.1.tar` & `alibabacloud_gpdb20160503_py2-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/
--rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2499 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)   224228 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/client.py
--rw-r--r--   0 root         (0) root         (0)   743982 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2499 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2929 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   225836 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503/client.py
+-rw-r--r--   0 root         (0) root         (0)   749031 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-08-02 02:10:33.000000 alibabacloud_gpdb20160503_py2-2.0.2/setup.py
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/ChangeLog.md` & `alibabacloud_gpdb20160503_py2-2.0.2/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-26 Version: 2.0.1
+- Add Cloud Disk Encryption.
+
 2023-07-10 Version: 2.0.0
 - Add Cloud Disk Encryption.
 
 2023-01-09 Version: 1.1.22
 - Support Pause and Resume Instance.
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/LICENSE` & `alibabacloud_gpdb20160503_py2-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/PKG-INFO` & `alibabacloud_gpdb20160503_py2-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gpdb20160503_py2
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/README-CN.md` & `alibabacloud_gpdb20160503_py2-2.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/README.md` & `alibabacloud_gpdb20160503_py2-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/client.py` & `alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1586,14 +1586,16 @@
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbinstance_index_usage_with_options(request, runtime)
 
     def describe_dbinstance_net_info_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.connection_string):
+            query['ConnectionString'] = request.connection_string
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBInstanceNetInfo',
@@ -3289,14 +3291,50 @@
             self.call_api(params, req, runtime)
         )
 
     def grant_collection(self, request):
         runtime = util_models.RuntimeOptions()
         return self.grant_collection_with_options(request, runtime)
 
+    def init_vector_database_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dbinstance_id):
+            query['DBInstanceId'] = request.dbinstance_id
+        if not UtilClient.is_unset(request.manager_account):
+            query['ManagerAccount'] = request.manager_account
+        if not UtilClient.is_unset(request.manager_account_password):
+            query['ManagerAccountPassword'] = request.manager_account_password
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='InitVectorDatabase',
+            version='2016-05-03',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            gpdb_20160503_models.InitVectorDatabaseResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def init_vector_database(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.init_vector_database_with_options(request, runtime)
+
     def list_collections_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/models.py` & `alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5887,35 +5887,40 @@
         if m.get('body') is not None:
             temp_model = DescribeDBInstanceIndexUsageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDBInstanceNetInfoRequest(TeaModel):
-    def __init__(self, dbinstance_id=None):
+    def __init__(self, connection_string=None, dbinstance_id=None):
+        self.connection_string = connection_string  # type: str
         # The ID of the instance.
         # 
         # >  You can call the [DescribeDBInstances](~~86911~~) operation to query details about all AnalyticDB for PostgreSQL instances in a specific region, including instance IDs.
         self.dbinstance_id = dbinstance_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDBInstanceNetInfoRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.connection_string is not None:
+            result['ConnectionString'] = self.connection_string
         if self.dbinstance_id is not None:
             result['DBInstanceId'] = self.dbinstance_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('ConnectionString') is not None:
+            self.connection_string = m.get('ConnectionString')
         if m.get('DBInstanceId') is not None:
             self.dbinstance_id = m.get('DBInstanceId')
         return self
 
 
 class DescribeDBInstanceNetInfoResponseBodyDBInstanceNetInfosDBInstanceNetInfo(TeaModel):
     def __init__(self, address_type=None, connection_string=None, ipaddress=None, iptype=None, port=None, vpcid=None,
@@ -13900,14 +13905,132 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GrantCollectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class InitVectorDatabaseRequest(TeaModel):
+    def __init__(self, dbinstance_id=None, manager_account=None, manager_account_password=None, owner_id=None,
+                 region_id=None):
+        self.dbinstance_id = dbinstance_id  # type: str
+        self.manager_account = manager_account  # type: str
+        self.manager_account_password = manager_account_password  # type: str
+        self.owner_id = owner_id  # type: long
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(InitVectorDatabaseRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dbinstance_id is not None:
+            result['DBInstanceId'] = self.dbinstance_id
+        if self.manager_account is not None:
+            result['ManagerAccount'] = self.manager_account
+        if self.manager_account_password is not None:
+            result['ManagerAccountPassword'] = self.manager_account_password
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DBInstanceId') is not None:
+            self.dbinstance_id = m.get('DBInstanceId')
+        if m.get('ManagerAccount') is not None:
+            self.manager_account = m.get('ManagerAccount')
+        if m.get('ManagerAccountPassword') is not None:
+            self.manager_account_password = m.get('ManagerAccountPassword')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class InitVectorDatabaseResponseBody(TeaModel):
+    def __init__(self, message=None, request_id=None, status=None):
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.status = status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(InitVectorDatabaseResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class InitVectorDatabaseResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: InitVectorDatabaseResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(InitVectorDatabaseResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = InitVectorDatabaseResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListCollectionsRequest(TeaModel):
     def __init__(self, dbinstance_id=None, namespace=None, namespace_password=None, owner_id=None, region_id=None):
         self.dbinstance_id = dbinstance_id  # type: str
         self.namespace = namespace  # type: str
         self.namespace_password = namespace_password  # type: str
         self.owner_id = owner_id  # type: long
         self.region_id = region_id  # type: str
@@ -16194,17 +16317,18 @@
         m = m or dict()
         if m.get('value') is not None:
             self.value = m.get('value')
         return self
 
 
 class QueryCollectionDataResponseBodyMatchesMatch(TeaModel):
-    def __init__(self, id=None, metadata=None, values=None):
+    def __init__(self, id=None, metadata=None, similarity=None, values=None):
         self.id = id  # type: str
         self.metadata = metadata  # type: dict[str, str]
+        self.similarity = similarity  # type: float
         self.values = values  # type: QueryCollectionDataResponseBodyMatchesMatchValues
 
     def validate(self):
         if self.values:
             self.values.validate()
 
     def to_map(self):
@@ -16213,24 +16337,28 @@
             return _map
 
         result = dict()
         if self.id is not None:
             result['Id'] = self.id
         if self.metadata is not None:
             result['Metadata'] = self.metadata
+        if self.similarity is not None:
+            result['Similarity'] = self.similarity
         if self.values is not None:
             result['Values'] = self.values.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('Metadata') is not None:
             self.metadata = m.get('Metadata')
+        if m.get('Similarity') is not None:
+            self.similarity = m.get('Similarity')
         if m.get('Values') is not None:
             temp_model = QueryCollectionDataResponseBodyMatchesMatchValues()
             self.values = temp_model.from_map(m['Values'])
         return self
 
 
 class QueryCollectionDataResponseBodyMatches(TeaModel):
@@ -16262,16 +16390,17 @@
             for k in m.get('match'):
                 temp_model = QueryCollectionDataResponseBodyMatchesMatch()
                 self.match.append(temp_model.from_map(k))
         return self
 
 
 class QueryCollectionDataResponseBody(TeaModel):
-    def __init__(self, matches=None, request_id=None, status=None):
+    def __init__(self, matches=None, message=None, request_id=None, status=None):
         self.matches = matches  # type: QueryCollectionDataResponseBodyMatches
+        self.message = message  # type: str
         self.request_id = request_id  # type: str
         self.status = status  # type: str
 
     def validate(self):
         if self.matches:
             self.matches.validate()
 
@@ -16279,25 +16408,29 @@
         _map = super(QueryCollectionDataResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.matches is not None:
             result['Matches'] = self.matches.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.status is not None:
             result['Status'] = self.status
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Matches') is not None:
             temp_model = QueryCollectionDataResponseBodyMatches()
             self.matches = temp_model.from_map(m['Matches'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO` & `alibabacloud_gpdb20160503_py2-2.0.2/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gpdb20160503-py2
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.1/setup.py` & `alibabacloud_gpdb20160503_py2-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gpdb20160503_py2.
 
-Created on 26/07/2023
+Created on 02/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gpdb20160503"
 NAME = "alibabacloud_gpdb20160503_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2"
```

