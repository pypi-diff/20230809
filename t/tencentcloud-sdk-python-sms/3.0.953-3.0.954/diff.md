# Comparing `tmp/tencentcloud-sdk-python-sms-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-sms-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.953.tar", last modified: Tue Aug  8 00:31:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.954.tar", last modified: Wed Aug  9 00:31:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sms-3.0.953.tar` & `tencentcloud-sdk-python-sms-3.0.954.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20210111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20210111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19342 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20210111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28405 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20210111/sms_client.py
--rw-r--r--   0 root         (0) root         (0)   104651 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20210111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20190711/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20190711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18520 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20190711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26631 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20190711/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    93545 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20190711/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud_sdk_python_sms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      653 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud_sdk_python_sms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/tencentcloud_sdk_python_sms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:31:16.000000 tencentcloud-sdk-python-sms-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20210111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20210111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19342 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20210111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28405 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20210111/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)   104651 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20210111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20190711/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20190711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18520 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20190711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26631 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20190711/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    93545 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20190711/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud_sdk_python_sms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud_sdk_python_sms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/tencentcloud_sdk_python_sms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-09 00:31:14.000000 tencentcloud-sdk-python-sms-3.0.954/README.rst
```

### Comparing `tencentcloud-sdk-python-sms-3.0.953/setup.py` & `tencentcloud-sdk-python-sms-3.0.954/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-sms',
-    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.954"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Sms SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20210111/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20210111/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,36 +139,36 @@
 
 # 请求的短信内容太长，短信长度规则请参考 [国内短信内容长度计算规则](https://cloud.tencent.com/document/product/382/18058)。
 INVALIDPARAMETERVALUE_CONTENTLENGTHLIMIT = 'InvalidParameterValue.ContentLengthLimit'
 
 # 参数 EndTime 校验失败。
 INVALIDPARAMETERVALUE_ENDTIMEVERIFYFAIL = 'InvalidParameterValue.EndTimeVerifyFail'
 
-# 上传的转码图片格式错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# 上传的转码图片格式错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_IMAGEINVALID = 'InvalidParameterValue.ImageInvalid'
 
 # 手机号格式错误。
 INVALIDPARAMETERVALUE_INCORRECTPHONENUMBER = 'InvalidParameterValue.IncorrectPhoneNumber'
 
-# DocumentType 字段校验错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# DocumentType 字段校验错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_INVALIDDOCUMENTTYPE = 'InvalidParameterValue.InvalidDocumentType'
 
-# International 字段校验错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# International 字段校验错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_INVALIDINTERNATIONAL = 'InvalidParameterValue.InvalidInternational'
 
-# SignPurpose 字段校验错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# SignPurpose 字段校验错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_INVALIDSIGNPURPOSE = 'InvalidParameterValue.InvalidSignPurpose'
 
 # 无效的拉取起始/截止时间，具体原因可能是请求的 SendDateTime 大于 EndDateTime。
 INVALIDPARAMETERVALUE_INVALIDSTARTTIME = 'InvalidParameterValue.InvalidStartTime'
 
 # 模板格式错误，请参考[正文模板审核标准](https://cloud.tencent.com/document/product/382/39023)。
 INVALIDPARAMETERVALUE_INVALIDTEMPLATEFORMAT = 'InvalidParameterValue.InvalidTemplateFormat'
 
-# UsedMethod 字段校验错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# UsedMethod 字段校验错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_INVALIDUSEDMETHOD = 'InvalidParameterValue.InvalidUsedMethod'
 
 # 参数 Limit 校验失败。
 INVALIDPARAMETERVALUE_LIMITVERIFYFAIL = 'InvalidParameterValue.LimitVerifyFail'
 
 # 参数 Offset 校验失败。
 INVALIDPARAMETERVALUE_OFFSETVERIFYFAIL = 'InvalidParameterValue.OffsetVerifyFail'
```

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20210111/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20210111/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20210111/models.py` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20210111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20190711/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20190711/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,30 +130,30 @@
 
 # 请求的短信内容太长，短信长度规则请参考 [国内短信内容长度计算规则](https://cloud.tencent.com/document/product/382/18058)。
 INVALIDPARAMETERVALUE_CONTENTLENGTHLIMIT = 'InvalidParameterValue.ContentLengthLimit'
 
 # 参数 EndTime 校验失败。
 INVALIDPARAMETERVALUE_ENDTIMEVERIFYFAIL = 'InvalidParameterValue.EndTimeVerifyFail'
 
-# 上传的转码图片格式错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# 上传的转码图片格式错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_IMAGEINVALID = 'InvalidParameterValue.ImageInvalid'
 
 # 手机号格式错误。
 INVALIDPARAMETERVALUE_INCORRECTPHONENUMBER = 'InvalidParameterValue.IncorrectPhoneNumber'
 
-# DocumentType 字段校验错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# DocumentType 字段校验错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_INVALIDDOCUMENTTYPE = 'InvalidParameterValue.InvalidDocumentType'
 
-# International 字段校验错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# International 字段校验错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_INVALIDINTERNATIONAL = 'InvalidParameterValue.InvalidInternational'
 
 # 无效的拉取起始/截止时间，具体原因可能是请求的 SendDateTime 大于 EndDateTime。
 INVALIDPARAMETERVALUE_INVALIDSTARTTIME = 'InvalidParameterValue.InvalidStartTime'
 
-# UsedMethod 字段校验错误，请参照 API 接口说明中对改字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
+# UsedMethod 字段校验错误，请参照 API 接口说明中对该字段的说明，如有需要请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
 INVALIDPARAMETERVALUE_INVALIDUSEDMETHOD = 'InvalidParameterValue.InvalidUsedMethod'
 
 # 无法识别签名，请确认是否已有签名通过申请，一般是签名未通过申请，可以查看 [签名审核](https://cloud.tencent.com/document/product/382/37745#.E6.AD.A5.E9.AA.A43.EF.BC.9A.E7.AD.89.E5.BE.85.E5.AE.A1.E6.A0.B8) 。
 INVALIDPARAMETERVALUE_MISSINGSIGNATURELIST = 'InvalidParameterValue.MissingSignatureList'
 
 # 禁止在模板变量中使用 URL。
 INVALIDPARAMETERVALUE_PROHIBITEDUSEURLINTEMPLATEPARAMETER = 'InvalidParameterValue.ProhibitedUseUrlInTemplateParameter'
```

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20190711/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20190711/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud/sms/v20190711/models.py` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud/sms/v20190711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.953/tencentcloud_sdk_python_sms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.954/tencentcloud_sdk_python_sms.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.954/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.953/README.rst` & `tencentcloud-sdk-python-sms-3.0.954/README.rst`

 * *Files identical despite different names*

