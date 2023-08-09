# Comparing `tmp/alibabacloud_cs20151215_py2-3.0.8.tar.gz` & `tmp/alibabacloud_cs20151215_py2-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cs20151215_py2-3.0.8.tar", last modified: Tue Mar 15 02:30:54 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cs20151215_py2-3.0.9.tar", last modified: Fri Mar 18 08:06:32 2022, max compression
```

## Comparing `alibabacloud_cs20151215_py2-3.0.8.tar` & `alibabacloud_cs20151215_py2-3.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/
--rw-r--r--   0 root         (0) root         (0)      875 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2466 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215/__init__.py
--rw-r--r--   0 root         (0) root         (0)   137724 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215/client.py
--rw-r--r--   0 root         (0) root         (0)   536975 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2466 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2898 2022-03-15 02:30:54.000000 alibabacloud_cs20151215_py2-3.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/
+-rw-r--r--   0 root         (0) root         (0)      933 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2466 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   137830 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215/client.py
+-rw-r--r--   0 root         (0) root         (0)   536969 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2466 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2898 2022-03-18 08:06:32.000000 alibabacloud_cs20151215_py2-3.0.9/setup.py
```

### Comparing `alibabacloud_cs20151215_py2-3.0.8/ChangeLog.md` & `alibabacloud_cs20151215_py2-3.0.9/ChangeLog.md`

 * *Files 10% similar despite different names*

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

### Comparing `alibabacloud_cs20151215_py2-3.0.8/LICENSE` & `alibabacloud_cs20151215_py2-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215_py2-3.0.8/PKG-INFO` & `alibabacloud_cs20151215_py2-3.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cs20151215_py2
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud CS (20151215) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cs20151215_py2-3.0.8/README-CN.md` & `alibabacloud_cs20151215_py2-3.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215_py2-3.0.8/README.md` & `alibabacloud_cs20151215_py2-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215/client.py` & `alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1488,14 +1488,16 @@
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

### Comparing `alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215/models.py` & `alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4019,23 +4019,21 @@
         if m.get('body') is not None:
             temp_model = DescribeClusterDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeClusterLogsResponseBody(TeaModel):
-    def __init__(self, id=None, cluster_id=None, cluster_log=None, log_level=None, created=None, updated=None):
+    def __init__(self, id=None, cluster_id=None, cluster_log=None, created=None, updated=None):
         # 日志ID。
         self.id = id  # type: long
         # 集群ID。
         self.cluster_id = cluster_id  # type: str
         # 日志内容。
         self.cluster_log = cluster_log  # type: str
-        # 日志等级。
-        self.log_level = log_level  # type: str
         # 日志创建时间。
         self.created = created  # type: str
         # 日志更新时间。
         self.updated = updated  # type: str
 
     def validate(self):
         pass
@@ -4048,32 +4046,28 @@
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
 
     def from_map(self, m=None):
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
 
 
@@ -6784,27 +6778,29 @@
                 temp_model = DescribeClustersResponseBody()
                 self.body.append(temp_model.from_map(k))
         return self
 
 
 class DescribeClustersV1Request(TeaModel):
     def __init__(self, cluster_spec=None, cluster_type=None, name=None, page_number=None, page_size=None,
-                 profile=None):
+                 profile=None, region_id=None):
         # 集群规格。
         self.cluster_spec = cluster_spec  # type: str
         # 集群类型。
         self.cluster_type = cluster_type  # type: str
         # 通过集群名称进行模糊查询。
         self.name = name  # type: str
         # 分页数。
         self.page_number = page_number  # type: long
         # 单页大小。
         self.page_size = page_size  # type: long
         # 集群标识。
         self.profile = profile  # type: str
+        # 地域。
+        self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeClustersV1Request, self).to_map()
         if _map is not None:
@@ -6819,14 +6815,16 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('cluster_spec') is not None:
             self.cluster_spec = m.get('cluster_spec')
         if m.get('cluster_type') is not None:
@@ -6835,14 +6833,16 @@
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
     def __init__(self, cluster_id=None, cluster_spec=None, cluster_type=None, created=None, current_version=None,
                  deletion_protection=None, docker_version=None, external_loadbalancer_id=None, init_version=None,
                  maintenance_window=None, master_url=None, meta_data=None, name=None, network_mode=None, next_version=None,
```

### Comparing `alibabacloud_cs20151215_py2-3.0.8/alibabacloud_cs20151215_py2.egg-info/PKG-INFO` & `alibabacloud_cs20151215_py2-3.0.9/alibabacloud_cs20151215_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cs20151215-py2
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud CS (20151215) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cs20151215_py2-3.0.8/setup.py` & `alibabacloud_cs20151215_py2-3.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cs20151215_py2.
 
-Created on 15/03/2022
+Created on 18/03/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cs20151215"
 NAME = "alibabacloud_cs20151215_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CS (20151215) SDK Library for Python2"
```

