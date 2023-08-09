# Comparing `tmp/tencentcloud-sdk-python-cat-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-cat-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cat-3.0.953.tar", last modified: Tue Aug  8 00:19:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cat-3.0.954.tar", last modified: Wed Aug  9 00:19:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cat-3.0.953.tar` & `tencentcloud-sdk-python-cat-3.0.954.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/v20180409/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/v20180409/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2879 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/v20180409/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    67446 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/v20180409/models.py
--rw-r--r--   0 root         (0) root         (0)    10939 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/v20180409/cat_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud_sdk_python_cat.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud_sdk_python_cat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud_sdk_python_cat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud_sdk_python_cat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud_sdk_python_cat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/tencentcloud_sdk_python_cat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:19:54.000000 tencentcloud-sdk-python-cat-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/v20180409/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/v20180409/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/v20180409/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    67446 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/v20180409/models.py
+-rw-r--r--   0 root         (0) root         (0)    10939 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/v20180409/cat_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud_sdk_python_cat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud_sdk_python_cat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud_sdk_python_cat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud_sdk_python_cat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud_sdk_python_cat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/tencentcloud_sdk_python_cat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-09 00:19:50.000000 tencentcloud-sdk-python-cat-3.0.954/README.rst
```

### Comparing `tencentcloud-sdk-python-cat-3.0.953/setup.py` & `tencentcloud-sdk-python-cat-3.0.954/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cat',
-    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.954"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cat SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cat-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cat-3.0.954/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/v20180409/errorcodes.py` & `tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/v20180409/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/v20180409/models.py` & `tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/v20180409/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cat-3.0.953/tencentcloud/cat/v20180409/cat_client.py` & `tencentcloud-sdk-python-cat-3.0.954/tencentcloud/cat/v20180409/cat_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cat-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-cat-3.0.954/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cat
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Cat SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cat-3.0.953/tencentcloud_sdk_python_cat.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cat-3.0.954/tencentcloud_sdk_python_cat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cat
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Cat SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cat-3.0.953/README.rst` & `tencentcloud-sdk-python-cat-3.0.954/README.rst`

 * *Files identical despite different names*

