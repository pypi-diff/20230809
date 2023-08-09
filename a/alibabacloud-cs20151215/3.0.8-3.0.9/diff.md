# Comparing `tmp/alibabacloud_cs20151215-3.0.8.tar.gz` & `tmp/alibabacloud_cs20151215-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cs20151215-3.0.8.tar", last modified: Tue Mar 15 02:30:59 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cs20151215-3.0.9.tar", last modified: Fri Mar 18 08:06:36 2022, max compression
```

## Comparing `alibabacloud_cs20151215-3.0.8.tar` & `alibabacloud_cs20151215-3.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/
--rw-r--r--   0 root         (0) root         (0)     2825 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2322 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1104 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215/__init__.py
--rw-r--r--   0 root         (0) root         (0)   323640 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215/client.py
--rw-r--r--   0 root         (0) root         (0)   532572 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2322 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-15 02:30:59.000000 alibabacloud_cs20151215-3.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2605 2022-03-15 02:30:58.000000 alibabacloud_cs20151215-3.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/
+-rw-r--r--   0 root         (0) root         (0)     2883 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2322 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1019 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1104 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   323852 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215/client.py
+-rw-r--r--   0 root         (0) root         (0)   532566 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2322 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2605 2022-03-18 08:06:36.000000 alibabacloud_cs20151215-3.0.9/setup.py
```

### Comparing `alibabacloud_cs20151215-3.0.8/ChangeLog.md` & `alibabacloud_cs20151215-3.0.9/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-03-15 Version: 3.0.8
+- Update ModifyPolicyInstance.
+
 2022-03-09 Version: 3.0.7
 - Update UpdateK8sClusterUserConfig.
 
 2022-02-21 Version: 3.0.6
 - Update DeployPolicyInstance.
 
 2022-01-07 Version: 3.0.5
```

### Comparing `alibabacloud_cs20151215-3.0.8/LICENSE` & `alibabacloud_cs20151215-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215-3.0.8/PKG-INFO` & `alibabacloud_cs20151215-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cs20151215
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud CS (20151215) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cs20151215-3.0.8/README-CN.md` & `alibabacloud_cs20151215-3.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215-3.0.8/README.md` & `alibabacloud_cs20151215-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215/client.py` & `alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3622,14 +3622,16 @@
             query['name'] = request.name
         if not UtilClient.is_unset(request.page_number):
             query['page_number'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['page_size'] = request.page_size
         if not UtilClient.is_unset(request.profile):
             query['profile'] = request.profile
+        if not UtilClient.is_unset(request.region_id):
+            query['region_id'] = request.region_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeClustersV1',
             version='2015-12-15',
@@ -3662,14 +3664,16 @@
             query['name'] = request.name
         if not UtilClient.is_unset(request.page_number):
             query['page_number'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['page_size'] = request.page_size
         if not UtilClient.is_unset(request.profile):
             query['profile'] = request.profile
+        if not UtilClient.is_unset(request.region_id):
+            query['region_id'] = request.region_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeClustersV1',
             version='2015-12-15',
```

### Comparing `alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215/models.py` & `alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4579,26 +4579,23 @@
 
 class DescribeClusterLogsResponseBody(TeaModel):
     def __init__(
         self,
         id: int = None,
         cluster_id: str = None,
         cluster_log: str = None,
-        log_level: str = None,
         created: str = None,
         updated: str = None,
     ):
         # 日志ID。
         self.id = id
         # 集群ID。
         self.cluster_id = cluster_id
         # 日志内容。
         self.cluster_log = cluster_log
-        # 日志等级。
-        self.log_level = log_level
         # 日志创建时间。
         self.created = created
         # 日志更新时间。
         self.updated = updated
 
     def validate(self):
         pass
@@ -4611,32 +4608,28 @@
         result = dict()
         if self.id is not None:
             result['ID'] = self.id
         if self.cluster_id is not None:
             result['cluster_id'] = self.cluster_id
         if self.cluster_log is not None:
             result['cluster_log'] = self.cluster_log
-        if self.log_level is not None:
-            result['log_level'] = self.log_level
         if self.created is not None:
             result['created'] = self.created
         if self.updated is not None:
             result['updated'] = self.updated
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ID') is not None:
             self.id = m.get('ID')
         if m.get('cluster_id') is not None:
             self.cluster_id = m.get('cluster_id')
         if m.get('cluster_log') is not None:
             self.cluster_log = m.get('cluster_log')
-        if m.get('log_level') is not None:
-            self.log_level = m.get('log_level')
         if m.get('created') is not None:
             self.created = m.get('created')
         if m.get('updated') is not None:
             self.updated = m.get('updated')
         return self
 
 
@@ -7683,27 +7676,30 @@
         self,
         cluster_spec: str = None,
         cluster_type: str = None,
         name: str = None,
         page_number: int = None,
         page_size: int = None,
         profile: str = None,
+        region_id: str = None,
     ):
         # 集群规格。
         self.cluster_spec = cluster_spec
         # 集群类型。
         self.cluster_type = cluster_type
         # 通过集群名称进行模糊查询。
         self.name = name
         # 分页数。
         self.page_number = page_number
         # 单页大小。
         self.page_size = page_size
         # 集群标识。
         self.profile = profile
+        # 地域。
+        self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -7718,14 +7714,16 @@
             result['name'] = self.name
         if self.page_number is not None:
             result['page_number'] = self.page_number
         if self.page_size is not None:
             result['page_size'] = self.page_size
         if self.profile is not None:
             result['profile'] = self.profile
+        if self.region_id is not None:
+            result['region_id'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('cluster_spec') is not None:
             self.cluster_spec = m.get('cluster_spec')
         if m.get('cluster_type') is not None:
@@ -7734,14 +7732,16 @@
             self.name = m.get('name')
         if m.get('page_number') is not None:
             self.page_number = m.get('page_number')
         if m.get('page_size') is not None:
             self.page_size = m.get('page_size')
         if m.get('profile') is not None:
             self.profile = m.get('profile')
+        if m.get('region_id') is not None:
+            self.region_id = m.get('region_id')
         return self
 
 
 class DescribeClustersV1ResponseBodyClusters(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
```

### Comparing `alibabacloud_cs20151215-3.0.8/alibabacloud_cs20151215.egg-info/PKG-INFO` & `alibabacloud_cs20151215-3.0.9/alibabacloud_cs20151215.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cs20151215
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud CS (20151215) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cs20151215-3.0.8/setup.py` & `alibabacloud_cs20151215-3.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cs20151215.
 
-Created on 15/03/2022
+Created on 18/03/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cs20151215"
 NAME = "alibabacloud_cs20151215" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CS (20151215) SDK Library for Python"
```

