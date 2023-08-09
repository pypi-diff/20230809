# Comparing `tmp/tencentcloud-sdk-python-iotvideo-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-iotvideo-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.952.tar", last modified: Mon Aug  7 08:56:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotvideo-3.0.953.tar", last modified: Tue Aug  8 00:27:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotvideo-3.0.952.tar` & `tencentcloud-sdk-python-iotvideo-3.0.953.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20211125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20211125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89241 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20211125/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20211125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   374676 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20211125/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20201215/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20201215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72567 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20201215/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20201215/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   303767 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20201215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20191126/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20191126/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64723 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20191126/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20191126/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   229605 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20191126/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud_sdk_python_iotvideo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      916 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud_sdk_python_iotvideo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:56:02.000000 tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20211125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20211125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89241 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20211125/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20211125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   374676 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20211125/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20201215/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20201215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72567 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20201215/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20201215/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   303767 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20201215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20191126/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20191126/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64723 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20191126/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20191126/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   229605 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20191126/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud_sdk_python_iotvideo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud_sdk_python_iotvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      916 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud_sdk_python_iotvideo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:27:15.000000 tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud_sdk_python_iotvideo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/setup.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-iotvideo',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Iotvideo SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20211125/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20211125/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20211125/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20211125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20211125/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20211125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20201215/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20201215/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20201215/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20201215/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20201215/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20201215/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20191126/iotvideo_client.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20191126/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20191126/errorcodes.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20191126/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/iotvideo/v20191126/models.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/iotvideo/v20191126/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.953/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/README.rst` & `tencentcloud-sdk-python-iotvideo-3.0.953/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud_sdk_python_iotvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotvideo-3.0.952/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotvideo-3.0.953/tencentcloud_sdk_python_iotvideo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotvideo
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Iotvideo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

