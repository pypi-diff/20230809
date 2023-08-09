# Comparing `tmp/tencentcloud-sdk-python-tem-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-tem-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tem-3.0.952.tar", last modified: Mon Aug  7 09:03:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tem-3.0.953.tar", last modified: Tue Aug  8 00:33:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tem-3.0.952.tar` & `tencentcloud-sdk-python-tem-3.0.953.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20210701/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20210701/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16604 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20210701/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46073 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20210701/tem_client.py
--rw-r--r--   0 root         (0) root         (0)   379283 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20210701/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20201221/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20201221/__init__.py
--rw-r--r--   0 root         (0) root         (0)      747 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20201221/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15824 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20201221/tem_client.py
--rw-r--r--   0 root         (0) root         (0)   117434 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20201221/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud_sdk_python_tem.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud_sdk_python_tem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      653 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud_sdk_python_tem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud_sdk_python_tem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/tencentcloud_sdk_python_tem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 09:03:49.000000 tencentcloud-sdk-python-tem-3.0.952/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20210701/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20210701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16604 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20210701/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46073 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20210701/tem_client.py
+-rw-r--r--   0 root         (0) root         (0)   379283 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20210701/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20201221/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20201221/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20201221/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20201221/tem_client.py
+-rw-r--r--   0 root         (0) root         (0)   117434 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20201221/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud_sdk_python_tem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud_sdk_python_tem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud_sdk_python_tem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud_sdk_python_tem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/tencentcloud_sdk_python_tem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:33:46.000000 tencentcloud-sdk-python-tem-3.0.953/README.rst
```

### Comparing `tencentcloud-sdk-python-tem-3.0.952/setup.py` & `tencentcloud-sdk-python-tem-3.0.953/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-tem',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Tem SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20210701/errorcodes.py` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20210701/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20210701/tem_client.py` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20210701/tem_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20210701/models.py` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20210701/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20201221/errorcodes.py` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20201221/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20201221/tem_client.py` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20201221/tem_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud/tem/v20201221/models.py` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud/tem/v20201221/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud_sdk_python_tem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tem-3.0.952/tencentcloud_sdk_python_tem.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tem-3.0.953/tencentcloud_sdk_python_tem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tem
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Tem SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tem-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-tem-3.0.953/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tem
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Tem SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tem-3.0.952/README.rst` & `tencentcloud-sdk-python-tem-3.0.953/README.rst`

 * *Files identical despite different names*

