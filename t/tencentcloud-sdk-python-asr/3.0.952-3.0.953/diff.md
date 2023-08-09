# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.952.tar", last modified: Mon Aug  7 08:45:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.953.tar", last modified: Tue Aug  8 00:17:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.952.tar` & `tencentcloud-sdk-python-asr-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud_sdk_python_asr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud_sdk_python_asr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29417 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   112189 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 08:45:59.000000 tencentcloud-sdk-python-asr-3.0.952/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud_sdk_python_asr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30297 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   114148 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:17:49.000000 tencentcloud-sdk-python-asr-3.0.953/README.rst
```

### Comparing `tencentcloud-sdk-python-asr-3.0.952/setup.py` & `tencentcloud-sdk-python-asr-3.0.953/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-asr',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Asr SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-asr-3.0.952/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.953/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/v20190614/asr_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,14 +508,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def VoicePrintCount(self, request):
+        """统计并返回注册的说话人id总数
+
+        :param request: Request instance for VoicePrintCount.
+        :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintCountRequest`
+        :rtype: :class:`tencentcloud.asr.v20190614.models.VoicePrintCountResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("VoicePrintCount", params, headers=headers)
+            response = json.loads(body)
+            model = models.VoicePrintCountResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def VoicePrintDelete(self, request):
         """本接口用于以删除已经注册的说话人信息（删除之后，原有的说话人ID和说话人音频数据都会失效）
 
         :param request: Request instance for VoicePrintDelete.
         :type request: :class:`tencentcloud.asr.v20190614.models.VoicePrintDeleteRequest`
         :rtype: :class:`tencentcloud.asr.v20190614.models.VoicePrintDeleteResponse`
```

### Comparing `tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.952/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.953/tencentcloud/asr/v20190614/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3265,14 +3265,93 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class VoicePrintCountData(AbstractModel):
+    """统计返回注册数量结构
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Total: 总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        """
+        self._Total = None
+
+    @property
+    def Total(self):
+        return self._Total
+
+    @Total.setter
+    def Total(self, Total):
+        self._Total = Total
+
+
+    def _deserialize(self, params):
+        self._Total = params.get("Total")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class VoicePrintCountRequest(AbstractModel):
+    """VoicePrintCount请求参数结构体
+
+    """
+
+
+class VoicePrintCountResponse(AbstractModel):
+    """VoicePrintCount返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 统计数据
+        :type Data: :class:`tencentcloud.asr.v20190614.models.VoicePrintCountData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = VoicePrintCountData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
 class VoicePrintDeleteRequest(AbstractModel):
     """VoicePrintDelete请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-asr-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.953/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.952/README.rst` & `tencentcloud-sdk-python-asr-3.0.953/README.rst`

 * *Files identical despite different names*

