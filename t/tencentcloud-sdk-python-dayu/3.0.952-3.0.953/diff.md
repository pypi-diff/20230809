# Comparing `tmp/tencentcloud-sdk-python-dayu-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-dayu-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dayu-3.0.952.tar", last modified: Mon Aug  7 08:51:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dayu-3.0.953.tar", last modified: Tue Aug  8 00:23:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dayu-3.0.952.tar` & `tencentcloud-sdk-python-dayu-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/v20180709/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   103066 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/v20180709/dayu_client.py
--rw-r--r--   0 root         (0) root         (0)   545180 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud_sdk_python_dayu.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud_sdk_python_dayu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      506 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud_sdk_python_dayu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud_sdk_python_dayu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud_sdk_python_dayu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/tencentcloud_sdk_python_dayu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-07 08:51:31.000000 tencentcloud-sdk-python-dayu-3.0.952/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/v20180709/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   103066 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/v20180709/dayu_client.py
+-rw-r--r--   0 root         (0) root         (0)   545180 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud_sdk_python_dayu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud_sdk_python_dayu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud_sdk_python_dayu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud_sdk_python_dayu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud_sdk_python_dayu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/tencentcloud_sdk_python_dayu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-08 00:23:08.000000 tencentcloud-sdk-python-dayu-3.0.953/README.rst
```

### Comparing `tencentcloud-sdk-python-dayu-3.0.952/setup.py` & `tencentcloud-sdk-python-dayu-3.0.953/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-dayu',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Dayu SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/v20180709/errorcodes.py` & `tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/v20180709/dayu_client.py` & `tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/v20180709/dayu_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dayu-3.0.952/tencentcloud/dayu/v20180709/models.py` & `tencentcloud-sdk-python-dayu-3.0.953/tencentcloud/dayu/v20180709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dayu-3.0.952/tencentcloud_sdk_python_dayu.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dayu-3.0.953/tencentcloud_sdk_python_dayu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dayu
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Dayu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dayu-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-dayu-3.0.953/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dayu
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Dayu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dayu-3.0.952/README.rst` & `tencentcloud-sdk-python-dayu-3.0.953/README.rst`

 * *Files identical despite different names*

