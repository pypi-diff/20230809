# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.952.tar", last modified: Mon Aug  7 08:51:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.953.tar", last modified: Tue Aug  8 00:22:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.952.tar` & `tencentcloud-sdk-python-cwp-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 08:51:00.000000 tencentcloud-sdk-python-cwp-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:51:00.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:51:00.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:51:00.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3900 2023-08-07 08:51:00.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1463419 2023-08-07 08:51:00.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)   253300 2023-08-07 08:51:00.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 08:51:00.000000 tencentcloud-sdk-python-cwp-3.0.952/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud_sdk_python_cwp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:51:01.000000 tencentcloud-sdk-python-cwp-3.0.952/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1463419 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)   253300 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud_sdk_python_cwp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:22:38.000000 tencentcloud-sdk-python-cwp-3.0.953/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.952/setup.py` & `tencentcloud-sdk-python-cwp-3.0.953/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cwp',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cwp SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,7 +123,10 @@
 RESOURCENOTFOUND_MACHINENOTFOUND = 'ResourceNotFound.MachineNotFound'
 
 # 资源不可用。
 RESOURCEUNAVAILABLE = 'ResourceUnavailable'
 
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
+
+# 操作不支持。
+UNSUPPORTEDOPERATION = 'UnsupportedOperation'
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/v20180228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.952/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.953/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.953/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.952/README.rst` & `tencentcloud-sdk-python-cwp-3.0.953/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.952/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.953/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

