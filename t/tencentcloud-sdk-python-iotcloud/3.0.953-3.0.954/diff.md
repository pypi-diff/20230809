# Comparing `tmp/tencentcloud-sdk-python-iotcloud-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-iotcloud-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.953.tar", last modified: Tue Aug  8 00:26:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.954.tar", last modified: Wed Aug  9 00:27:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotcloud-3.0.953.tar` & `tencentcloud-sdk-python-iotcloud-3.0.954.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20210408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20210408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67173 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20210408/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)    12818 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20210408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   278249 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20210408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20180614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20180614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64562 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20180614/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)    12668 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20180614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   281180 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20180614/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud_sdk_python_iotcloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      733 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud_sdk_python_iotcloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-08-08 00:26:58.000000 tencentcloud-sdk-python-iotcloud-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20210408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20210408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67173 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20210408/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)    12818 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20210408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   280299 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20210408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20180614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20180614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64562 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20180614/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)    12668 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20180614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   281180 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20180614/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud_sdk_python_iotcloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      733 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud_sdk_python_iotcloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-09 00:27:01.000000 tencentcloud-sdk-python-iotcloud-3.0.954/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-09 00:27:00.000000 tencentcloud-sdk-python-iotcloud-3.0.954/README.rst
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.953'
+__version__ = '3.0.954'
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20210408/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20210408/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20210408/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20210408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20210408/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20210408/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,23 +512,26 @@
         :type Result: str
         :param _Scene: 模块
         :type Scene: str
         :param _Time: 日志时间
         :type Time: str
         :param _Userid: 腾讯云账号
         :type Userid: str
+        :param _UserId: 腾讯云账号
+        :type UserId: str
         """
         self._Content = None
         self._DeviceName = None
         self._ProductId = None
         self._RequestId = None
         self._Result = None
         self._Scene = None
         self._Time = None
         self._Userid = None
+        self._UserId = None
 
     @property
     def Content(self):
         return self._Content
 
     @Content.setter
     def Content(self, Content):
@@ -580,30 +583,43 @@
 
     @Time.setter
     def Time(self, Time):
         self._Time = Time
 
     @property
     def Userid(self):
+        warnings.warn("parameter `Userid` is deprecated", DeprecationWarning) 
+
         return self._Userid
 
     @Userid.setter
     def Userid(self, Userid):
+        warnings.warn("parameter `Userid` is deprecated", DeprecationWarning) 
+
         self._Userid = Userid
 
+    @property
+    def UserId(self):
+        return self._UserId
+
+    @UserId.setter
+    def UserId(self, UserId):
+        self._UserId = UserId
+
 
     def _deserialize(self, params):
         self._Content = params.get("Content")
         self._DeviceName = params.get("DeviceName")
         self._ProductId = params.get("ProductId")
         self._RequestId = params.get("RequestId")
         self._Result = params.get("Result")
         self._Scene = params.get("Scene")
         self._Time = params.get("Time")
         self._Userid = params.get("Userid")
+        self._UserId = params.get("UserId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -2535,15 +2551,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _DeviceName: 设备名
         :type DeviceName: str
-        :param _Online: 设备是否在线，0不在线，1在线
+        :param _Online: 设备是否在线，0不在线，1在线，3未激活
         :type Online: int
         :param _LoginTime: 设备登录时间
         :type LoginTime: int
         :param _Version: 设备固件版本
         :type Version: str
         :param _LastUpdateTime: 设备最后更新时间
         :type LastUpdateTime: int
@@ -2593,14 +2609,16 @@
         :type ClientIP: str
         :param _FirmwareUpdateTime: 设备固件更新时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type FirmwareUpdateTime: int
         :param _CreateUserId: 创建者账号ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateUserId: int
+        :param _NBIoTDeviceID: NB IoT运营商处的DeviceID
+        :type NBIoTDeviceID: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._DeviceName = None
         self._Online = None
         self._LoginTime = None
         self._Version = None
@@ -2621,14 +2639,15 @@
         self._CreateTime = None
         self._CertState = None
         self._EnableState = None
         self._Labels = None
         self._ClientIP = None
         self._FirmwareUpdateTime = None
         self._CreateUserId = None
+        self._NBIoTDeviceID = None
         self._RequestId = None
 
     @property
     def DeviceName(self):
         return self._DeviceName
 
     @DeviceName.setter
@@ -2721,18 +2740,22 @@
 
     @ConnIP.setter
     def ConnIP(self, ConnIP):
         self._ConnIP = ConnIP
 
     @property
     def NbiotDeviceID(self):
+        warnings.warn("parameter `NbiotDeviceID` is deprecated", DeprecationWarning) 
+
         return self._NbiotDeviceID
 
     @NbiotDeviceID.setter
     def NbiotDeviceID(self, NbiotDeviceID):
+        warnings.warn("parameter `NbiotDeviceID` is deprecated", DeprecationWarning) 
+
         self._NbiotDeviceID = NbiotDeviceID
 
     @property
     def LoraDevEui(self):
         return self._LoraDevEui
 
     @LoraDevEui.setter
@@ -2824,14 +2847,22 @@
         return self._CreateUserId
 
     @CreateUserId.setter
     def CreateUserId(self, CreateUserId):
         self._CreateUserId = CreateUserId
 
     @property
+    def NBIoTDeviceID(self):
+        return self._NBIoTDeviceID
+
+    @NBIoTDeviceID.setter
+    def NBIoTDeviceID(self, NBIoTDeviceID):
+        self._NBIoTDeviceID = NBIoTDeviceID
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -2868,14 +2899,15 @@
             for item in params.get("Labels"):
                 obj = DeviceLabel()
                 obj._deserialize(item)
                 self._Labels.append(obj)
         self._ClientIP = params.get("ClientIP")
         self._FirmwareUpdateTime = params.get("FirmwareUpdateTime")
         self._CreateUserId = params.get("CreateUserId")
+        self._NBIoTDeviceID = params.get("NBIoTDeviceID")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeDeviceShadowRequest(AbstractModel):
     """DescribeDeviceShadow请求参数结构体
 
     """
@@ -5320,14 +5352,16 @@
         :type ClientIP: str
         :param _FirmwareUpdateTime: ota最后更新时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type FirmwareUpdateTime: int
         :param _CreateUserId: 创建者 Uin
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateUserId: int
+        :param _NBIoTDeviceID: NB IOT运营商处的DeviceID
+        :type NBIoTDeviceID: str
         """
         self._DeviceName = None
         self._Online = None
         self._LoginTime = None
         self._Version = None
         self._DeviceCert = None
         self._DevicePsk = None
@@ -5346,14 +5380,15 @@
         self._LogLevel = None
         self._CertState = None
         self._EnableState = None
         self._Labels = None
         self._ClientIP = None
         self._FirmwareUpdateTime = None
         self._CreateUserId = None
+        self._NBIoTDeviceID = None
 
     @property
     def DeviceName(self):
         return self._DeviceName
 
     @DeviceName.setter
     def DeviceName(self, DeviceName):
@@ -5429,18 +5464,22 @@
 
     @Isp.setter
     def Isp(self, Isp):
         self._Isp = Isp
 
     @property
     def NbiotDeviceID(self):
+        warnings.warn("parameter `NbiotDeviceID` is deprecated", DeprecationWarning) 
+
         return self._NbiotDeviceID
 
     @NbiotDeviceID.setter
     def NbiotDeviceID(self, NbiotDeviceID):
+        warnings.warn("parameter `NbiotDeviceID` is deprecated", DeprecationWarning) 
+
         self._NbiotDeviceID = NbiotDeviceID
 
     @property
     def ConnIP(self):
         return self._ConnIP
 
     @ConnIP.setter
@@ -5547,14 +5586,22 @@
     def CreateUserId(self):
         return self._CreateUserId
 
     @CreateUserId.setter
     def CreateUserId(self, CreateUserId):
         self._CreateUserId = CreateUserId
 
+    @property
+    def NBIoTDeviceID(self):
+        return self._NBIoTDeviceID
+
+    @NBIoTDeviceID.setter
+    def NBIoTDeviceID(self, NBIoTDeviceID):
+        self._NBIoTDeviceID = NBIoTDeviceID
+
 
     def _deserialize(self, params):
         self._DeviceName = params.get("DeviceName")
         self._Online = params.get("Online")
         self._LoginTime = params.get("LoginTime")
         self._Version = params.get("Version")
         self._DeviceCert = params.get("DeviceCert")
@@ -5584,14 +5631,15 @@
             for item in params.get("Labels"):
                 obj = DeviceLabel()
                 obj._deserialize(item)
                 self._Labels.append(obj)
         self._ClientIP = params.get("ClientIP")
         self._FirmwareUpdateTime = params.get("FirmwareUpdateTime")
         self._CreateUserId = params.get("CreateUserId")
+        self._NBIoTDeviceID = params.get("NBIoTDeviceID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7702,14 +7750,16 @@
         :type PrivateCAName: str
         :param _OriginUserId: 划归的产品，展示为源用户ID，其余为空
         :type OriginUserId: int
         :param _DeviceLimit: 设备限制
         :type DeviceLimit: int
         :param _ForbiddenStatus: 产品禁用状态
         :type ForbiddenStatus: int
+        :param _AppEUI: LoRa产品运营侧APPEUI，只有LoRa产品需要填写
+        :type AppEUI: str
         """
         self._ProductDescription = None
         self._EncryptionType = None
         self._Region = None
         self._ProductType = None
         self._Format = None
         self._Platform = None
@@ -7721,14 +7771,15 @@
         self._ProductSecret = None
         self._RegisterLimit = None
         self._OriginProductId = None
         self._PrivateCAName = None
         self._OriginUserId = None
         self._DeviceLimit = None
         self._ForbiddenStatus = None
+        self._AppEUI = None
 
     @property
     def ProductDescription(self):
         return self._ProductDescription
 
     @ProductDescription.setter
     def ProductDescription(self, ProductDescription):
@@ -7772,18 +7823,22 @@
 
     @Platform.setter
     def Platform(self, Platform):
         self._Platform = Platform
 
     @property
     def Appeui(self):
+        warnings.warn("parameter `Appeui` is deprecated", DeprecationWarning) 
+
         return self._Appeui
 
     @Appeui.setter
     def Appeui(self, Appeui):
+        warnings.warn("parameter `Appeui` is deprecated", DeprecationWarning) 
+
         self._Appeui = Appeui
 
     @property
     def ModelId(self):
         return self._ModelId
 
     @ModelId.setter
@@ -7866,14 +7921,22 @@
     def ForbiddenStatus(self):
         return self._ForbiddenStatus
 
     @ForbiddenStatus.setter
     def ForbiddenStatus(self, ForbiddenStatus):
         self._ForbiddenStatus = ForbiddenStatus
 
+    @property
+    def AppEUI(self):
+        return self._AppEUI
+
+    @AppEUI.setter
+    def AppEUI(self, AppEUI):
+        self._AppEUI = AppEUI
+
 
     def _deserialize(self, params):
         self._ProductDescription = params.get("ProductDescription")
         self._EncryptionType = params.get("EncryptionType")
         self._Region = params.get("Region")
         self._ProductType = params.get("ProductType")
         self._Format = params.get("Format")
@@ -7886,14 +7949,15 @@
         self._ProductSecret = params.get("ProductSecret")
         self._RegisterLimit = params.get("RegisterLimit")
         self._OriginProductId = params.get("OriginProductId")
         self._PrivateCAName = params.get("PrivateCAName")
         self._OriginUserId = params.get("OriginUserId")
         self._DeviceLimit = params.get("DeviceLimit")
         self._ForbiddenStatus = params.get("ForbiddenStatus")
+        self._AppEUI = params.get("AppEUI")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20180614/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20180614/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20180614/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20180614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud/iotcloud/v20180614/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud/iotcloud/v20180614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.954/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.954/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.953/README.rst` & `tencentcloud-sdk-python-iotcloud-3.0.954/README.rst`

 * *Files identical despite different names*

