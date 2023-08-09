# Comparing `tmp/tencentcloud-sdk-python-csip-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-csip-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.952.tar", last modified: Mon Aug  7 08:50:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.953.tar", last modified: Tue Aug  8 00:22:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-csip-3.0.952.tar` & `tencentcloud-sdk-python-csip-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud_sdk_python_csip.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      506 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud_sdk_python_csip.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud_sdk_python_csip.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/v20221121/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/v20221121/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/v20221121/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    14571 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/v20221121/csip_client.py
--rw-r--r--   0 root         (0) root         (0)   190268 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/v20221121/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-07 08:50:44.000000 tencentcloud-sdk-python-csip-3.0.952/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud_sdk_python_csip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud_sdk_python_csip.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud_sdk_python_csip.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/v20221121/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/v20221121/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/v20221121/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    14571 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/v20221121/csip_client.py
+-rw-r--r--   0 root         (0) root         (0)   196206 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/v20221121/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-08 00:22:19.000000 tencentcloud-sdk-python-csip-3.0.953/README.rst
```

### Comparing `tencentcloud-sdk-python-csip-3.0.952/setup.py` & `tencentcloud-sdk-python-csip-3.0.953/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-csip',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Csip SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-csip-3.0.952/tencentcloud_sdk_python_csip.egg-info/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.953/tencentcloud_sdk_python_csip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-csip-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/v20221121/errorcodes.py` & `tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/v20221121/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/v20221121/csip_client.py` & `tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/v20221121/csip_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.952/tencentcloud/csip/v20221121/models.py` & `tencentcloud-sdk-python-csip-3.0.953/tencentcloud/csip/v20221121/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -519,14 +519,17 @@
         :type PublicIp: str
         :param _PrivateIp: 内网ip
 注意：此字段可能返回 null，表示取不到有效值。
         :type PrivateIp: str
         :param _IsCore: 是否核心：1:核心，2:非核心
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsCore: int
+        :param _IsNewAsset: 是否新资产 1新
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNewAsset: int
         """
         self._AppId = None
         self._Uin = None
         self._Nick = None
         self._Region = None
         self._AssetId = None
         self._AssetName = None
@@ -539,14 +542,15 @@
         self._MachineName = None
         self._PodIp = None
         self._ServiceCount = None
         self._ContainerCount = None
         self._PublicIp = None
         self._PrivateIp = None
         self._IsCore = None
+        self._IsNewAsset = None
 
     @property
     def AppId(self):
         return self._AppId
 
     @AppId.setter
     def AppId(self, AppId):
@@ -692,14 +696,22 @@
     def IsCore(self):
         return self._IsCore
 
     @IsCore.setter
     def IsCore(self, IsCore):
         self._IsCore = IsCore
 
+    @property
+    def IsNewAsset(self):
+        return self._IsNewAsset
+
+    @IsNewAsset.setter
+    def IsNewAsset(self, IsNewAsset):
+        self._IsNewAsset = IsNewAsset
+
 
     def _deserialize(self, params):
         self._AppId = params.get("AppId")
         self._Uin = params.get("Uin")
         self._Nick = params.get("Nick")
         self._Region = params.get("Region")
         self._AssetId = params.get("AssetId")
@@ -713,14 +725,15 @@
         self._MachineName = params.get("MachineName")
         self._PodIp = params.get("PodIp")
         self._ServiceCount = params.get("ServiceCount")
         self._ContainerCount = params.get("ContainerCount")
         self._PublicIp = params.get("PublicIp")
         self._PrivateIp = params.get("PrivateIp")
         self._IsCore = params.get("IsCore")
+        self._IsNewAsset = params.get("IsNewAsset")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1551,14 +1564,17 @@
         :type Os: str
         :param _RiskExposure: 风险服务暴露
 注意：此字段可能返回 null，表示取不到有效值。
         :type RiskExposure: int
         :param _BASAgentStatus: 模拟攻击工具状态。0代表未安装，1代表已安装，2代表已离线
 注意：此字段可能返回 null，表示取不到有效值。
         :type BASAgentStatus: int
+        :param _IsNewAsset: 1新资产；0 非新资产
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNewAsset: int
         """
         self._AssetId = None
         self._AssetName = None
         self._AssetType = None
         self._Region = None
         self._CWPStatus = None
         self._AssetCreateTime = None
@@ -1602,14 +1618,15 @@
         self._ConfigurationRisk = None
         self._ScanTask = None
         self._Tag = None
         self._MemberId = None
         self._Os = None
         self._RiskExposure = None
         self._BASAgentStatus = None
+        self._IsNewAsset = None
 
     @property
     def AssetId(self):
         return self._AssetId
 
     @AssetId.setter
     def AssetId(self, AssetId):
@@ -2003,14 +2020,22 @@
     def BASAgentStatus(self):
         return self._BASAgentStatus
 
     @BASAgentStatus.setter
     def BASAgentStatus(self, BASAgentStatus):
         self._BASAgentStatus = BASAgentStatus
 
+    @property
+    def IsNewAsset(self):
+        return self._IsNewAsset
+
+    @IsNewAsset.setter
+    def IsNewAsset(self, IsNewAsset):
+        self._IsNewAsset = IsNewAsset
+
 
     def _deserialize(self, params):
         self._AssetId = params.get("AssetId")
         self._AssetName = params.get("AssetName")
         self._AssetType = params.get("AssetType")
         self._Region = params.get("Region")
         self._CWPStatus = params.get("CWPStatus")
@@ -2060,14 +2085,15 @@
                 obj = Tag()
                 obj._deserialize(item)
                 self._Tag.append(obj)
         self._MemberId = params.get("MemberId")
         self._Os = params.get("Os")
         self._RiskExposure = params.get("RiskExposure")
         self._BASAgentStatus = params.get("BASAgentStatus")
+        self._IsNewAsset = params.get("IsNewAsset")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2151,15 +2177,15 @@
 
     def __init__(self):
         r"""
         :param _TaskName: 任务名称
         :type TaskName: str
         :param _ScanAssetType: 0-全扫，1-指定资产扫，2-排除资产扫，3-手动填写扫；1和2则Assets字段必填，3则SelfDefiningAssets必填
         :type ScanAssetType: int
-        :param _ScanItem: 扫描项目；port/poc/weakpass/webcontent/configrisk
+        :param _ScanItem: 扫描项目；port/poc/weakpass/webcontent/configrisk/exposedserver
         :type ScanItem: list of str
         :param _ScanPlanType: 0-周期任务,1-立即扫描,2-定时扫描,3-自定义；0,2,3则ScanPlanContent必填
         :type ScanPlanType: int
         :param _Assets: 扫描资产信息列表
         :type Assets: list of TaskAssetObject
         :param _ScanPlanContent: 扫描计划详情
         :type ScanPlanContent: str
@@ -2285,39 +2311,63 @@
 
     """
 
     def __init__(self):
         r"""
         :param _TaskId: 任务id
         :type TaskId: str
+        :param _Status: 0,任务创建成功；小于0失败；-1为存在资产未认证
+        :type Status: int
+        :param _UnAuthAsset: 未认证资产列表
+        :type UnAuthAsset: list of str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TaskId = None
+        self._Status = None
+        self._UnAuthAsset = None
         self._RequestId = None
 
     @property
     def TaskId(self):
         return self._TaskId
 
     @TaskId.setter
     def TaskId(self, TaskId):
         self._TaskId = TaskId
 
     @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def UnAuthAsset(self):
+        return self._UnAuthAsset
+
+    @UnAuthAsset.setter
+    def UnAuthAsset(self, UnAuthAsset):
+        self._UnAuthAsset = UnAuthAsset
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
+        self._Status = params.get("Status")
+        self._UnAuthAsset = params.get("UnAuthAsset")
         self._RequestId = params.get("RequestId")
 
 
 class DBAssetVO(AbstractModel):
     """db资产输出字段
 
     """
@@ -2386,14 +2436,17 @@
         :type PublicIp: str
         :param _Status: 状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: int
         :param _IsCore: 是否核心
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsCore: int
+        :param _IsNewAsset: 是否新资产: 1新
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNewAsset: int
         """
         self._AssetId = None
         self._AssetName = None
         self._AssetType = None
         self._VpcId = None
         self._VpcName = None
         self._Region = None
@@ -2409,14 +2462,15 @@
         self._NickName = None
         self._Port = None
         self._Tag = None
         self._PrivateIp = None
         self._PublicIp = None
         self._Status = None
         self._IsCore = None
+        self._IsNewAsset = None
 
     @property
     def AssetId(self):
         return self._AssetId
 
     @AssetId.setter
     def AssetId(self, AssetId):
@@ -2586,14 +2640,22 @@
     def IsCore(self):
         return self._IsCore
 
     @IsCore.setter
     def IsCore(self, IsCore):
         self._IsCore = IsCore
 
+    @property
+    def IsNewAsset(self):
+        return self._IsNewAsset
+
+    @IsNewAsset.setter
+    def IsNewAsset(self, IsNewAsset):
+        self._IsNewAsset = IsNewAsset
+
 
     def _deserialize(self, params):
         self._AssetId = params.get("AssetId")
         self._AssetName = params.get("AssetName")
         self._AssetType = params.get("AssetType")
         self._VpcId = params.get("VpcId")
         self._VpcName = params.get("VpcName")
@@ -2615,14 +2677,15 @@
                 obj = Tag()
                 obj._deserialize(item)
                 self._Tag.append(obj)
         self._PrivateIp = params.get("PrivateIp")
         self._PublicIp = params.get("PublicIp")
         self._Status = params.get("Status")
         self._IsCore = params.get("IsCore")
+        self._IsNewAsset = params.get("IsNewAsset")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -4731,14 +4794,26 @@
         :type CCAttack: int
         :param _WebAttack: web攻击
 注意：此字段可能返回 null，表示取不到有效值。
         :type WebAttack: int
         :param _ServiceRisk: 风险服务暴露数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type ServiceRisk: int
+        :param _IsNewAsset: 是否新资产 1新
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNewAsset: int
+        :param _VerifyDomain: 待确认资产的随机三级域名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VerifyDomain: str
+        :param _VerifyTXTRecord: 待确认资产的TXT记录内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VerifyTXTRecord: str
+        :param _VerifyStatus: 待确认资产的认证状态，0-待认证，1-认证成功，2-认证中，3-txt认证失败，4-人工认证失败
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VerifyStatus: int
         """
         self._AssetId = None
         self._AssetName = None
         self._AssetType = None
         self._Region = None
         self._WAFStatus = None
         self._AssetCreateTime = None
@@ -4766,14 +4841,18 @@
         self._WebContentRisk = None
         self._Tag = None
         self._SourceType = None
         self._MemberId = None
         self._CCAttack = None
         self._WebAttack = None
         self._ServiceRisk = None
+        self._IsNewAsset = None
+        self._VerifyDomain = None
+        self._VerifyTXTRecord = None
+        self._VerifyStatus = None
 
     @property
     def AssetId(self):
         return self._AssetId
 
     @AssetId.setter
     def AssetId(self, AssetId):
@@ -5039,14 +5118,46 @@
     def ServiceRisk(self):
         return self._ServiceRisk
 
     @ServiceRisk.setter
     def ServiceRisk(self, ServiceRisk):
         self._ServiceRisk = ServiceRisk
 
+    @property
+    def IsNewAsset(self):
+        return self._IsNewAsset
+
+    @IsNewAsset.setter
+    def IsNewAsset(self, IsNewAsset):
+        self._IsNewAsset = IsNewAsset
+
+    @property
+    def VerifyDomain(self):
+        return self._VerifyDomain
+
+    @VerifyDomain.setter
+    def VerifyDomain(self, VerifyDomain):
+        self._VerifyDomain = VerifyDomain
+
+    @property
+    def VerifyTXTRecord(self):
+        return self._VerifyTXTRecord
+
+    @VerifyTXTRecord.setter
+    def VerifyTXTRecord(self, VerifyTXTRecord):
+        self._VerifyTXTRecord = VerifyTXTRecord
+
+    @property
+    def VerifyStatus(self):
+        return self._VerifyStatus
+
+    @VerifyStatus.setter
+    def VerifyStatus(self, VerifyStatus):
+        self._VerifyStatus = VerifyStatus
+
 
     def _deserialize(self, params):
         self._AssetId = params.get("AssetId")
         self._AssetName = params.get("AssetName")
         self._AssetType = params.get("AssetType")
         self._Region = params.get("Region")
         self._WAFStatus = params.get("WAFStatus")
@@ -5080,14 +5191,18 @@
                 obj._deserialize(item)
                 self._Tag.append(obj)
         self._SourceType = params.get("SourceType")
         self._MemberId = params.get("MemberId")
         self._CCAttack = params.get("CCAttack")
         self._WebAttack = params.get("WebAttack")
         self._ServiceRisk = params.get("ServiceRisk")
+        self._IsNewAsset = params.get("IsNewAsset")
+        self._VerifyDomain = params.get("VerifyDomain")
+        self._VerifyTXTRecord = params.get("VerifyTXTRecord")
+        self._VerifyStatus = params.get("VerifyStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5351,14 +5466,20 @@
         :type AddressId: str
         :param _MemberId: memberid信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type MemberId: str
         :param _RiskExposure: 风险服务暴露
 注意：此字段可能返回 null，表示取不到有效值。
         :type RiskExposure: int
+        :param _IsNewAsset: 是否新资产 1新
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNewAsset: int
+        :param _VerifyStatus: 资产认证状态，0-待认证，1-认证成功，2-认证中，3+-认证失败
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VerifyStatus: int
         """
         self._AssetId = None
         self._AssetName = None
         self._AssetType = None
         self._Region = None
         self._CFWStatus = None
         self._AssetCreateTime = None
@@ -5385,14 +5506,16 @@
         self._ScanTask = None
         self._WeakPassword = None
         self._WebContentRisk = None
         self._Tag = None
         self._AddressId = None
         self._MemberId = None
         self._RiskExposure = None
+        self._IsNewAsset = None
+        self._VerifyStatus = None
 
     @property
     def AssetId(self):
         return self._AssetId
 
     @AssetId.setter
     def AssetId(self, AssetId):
@@ -5650,14 +5773,30 @@
     def RiskExposure(self):
         return self._RiskExposure
 
     @RiskExposure.setter
     def RiskExposure(self, RiskExposure):
         self._RiskExposure = RiskExposure
 
+    @property
+    def IsNewAsset(self):
+        return self._IsNewAsset
+
+    @IsNewAsset.setter
+    def IsNewAsset(self, IsNewAsset):
+        self._IsNewAsset = IsNewAsset
+
+    @property
+    def VerifyStatus(self):
+        return self._VerifyStatus
+
+    @VerifyStatus.setter
+    def VerifyStatus(self, VerifyStatus):
+        self._VerifyStatus = VerifyStatus
+
 
     def _deserialize(self, params):
         self._AssetId = params.get("AssetId")
         self._AssetName = params.get("AssetName")
         self._AssetType = params.get("AssetType")
         self._Region = params.get("Region")
         self._CFWStatus = params.get("CFWStatus")
@@ -5690,14 +5829,16 @@
             for item in params.get("Tag"):
                 obj = Tag()
                 obj._deserialize(item)
                 self._Tag.append(obj)
         self._AddressId = params.get("AddressId")
         self._MemberId = params.get("MemberId")
         self._RiskExposure = params.get("RiskExposure")
+        self._IsNewAsset = params.get("IsNewAsset")
+        self._VerifyStatus = params.get("VerifyStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5922,14 +6063,17 @@
         :param _ScanTask: 任务数
         :type ScanTask: int
         :param _LastScanTime: 最后扫描时间
         :type LastScanTime: str
         :param _IsCore: 是否核心
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsCore: int
+        :param _IsNewAsset: 是否新资产 1新
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNewAsset: int
         """
         self._AppId = None
         self._Uin = None
         self._AssetId = None
         self._AssetName = None
         self._Region = None
         self._VpcId = None
@@ -5941,14 +6085,15 @@
         self._CVM = None
         self._AvailableIp = None
         self._CreateTime = None
         self._ConfigureRisk = None
         self._ScanTask = None
         self._LastScanTime = None
         self._IsCore = None
+        self._IsNewAsset = None
 
     @property
     def AppId(self):
         return self._AppId
 
     @AppId.setter
     def AppId(self, AppId):
@@ -6086,14 +6231,22 @@
     def IsCore(self):
         return self._IsCore
 
     @IsCore.setter
     def IsCore(self, IsCore):
         self._IsCore = IsCore
 
+    @property
+    def IsNewAsset(self):
+        return self._IsNewAsset
+
+    @IsNewAsset.setter
+    def IsNewAsset(self, IsNewAsset):
+        self._IsNewAsset = IsNewAsset
+
 
     def _deserialize(self, params):
         self._AppId = params.get("AppId")
         self._Uin = params.get("Uin")
         self._AssetId = params.get("AssetId")
         self._AssetName = params.get("AssetName")
         self._Region = params.get("Region")
@@ -6111,14 +6264,15 @@
         self._CVM = params.get("CVM")
         self._AvailableIp = params.get("AvailableIp")
         self._CreateTime = params.get("CreateTime")
         self._ConfigureRisk = params.get("ConfigureRisk")
         self._ScanTask = params.get("ScanTask")
         self._LastScanTime = params.get("LastScanTime")
         self._IsCore = params.get("IsCore")
+        self._IsNewAsset = params.get("IsNewAsset")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -6505,28 +6659,36 @@
         :type CreateTime: str
         :param _AppId: appid
         :type AppId: str
         :param _Uin: uin
         :type Uin: str
         :param _Nick: 昵称
         :type Nick: str
+        :param _IsNewAsset: 是否新资产 1新
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsNewAsset: int
+        :param _IsCore: 是否核心资产1是 2不是
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsCore: int
         """
         self._Subnet = None
         self._ConnectedVpc = None
         self._AssetId = None
         self._Region = None
         self._CVM = None
         self._Tag = None
         self._DNS = None
         self._AssetName = None
         self._CIDR = None
         self._CreateTime = None
         self._AppId = None
         self._Uin = None
         self._Nick = None
+        self._IsNewAsset = None
+        self._IsCore = None
 
     @property
     def Subnet(self):
         return self._Subnet
 
     @Subnet.setter
     def Subnet(self, Subnet):
@@ -6624,14 +6786,30 @@
     def Nick(self):
         return self._Nick
 
     @Nick.setter
     def Nick(self, Nick):
         self._Nick = Nick
 
+    @property
+    def IsNewAsset(self):
+        return self._IsNewAsset
+
+    @IsNewAsset.setter
+    def IsNewAsset(self, IsNewAsset):
+        self._IsNewAsset = IsNewAsset
+
+    @property
+    def IsCore(self):
+        return self._IsCore
+
+    @IsCore.setter
+    def IsCore(self, IsCore):
+        self._IsCore = IsCore
+
 
     def _deserialize(self, params):
         self._Subnet = params.get("Subnet")
         self._ConnectedVpc = params.get("ConnectedVpc")
         self._AssetId = params.get("AssetId")
         self._Region = params.get("Region")
         self._CVM = params.get("CVM")
@@ -6644,14 +6822,16 @@
         self._DNS = params.get("DNS")
         self._AssetName = params.get("AssetName")
         self._CIDR = params.get("CIDR")
         self._CreateTime = params.get("CreateTime")
         self._AppId = params.get("AppId")
         self._Uin = params.get("Uin")
         self._Nick = params.get("Nick")
+        self._IsNewAsset = params.get("IsNewAsset")
+        self._IsCore = params.get("IsCore")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -6665,15 +6845,18 @@
 
     def __init__(self):
         r"""
         :param _Name: 过滤的项
         :type Name: str
         :param _Values: 过滤的值
         :type Values: list of str
-        :param _OperatorType: 精确匹配填 7 模糊匹配填9 ， 兼容 中台定的结构
+        :param _OperatorType: 中台定义：
+1等于 2大于 3小于 4大于等于 5小于等于 6不等于 9模糊匹配 13非模糊匹配 14按位与
+精确匹配填 7 模糊匹配填9 兼容 中台定的结构
+
         :type OperatorType: int
         """
         self._Name = None
         self._Values = None
         self._OperatorType = None
 
     @property
```

### Comparing `tencentcloud-sdk-python-csip-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.953/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.952/README.rst` & `tencentcloud-sdk-python-csip-3.0.953/README.rst`

 * *Files identical despite different names*

