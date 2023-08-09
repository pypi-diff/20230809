# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.953.tar", last modified: Tue Aug  8 00:24:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.954.tar", last modified: Wed Aug  9 00:25:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.953.tar` & `tencentcloud-sdk-python-essbasic-3.0.954.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    57837 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   394018 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      733 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    57838 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   394117 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      733 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:25:04.000000 tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.954/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-essbasic',
-    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.954"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Essbasic SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1009,15 +1009,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeUsage(self, request):
         """此接口（DescribeUsage）用于获取第三方平台所有合作企业流量消耗情况。
-         注: 此接口每日限频2次，若要扩大限制次数,请提前与客服经理或邮件至e-contract@tencent.com进行联系。
+         注: 此接口每日限频50次，若要扩大限制次数,请提前与客服经理或邮件至e-contract@tencent.com进行联系。
 
         :param request: Request instance for DescribeUsage.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.DescribeUsageRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.DescribeUsageResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7898,20 +7898,21 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Name: 签署人姓名，最大长度50个字符
         :type Name: str
-        :param _IdCardType: 签署人身份证件类型
+        :param _IdCardType: 签署人的证件类型
 1.ID_CARD 居民身份证
 2.HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证
 3.HONGKONG_AND_MACAO 港澳居民来往内地通行证
+4.OTHER_CARD_TYPE 其他（需要使用该类型请先联系运营经理）
         :type IdCardType: str
-        :param _IdCardNumber: 签署人证件号
+        :param _IdCardNumber: 签署人证件号（长度不超过18位）
         :type IdCardNumber: str
         :param _Mobile: 签署人手机号，脱敏显示。大陆手机号为11位，暂不支持海外手机号。
         :type Mobile: str
         :param _OrganizationName: 企业签署方工商营业执照上的企业名称，签署方为非发起方企业场景下必传，最大长度64个字符；
         :type OrganizationName: str
         :param _NotChannelOrganization: 指定签署人非第三方平台子客企业下员工，在ApproverType为ORGANIZATION时指定。
 默认为false，即签署人位于同一个第三方平台应用号下；默认为false，即签署人位于同一个第三方应用号下；
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.954/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.954/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.954/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

