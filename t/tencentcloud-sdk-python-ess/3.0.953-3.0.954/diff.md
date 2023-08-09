# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.953.tar", last modified: Tue Aug  8 00:24:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.954.tar", last modified: Wed Aug  9 00:24:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.953.tar` & `tencentcloud-sdk-python-ess-3.0.954.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    68335 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   479921 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    68336 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24653 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   480093 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud_sdk_python_ess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-09 00:24:58.000000 tencentcloud-sdk-python-ess-3.0.954/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.953/setup.py` & `tencentcloud-sdk-python-ess-3.0.954/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ess',
-    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.954"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ess SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ess-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.954/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -966,15 +966,15 @@
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowBriefs(self, request):
         """查询流程基础信息
         适用场景：可用于主动查询某个合同流程的签署状态信息。可以配合回调通知使用。
-        每个企业限制日调用量限制：10W，当日超过此限制后再调用接口返回错误
+        每个企业限制日调用量限制：100W，当日超过此限制后再调用接口返回错误
 
         :param request: Request instance for DescribeFlowBriefs.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowBriefsRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowBriefsResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # CAM签名/鉴权错误。
 AUTHFAILURE = 'AuthFailure'
 
-# DryRun 操作，代表请求将会是成功的，只是多传了 DryRun 参数。
-DRYRUNOPERATION = 'DryRunOperation'
-
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
-# 实名认证失败。
-FAILEDOPERATION_ACCOUNTVERIFYFAIL = 'FailedOperation.AccountVerifyFail'
-
 # 年龄限制无法使用电子签服务，请联系客服咨询处理。
 FAILEDOPERATION_AGENOTACHIEVENORMALLEGAL = 'FailedOperation.AgeNotAchieveNormalLegal'
 
 # 签署流程已有关联文档，请检查参数修改后重试。
 FAILEDOPERATION_FLOWHASDOCUMENT = 'FailedOperation.FlowHasDocument'
 
 # 流程未找到关联的电子文件信息，请检查操作步骤，检查参数，并在修改后重试。
@@ -235,17 +229,14 @@
 
 # 姓名不正确。
 INVALIDPARAMETER_INVALIDNAME = 'InvalidParameter.InvalidName'
 
 # 参数Offset不正确。
 INVALIDPARAMETER_INVALIDOFFSET = 'InvalidParameter.InvalidOffset'
 
-# OpenId不正确。
-INVALIDPARAMETER_INVALIDOPENID = 'InvalidParameter.InvalidOpenId'
-
 # 操作人ID不正确。
 INVALIDPARAMETER_INVALIDOPERATORID = 'InvalidParameter.InvalidOperatorId'
 
 # 机构ID不正确。
 INVALIDPARAMETER_INVALIDORGANIZATIONID = 'InvalidParameter.InvalidOrganizationId'
 
 # 组织机构名称不正确。
@@ -256,17 +247,14 @@
 
 # 角色名称不正确。
 INVALIDPARAMETER_INVALIDROLENAME = 'InvalidParameter.InvalidRoleName'
 
 # 实名认证渠道不正确。
 INVALIDPARAMETER_INVALIDVERIFYCHANNEL = 'InvalidParameter.InvalidVerifyChannel'
 
-# 验证码不正确。
-INVALIDPARAMETER_INVALIDVERIFYCODE = 'InvalidParameter.InvalidVerifyCode'
-
 # Limit参数超出最大限制
 INVALIDPARAMETER_LIMIT = 'InvalidParameter.Limit'
 
 # 缺少必填控件的值。
 INVALIDPARAMETER_MISSINGREQUIREDCOMPONENTVALUE = 'InvalidParameter.MissingRequiredComponentValue'
 
 # 不合法的手机号，请检查后重试。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.954/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,21 +163,22 @@
         :type ApproverName: str
         :param _ApproverMobile: 签署人的手机号，11位数字
         :type ApproverMobile: str
         :param _OrganizationName: 如果签署方是企业签署方，则为企业名
         :type OrganizationName: str
         :param _SignComponents: 签署人的签署控件列表
         :type SignComponents: list of Component
-        :param _ApproverIdCardNumber: 签署人的身份证号
-        :type ApproverIdCardNumber: str
-        :param _ApproverIdCardType: 签署人的身份证件类型 
+        :param _ApproverIdCardType: 签署人的证件类型
 ID_CARD 身份证
 HONGKONG_AND_MACAO 港澳居民来往内地通行证
 HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证(格式同居民身份证)
+OTHER_CARD_TYPE 其他（需要使用该类型请先联系运营经理）
         :type ApproverIdCardType: str
+        :param _ApproverIdCardNumber: 签署人证件号（长度不超过18位）	
+        :type ApproverIdCardNumber: str
         :param _NotifyType: 签署通知类型：sms--短信，none--不通知
         :type NotifyType: str
         :param _ApproverRole: 签署人角色类型：1--收款人、2--开具人、3--见证人
         :type ApproverRole: int
         :param _VerifyChannel: 签署意愿确认渠道，默认为WEIXINAPP:人脸识别
         :type VerifyChannel: list of str
         :param _PreReadTime: 合同的强制预览时间：3~300s，未指定则按合同页数计算
@@ -204,16 +205,16 @@
         :type ApproverNeedSignReview: bool
         """
         self._ApproverType = None
         self._ApproverName = None
         self._ApproverMobile = None
         self._OrganizationName = None
         self._SignComponents = None
-        self._ApproverIdCardNumber = None
         self._ApproverIdCardType = None
+        self._ApproverIdCardNumber = None
         self._NotifyType = None
         self._ApproverRole = None
         self._VerifyChannel = None
         self._PreReadTime = None
         self._UserId = None
         self._ApproverSource = None
         self._CustomApproverTag = None
@@ -259,30 +260,30 @@
         return self._SignComponents
 
     @SignComponents.setter
     def SignComponents(self, SignComponents):
         self._SignComponents = SignComponents
 
     @property
-    def ApproverIdCardNumber(self):
-        return self._ApproverIdCardNumber
-
-    @ApproverIdCardNumber.setter
-    def ApproverIdCardNumber(self, ApproverIdCardNumber):
-        self._ApproverIdCardNumber = ApproverIdCardNumber
-
-    @property
     def ApproverIdCardType(self):
         return self._ApproverIdCardType
 
     @ApproverIdCardType.setter
     def ApproverIdCardType(self, ApproverIdCardType):
         self._ApproverIdCardType = ApproverIdCardType
 
     @property
+    def ApproverIdCardNumber(self):
+        return self._ApproverIdCardNumber
+
+    @ApproverIdCardNumber.setter
+    def ApproverIdCardNumber(self, ApproverIdCardNumber):
+        self._ApproverIdCardNumber = ApproverIdCardNumber
+
+    @property
     def NotifyType(self):
         return self._NotifyType
 
     @NotifyType.setter
     def NotifyType(self, NotifyType):
         self._NotifyType = NotifyType
 
@@ -374,16 +375,16 @@
         self._OrganizationName = params.get("OrganizationName")
         if params.get("SignComponents") is not None:
             self._SignComponents = []
             for item in params.get("SignComponents"):
                 obj = Component()
                 obj._deserialize(item)
                 self._SignComponents.append(obj)
-        self._ApproverIdCardNumber = params.get("ApproverIdCardNumber")
         self._ApproverIdCardType = params.get("ApproverIdCardType")
+        self._ApproverIdCardNumber = params.get("ApproverIdCardNumber")
         self._NotifyType = params.get("NotifyType")
         self._ApproverRole = params.get("ApproverRole")
         self._VerifyChannel = params.get("VerifyChannel")
         self._PreReadTime = params.get("PreReadTime")
         self._UserId = params.get("UserId")
         self._ApproverSource = params.get("ApproverSource")
         self._CustomApproverTag = params.get("CustomApproverTag")
@@ -10721,19 +10722,21 @@
         :param _ApproverName: 签署方经办人姓名
 <br/>在未指定签署人电子签UserId情况下，为必填参数
         :type ApproverName: str
         :param _ApproverMobile: 签署方经办人手机号码
 <br/>在未指定签署人电子签UserId情况下，为必填参数
 
         :type ApproverMobile: str
-        :param _ApproverIdCardType: 签署方经办人证件类型ID_CARD 身份证
+        :param _ApproverIdCardType: 签署人的证件类型
+ID_CARD 身份证
 HONGKONG_AND_MACAO 港澳居民来往内地通行证
 HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证(格式同居民身份证)
+OTHER_CARD_TYPE 其他（需要使用该类型请先联系运营经理）
         :type ApproverIdCardType: str
-        :param _ApproverIdCardNumber: 签署方经办人证件号码
+        :param _ApproverIdCardNumber: 签署人证件号（长度不超过18位）	
         :type ApproverIdCardNumber: str
         :param _RecipientId: 签署方经办人在模板中的参与方ID
 <br/>模板发起合同时，该参数为必填项
 <br/>文件发起合同是，该参数无序传值
 
         :type RecipientId: str
         :param _VerifyChannel: 签署意愿确认渠道,WEIXINAPP:人脸识别
```

### Comparing `tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.954/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.954/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.953/README.rst` & `tencentcloud-sdk-python-ess-3.0.954/README.rst`

 * *Files identical despite different names*

