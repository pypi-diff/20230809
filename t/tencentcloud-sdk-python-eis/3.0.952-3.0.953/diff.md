# Comparing `tmp/tencentcloud-sdk-python-eis-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-eis-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.952.tar", last modified: Mon Aug  7 08:53:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.953.tar", last modified: Tue Aug  8 00:24:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eis-3.0.952.tar` & `tencentcloud-sdk-python-eis-3.0.953.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud_sdk_python_eis.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      653 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud_sdk_python_eis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud_sdk_python_eis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20210601/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20210601/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20210601/eis_client.py
--rw-r--r--   0 root         (0) root         (0)     2977 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20210601/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39966 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20210601/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20200715/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20200715/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20200715/eis_client.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20200715/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    17929 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20200715/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 08:53:18.000000 tencentcloud-sdk-python-eis-3.0.952/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud_sdk_python_eis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud_sdk_python_eis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud_sdk_python_eis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20210601/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20210601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20210601/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20210601/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    40984 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20210601/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20200715/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20200715/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20200715/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20200715/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    17929 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20200715/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:24:37.000000 tencentcloud-sdk-python-eis-3.0.953/README.rst
```

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud_sdk_python_eis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud_sdk_python_eis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.952/setup.py` & `tencentcloud-sdk-python-eis-3.0.953/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-eis',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Eis SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20210601/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20210601/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20210601/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20210601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20210601/models.py` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20210601/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,25 +42,29 @@
         :param _ExpiredAt: 环境过期时间
         :type ExpiredAt: int
         :param _RuntimeClass: 环境运行类型：0:运行时类型、1:api类型
         :type RuntimeClass: int
         :param _Deployed: 是否已在当前环境发布
 注意：此字段可能返回 null，表示取不到有效值。
         :type Deployed: bool
+        :param _MatchExtensions: 环境扩展组件是否满足应用要求：0=true, 1=false 表示该应用需要扩展组件0(cdc)以及1(java)，但是独立环境有cdc无java，不满足发布要求
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MatchExtensions: str
         """
         self._RuntimeId = None
         self._DisplayName = None
         self._Type = None
         self._Zone = None
         self._Area = None
         self._Addr = None
         self._Status = None
         self._ExpiredAt = None
         self._RuntimeClass = None
         self._Deployed = None
+        self._MatchExtensions = None
 
     @property
     def RuntimeId(self):
         return self._RuntimeId
 
     @RuntimeId.setter
     def RuntimeId(self, RuntimeId):
@@ -134,26 +138,35 @@
     def Deployed(self):
         return self._Deployed
 
     @Deployed.setter
     def Deployed(self, Deployed):
         self._Deployed = Deployed
 
+    @property
+    def MatchExtensions(self):
+        return self._MatchExtensions
+
+    @MatchExtensions.setter
+    def MatchExtensions(self, MatchExtensions):
+        self._MatchExtensions = MatchExtensions
+
 
     def _deserialize(self, params):
         self._RuntimeId = params.get("RuntimeId")
         self._DisplayName = params.get("DisplayName")
         self._Type = params.get("Type")
         self._Zone = params.get("Zone")
         self._Area = params.get("Area")
         self._Addr = params.get("Addr")
         self._Status = params.get("Status")
         self._ExpiredAt = params.get("ExpiredAt")
         self._RuntimeClass = params.get("RuntimeClass")
         self._Deployed = params.get("Deployed")
+        self._MatchExtensions = params.get("MatchExtensions")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -424,18 +437,21 @@
         r"""
         :param _ProjectId: 应用id
         :type ProjectId: int
         :param _InstanceId: 实例id
         :type InstanceId: int
         :param _PlanType: 版本类型 0-pro 1-lite
         :type PlanType: int
+        :param _RuntimeClass: 0：应用集成，1：API，2：ETL
+        :type RuntimeClass: int
         """
         self._ProjectId = None
         self._InstanceId = None
         self._PlanType = None
+        self._RuntimeClass = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -453,19 +469,28 @@
     def PlanType(self):
         return self._PlanType
 
     @PlanType.setter
     def PlanType(self, PlanType):
         self._PlanType = PlanType
 
+    @property
+    def RuntimeClass(self):
+        return self._RuntimeClass
+
+    @RuntimeClass.setter
+    def RuntimeClass(self, RuntimeClass):
+        self._RuntimeClass = RuntimeClass
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._InstanceId = params.get("InstanceId")
         self._PlanType = params.get("PlanType")
+        self._RuntimeClass = params.get("RuntimeClass")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1002,15 +1027,15 @@
 class RuntimeExtensionMC(AbstractModel):
     """运行环境扩展组件
 
     """
 
     def __init__(self):
         r"""
-        :param _Type: 扩展组件类型：0:cdc
+        :param _Type: 扩展组件类型：0:cdc 1:dataway-java
         :type Type: int
         :param _Size: 部署规格vcore数
         :type Size: float
         :param _Replica: 副本数
         :type Replica: int
         :param _Name: 扩展组件名称
         :type Name: str
@@ -1155,15 +1180,15 @@
         :type AutoRenewal: bool
         :param _WorkerExtensions: 扩展组件列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type WorkerExtensions: list of RuntimeExtensionMC
         :param _RuntimeType: 环境类型：0: sandbox, 1:shared, 2:private 3: trial
 注意：此字段可能返回 null，表示取不到有效值。
         :type RuntimeType: int
-        :param _RuntimeClass: 环境运行类型：0:运行时类型、1:api类型
+        :param _RuntimeClass: 环境运行类型：0:运行时类型、1:api类型、2:etl环境
 注意：此字段可能返回 null，表示取不到有效值。
         :type RuntimeClass: int
         :param _BandwidthOutUsed: 已使用出带宽 Mbps
 注意：此字段可能返回 null，表示取不到有效值。
         :type BandwidthOutUsed: float
         :param _BandwidthOutLimit: 出带宽上限 Mbps
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20200715/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20200715/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20200715/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20200715/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud/eis/v20200715/models.py` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud/eis/v20200715/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eis-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-eis-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.953/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.952/README.rst` & `tencentcloud-sdk-python-eis-3.0.953/README.rst`

 * *Files identical despite different names*

