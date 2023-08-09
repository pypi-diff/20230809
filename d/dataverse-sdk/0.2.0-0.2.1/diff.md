# Comparing `tmp/dataverse-sdk-0.2.0.tar.gz` & `tmp/dataverse-sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-sdk-0.2.0.tar", last modified: Mon Jul 10 09:14:56 2023, max compression
+gzip compressed data, was "dataverse-sdk-0.2.1.tar", last modified: Wed Aug  9 05:40:10 2023, max compression
```

## Comparing `dataverse-sdk-0.2.0.tar` & `dataverse-sdk-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.245447 dataverse-sdk-0.2.0/
--rw-r--r--   0 jasper     (501) staff       (20)     6112 2023-07-10 09:14:56.245239 dataverse-sdk-0.2.0/PKG-INFO
--rw-r--r--   0 jasper     (501) staff       (20)     5872 2023-07-10 08:54:11.000000 dataverse-sdk-0.2.0/README.md
-drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.241631 dataverse-sdk-0.2.0/dataverse_sdk/
--rw-r--r--   0 jasper     (501) staff       (20)      825 2023-05-23 03:49:12.000000 dataverse-sdk-0.2.0/dataverse_sdk/__init__.py
-drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.242953 dataverse-sdk-0.2.0/dataverse_sdk/apis/
--rw-r--r--   0 jasper     (501) staff       (20)        0 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 jasper     (501) staff       (20)    10397 2023-07-03 05:45:07.000000 dataverse-sdk-0.2.0/dataverse_sdk/apis/backend.py
--rw-r--r--   0 jasper     (501) staff       (20)    21842 2023-07-03 05:45:07.000000 dataverse-sdk-0.2.0/dataverse_sdk/client.py
--rw-r--r--   0 jasper     (501) staff       (20)     1550 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/connections.py
--rw-r--r--   0 jasper     (501) staff       (20)      685 2023-07-10 08:53:08.000000 dataverse-sdk-0.2.0/dataverse_sdk/constants.py
-drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.243482 dataverse-sdk-0.2.0/dataverse_sdk/exceptions/
--rw-r--r--   0 jasper     (501) staff       (20)        0 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 jasper     (501) staff       (20)       49 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.244515 dataverse-sdk-0.2.0/dataverse_sdk/schemas/
--rw-r--r--   0 jasper     (501) staff       (20)        0 2022-11-24 06:20:23.000000 dataverse-sdk-0.2.0/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 jasper     (501) staff       (20)     3036 2023-05-23 03:49:12.000000 dataverse-sdk-0.2.0/dataverse_sdk/schemas/api.py
--rw-r--r--   0 jasper     (501) staff       (20)    10179 2023-07-03 05:45:07.000000 dataverse-sdk-0.2.0/dataverse_sdk/schemas/client.py
--rw-r--r--   0 jasper     (501) staff       (20)     1164 2023-05-23 03:49:12.000000 dataverse-sdk-0.2.0/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.244899 dataverse-sdk-0.2.0/dataverse_sdk/utils/
--rw-r--r--   0 jasper     (501) staff       (20)        0 2023-05-23 03:49:12.000000 dataverse-sdk-0.2.0/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 jasper     (501) staff       (20)      657 2023-07-03 05:45:07.000000 dataverse-sdk-0.2.0/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 jasper     (501) staff       (20)        0 2023-07-10 09:14:56.242637 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/
--rw-r--r--   0 jasper     (501) staff       (20)     6112 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jasper     (501) staff       (20)      629 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jasper     (501) staff       (20)        1 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jasper     (501) staff       (20)       18 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 jasper     (501) staff       (20)       14 2023-07-10 09:14:56.000000 dataverse-sdk-0.2.0/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 jasper     (501) staff       (20)       38 2023-07-10 09:14:56.245496 dataverse-sdk-0.2.0/setup.cfg
--rw-r--r--   0 jasper     (501) staff       (20)      613 2023-07-10 08:54:32.000000 dataverse-sdk-0.2.0/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-08-09 05:40:10.213060 dataverse-sdk-0.2.1/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     8669 2023-08-09 05:40:10.212846 dataverse-sdk-0.2.1/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     8429 2023-08-09 05:39:12.000000 dataverse-sdk-0.2.1/README.md
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-08-09 05:40:10.210191 dataverse-sdk-0.2.1/dataverse_sdk/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/__init__.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-08-09 05:40:10.211168 dataverse-sdk-0.2.1/dataverse_sdk/apis/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    11208 2023-08-09 05:39:12.000000 dataverse-sdk-0.2.1/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    28880 2023-08-09 05:39:12.000000 dataverse-sdk-0.2.1/dataverse_sdk/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/connections.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      685 2023-07-31 02:10:36.000000 dataverse-sdk-0.2.1/dataverse_sdk/constants.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-08-09 05:40:10.211432 dataverse-sdk-0.2.1/dataverse_sdk/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-08-09 05:40:10.212285 dataverse-sdk-0.2.1/dataverse_sdk/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.2.1/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    11304 2023-08-09 05:39:12.000000 dataverse-sdk-0.2.1/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-08-09 05:40:10.212521 dataverse-sdk-0.2.1/dataverse_sdk/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-06-17 03:34:04.000000 dataverse-sdk-0.2.1/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-08-09 05:40:10.210944 dataverse-sdk-0.2.1/dataverse_sdk.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     8669 2023-08-09 05:40:10.000000 dataverse-sdk-0.2.1/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-08-09 05:40:10.000000 dataverse-sdk-0.2.1/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-08-09 05:40:10.000000 dataverse-sdk-0.2.1/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       23 2023-08-09 05:40:10.000000 dataverse-sdk-0.2.1/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-08-09 05:40:10.000000 dataverse-sdk-0.2.1/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-08-09 05:40:10.213107 dataverse-sdk-0.2.1/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      618 2023-08-09 05:39:12.000000 dataverse-sdk-0.2.1/setup.py
```

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/__init__.py` & `dataverse-sdk-0.2.1/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/apis/backend.py` & `dataverse-sdk-0.2.1/dataverse_sdk/apis/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,39 @@
                 "name": name,
                 "ontology_data": ontology_data,
                 "sensor_data": sensor_data,
                 "project_tag_data": project_tag_data,
                 "description": description,
             },
         )
+        return resp.json()
 
+    def edit_project(
+        self,
+        project_id: int,
+        name: Optional[str] = None,
+        ontology_data: Optional[dict] = None,
+        project_tag_data: Optional[dict] = None,
+        description: Optional[str] = None,
+    ) -> dict:
+        data = {}
+        if name is not None:
+            data["name"] = name
+        if description is not None:
+            data["description"] = description
+        if ontology_data is not None:
+            data["ontology_data"] = ontology_data
+        if project_tag_data is not None:
+            data["project_tag_data"] = project_tag_data
+        resp = self.send_request(
+            url=f"{self.host}/api/projects/{project_id}/",
+            method="patch",
+            headers=self.headers,
+            data=data,
+        )
         return resp.json()
 
     def get_project(self, project_id) -> dict:
         resp = self.send_request(
             url=f"{self.host}/api/projects/{project_id}",
             method="get",
             headers=self.headers,
```

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/client.py` & `dataverse-sdk-0.2.1/dataverse_sdk/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,22 +16,37 @@
     ProjectTagAPISchema,
 )
 from .schemas.client import (
     Dataset,
     DataSource,
     MLModel,
     Ontology,
+    OntologyClass,
     Project,
     ProjectTag,
     Sensor,
 )
 from .schemas.common import AnnotationFormat, DatasetType, OntologyImageType, SensorType
 from .utils.utils import download_file_from_response, get_filepaths
 
 
+def parse_attribute(attr_list: list) -> list:
+    new_attribute_list: list[AttributeAPISchema] = []
+    for attr in attr_list:
+        attr.pop("id", None)
+        if attr["type"] != "option":
+            new_attribute_list.append(attr)
+            continue
+        attr["option_data"] = [
+            opt_data["value"] for opt_data in attr.pop("options", [])
+        ]
+        new_attribute_list.append(attr)
+    return new_attribute_list
+
+
 class DataverseClient:
     def __init__(
         self,
         host: DataverseHost,
         email: Optional[str] = None,
         password: Optional[str] = None,
         access_token: Optional[str] = None,
@@ -118,27 +133,14 @@
         ------
         ValidationError
             raise exception if there is any error occurs when composing the request body.
         ClientConnectionError
             raise exception if there is any error occurs when calling backend APIs.
         """
 
-        def parse_attribute(attr_list: list) -> list:
-            new_attribute_list: list[AttributeAPISchema] = []
-            for attr in attr_list:
-                attr.pop("id", None)
-                if attr["type"] != "option":
-                    new_attribute_list.append(attr)
-                    continue
-                attr["option_data"] = [
-                    opt_data["value"] for opt_data in attr.pop("options", [])
-                ]
-                new_attribute_list.append(attr)
-            return new_attribute_list
-
         if client is None:
             client = DataverseClient.get_client()
 
         raw_ontology_data: dict = ontology.dict(exclude_none=True)
         classes_data_list: list[dict] = []
         rank = 1
         # remove `id` field in OntologyClass and Attribute
@@ -250,14 +252,225 @@
         try:
             project_data: dict = api.get_project(project_id=project_id)
         except Exception as e:
             raise ClientConnectionError(f"Failed to get the project: {e}")
         return Project.create(project_data)
 
     @staticmethod
+    def add_project_tag(
+        project_id: int,
+        project_tag: ProjectTag,
+        client: Optional["DataverseClient"] = None,
+        project: Optional["Project"] = None,
+    ) -> dict:
+        """Add New Project Tag
+
+        Parameters
+        ----------
+        project_id : int
+        project_tag : ProjectTag
+        client : Optional["DataverseClient"], optional
+            clientclass, by default None
+        project : Optional["Project"], optional
+            project basemodel, by default None
+        Returns
+        -------
+        dict
+            dictionary with project id and project name info
+
+        Raises
+        ------
+        ClientConnectionError
+            API error when creating new project tag
+        """
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
+        if project is None:
+            project = DataverseClient.get_project(project_id=project_id)
+
+        raw_project_tag: dict = project_tag.dict(exclude_none=True)
+        # new project tag attributes to be creaeted
+        new_attribute_data: list = parse_attribute(
+            raw_project_tag.get("attributes", [])
+        )
+        project_tag_data = {"new_attribute_data": new_attribute_data}
+        try:
+            project_data: dict = api.edit_project(
+                project_id=project_id, project_tag_data=project_tag_data
+            )
+        except Exception as e:
+            raise ClientConnectionError(
+                f"Failed to add project tag, please check your data: {e}"
+            )
+        return project_data
+
+    @staticmethod
+    def edit_project_tag(
+        project_id: int,
+        project_tag: ProjectTag,
+        client: Optional["DataverseClient"] = None,
+        project: Optional["Project"] = None,
+    ) -> dict:
+        """Edit existing project tag
+
+        Parameters
+        ----------
+        project_id : int
+        project_tag : ProjectTag
+        client : Optional["DataverseClient"], optional
+            clientclass, by default None
+        project : Optional["Project"], optional
+            project basemodel, by default None
+
+        Returns
+        -------
+        dict
+            dictionary with project id and project name info
+
+        Raises
+        ------
+        ClientConnectionError
+            API error when editing project tag
+        """
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
+        if project is None:
+            project = DataverseClient.get_project(project_id=project_id)
+
+        raw_project_tag: dict = project_tag.dict(exclude_none=True)
+        # old project tag attributes to be extended
+        patched_attribute_data: list = parse_attribute(
+            raw_project_tag.get("attributes", [])
+        )
+        project_tag_data = {"patched_attribute_data": patched_attribute_data}
+        try:
+            project_data: dict = api.edit_project(
+                project_id=project_id, project_tag_data=project_tag_data
+            )
+        except Exception as e:
+            raise ClientConnectionError(
+                f"Failed to edit project tag, please check your data: {e}"
+            )
+        return project_data
+
+    @staticmethod
+    def add_ontology_classes(
+        project_id: int,
+        ontology_classes: list[OntologyClass],
+        client: Optional["DataverseClient"] = None,
+        project: Optional["Project"] = None,
+    ) -> dict:
+        """Add new ontology classes
+
+        Parameters
+        ----------
+        project_id : int
+        ontology_classes : list[OntologyClass]
+        client : Optional["DataverseClient"], optional
+            clientclass, by default None
+        project : Optional["Project"], optional
+            project basemodel, by default None
+
+        Returns
+        -------
+        dict
+            dictionary with project id and project name info
+
+        Raises
+        ------
+        ClientConnectionError
+            API error when creating new ontology class
+        """
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
+        if project is None:
+            project = DataverseClient.get_project(project_id=project_id)
+        # new ontology classes to be creaeted
+        new_classes_data = []
+        for ontology_class in ontology_classes:
+            raw_ontology_class: dict = ontology_class.dict(exclude_none=True)
+            attribute_data: list = parse_attribute(
+                raw_ontology_class.get("attributes", [])
+            )
+            new_classes_data.append(
+                {
+                    "name": ontology_class.name,
+                    "color": ontology_class.color,
+                    "attribute_data": attribute_data,
+                }
+            )
+        ontology_data = {"new_classes_data": new_classes_data}
+        try:
+            project_data: dict = api.edit_project(
+                project_id=project_id, ontology_data=ontology_data
+            )
+        except Exception as e:
+            raise ClientConnectionError(
+                f"Failed to add ontology classes, please check your data: {e}"
+            )
+        return project_data
+
+    @staticmethod
+    def edit_ontology_classes(
+        project_id: int,
+        ontology_classes: list[OntologyClass],
+        client: Optional["DataverseClient"] = None,
+        project: Optional["Project"] = None,
+    ) -> dict:
+        """Edit ontology classes
+
+        Parameters
+        ----------
+        project_id : int
+        ontology_classes : list[OntologyClass]
+        client : Optional["DataverseClient"], optional
+            clientclass, by default None
+        project : Optional["Project"], optional
+            project basemodel, by default None
+
+        Returns
+        -------
+        dict
+            dictionary with project id and project name info
+
+        Raises
+        ------
+        ClientConnectionError
+            API error when editing ontology classes
+        """
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
+        if project is None:
+            project = DataverseClient.get_project(project_id=project_id)
+        # ontology classes to be edited
+        patched_classes_data = []
+        for ontology_class in ontology_classes:
+            raw_ontology_class: dict = ontology_class.dict(exclude_none=True)
+            attribute_data: list = parse_attribute(
+                raw_ontology_class.get("attributes", [])
+            )
+            patched_classes_data.append(
+                {"name": ontology_class.name, "attribute_data": attribute_data}
+            )
+        ontology_data = {"patched_classes_data": patched_classes_data}
+        try:
+            project_data: dict = api.edit_project(
+                project_id=project_id, ontology_data=ontology_data
+            )
+        except Exception as e:
+            raise ClientConnectionError(
+                f"Failed to edit ontology classes, please check your data: {e}"
+            )
+        return project_data
+
+    @staticmethod
     def list_models(
         project_id: int,
         client: Optional["DataverseClient"] = None,
         project: Optional["Project"] = None,
     ) -> list[MLModel]:
         """Get the model list by project id
```

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/connections.py` & `dataverse-sdk-0.2.1/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/constants.py` & `dataverse-sdk-0.2.1/dataverse_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/schemas/api.py` & `dataverse-sdk-0.2.1/dataverse_sdk/schemas/api.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/schemas/client.py` & `dataverse-sdk-0.2.1/dataverse_sdk/schemas/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -155,14 +155,48 @@
             description=project_data["description"],
             ego_car=project_data["ego_car"],
             ontology=ontology,
             sensors=sensors,
             project_tag=project_tag,
         )
 
+    def add_project_tag(self, project_tag: ProjectTag):
+        from ..client import DataverseClient
+
+        project = DataverseClient.add_project_tag(
+            project_tag=project_tag, project=self, project_id=self.id
+        )
+        return project
+
+    def edit_project_tag(self, project_tag: ProjectTag):
+        from ..client import DataverseClient
+
+        project = DataverseClient.edit_project_tag(
+            project_tag=project_tag, project=self, project_id=self.id
+        )
+        return project
+
+    def add_ontology_classes(self, ontology_classes: list[OntologyClass]):
+        from ..client import DataverseClient
+
+        project = DataverseClient.add_ontology_classes(
+            ontology_classes=ontology_classes, project=self, project_id=self.id
+        )
+        return project
+
+    def edit_ontology_classes(self, ontology_classes: list[OntologyClass]):
+        from ..client import DataverseClient
+
+        project = DataverseClient.edit_ontology_classes(
+            ontology_classes=ontology_classes,
+            project=self,
+            project_id=self.id,
+        )
+        return project
+
     def list_models(self) -> list:
         from ..client import DataverseClient
 
         model_list: list = DataverseClient.list_models(project_id=self.id, project=self)
         return model_list
 
     def get_model(self, model_id: int):
```

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/schemas/common.py` & `dataverse-sdk-0.2.1/dataverse_sdk/schemas/common.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk/utils/utils.py` & `dataverse-sdk-0.2.1/dataverse_sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.2.0/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse-sdk-0.2.1/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.2.0/setup.py` & `dataverse-sdk-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "0.2.0"
+PACKAGE_VERSION = "0.2.1"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
     packages=find_packages(),
     python_requires=">=3.9, <4",
     author=AUTHOR,
     url="",
     description=DESC,
-    install_requires=["pydantic", "requests"],
+    install_requires=["pydantic==1.*", "requests"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=["Programming Language :: Python :: 3"],
 )
```

