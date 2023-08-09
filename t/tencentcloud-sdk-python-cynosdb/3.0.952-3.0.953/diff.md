# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.952.tar", last modified: Mon Aug  7 08:51:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.953.tar", last modified: Tue Aug  8 00:22:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.952.tar` & `tencentcloud-sdk-python-cynosdb-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)   120018 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11292 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   688377 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      539 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud_sdk_python_cynosdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:51:13.000000 tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)   120018 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11401 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   688412 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud_sdk_python_cynosdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:22:49.000000 tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.953/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cynosdb',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cynosdb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.952'
+__version__ = '3.0.953'
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,17 @@
 
 # 参数值无效，超过允许范围。
 INVALIDPARAMETERVALUE_PARAMETEROUTRANGEERROR = 'InvalidParameterValue.ParameterOutRangeError'
 
 # 预付费类型不允许该操作。
 INVALIDPARAMETERVALUE_PREPAYPAYMODEERROR = 'InvalidParameterValue.PrePayPayModeError'
 
+# 找不到该ProjectId
+INVALIDPARAMETERVALUE_PROJECTIDNOTFOUND = 'InvalidParameterValue.ProjectIdNotFound'
+
 # 所选地域和可用区不可用。
 INVALIDPARAMETERVALUE_REGIONZONEUNAVAILABLE = 'InvalidParameterValue.RegionZoneUnavailable'
 
 # 未找到相关存储pool。
 INVALIDPARAMETERVALUE_STORAGEPOOLNOTFOUND = 'InvalidParameterValue.StoragePoolNotFound'
 
 # 找不到所选子网。
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud/cynosdb/v20190107/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,15 @@
 class Addr(AbstractModel):
     """数据库地址
 
     """
 
     def __init__(self):
         r"""
-        :param _IP: IP
+        :param _IP: IP地址
         :type IP: str
         :param _Port: 端口
         :type Port: int
         """
         self._IP = None
         self._Port = None
 
@@ -3183,18 +3183,18 @@
         :type DbVersion: str
         :param _ProjectId: 所属项目ID
         :type ProjectId: int
         :param _Cpu: 当DbMode为NORMAL或不填时必选
 普通实例Cpu核数
         :type Cpu: int
         :param _Memory: 当DbMode为NORMAL或不填时必选
-普通实例内存,单位G
+普通实例内存,单位GB
         :type Memory: int
         :param _Storage: 该参数无实际意义，已废弃。
-存储大小，单位G。
+存储大小，单位GB。
         :type Storage: int
         :param _ClusterName: 集群名称，长度小于64个字符，每个字符取值范围：大/小写字母，数字，特殊符号（'-','_','.'）
         :type ClusterName: str
         :param _AdminPassword: 账号密码(8-64个字符，包含大小写英文字母、数字和符号~!@#$%^&*_-+=`|\(){}[]:;'<>,.?/中的任意三种)
         :type AdminPassword: str
         :param _Port: 端口，默认3306，取值范围[0, 65535)
         :type Port: int
@@ -5314,15 +5314,15 @@
         :type StorageLimit: int
         :param _UsedStorage: 使用容量
         :type UsedStorage: int
         :param _Vip: vip地址
         :type Vip: str
         :param _Vport: vport端口
         :type Vport: int
-        :param _RoAddr: 读写分离Vport
+        :param _RoAddr: 集群只读实例的vip地址和vport端口
         :type RoAddr: list of Addr
         :param _Ability: 集群支持的功能
 注意：此字段可能返回 null，表示取不到有效值。
         :type Ability: :class:`tencentcloud.cynosdb.v20190107.models.Ability`
         :param _CynosVersion: cynos版本
 注意：此字段可能返回 null，表示取不到有效值。
         :type CynosVersion: str
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.953/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.953/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.952/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.953/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

