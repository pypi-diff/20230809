# Comparing `tmp/tencentcloud-sdk-python-tia-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-tia-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tia-3.0.952.tar", last modified: Mon Aug  7 09:04:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tia-3.0.953.tar", last modified: Tue Aug  8 00:34:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tia-3.0.952.tar` & `tencentcloud-sdk-python-tia-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/v20180226/
--rw-r--r--   0 root         (0) root         (0)    10682 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/v20180226/tia_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/v20180226/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/v20180226/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49879 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/v20180226/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud_sdk_python_tia.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud_sdk_python_tia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud_sdk_python_tia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud_sdk_python_tia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud_sdk_python_tia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 09:04:08.000000 tencentcloud-sdk-python-tia-3.0.952/tencentcloud_sdk_python_tia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/v20180226/
+-rw-r--r--   0 root         (0) root         (0)    10682 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/v20180226/tia_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/v20180226/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/v20180226/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49879 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/v20180226/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud_sdk_python_tia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud_sdk_python_tia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud_sdk_python_tia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud_sdk_python_tia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud_sdk_python_tia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:34:01.000000 tencentcloud-sdk-python-tia-3.0.953/tencentcloud_sdk_python_tia.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tia-3.0.952/setup.py` & `tencentcloud-sdk-python-tia-3.0.953/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tia',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tia SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/v20180226/tia_client.py` & `tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/v20180226/tia_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/v20180226/errorcodes.py` & `tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/v20180226/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.952/tencentcloud/tia/v20180226/models.py` & `tencentcloud-sdk-python-tia-3.0.953/tencentcloud/tia/v20180226/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tia-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tia-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-tia-3.0.953/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tia
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Tia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tia-3.0.952/README.rst` & `tencentcloud-sdk-python-tia-3.0.953/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.952/tencentcloud_sdk_python_tia.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tia-3.0.953/tencentcloud_sdk_python_tia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tia
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Tia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

