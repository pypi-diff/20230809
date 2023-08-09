# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.953.tar", last modified: Tue Aug  8 00:29:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.954.tar", last modified: Wed Aug  9 00:29:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.953.tar` & `tencentcloud-sdk-python-ocr-3.0.954.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   113621 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   807406 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud_sdk_python_ocr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   110398 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   778064 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud_sdk_python_ocr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-09 00:29:41.000000 tencentcloud-sdk-python-ocr-3.0.954/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.953/setup.py` & `tencentcloud-sdk-python-ocr-3.0.954/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ocr',
-    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.954"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ocr SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 
 # 身份证CardSide类型错误
 FAILEDOPERATION_CARDSIDEERROR = 'FailedOperation.CardSideError'
 
 # 今日次数达到限制。
 FAILEDOPERATION_COUNTLIMITERROR = 'FailedOperation.CountLimitError'
 
-# 数据源查询失败。
-FAILEDOPERATION_DATASOURCEQUERYFAILED = 'FailedOperation.DataSourceQueryFailed'
-
 # 数据库异常。
 FAILEDOPERATION_DBERROR = 'FailedOperation.DbError'
 
 # 检测失败。
 FAILEDOPERATION_DETECTFAILED = 'FailedOperation.DetectFailed'
 
 # 文件下载失败。
@@ -94,17 +91,14 @@
 
 # 非护照。
 FAILEDOPERATION_NOPASSPORT = 'FailedOperation.NoPassport'
 
 # OCR识别失败。
 FAILEDOPERATION_OCRFAILED = 'FailedOperation.OcrFailed'
 
-# 查询无记录。
-FAILEDOPERATION_QUERYNORECORD = 'FailedOperation.QueryNoRecord'
-
 # 未知错误。
 FAILEDOPERATION_UNKNOWERROR = 'FailedOperation.UnKnowError'
 
 # 服务未开通。
 FAILEDOPERATION_UNOPENERROR = 'FailedOperation.UnOpenError'
 
 # 剩余识别次数不足，请检查资源包状态。
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2342,70 +2342,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def VerifyBasicBizLicense(self, request):
-        """库源服务调整，该接口在2023年6月1日将正式下线。
-
-        本接口支持营业执照信息的识别与准确性核验。
-
-        您可以通过输入营业执照注册号或营业执照图片（若两者都输入则只用注册号做查询）进行核验，接口返回查询到的工商照面信息，并比对要校验的字段与查询结果的一致性。查询到工商信息包括：统一社会信用代码、经营期限、法人姓名、经营状态、经营业务范围、注册资本等。
-
-        :param request: Request instance for VerifyBasicBizLicense.
-        :type request: :class:`tencentcloud.ocr.v20181119.models.VerifyBasicBizLicenseRequest`
-        :rtype: :class:`tencentcloud.ocr.v20181119.models.VerifyBasicBizLicenseResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("VerifyBasicBizLicense", params, headers=headers)
-            response = json.loads(body)
-            model = models.VerifyBasicBizLicenseResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
-    def VerifyBizLicense(self, request):
-        """库源服务调整，该接口在2023年6月1日将正式下线。
-
-        本接口支持营业执照信息的识别与准确性核验，返回的真实工商照面信息比营业执照识别及核验（基础版）接口更详细。
-
-        您可以输入营业执照注册号或营业执照图片（若两者都输入则只用注册号做查询），接口返回查询到的工商照面信息，并比对要校验的字段与查询结果的一致性。
-
-        查询到工商信息包括：统一社会信用代码、组织机构代码、经营期限、法人姓名、经营状态、经营业务范围及方式、注册资金、注册币种、登记机关、开业日期、企业（机构）类型、注销日期、吊销日期、许可经营项目、一般经营项目、核准时间、省、地级市、区/县、住所所在行政区划代码、行业门类代码、行业门类名称、国民经济行业代码、国民经济行业名称、经营（业务）范围等。
-
-        :param request: Request instance for VerifyBizLicense.
-        :type request: :class:`tencentcloud.ocr.v20181119.models.VerifyBizLicenseRequest`
-        :rtype: :class:`tencentcloud.ocr.v20181119.models.VerifyBizLicenseResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("VerifyBizLicense", params, headers=headers)
-            response = json.loads(body)
-            model = models.VerifyBizLicenseResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def VerifyOfdVatInvoiceOCR(self, request):
         """本接口支持OFD格式的增值税电子普通发票和增值税电子专用发票的识别，返回发票代码、发票号码、开票日期、验证码、机器编号、密码区，购买方和销售方信息，包括名称、纳税人识别号、地址电话、开户行及账号，以及价税合计、开票人、收款人、复核人、税额、不含税金额等字段信息。
 
         :param request: Request instance for VerifyOfdVatInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.VerifyOfdVatInvoiceOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.VerifyOfdVatInvoiceOCRResponse`
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.953/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.954/tencentcloud/ocr/v20181119/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1378,76 +1378,14 @@
         self._RecognizeWarnCode = params.get("RecognizeWarnCode")
         self._RecognizeWarnMsg = params.get("RecognizeWarnMsg")
         self._IsDuplication = params.get("IsDuplication")
         self._RegistrationDate = params.get("RegistrationDate")
         self._RequestId = params.get("RequestId")
 
 
-class BizLicenseVerifyResult(AbstractModel):
-    """验真接口
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RegNum: “0“：一致
-“-1”：不一致
-        :type RegNum: str
-        :param _Name: “0“：一致
-“-1”：不一致
-“”：不验真
-        :type Name: str
-        :param _Address: “0“：一致
-“-1”：不一致
-“”：不验真
-        :type Address: str
-        """
-        self._RegNum = None
-        self._Name = None
-        self._Address = None
-
-    @property
-    def RegNum(self):
-        return self._RegNum
-
-    @RegNum.setter
-    def RegNum(self, RegNum):
-        self._RegNum = RegNum
-
-    @property
-    def Name(self):
-        return self._Name
-
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
-
-    @property
-    def Address(self):
-        return self._Address
-
-    @Address.setter
-    def Address(self, Address):
-        self._Address = Address
-
-
-    def _deserialize(self, params):
-        self._RegNum = params.get("RegNum")
-        self._Name = params.get("Name")
-        self._Address = params.get("Address")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class BusInvoice(AbstractModel):
     """汽车票
 
     """
 
     def __init__(self):
         r"""
@@ -25207,922 +25145,14 @@
             for item in params.get("VehicleRegCertInfos"):
                 obj = VehicleRegCertInfo()
                 obj._deserialize(item)
                 self._VehicleRegCertInfos.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class VerifyBasicBizLicenseRequest(AbstractModel):
-    """VerifyBasicBizLicense请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ImageBase64: 用于入参是营业执照图片的场景，ImageBase64和ImageUrl必须提供一个，如果都提供，只使用 ImageUrl。
-支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
-支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
-        :type ImageBase64: str
-        :param _ImageUrl: 用于入参是营业执照图片的场景，ImageBase64和ImageUrl必须提供一个，如果都提供，只使用 ImageUrl。
-支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
-支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
-        :type ImageUrl: str
-        :param _ImageConfig: 用于入参是营业执照图片的场景，表示需要校验的参数：RegNum（注册号或者统一社会信用代码），Name（企业名称），Address（经营地址）。选择后会返回相关参数校验结果。RegNum为必选，Name和Address可选。
-格式为{RegNum: true, Name:true/false, Address:true/false}
-
-设置方式参考：
-Config = Json.stringify({"Name":true,"Address":true})
-API 3.0 Explorer 设置方式参考：
-Config = {"Name":true,"Address":true}
-        :type ImageConfig: str
-        :param _RegNum: 用于入参是文本的场景，RegNum表示注册号或者统一社会信用代码。若没有传入营业执照图片，则RegNum为必选项，若图片和RegNum都传入，则只使用RegNum。
-        :type RegNum: str
-        :param _Name: 用于入参是文本的场景，Name表示企业名称。Name为可选项，填写后会返回Name的校验结果。
-        :type Name: str
-        :param _Address: 用于入参是文本的场景，Address表示经营地址。Address为可选项，填写后会返回Address的校验结果。
-        :type Address: str
-        :param _RegCapital: 1表示输出注册资本字段（单位：万元），其他值表示不输出。默认不输出。
-        :type RegCapital: int
-        :param _EstablishTime: true表示展示成立/注册日期
-        :type EstablishTime: bool
-        """
-        self._ImageBase64 = None
-        self._ImageUrl = None
-        self._ImageConfig = None
-        self._RegNum = None
-        self._Name = None
-        self._Address = None
-        self._RegCapital = None
-        self._EstablishTime = None
-
-    @property
-    def ImageBase64(self):
-        return self._ImageBase64
-
-    @ImageBase64.setter
-    def ImageBase64(self, ImageBase64):
-        self._ImageBase64 = ImageBase64
-
-    @property
-    def ImageUrl(self):
-        return self._ImageUrl
-
-    @ImageUrl.setter
-    def ImageUrl(self, ImageUrl):
-        self._ImageUrl = ImageUrl
-
-    @property
-    def ImageConfig(self):
-        return self._ImageConfig
-
-    @ImageConfig.setter
-    def ImageConfig(self, ImageConfig):
-        self._ImageConfig = ImageConfig
-
-    @property
-    def RegNum(self):
-        return self._RegNum
-
-    @RegNum.setter
-    def RegNum(self, RegNum):
-        self._RegNum = RegNum
-
-    @property
-    def Name(self):
-        return self._Name
-
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
-
-    @property
-    def Address(self):
-        return self._Address
-
-    @Address.setter
-    def Address(self, Address):
-        self._Address = Address
-
-    @property
-    def RegCapital(self):
-        return self._RegCapital
-
-    @RegCapital.setter
-    def RegCapital(self, RegCapital):
-        self._RegCapital = RegCapital
-
-    @property
-    def EstablishTime(self):
-        return self._EstablishTime
-
-    @EstablishTime.setter
-    def EstablishTime(self, EstablishTime):
-        self._EstablishTime = EstablishTime
-
-
-    def _deserialize(self, params):
-        self._ImageBase64 = params.get("ImageBase64")
-        self._ImageUrl = params.get("ImageUrl")
-        self._ImageConfig = params.get("ImageConfig")
-        self._RegNum = params.get("RegNum")
-        self._Name = params.get("Name")
-        self._Address = params.get("Address")
-        self._RegCapital = params.get("RegCapital")
-        self._EstablishTime = params.get("EstablishTime")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class VerifyBasicBizLicenseResponse(AbstractModel):
-    """VerifyBasicBizLicense返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ErrorCode: 状态码，成功时返回0
-        :type ErrorCode: int
-        :param _CreditCode: 统一社会信用代码
-        :type CreditCode: str
-        :param _Opfrom: 经营期限自（YYYY-MM-DD）
-        :type Opfrom: str
-        :param _Opto: 经营期限至（YYYY-MM-DD）
-        :type Opto: str
-        :param _Frname: 法人姓名
-        :type Frname: str
-        :param _Entstatus: 经营状态，包括：成立、筹建、存续、在营、开业、在册、正常经营、开业登记中、登记成立、撤销、撤销登记、非正常户、告解、个体暂时吊销、个体转企业、吊销（未注销）、拟注销、已注销、（待）迁入、（待）迁出、停业、歇业、清算等。
-        :type Entstatus: str
-        :param _Zsopscope: 经营业务范围
-        :type Zsopscope: str
-        :param _Reason: 查询的状态信息
-        :type Reason: str
-        :param _Oriregno: 原注册号
-        :type Oriregno: str
-        :param _VerifyRegno: 要核验的工商注册号
-        :type VerifyRegno: str
-        :param _Regno: 工商注册号
-        :type Regno: str
-        :param _VerifyEntname: 要核验的企业名称
-        :type VerifyEntname: str
-        :param _Entname: 企业名称
-        :type Entname: str
-        :param _VerifyDom: 要核验的住址
-        :type VerifyDom: str
-        :param _Dom: 住址
-        :type Dom: str
-        :param _RegNumResult: 验证结果
-        :type RegNumResult: :class:`tencentcloud.ocr.v20181119.models.BizLicenseVerifyResult`
-        :param _RegCapital: 注册资本（单位：万元）,只有输入参数regCapital为1的时候才输出
-        :type RegCapital: str
-        :param _EstablishTime: 成立/注册日期，只有输入参数EstablishTime为true时展示，默认为空
-        :type EstablishTime: str
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._ErrorCode = None
-        self._CreditCode = None
-        self._Opfrom = None
-        self._Opto = None
-        self._Frname = None
-        self._Entstatus = None
-        self._Zsopscope = None
-        self._Reason = None
-        self._Oriregno = None
-        self._VerifyRegno = None
-        self._Regno = None
-        self._VerifyEntname = None
-        self._Entname = None
-        self._VerifyDom = None
-        self._Dom = None
-        self._RegNumResult = None
-        self._RegCapital = None
-        self._EstablishTime = None
-        self._RequestId = None
-
-    @property
-    def ErrorCode(self):
-        return self._ErrorCode
-
-    @ErrorCode.setter
-    def ErrorCode(self, ErrorCode):
-        self._ErrorCode = ErrorCode
-
-    @property
-    def CreditCode(self):
-        return self._CreditCode
-
-    @CreditCode.setter
-    def CreditCode(self, CreditCode):
-        self._CreditCode = CreditCode
-
-    @property
-    def Opfrom(self):
-        return self._Opfrom
-
-    @Opfrom.setter
-    def Opfrom(self, Opfrom):
-        self._Opfrom = Opfrom
-
-    @property
-    def Opto(self):
-        return self._Opto
-
-    @Opto.setter
-    def Opto(self, Opto):
-        self._Opto = Opto
-
-    @property
-    def Frname(self):
-        return self._Frname
-
-    @Frname.setter
-    def Frname(self, Frname):
-        self._Frname = Frname
-
-    @property
-    def Entstatus(self):
-        return self._Entstatus
-
-    @Entstatus.setter
-    def Entstatus(self, Entstatus):
-        self._Entstatus = Entstatus
-
-    @property
-    def Zsopscope(self):
-        return self._Zsopscope
-
-    @Zsopscope.setter
-    def Zsopscope(self, Zsopscope):
-        self._Zsopscope = Zsopscope
-
-    @property
-    def Reason(self):
-        return self._Reason
-
-    @Reason.setter
-    def Reason(self, Reason):
-        self._Reason = Reason
-
-    @property
-    def Oriregno(self):
-        return self._Oriregno
-
-    @Oriregno.setter
-    def Oriregno(self, Oriregno):
-        self._Oriregno = Oriregno
-
-    @property
-    def VerifyRegno(self):
-        return self._VerifyRegno
-
-    @VerifyRegno.setter
-    def VerifyRegno(self, VerifyRegno):
-        self._VerifyRegno = VerifyRegno
-
-    @property
-    def Regno(self):
-        return self._Regno
-
-    @Regno.setter
-    def Regno(self, Regno):
-        self._Regno = Regno
-
-    @property
-    def VerifyEntname(self):
-        return self._VerifyEntname
-
-    @VerifyEntname.setter
-    def VerifyEntname(self, VerifyEntname):
-        self._VerifyEntname = VerifyEntname
-
-    @property
-    def Entname(self):
-        return self._Entname
-
-    @Entname.setter
-    def Entname(self, Entname):
-        self._Entname = Entname
-
-    @property
-    def VerifyDom(self):
-        return self._VerifyDom
-
-    @VerifyDom.setter
-    def VerifyDom(self, VerifyDom):
-        self._VerifyDom = VerifyDom
-
-    @property
-    def Dom(self):
-        return self._Dom
-
-    @Dom.setter
-    def Dom(self, Dom):
-        self._Dom = Dom
-
-    @property
-    def RegNumResult(self):
-        return self._RegNumResult
-
-    @RegNumResult.setter
-    def RegNumResult(self, RegNumResult):
-        self._RegNumResult = RegNumResult
-
-    @property
-    def RegCapital(self):
-        return self._RegCapital
-
-    @RegCapital.setter
-    def RegCapital(self, RegCapital):
-        self._RegCapital = RegCapital
-
-    @property
-    def EstablishTime(self):
-        return self._EstablishTime
-
-    @EstablishTime.setter
-    def EstablishTime(self, EstablishTime):
-        self._EstablishTime = EstablishTime
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._ErrorCode = params.get("ErrorCode")
-        self._CreditCode = params.get("CreditCode")
-        self._Opfrom = params.get("Opfrom")
-        self._Opto = params.get("Opto")
-        self._Frname = params.get("Frname")
-        self._Entstatus = params.get("Entstatus")
-        self._Zsopscope = params.get("Zsopscope")
-        self._Reason = params.get("Reason")
-        self._Oriregno = params.get("Oriregno")
-        self._VerifyRegno = params.get("VerifyRegno")
-        self._Regno = params.get("Regno")
-        self._VerifyEntname = params.get("VerifyEntname")
-        self._Entname = params.get("Entname")
-        self._VerifyDom = params.get("VerifyDom")
-        self._Dom = params.get("Dom")
-        if params.get("RegNumResult") is not None:
-            self._RegNumResult = BizLicenseVerifyResult()
-            self._RegNumResult._deserialize(params.get("RegNumResult"))
-        self._RegCapital = params.get("RegCapital")
-        self._EstablishTime = params.get("EstablishTime")
-        self._RequestId = params.get("RequestId")
-
-
-class VerifyBizLicenseRequest(AbstractModel):
-    """VerifyBizLicense请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ImageBase64: 用于入参是营业执照图片的场景，ImageBase64和ImageUrl必须提供一个，如果都提供，只使用 ImageUrl。
-支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
-支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
-        :type ImageBase64: str
-        :param _ImageUrl: 用于入参是营业执照图片的场景，ImageBase64和ImageUrl必须提供一个，如果都提供，只使用 ImageUrl。
-支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。
-支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。
-        :type ImageUrl: str
-        :param _ImageConfig: 用于入参是营业执照图片的场景，表示需要校验的参数：RegNum（注册号或者统一社会信用代码），Name（企业名称），Address（经营地址）。选择后会返回相关参数校验结果。RegNum为必选，Name和Address可选。
-格式为{RegNum: true, Name:true/false, Address:true/false}
-
-设置方式参考：
-Config = Json.stringify({"Name":true,"Address":true})
-API 3.0 Explorer 设置方式参考：
-Config = {"Name":true,"Address":true}
-        :type ImageConfig: str
-        :param _RegNum: 用于入参是文本的场景，RegNum表示注册号或者统一社会信用代码。若没有传入营业执照图片，则RegNum为必选项，若图片和RegNum都传入，则只使用RegNum。
-        :type RegNum: str
-        :param _Name: 用于入参是文本的场景，Name表示企业名称。Name为可选项，填写后会返回Name的校验结果。
-        :type Name: str
-        :param _Address: 用于入参是文本的场景，Address表示经营地址，填写后会返回Address的校验结果。
-        :type Address: str
-        """
-        self._ImageBase64 = None
-        self._ImageUrl = None
-        self._ImageConfig = None
-        self._RegNum = None
-        self._Name = None
-        self._Address = None
-
-    @property
-    def ImageBase64(self):
-        return self._ImageBase64
-
-    @ImageBase64.setter
-    def ImageBase64(self, ImageBase64):
-        self._ImageBase64 = ImageBase64
-
-    @property
-    def ImageUrl(self):
-        return self._ImageUrl
-
-    @ImageUrl.setter
-    def ImageUrl(self, ImageUrl):
-        self._ImageUrl = ImageUrl
-
-    @property
-    def ImageConfig(self):
-        return self._ImageConfig
-
-    @ImageConfig.setter
-    def ImageConfig(self, ImageConfig):
-        self._ImageConfig = ImageConfig
-
-    @property
-    def RegNum(self):
-        return self._RegNum
-
-    @RegNum.setter
-    def RegNum(self, RegNum):
-        self._RegNum = RegNum
-
-    @property
-    def Name(self):
-        return self._Name
-
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
-
-    @property
-    def Address(self):
-        return self._Address
-
-    @Address.setter
-    def Address(self, Address):
-        self._Address = Address
-
-
-    def _deserialize(self, params):
-        self._ImageBase64 = params.get("ImageBase64")
-        self._ImageUrl = params.get("ImageUrl")
-        self._ImageConfig = params.get("ImageConfig")
-        self._RegNum = params.get("RegNum")
-        self._Name = params.get("Name")
-        self._Address = params.get("Address")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class VerifyBizLicenseResponse(AbstractModel):
-    """VerifyBizLicense返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ErrorCode: 状态码
-        :type ErrorCode: int
-        :param _CreditCode: 统一社会信用代码
-        :type CreditCode: str
-        :param _OrgCode: 组织机构代码
-        :type OrgCode: str
-        :param _OpenFrom: 经营期限自（YYYY-MM-DD）
-        :type OpenFrom: str
-        :param _OpenTo: 经营期限至（YYYY-MM-DD）
-        :type OpenTo: str
-        :param _FrName: 法人姓名
-        :type FrName: str
-        :param _EnterpriseStatus: 经营状态，包括：成立、筹建、存续、在营、开业、在册、正常经营、开业登记中、登记成立、撤销、撤销登记、非正常户、告解、个体暂时吊销、个体转企业、吊销（未注销）、拟注销、已注销、（待）迁入、（待）迁出、停业、歇业、清算等。
-        :type EnterpriseStatus: str
-        :param _OperateScopeAndForm: 经营（业务）范围及方式
-        :type OperateScopeAndForm: str
-        :param _RegCap: 注册资金（单位:万元）
-        :type RegCap: str
-        :param _RegCapCur: 注册币种
-        :type RegCapCur: str
-        :param _RegOrg: 登记机关
-        :type RegOrg: str
-        :param _EsDate: 开业日期（YYYY-MM-DD）
-        :type EsDate: str
-        :param _EnterpriseType: 企业（机构）类型
-        :type EnterpriseType: str
-        :param _CancelDate: 注销日期
-        :type CancelDate: str
-        :param _RevokeDate: 吊销日期
-        :type RevokeDate: str
-        :param _AbuItem: 许可经营项目
-        :type AbuItem: str
-        :param _CbuItem: 一般经营项目
-        :type CbuItem: str
-        :param _ApprDate: 核准时间
-        :type ApprDate: str
-        :param _Province: 省（返回空值）
-        :type Province: str
-        :param _City: 地级市（返回空值）
-        :type City: str
-        :param _County: 区\县（返回空值）
-        :type County: str
-        :param _AreaCode: 住所所在行政区划代码（返回空值）
-        :type AreaCode: str
-        :param _IndustryPhyCode: 行业门类代码（返回空值）
-        :type IndustryPhyCode: str
-        :param _IndustryPhyName: 行业门类名称（返回空值）
-        :type IndustryPhyName: str
-        :param _IndustryCode: 国民经济行业代码（返回空值）
-        :type IndustryCode: str
-        :param _IndustryName: 国民经济行业名称（返回空值）
-        :type IndustryName: str
-        :param _OperateScope: 经营（业务）范围
-        :type OperateScope: str
-        :param _VerifyRegNo: 要核验的工商注册号
-        :type VerifyRegNo: str
-        :param _RegNo: 工商注册号
-        :type RegNo: str
-        :param _VerifyEnterpriseName: 要核验的企业名称
-        :type VerifyEnterpriseName: str
-        :param _EnterpriseName: 企业名称
-        :type EnterpriseName: str
-        :param _VerifyAddress: 要核验的注册地址
-        :type VerifyAddress: str
-        :param _Address: 注册地址
-        :type Address: str
-        :param _RegNumResult: 验证结果
-        :type RegNumResult: :class:`tencentcloud.ocr.v20181119.models.BizLicenseVerifyResult`
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._ErrorCode = None
-        self._CreditCode = None
-        self._OrgCode = None
-        self._OpenFrom = None
-        self._OpenTo = None
-        self._FrName = None
-        self._EnterpriseStatus = None
-        self._OperateScopeAndForm = None
-        self._RegCap = None
-        self._RegCapCur = None
-        self._RegOrg = None
-        self._EsDate = None
-        self._EnterpriseType = None
-        self._CancelDate = None
-        self._RevokeDate = None
-        self._AbuItem = None
-        self._CbuItem = None
-        self._ApprDate = None
-        self._Province = None
-        self._City = None
-        self._County = None
-        self._AreaCode = None
-        self._IndustryPhyCode = None
-        self._IndustryPhyName = None
-        self._IndustryCode = None
-        self._IndustryName = None
-        self._OperateScope = None
-        self._VerifyRegNo = None
-        self._RegNo = None
-        self._VerifyEnterpriseName = None
-        self._EnterpriseName = None
-        self._VerifyAddress = None
-        self._Address = None
-        self._RegNumResult = None
-        self._RequestId = None
-
-    @property
-    def ErrorCode(self):
-        return self._ErrorCode
-
-    @ErrorCode.setter
-    def ErrorCode(self, ErrorCode):
-        self._ErrorCode = ErrorCode
-
-    @property
-    def CreditCode(self):
-        return self._CreditCode
-
-    @CreditCode.setter
-    def CreditCode(self, CreditCode):
-        self._CreditCode = CreditCode
-
-    @property
-    def OrgCode(self):
-        return self._OrgCode
-
-    @OrgCode.setter
-    def OrgCode(self, OrgCode):
-        self._OrgCode = OrgCode
-
-    @property
-    def OpenFrom(self):
-        return self._OpenFrom
-
-    @OpenFrom.setter
-    def OpenFrom(self, OpenFrom):
-        self._OpenFrom = OpenFrom
-
-    @property
-    def OpenTo(self):
-        return self._OpenTo
-
-    @OpenTo.setter
-    def OpenTo(self, OpenTo):
-        self._OpenTo = OpenTo
-
-    @property
-    def FrName(self):
-        return self._FrName
-
-    @FrName.setter
-    def FrName(self, FrName):
-        self._FrName = FrName
-
-    @property
-    def EnterpriseStatus(self):
-        return self._EnterpriseStatus
-
-    @EnterpriseStatus.setter
-    def EnterpriseStatus(self, EnterpriseStatus):
-        self._EnterpriseStatus = EnterpriseStatus
-
-    @property
-    def OperateScopeAndForm(self):
-        return self._OperateScopeAndForm
-
-    @OperateScopeAndForm.setter
-    def OperateScopeAndForm(self, OperateScopeAndForm):
-        self._OperateScopeAndForm = OperateScopeAndForm
-
-    @property
-    def RegCap(self):
-        return self._RegCap
-
-    @RegCap.setter
-    def RegCap(self, RegCap):
-        self._RegCap = RegCap
-
-    @property
-    def RegCapCur(self):
-        return self._RegCapCur
-
-    @RegCapCur.setter
-    def RegCapCur(self, RegCapCur):
-        self._RegCapCur = RegCapCur
-
-    @property
-    def RegOrg(self):
-        return self._RegOrg
-
-    @RegOrg.setter
-    def RegOrg(self, RegOrg):
-        self._RegOrg = RegOrg
-
-    @property
-    def EsDate(self):
-        return self._EsDate
-
-    @EsDate.setter
-    def EsDate(self, EsDate):
-        self._EsDate = EsDate
-
-    @property
-    def EnterpriseType(self):
-        return self._EnterpriseType
-
-    @EnterpriseType.setter
-    def EnterpriseType(self, EnterpriseType):
-        self._EnterpriseType = EnterpriseType
-
-    @property
-    def CancelDate(self):
-        return self._CancelDate
-
-    @CancelDate.setter
-    def CancelDate(self, CancelDate):
-        self._CancelDate = CancelDate
-
-    @property
-    def RevokeDate(self):
-        return self._RevokeDate
-
-    @RevokeDate.setter
-    def RevokeDate(self, RevokeDate):
-        self._RevokeDate = RevokeDate
-
-    @property
-    def AbuItem(self):
-        return self._AbuItem
-
-    @AbuItem.setter
-    def AbuItem(self, AbuItem):
-        self._AbuItem = AbuItem
-
-    @property
-    def CbuItem(self):
-        return self._CbuItem
-
-    @CbuItem.setter
-    def CbuItem(self, CbuItem):
-        self._CbuItem = CbuItem
-
-    @property
-    def ApprDate(self):
-        return self._ApprDate
-
-    @ApprDate.setter
-    def ApprDate(self, ApprDate):
-        self._ApprDate = ApprDate
-
-    @property
-    def Province(self):
-        return self._Province
-
-    @Province.setter
-    def Province(self, Province):
-        self._Province = Province
-
-    @property
-    def City(self):
-        return self._City
-
-    @City.setter
-    def City(self, City):
-        self._City = City
-
-    @property
-    def County(self):
-        return self._County
-
-    @County.setter
-    def County(self, County):
-        self._County = County
-
-    @property
-    def AreaCode(self):
-        return self._AreaCode
-
-    @AreaCode.setter
-    def AreaCode(self, AreaCode):
-        self._AreaCode = AreaCode
-
-    @property
-    def IndustryPhyCode(self):
-        return self._IndustryPhyCode
-
-    @IndustryPhyCode.setter
-    def IndustryPhyCode(self, IndustryPhyCode):
-        self._IndustryPhyCode = IndustryPhyCode
-
-    @property
-    def IndustryPhyName(self):
-        return self._IndustryPhyName
-
-    @IndustryPhyName.setter
-    def IndustryPhyName(self, IndustryPhyName):
-        self._IndustryPhyName = IndustryPhyName
-
-    @property
-    def IndustryCode(self):
-        return self._IndustryCode
-
-    @IndustryCode.setter
-    def IndustryCode(self, IndustryCode):
-        self._IndustryCode = IndustryCode
-
-    @property
-    def IndustryName(self):
-        return self._IndustryName
-
-    @IndustryName.setter
-    def IndustryName(self, IndustryName):
-        self._IndustryName = IndustryName
-
-    @property
-    def OperateScope(self):
-        return self._OperateScope
-
-    @OperateScope.setter
-    def OperateScope(self, OperateScope):
-        self._OperateScope = OperateScope
-
-    @property
-    def VerifyRegNo(self):
-        return self._VerifyRegNo
-
-    @VerifyRegNo.setter
-    def VerifyRegNo(self, VerifyRegNo):
-        self._VerifyRegNo = VerifyRegNo
-
-    @property
-    def RegNo(self):
-        return self._RegNo
-
-    @RegNo.setter
-    def RegNo(self, RegNo):
-        self._RegNo = RegNo
-
-    @property
-    def VerifyEnterpriseName(self):
-        return self._VerifyEnterpriseName
-
-    @VerifyEnterpriseName.setter
-    def VerifyEnterpriseName(self, VerifyEnterpriseName):
-        self._VerifyEnterpriseName = VerifyEnterpriseName
-
-    @property
-    def EnterpriseName(self):
-        return self._EnterpriseName
-
-    @EnterpriseName.setter
-    def EnterpriseName(self, EnterpriseName):
-        self._EnterpriseName = EnterpriseName
-
-    @property
-    def VerifyAddress(self):
-        return self._VerifyAddress
-
-    @VerifyAddress.setter
-    def VerifyAddress(self, VerifyAddress):
-        self._VerifyAddress = VerifyAddress
-
-    @property
-    def Address(self):
-        return self._Address
-
-    @Address.setter
-    def Address(self, Address):
-        self._Address = Address
-
-    @property
-    def RegNumResult(self):
-        return self._RegNumResult
-
-    @RegNumResult.setter
-    def RegNumResult(self, RegNumResult):
-        self._RegNumResult = RegNumResult
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._ErrorCode = params.get("ErrorCode")
-        self._CreditCode = params.get("CreditCode")
-        self._OrgCode = params.get("OrgCode")
-        self._OpenFrom = params.get("OpenFrom")
-        self._OpenTo = params.get("OpenTo")
-        self._FrName = params.get("FrName")
-        self._EnterpriseStatus = params.get("EnterpriseStatus")
-        self._OperateScopeAndForm = params.get("OperateScopeAndForm")
-        self._RegCap = params.get("RegCap")
-        self._RegCapCur = params.get("RegCapCur")
-        self._RegOrg = params.get("RegOrg")
-        self._EsDate = params.get("EsDate")
-        self._EnterpriseType = params.get("EnterpriseType")
-        self._CancelDate = params.get("CancelDate")
-        self._RevokeDate = params.get("RevokeDate")
-        self._AbuItem = params.get("AbuItem")
-        self._CbuItem = params.get("CbuItem")
-        self._ApprDate = params.get("ApprDate")
-        self._Province = params.get("Province")
-        self._City = params.get("City")
-        self._County = params.get("County")
-        self._AreaCode = params.get("AreaCode")
-        self._IndustryPhyCode = params.get("IndustryPhyCode")
-        self._IndustryPhyName = params.get("IndustryPhyName")
-        self._IndustryCode = params.get("IndustryCode")
-        self._IndustryName = params.get("IndustryName")
-        self._OperateScope = params.get("OperateScope")
-        self._VerifyRegNo = params.get("VerifyRegNo")
-        self._RegNo = params.get("RegNo")
-        self._VerifyEnterpriseName = params.get("VerifyEnterpriseName")
-        self._EnterpriseName = params.get("EnterpriseName")
-        self._VerifyAddress = params.get("VerifyAddress")
-        self._Address = params.get("Address")
-        if params.get("RegNumResult") is not None:
-            self._RegNumResult = BizLicenseVerifyResult()
-            self._RegNumResult._deserialize(params.get("RegNumResult"))
-        self._RequestId = params.get("RequestId")
-
-
 class VerifyOfdVatInvoiceOCRRequest(AbstractModel):
     """VerifyOfdVatInvoiceOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.953/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.954/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.954/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.953/README.rst` & `tencentcloud-sdk-python-ocr-3.0.954/README.rst`

 * *Files identical despite different names*

