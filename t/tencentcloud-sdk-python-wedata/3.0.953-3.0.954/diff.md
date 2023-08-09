# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.953.tar", last modified: Tue Aug  8 00:36:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.954.tar", last modified: Wed Aug  9 00:36:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.953.tar` & `tencentcloud-sdk-python-wedata-3.0.954.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      528 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1968638 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)   276930 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      528 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud_sdk_python_wedata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1975246 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)   276930 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-08-09 00:36:49.000000 tencentcloud-sdk-python-wedata-3.0.954/README.rst
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/setup.py` & `tencentcloud-sdk-python-wedata-3.0.954/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-wedata',
-    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.954"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Wedata SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-wedata-3.0.954/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.954/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/v20210820/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -29405,19 +29405,28 @@
         :type ProjectId: str
         :param _TaskTypeId: 任务类型ID
         :type TaskTypeId: str
         :param _ExecutionGroupId: 执行资源组ID
         :type ExecutionGroupId: str
         :param _ExecutionGroupName: 执行资源组名字
         :type ExecutionGroupName: str
+        :param _StartTime: 开始时间
+        :type StartTime: str
+        :param _EndTime: 结束时间
+        :type EndTime: str
+        :param _InCharge: 责任人
+        :type InCharge: str
         """
         self._ProjectId = None
         self._TaskTypeId = None
         self._ExecutionGroupId = None
         self._ExecutionGroupName = None
+        self._StartTime = None
+        self._EndTime = None
+        self._InCharge = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -29443,20 +29452,47 @@
     def ExecutionGroupName(self):
         return self._ExecutionGroupName
 
     @ExecutionGroupName.setter
     def ExecutionGroupName(self, ExecutionGroupName):
         self._ExecutionGroupName = ExecutionGroupName
 
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def InCharge(self):
+        return self._InCharge
+
+    @InCharge.setter
+    def InCharge(self, InCharge):
+        self._InCharge = InCharge
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._TaskTypeId = params.get("TaskTypeId")
         self._ExecutionGroupId = params.get("ExecutionGroupId")
         self._ExecutionGroupName = params.get("ExecutionGroupName")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._InCharge = params.get("InCharge")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -29519,20 +29555,26 @@
         :type CycleUnit: str
         :param _TimeUnit: 时间单元 eg: 12h
         :type TimeUnit: str
         :param _StartTime: 开始日期：2023-03-02
         :type StartTime: str
         :param _EndTime: 结束日前：2023-03-20
         :type EndTime: str
+        :param _TaskType: 1
+        :type TaskType: int
+        :param _InCharge: 1
+        :type InCharge: str
         """
         self._ProjectId = None
         self._CycleUnit = None
         self._TimeUnit = None
         self._StartTime = None
         self._EndTime = None
+        self._TaskType = None
+        self._InCharge = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -29566,21 +29608,39 @@
     def EndTime(self):
         return self._EndTime
 
     @EndTime.setter
     def EndTime(self, EndTime):
         self._EndTime = EndTime
 
+    @property
+    def TaskType(self):
+        return self._TaskType
+
+    @TaskType.setter
+    def TaskType(self, TaskType):
+        self._TaskType = TaskType
+
+    @property
+    def InCharge(self):
+        return self._InCharge
+
+    @InCharge.setter
+    def InCharge(self, InCharge):
+        self._InCharge = InCharge
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._CycleUnit = params.get("CycleUnit")
         self._TimeUnit = params.get("TimeUnit")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
+        self._TaskType = params.get("TaskType")
+        self._InCharge = params.get("InCharge")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -29639,18 +29699,21 @@
         r"""
         :param _TaskType: 1
         :type TaskType: int
         :param _TypeName: Y
         :type TypeName: str
         :param _ProjectId: 111
         :type ProjectId: str
+        :param _InCharge: 1
+        :type InCharge: str
         """
         self._TaskType = None
         self._TypeName = None
         self._ProjectId = None
+        self._InCharge = None
 
     @property
     def TaskType(self):
         return self._TaskType
 
     @TaskType.setter
     def TaskType(self, TaskType):
@@ -29668,19 +29731,28 @@
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
         self._ProjectId = ProjectId
 
+    @property
+    def InCharge(self):
+        return self._InCharge
+
+    @InCharge.setter
+    def InCharge(self, InCharge):
+        self._InCharge = InCharge
+
 
     def _deserialize(self, params):
         self._TaskType = params.get("TaskType")
         self._TypeName = params.get("TypeName")
         self._ProjectId = params.get("ProjectId")
+        self._InCharge = params.get("InCharge")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -29735,28 +29807,40 @@
 
     """
 
     def __init__(self):
         r"""
         :param _ProjectId: 项目ID
         :type ProjectId: str
+        :param _InCharge: 1
+        :type InCharge: str
         """
         self._ProjectId = None
+        self._InCharge = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
         self._ProjectId = ProjectId
 
+    @property
+    def InCharge(self):
+        return self._InCharge
+
+    @InCharge.setter
+    def InCharge(self, InCharge):
+        self._InCharge = InCharge
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
+        self._InCharge = params.get("InCharge")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -30193,23 +30277,38 @@
         :type StartTime: str
         :param _EndTime: 结束时间
         :type EndTime: str
         :param _ExecutionGroupId: 资源组ID
         :type ExecutionGroupId: str
         :param _ExecutionGroupName: 资源组名称
         :type ExecutionGroupName: str
+        :param _InCharge: 1
+        :type InCharge: str
+        :param _TaskType: 1
+        :type TaskType: int
+        :param _StateList: 1
+        :type StateList: list of int
+        :param _AggregationUnit: D代表天，H代表小时
+        :type AggregationUnit: str
+        :param _AverageWindowSize: 1
+        :type AverageWindowSize: int
         """
         self._ProjectId = None
         self._TaskTypeId = None
         self._TimeType = None
         self._TypeName = None
         self._StartTime = None
         self._EndTime = None
         self._ExecutionGroupId = None
         self._ExecutionGroupName = None
+        self._InCharge = None
+        self._TaskType = None
+        self._StateList = None
+        self._AggregationUnit = None
+        self._AverageWindowSize = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -30267,24 +30366,69 @@
     def ExecutionGroupName(self):
         return self._ExecutionGroupName
 
     @ExecutionGroupName.setter
     def ExecutionGroupName(self, ExecutionGroupName):
         self._ExecutionGroupName = ExecutionGroupName
 
+    @property
+    def InCharge(self):
+        return self._InCharge
+
+    @InCharge.setter
+    def InCharge(self, InCharge):
+        self._InCharge = InCharge
+
+    @property
+    def TaskType(self):
+        return self._TaskType
+
+    @TaskType.setter
+    def TaskType(self, TaskType):
+        self._TaskType = TaskType
+
+    @property
+    def StateList(self):
+        return self._StateList
+
+    @StateList.setter
+    def StateList(self, StateList):
+        self._StateList = StateList
+
+    @property
+    def AggregationUnit(self):
+        return self._AggregationUnit
+
+    @AggregationUnit.setter
+    def AggregationUnit(self, AggregationUnit):
+        self._AggregationUnit = AggregationUnit
+
+    @property
+    def AverageWindowSize(self):
+        return self._AverageWindowSize
+
+    @AverageWindowSize.setter
+    def AverageWindowSize(self, AverageWindowSize):
+        self._AverageWindowSize = AverageWindowSize
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._TaskTypeId = params.get("TaskTypeId")
         self._TimeType = params.get("TimeType")
         self._TypeName = params.get("TypeName")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._ExecutionGroupId = params.get("ExecutionGroupId")
         self._ExecutionGroupName = params.get("ExecutionGroupName")
+        self._InCharge = params.get("InCharge")
+        self._TaskType = params.get("TaskType")
+        self._StateList = params.get("StateList")
+        self._AggregationUnit = params.get("AggregationUnit")
+        self._AverageWindowSize = params.get("AverageWindowSize")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -31563,28 +31707,40 @@
 
     """
 
     def __init__(self):
         r"""
         :param _ProjectId: 项目ID
         :type ProjectId: str
+        :param _InCharge: 1
+        :type InCharge: str
         """
         self._ProjectId = None
+        self._InCharge = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
         self._ProjectId = ProjectId
 
+    @property
+    def InCharge(self):
+        return self._InCharge
+
+    @InCharge.setter
+    def InCharge(self, InCharge):
+        self._InCharge = InCharge
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
+        self._InCharge = params.get("InCharge")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -31648,21 +31804,33 @@
         :type TaskType: str
         :param _TypeName: 类型名称
         :type TypeName: str
         :param _StartTime: 开始时间
         :type StartTime: str
         :param _EndTime: 结束时间
         :type EndTime: str
+        :param _AggregationUnit: 无
+        :type AggregationUnit: str
+        :param _CycleUnit: 无
+        :type CycleUnit: str
+        :param _Status: 无
+        :type Status: str
+        :param _InCharge: 无
+        :type InCharge: str
         """
         self._ProjectId = None
         self._Type = None
         self._TaskType = None
         self._TypeName = None
         self._StartTime = None
         self._EndTime = None
+        self._AggregationUnit = None
+        self._CycleUnit = None
+        self._Status = None
+        self._InCharge = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -31704,22 +31872,58 @@
     def EndTime(self):
         return self._EndTime
 
     @EndTime.setter
     def EndTime(self, EndTime):
         self._EndTime = EndTime
 
+    @property
+    def AggregationUnit(self):
+        return self._AggregationUnit
+
+    @AggregationUnit.setter
+    def AggregationUnit(self, AggregationUnit):
+        self._AggregationUnit = AggregationUnit
+
+    @property
+    def CycleUnit(self):
+        return self._CycleUnit
+
+    @CycleUnit.setter
+    def CycleUnit(self, CycleUnit):
+        self._CycleUnit = CycleUnit
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def InCharge(self):
+        return self._InCharge
+
+    @InCharge.setter
+    def InCharge(self, InCharge):
+        self._InCharge = InCharge
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._Type = params.get("Type")
         self._TaskType = params.get("TaskType")
         self._TypeName = params.get("TypeName")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
+        self._AggregationUnit = params.get("AggregationUnit")
+        self._CycleUnit = params.get("CycleUnit")
+        self._Status = params.get("Status")
+        self._InCharge = params.get("InCharge")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -42119,20 +42323,28 @@
         :param _InstanceStatus: 实例状态标识：WAITING_RUNNING、KILLING、FAILED、FAILED_TRYING、SUCCEED 分别表示等待执行、正在终止、失败、失败重试、成功，用于实例状态分布和实例状态趋势
         :type InstanceStatus: str
         :param _InstanceCount: 用于实例状态分布计数
         :type InstanceCount: int
         :param _ShowTime: 当前展示时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type ShowTime: str
+        :param _ReportTime: 1
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ReportTime: str
+        :param _Count: 1
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Count: int
         """
         self._CountList = None
         self._TimeList = None
         self._InstanceStatus = None
         self._InstanceCount = None
         self._ShowTime = None
+        self._ReportTime = None
+        self._Count = None
 
     @property
     def CountList(self):
         return self._CountList
 
     @CountList.setter
     def CountList(self, CountList):
@@ -42166,21 +42378,39 @@
     def ShowTime(self):
         return self._ShowTime
 
     @ShowTime.setter
     def ShowTime(self, ShowTime):
         self._ShowTime = ShowTime
 
+    @property
+    def ReportTime(self):
+        return self._ReportTime
+
+    @ReportTime.setter
+    def ReportTime(self, ReportTime):
+        self._ReportTime = ReportTime
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
 
     def _deserialize(self, params):
         self._CountList = params.get("CountList")
         self._TimeList = params.get("TimeList")
         self._InstanceStatus = params.get("InstanceStatus")
         self._InstanceCount = params.get("InstanceCount")
         self._ShowTime = params.get("ShowTime")
+        self._ReportTime = params.get("ReportTime")
+        self._Count = params.get("Count")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -62195,19 +62425,25 @@
         :type ShowTimeGroup: str
         :param _Status: 状态
 注意：此字段可能返回 null，表示取不到有效值。
         :type Status: str
         :param _CycleUnit: 周期单位
 注意：此字段可能返回 null，表示取不到有效值。
         :type CycleUnit: str
+        :param _ReportTime: 1
+        :type ReportTime: str
+        :param _Count: 1
+        :type Count: int
         """
         self._CountGroup = None
         self._ShowTimeGroup = None
         self._Status = None
         self._CycleUnit = None
+        self._ReportTime = None
+        self._Count = None
 
     @property
     def CountGroup(self):
         return self._CountGroup
 
     @CountGroup.setter
     def CountGroup(self, CountGroup):
@@ -62233,20 +62469,38 @@
     def CycleUnit(self):
         return self._CycleUnit
 
     @CycleUnit.setter
     def CycleUnit(self, CycleUnit):
         self._CycleUnit = CycleUnit
 
+    @property
+    def ReportTime(self):
+        return self._ReportTime
+
+    @ReportTime.setter
+    def ReportTime(self, ReportTime):
+        self._ReportTime = ReportTime
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
 
     def _deserialize(self, params):
         self._CountGroup = params.get("CountGroup")
         self._ShowTimeGroup = params.get("ShowTimeGroup")
         self._Status = params.get("Status")
         self._CycleUnit = params.get("CycleUnit")
+        self._ReportTime = params.get("ReportTime")
+        self._Count = params.get("Count")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.954/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.954/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.953/README.rst` & `tencentcloud-sdk-python-wedata-3.0.954/README.rst`

 * *Files identical despite different names*

