# Comparing `tmp/tencentcloud-sdk-python-dasb-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-dasb-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.953.tar", last modified: Tue Aug  8 00:22:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.954.tar", last modified: Wed Aug  9 00:22:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dasb-3.0.953.tar` & `tencentcloud-sdk-python-dasb-3.0.954.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)    45781 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   260936 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      506 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-09 00:22:54.000000 tencentcloud-sdk-python-dasb-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:22:54.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)    45781 2023-08-09 00:22:54.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:22:54.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-08-09 00:22:54.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/v20191018/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   260936 2023-08-09 00:22:54.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:22:54.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud_sdk_python_dasb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud_sdk_python_dasb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-09 00:22:55.000000 tencentcloud-sdk-python-dasb-3.0.954/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-09 00:22:54.000000 tencentcloud-sdk-python-dasb-3.0.954/README.rst
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.953/setup.py` & `tencentcloud-sdk-python-dasb-3.0.954/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-dasb',
-    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.954"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Dasb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/dasb/v20191018/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dasb-3.0.954/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.954/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.954/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.953/README.rst` & `tencentcloud-sdk-python-dasb-3.0.954/README.rst`

 * *Files identical despite different names*

