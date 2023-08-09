# Comparing `tmp/alibabacloud_servicemesh20200111-3.0.0.tar.gz` & `tmp/alibabacloud_servicemesh20200111-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_servicemesh20200111-3.0.0.tar", last modified: Thu Jul 27 03:23:14 2023, max compression
+gzip compressed data, was "dist/alibabacloud_servicemesh20200111-3.0.1.tar", last modified: Wed Aug  9 02:06:46 2023, max compression
```

## Comparing `alibabacloud_servicemesh20200111-3.0.0.tar` & `alibabacloud_servicemesh20200111-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2391 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   320481 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111/client.py
--rw-r--r--   0 root         (0) root         (0)   775965 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2391 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 03:23:14.000000 alibabacloud_servicemesh20200111-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2666 2023-07-27 03:23:13.000000 alibabacloud_servicemesh20200111-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   320713 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111/client.py
+-rw-r--r--   0 root         (0) root         (0)   776243 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-08-09 02:06:46.000000 alibabacloud_servicemesh20200111-3.0.1/setup.py
```

### Comparing `alibabacloud_servicemesh20200111-3.0.0/ChangeLog.md` & `alibabacloud_servicemesh20200111-3.0.1/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-27 Version: 3.0.0
+- Support setting revision for UpdateIstioInjectionConfig.
+- Remove DescribeIngressGateways.
+
 2023-05-08 Version: 2.0.27
 - Support setting TPROXY mode.
 
 2022-12-01 Version: 2.0.26
 - Support setting TPROXY mode.
 
 2022-11-24 Version: 2.0.25
```

### Comparing `alibabacloud_servicemesh20200111-3.0.0/LICENSE` & `alibabacloud_servicemesh20200111-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicemesh20200111-3.0.0/PKG-INFO` & `alibabacloud_servicemesh20200111-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_servicemesh20200111
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud Alibaba Cloud Service Mesh (20200111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_servicemesh20200111-3.0.0/README-CN.md` & `alibabacloud_servicemesh20200111-3.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicemesh20200111-3.0.0/README.md` & `alibabacloud_servicemesh20200111-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111/client.py` & `alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,14 +669,16 @@
             body['ExistingRootCaCert'] = request.existing_root_ca_cert
         if not UtilClient.is_unset(request.existing_root_ca_key):
             body['ExistingRootCaKey'] = request.existing_root_ca_key
         if not UtilClient.is_unset(request.filter_gateway_cluster_config):
             body['FilterGatewayClusterConfig'] = request.filter_gateway_cluster_config
         if not UtilClient.is_unset(request.gateway_apienabled):
             body['GatewayAPIEnabled'] = request.gateway_apienabled
+        if not UtilClient.is_unset(request.guest_cluster):
+            body['GuestCluster'] = request.guest_cluster
         if not UtilClient.is_unset(request.include_ipranges):
             body['IncludeIPRanges'] = request.include_ipranges
         if not UtilClient.is_unset(request.istio_version):
             body['IstioVersion'] = request.istio_version
         if not UtilClient.is_unset(request.kiali_enabled):
             body['KialiEnabled'] = request.kiali_enabled
         if not UtilClient.is_unset(request.locality_lbconf):
@@ -837,14 +839,16 @@
             body['ExistingRootCaCert'] = request.existing_root_ca_cert
         if not UtilClient.is_unset(request.existing_root_ca_key):
             body['ExistingRootCaKey'] = request.existing_root_ca_key
         if not UtilClient.is_unset(request.filter_gateway_cluster_config):
             body['FilterGatewayClusterConfig'] = request.filter_gateway_cluster_config
         if not UtilClient.is_unset(request.gateway_apienabled):
             body['GatewayAPIEnabled'] = request.gateway_apienabled
+        if not UtilClient.is_unset(request.guest_cluster):
+            body['GuestCluster'] = request.guest_cluster
         if not UtilClient.is_unset(request.include_ipranges):
             body['IncludeIPRanges'] = request.include_ipranges
         if not UtilClient.is_unset(request.istio_version):
             body['IstioVersion'] = request.istio_version
         if not UtilClient.is_unset(request.kiali_enabled):
             body['KialiEnabled'] = request.kiali_enabled
         if not UtilClient.is_unset(request.locality_lbconf):
```

### Comparing `alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111/models.py` & `alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1980,14 +1980,15 @@
         existing_ca_cert: str = None,
         existing_ca_key: str = None,
         existing_ca_type: str = None,
         existing_root_ca_cert: str = None,
         existing_root_ca_key: str = None,
         filter_gateway_cluster_config: bool = None,
         gateway_apienabled: bool = None,
+        guest_cluster: str = None,
         include_ipranges: str = None,
         istio_version: str = None,
         kiali_enabled: bool = None,
         locality_lbconf: str = None,
         locality_load_balancing: bool = None,
         mseenabled: bool = None,
         multi_buffer_enabled: bool = None,
@@ -2186,14 +2187,15 @@
         # Specifies whether to enable Gateway API. Valid values:
         # 
         # *   `true`
         # *   `false`
         # 
         # Default value: `false`.
         self.gateway_apienabled = gateway_apienabled
+        self.guest_cluster = guest_cluster
         # The IP ranges in CIDR form for which traffic is to be redirected to the sidecar proxy in the ASM instance.
         self.include_ipranges = include_ipranges
         # The Istio version of the ASM instance.
         self.istio_version = istio_version
         # Specifies whether to enable the mesh topology feature. To enable this feature, make sure that you have enabled Prometheus monitoring. If Prometheus monitoring is disabled, you must set this parameter to `false`.`` Valid values:
         # 
         # *   `true`
@@ -2400,14 +2402,16 @@
             result['ExistingRootCaCert'] = self.existing_root_ca_cert
         if self.existing_root_ca_key is not None:
             result['ExistingRootCaKey'] = self.existing_root_ca_key
         if self.filter_gateway_cluster_config is not None:
             result['FilterGatewayClusterConfig'] = self.filter_gateway_cluster_config
         if self.gateway_apienabled is not None:
             result['GatewayAPIEnabled'] = self.gateway_apienabled
+        if self.guest_cluster is not None:
+            result['GuestCluster'] = self.guest_cluster
         if self.include_ipranges is not None:
             result['IncludeIPRanges'] = self.include_ipranges
         if self.istio_version is not None:
             result['IstioVersion'] = self.istio_version
         if self.kiali_enabled is not None:
             result['KialiEnabled'] = self.kiali_enabled
         if self.locality_lbconf is not None:
@@ -2546,14 +2550,16 @@
             self.existing_root_ca_cert = m.get('ExistingRootCaCert')
         if m.get('ExistingRootCaKey') is not None:
             self.existing_root_ca_key = m.get('ExistingRootCaKey')
         if m.get('FilterGatewayClusterConfig') is not None:
             self.filter_gateway_cluster_config = m.get('FilterGatewayClusterConfig')
         if m.get('GatewayAPIEnabled') is not None:
             self.gateway_apienabled = m.get('GatewayAPIEnabled')
+        if m.get('GuestCluster') is not None:
+            self.guest_cluster = m.get('GuestCluster')
         if m.get('IncludeIPRanges') is not None:
             self.include_ipranges = m.get('IncludeIPRanges')
         if m.get('IstioVersion') is not None:
             self.istio_version = m.get('IstioVersion')
         if m.get('KialiEnabled') is not None:
             self.kiali_enabled = m.get('KialiEnabled')
         if m.get('LocalityLBConf') is not None:
```

### Comparing `alibabacloud_servicemesh20200111-3.0.0/alibabacloud_servicemesh20200111.egg-info/PKG-INFO` & `alibabacloud_servicemesh20200111-3.0.1/alibabacloud_servicemesh20200111.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-servicemesh20200111
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud Alibaba Cloud Service Mesh (20200111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_servicemesh20200111-3.0.0/setup.py` & `alibabacloud_servicemesh20200111-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_servicemesh20200111.
 
-Created on 27/07/2023
+Created on 09/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_servicemesh20200111"
 NAME = "alibabacloud_servicemesh20200111" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Alibaba Cloud Service Mesh (20200111) SDK Library for Python"
```

