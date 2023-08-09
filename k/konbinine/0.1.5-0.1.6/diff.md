# Comparing `tmp/konbinine-0.1.5.tar.gz` & `tmp/konbinine-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konbinine-0.1.5.tar", last modified: Mon Aug  7 08:50:52 2023, max compression
+gzip compressed data, was "konbinine-0.1.6.tar", last modified: Wed Aug  9 02:39:21 2023, max compression
```

## Comparing `konbinine-0.1.5.tar` & `konbinine-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-07 08:50:52.824005 konbinine-0.1.5/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.5/LICENSE
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4450 2023-08-07 08:50:52.824005 konbinine-0.1.5/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     2128 2023-07-24 10:10:35.000000 konbinine-0.1.5/README.md
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-07 08:50:52.814005 konbinine-0.1.5/konbinine/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)    29922 2023-08-07 08:45:43.000000 konbinine-0.1.5/konbinine/__init__.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      873 2023-06-29 09:15:35.000000 konbinine-0.1.5/konbinine/enums.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      392 2023-07-03 01:33:22.000000 konbinine-0.1.5/konbinine/exceptions.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      365 2023-08-07 08:14:30.000000 konbinine-0.1.5/konbinine/fields.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      145 2023-07-03 01:33:22.000000 konbinine-0.1.5/konbinine/logs.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     7844 2023-08-07 08:45:31.000000 konbinine-0.1.5/konbinine/models.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1828 2023-08-07 08:07:50.000000 konbinine-0.1.5/konbinine/utils.py
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-07 08:50:52.824005 konbinine-0.1.5/konbinine.egg-info/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4450 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      402 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/SOURCES.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/dependency_links.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/requires.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       10 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/top_level.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.5/konbinine.egg-info/zip-safe
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1268 2023-07-24 09:56:01.000000 konbinine-0.1.5/pyproject.toml
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-07 02:46:56.000000 konbinine-0.1.5/requirements.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1058 2023-08-07 08:50:52.824005 konbinine-0.1.5/setup.cfg
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:47:46.000000 konbinine-0.1.5/setup.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-09 02:39:21.717250 konbinine-0.1.6/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.6/LICENSE
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4666 2023-08-09 02:39:21.717250 konbinine-0.1.6/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     2344 2023-08-09 02:38:56.000000 konbinine-0.1.6/README.md
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-09 02:39:21.717250 konbinine-0.1.6/konbinine/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)    36329 2023-08-09 02:38:56.000000 konbinine-0.1.6/konbinine/__init__.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      873 2023-06-29 09:15:35.000000 konbinine-0.1.6/konbinine/enums.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      392 2023-07-03 01:33:22.000000 konbinine-0.1.6/konbinine/exceptions.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1579 2023-08-09 02:38:56.000000 konbinine-0.1.6/konbinine/fields.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      145 2023-07-03 01:33:22.000000 konbinine-0.1.6/konbinine/logs.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)    10123 2023-08-09 02:38:56.000000 konbinine-0.1.6/konbinine/models.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      160 2023-08-09 02:38:56.000000 konbinine-0.1.6/konbinine/types.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1828 2023-08-08 06:18:27.000000 konbinine-0.1.6/konbinine/utils.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-09 02:39:21.717250 konbinine-0.1.6/konbinine.egg-info/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4666 2023-08-09 02:39:21.000000 konbinine-0.1.6/konbinine.egg-info/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      421 2023-08-09 02:39:21.000000 konbinine-0.1.6/konbinine.egg-info/SOURCES.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-08-09 02:39:21.000000 konbinine-0.1.6/konbinine.egg-info/dependency_links.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-08-09 02:39:21.000000 konbinine-0.1.6/konbinine.egg-info/requires.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       10 2023-08-09 02:39:21.000000 konbinine-0.1.6/konbinine.egg-info/top_level.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.6/konbinine.egg-info/zip-safe
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1268 2023-07-24 09:56:01.000000 konbinine-0.1.6/pyproject.toml
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-07 02:46:56.000000 konbinine-0.1.6/requirements.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1058 2023-08-09 02:39:21.717250 konbinine-0.1.6/setup.cfg
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:47:46.000000 konbinine-0.1.6/setup.py
```

### Comparing `konbinine-0.1.5/LICENSE` & `konbinine-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.5/PKG-INFO` & `konbinine-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.5
+Version: 0.1.6
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
@@ -54,18 +54,19 @@
 because the API usage requirements is 便利じゃないでしょう？
 
 > コンビニね～ As there is an existing PyPI project using **_konbini_** name, this repo project name
 > on PyPI will be **konbinine**.
 
 ## How to Use
 
-> For Python 3.7 and newer! While Autodesk made **shotgun_api3** to be compatible with Python 2 and 3, **konbinine**
-> uses `dataclass` that is only available in Python 3.7 onwards.
+> For Python 3.8 and newer! While Autodesk made **shotgun_api3** to be compatible with Python 2 and 3, **konbinine**
+> uses `dataclass` that is only available in Python 3.7 onwards. Starting with v0.1.6, Python 3.8 will be the minimum
+> version due to the usage of TypedDict.
 
-**konbinine** is designed to be use with web framework (such as Django, Flask, etc) that interacts with ShotGrid. This
+**konbinine** is designed to be used with web framework (such as Django, Flask, etc.) that interacts with ShotGrid. This
 library has not been tested inside Digital Content Creation (DCC) software such as Maya, 3ds Max or Houdini.
 
 Technically it should just work but that is outside the scope of this library.
 
 ### New Project
 
 #### First time setup
@@ -107,7 +108,12 @@
 ```commandline
 pip install -r requirements.txt
 ```
 
 ## Extending konbinine
 
 Coming soon!
+
+## TODO
+
+1. Implement `Sequence` dataclass
+2. Handle Image/Movie upload gracefully (currently for Project entity only)
```

### Comparing `konbinine-0.1.5/README.md` & `konbinine-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 because the API usage requirements is 便利じゃないでしょう？
 
 > コンビニね～ As there is an existing PyPI project using **_konbini_** name, this repo project name
 > on PyPI will be **konbinine**.
 
 ## How to Use
 
-> For Python 3.7 and newer! While Autodesk made **shotgun_api3** to be compatible with Python 2 and 3, **konbinine**
-> uses `dataclass` that is only available in Python 3.7 onwards.
+> For Python 3.8 and newer! While Autodesk made **shotgun_api3** to be compatible with Python 2 and 3, **konbinine**
+> uses `dataclass` that is only available in Python 3.7 onwards. Starting with v0.1.6, Python 3.8 will be the minimum
+> version due to the usage of TypedDict.
 
-**konbinine** is designed to be use with web framework (such as Django, Flask, etc) that interacts with ShotGrid. This
+**konbinine** is designed to be used with web framework (such as Django, Flask, etc.) that interacts with ShotGrid. This
 library has not been tested inside Digital Content Creation (DCC) software such as Maya, 3ds Max or Houdini.
 
 Technically it should just work but that is outside the scope of this library.
 
 ### New Project
 
 #### First time setup
@@ -59,7 +60,12 @@
 ```commandline
 pip install -r requirements.txt
 ```
 
 ## Extending konbinine
 
 Coming soon!
+
+## TODO
+
+1. Implement `Sequence` dataclass
+2. Handle Image/Movie upload gracefully (currently for Project entity only)
```

### Comparing `konbinine-0.1.5/konbinine/__init__.py` & `konbinine-0.1.6/konbinine/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,42 @@
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 import calendar
 import datetime
 import logging
 import os
-from typing import List, Optional, Set, Union
+from typing import List, Optional, Set, Tuple, Union
 
 import shotgun_api3
 from urllib3.exceptions import ProtocolError
 
 from konbinine.enums import SgEntity, SgHumanUserStatus
 from konbinine.exceptions import MissingValueError
 from konbinine.fields import (
+    ASSET_FIELDS,
+    BOOKING_FIELDS,
     HUMANUSER_FIELDS,
+    NOTE_FIELDS,
     PROJECT_FIELDS,
+    SHOT_FIELDS,
+    TASK_FIELDS,
+    TIMELOG_FIELDS,
+    VERSION_FIELDS,
 )
 from konbinine.logs import KonbiniAdapter
 from konbinine.models import (
+    SgAsset,
     SgBooking,
     SgHumanUser,
+    SgNote,
     SgProject,
+    SgShot,
+    SgTask,
     SgTimeLog,
+    SgVersion,
 )
 from konbinine.utils import SG_DATE_FORMAT
 
 logger = KonbiniAdapter(logging.getLogger(__name__), {})
 logger.setLevel(logging.ERROR)
 
 
@@ -98,14 +110,37 @@
         list
             The list of fields belonging to the entity type
 
         """
         fields = self.sg.schema_field_read(entity_type=entity)
         return list(fields.keys())
 
+    def get_valid_values(self, entity: str, field_name: str) -> List[str]:
+        """Get Valid Values
+
+        Parameters
+        ----------
+        entity : str
+            The entity type (e.g. Asset, Shot, Timelog, etc)
+        field_name : str
+            The field name (e.g. sg_status, sg_status_list, etc)
+
+        Returns
+        -------
+        list of str
+
+        """
+        response_data = self.sg.schema_field_read(entity, field_name)
+        try:
+            valid_values: List[str] = response_data[field_name]["properties"]["valid_values"]["value"]
+        except (KeyError, Exception) as e:
+            raise e
+
+        return valid_values
+
     def get_sg_projects(
             self,
             project_id: Optional[int] = None,
             custom_fields: Optional[List[str]] = None,
     ) -> List[SgProject]:
         """Get SG Projects
 
@@ -143,14 +178,52 @@
         projects = []
         for project in _projects:
             sg_project = SgProject.from_dict(project)
             projects.append(sg_project)
 
         return projects
 
+    def create_sg_project(self, data: SgProject) -> Tuple[int, bool]:
+        if not isinstance(data, SgProject):
+            raise Exception("Data must be instance of SgProject!")
+
+        create_data = {
+            "name": data.name,
+            "sg_description": data.sg_description,
+        }
+        if data.sg_status:
+            valid_values = self.get_valid_values(SgEntity.PROJECT, "sg_status")
+            if data.sg_status not in valid_values:
+                raise Exception(f"Invalid {data.sg_status} value! Valid values: {valid_values}")
+
+            create_data["sg_status"] = data.sg_status
+
+        # Make sure it is str, bytes or os.PathLike object
+        if data.image_upload:
+            create_data["image"] = data.image_upload,
+
+        is_created = True
+        sg_id = 0
+
+        try:
+            response_data = self.sg.create(
+                entity_type=SgEntity.PROJECT,
+                data=create_data,
+            )
+            sg_id = response_data["id"]
+            logger.info(f"SgProject {response_data['id']} successfully created")
+        except shotgun_api3.ShotgunError as e:
+            logger.error(f"Error creating SgProject for Project {data.name}: {e}")
+            is_created = False
+        except Exception as e:
+            logger.error(f"Unhandled exception when creating SgProject {data.name}: {e}")
+            is_created = False
+
+        return sg_id, is_created
+
     def update_sg_project(self, data: SgProject) -> bool:
         """Update SG Project
 
         Parameters
         ----------
         data : SgProject
             The SgProject data for update
@@ -163,33 +236,47 @@
         """
         if not isinstance(data, SgProject):
             raise Exception("Data must be instance of SgProject!")
 
         if not data.id:
             raise Exception("No SgProject ID found!")
 
+        if data.sg_status:
+            valid_values = self.get_valid_values(SgEntity.PROJECT, "sg_status")
+            if data.sg_status not in valid_values:
+                raise Exception(f"Invalid {data.sg_status} value! Valid values: {valid_values}")
+
         is_updated = True
         data_ = data.to_dict()
 
         # Project start and end date is read only (only can be modified using Project Planning app on SG Web)
         data_.pop("start_date", None)
         data_.pop("end_date", None)
         data_.pop("duration", None)
         data_.pop("updated_at", None)
+        data_.pop("image", None)
+
+        # Make sure it is str, bytes or os.PathLike object
+        is_image_upload = data_.pop("image_upload", None)
+        if is_image_upload:
+            data_["image"] = is_image_upload
 
         try:
             self.sg.update(
                 entity_type=SgEntity.PROJECT,
                 entity_id=data.id,
                 data=data_,
             )
             logger.info(f"Update SgProject {data.id} successful")
         except shotgun_api3.ShotgunError as e:
             logger.error(f"Error updating SgProject {data.id}: {e}")
             is_updated = False
+        except Exception as e:
+            logger.error(f"Unhandled exception when updating SgProject {data.id}: {e}")
+            is_updated = False
 
         return is_updated
 
     def get_sg_humanusers(
             self,
             humanuser_id: Optional[int] = None,
             custom_fields: Optional[List[str]] = None,
@@ -201,15 +288,15 @@
         humanuser_id : int
             ShotGrid HumanUser ID. Default None which retrieve all valid HumanUser
         custom_fields : list[str]
             List of custom fields
 
         Returns
         -------
-        list
+        list[SgHumanUser]
             List of SgHumanUser or empty list if no results from ShotGrid
 
         """
         filters = []
         if humanuser_id:
             filters = [
                 [
@@ -296,14 +383,19 @@
             "name": "Kepci Bin Mekdi",
         }
 
         """
         is_created = True
         response_data = {}
 
+        if data.sg_status_list:
+            valid_values = self.get_valid_values(SgEntity.HUMANUSER, "sg_status_list")
+            if data.sg_status_list not in valid_values:
+                raise Exception(f"Invalid {data.sg_status_list} value! Valid values: {valid_values}")
+
         create_data = data.to_dict()
         try:
             response_data = self.sg.create(SgEntity.HUMANUSER, create_data)
         except (shotgun_api3.Fault, shotgun_api3.ShotgunError) as e:
             logger.error(
                 {
                     "msg": "Fail to create SG HumanUser",
@@ -336,14 +428,19 @@
         """
         if not isinstance(data, SgHumanUser):
             raise Exception("Data must be instance of SgHumanUser!")
 
         if not data.id:
             raise Exception("No SgHumanUser ID found!")
 
+        if data.sg_status_list:
+            valid_values = self.get_valid_values(SgEntity.HUMANUSER, "sg_status_list")
+            if data.sg_status_list not in valid_values:
+                raise Exception(f"Invalid {data.sg_status_list} value! Valid values: {valid_values}")
+
         is_updated = True
         data_ = data.to_dict()
 
         # Requires Autodesk Account Portal to update the following fields
         data_.pop("email", None)
         data_.pop("firstname", None)
         data_.pop("lastname", None)
@@ -393,20 +490,15 @@
                             "id": humanuser_id,
                             "type": SgEntity.HUMANUSER,
                         }
                     ]
                 ]
             ]
 
-        fields = [
-            "start_date",
-            "end_date",
-            "vacation",
-            "user",
-        ]
+        fields = BOOKING_FIELDS
         if custom_fields:
             fields = custom_fields
 
         _bookings: List[dict] = self.sg.find(SgEntity.BOOKING, filters, fields)
         if not _bookings:
             return []
 
@@ -464,21 +556,15 @@
                             "id": humanuser_id,
                             "type": SgEntity.HUMANUSER,
                         }
                     ]
                 ]
             )
 
-        fields = [
-            "start_date",
-            "end_date",
-            "vacation",
-            "user",
-            "note",
-        ]
+        fields = BOOKING_FIELDS
         if custom_fields:
             fields = custom_fields
 
         order = [
             {
                 "field_name": "start_date",
                 "direction": "asc",
@@ -568,21 +654,15 @@
                             "id": humanuser_id,
                             "type": SgEntity.HUMANUSER,
                         }
                     ]
                 ]
             )
 
-        fields = [
-            "start_date",
-            "end_date",
-            "vacation",
-            "user",
-            "note",
-        ]
+        fields = BOOKING_FIELDS
         if custom_fields:
             fields = custom_fields
 
         order = [
             {
                 "field_name": "start_date",
                 "direction": "asc",
@@ -634,14 +714,19 @@
                 },
             }
             
         """
         is_created = True
         response_data = {}
 
+        if data.sg_status_list:
+            valid_values = self.get_valid_values(SgEntity.BOOKING, "sg_status_list")
+            if data.sg_status_list not in valid_values:
+                raise Exception(f"Invalid {data.sg_status_list} value! Valid values: {valid_values}")
+
         create_data = data.to_dict()
         create_data.update(
             {
                 "user": {
                     "id": data.user.id,
                     "type": SgEntity.HUMANUSER,
                 }
@@ -692,108 +777,148 @@
                     "msg": f"Fail to delete SG Booking ID {sg_booking_id}",
                     "error": e,
                 }
             )
 
         return is_deleted
 
-    def get_sg_notes(self, project_id: int) -> List[dict]:
-        """Get SG Notes
+    def get_sg_notes_by_project(self, project_id: int) -> List[SgNote]:
+        """Get SG Notes by Project
         
         Parameters
         ----------
         project_id : int
             ShotGrid Project ID.
         
         Returns
         -------
-        list[dict]
-            List of dict or empty list if no results from ShotGrid
+        list[SgNote]
+            List of SgNote or empty list if no results from ShotGrid
         
         """
         filters = [
             [
                 "project",
                 "is",
                 [
                     {
                         "id": project_id,
                         "type": SgEntity.PROJECT,
                     }
                 ]
             ]
         ]
-        fields = [
-            "subject",
-            "content",
-            "note_links",
-        ]
+        fields = NOTE_FIELDS
 
-        notes = self.sg.find(SgEntity.NOTE, filters, fields)
+        notes_ = self.sg.find(SgEntity.NOTE, filters, fields)
+        notes = [SgNote.from_dict(n) for n in notes_]
         return notes
 
-    def get_sg_shots(
+    def get_sg_assets(
+            self,
+            assets_id: Union[int, Set[int], List[int]],
+            custom_fields: Optional[List[str]] = None,
+    ) -> List[SgAsset]:
+        """Get SG Assets
+
+        Parameters
+        ----------
+        custom_fields: list[str]
+        assets_id : int | set[int] | list[int]
+            ShotGrid Asset ID.
+
+        Returns
+        -------
+        list of SgAsset
+            List of SgAsset or empty list if no results from ShotGrid
+
+        Notes
+        -----
+        If content is 'Idle' or 'Report', the entity value will be None
+
+        """
+        if isinstance(assets_id, int):
+            assets_id = [assets_id]
+
+        if isinstance(assets_id, set):
+            assets_id = list(assets_id)
+
+        filters = [
+            [
+                "id",
+                "in",
+                assets_id
+            ]
+        ]
+        fields = ASSET_FIELDS
+        if custom_fields:
+            fields = custom_fields
+
+        # If content is 'Idle', the entity value will be None
+        assets_: List[dict] = self.sg.find(SgEntity.ASSET, filters, fields)
+        assets = [SgAsset.from_dict(t) for t in assets_]
+        return assets
+
+    def get_sg_shots_by_project(
             self,
             project_id: int,
             custom_fields: Optional[List[str]] = None,
-    ) -> List[dict]:
+    ) -> List[SgShot]:
         """Get SG Shots
         
         Parameters
         ----------
         project_id : int
             ShotGrid Project ID.
         custom_fields: list[str]
             List of custom fields
         
         Returns
         -------
-        list[dict]
-            List of dict or empty list if no results from ShotGrid
+        list[SgShot]
+            List of SgShot or empty list if no results from ShotGrid
             
         """
         filters = [
             [
                 "project",
                 "is",
                 [
                     {
                         "id": project_id,
                         "type": SgEntity.PROJECT,
                     }
                 ]
             ]
         ]
-        fields = [
-            "code",
-            "description",
-        ]
+        fields = SHOT_FIELDS
         if custom_fields:
             fields = custom_fields
 
-        notes = self.sg.find(SgEntity.SHOT, filters, fields)
-        return notes
+        shots_ = self.sg.find(SgEntity.SHOT, filters, fields)
+        shots = [SgShot.from_dict(s) for s in shots_]
+        return shots
 
     def get_sg_tasks(
             self,
             tasks_id: Union[int, Set[int], List[int]],
             custom_fields: Optional[List[str]] = None,
-    ) -> List[dict]:
+    ) -> List[SgTask]:
         """Get SG Tasks
 
         Parameters
         ----------
         custom_fields: list[str]
         tasks_id : int | set[int] | list[int]
             ShotGrid Task ID.
 
         Returns
         -------
-        list
-            List of dict or empty list if no results from ShotGrid
+        list of SgTask
+            List of SgTask or empty list if no results from ShotGrid
 
         Notes
         -----
         If content is 'Idle' or 'Report', the entity value will be None
 
         """
         if isinstance(tasks_id, int):
@@ -805,27 +930,84 @@
         filters = [
             [
                 "id",
                 "in",
                 tasks_id
             ]
         ]
-        fields = [
-            "content",
-            "entity",
-            "project",
-        ]
+        fields = TASK_FIELDS
         if custom_fields:
             fields = custom_fields
 
         # If content is 'Idle', the entity value will be None
-        tasks = self.sg.find(SgEntity.TASK, filters, fields)
+        tasks_: List[dict] = self.sg.find(SgEntity.TASK, filters, fields)
+        tasks = [SgTask.from_dict(t) for t in tasks_]
         return tasks
 
-    def bulk_update_sg_task_status(self, task_ids: List[int], status: str) -> bool:
+    def create_sg_task(self, data: SgTask) -> bool:
+        """Create SG Task
+
+        Create SG Task entity. Refer to the data structure in Examples for
+        the bare minimum key values to successfully create a Task entity.
+
+        Parameters
+        ----------
+        data : SgTask
+            The SG Task data for create
+
+        Returns
+        -------
+        bool
+            True if created successfully
+
+        Examples
+        --------
+        Content: Valid string format
+            {
+                "project": {
+                    "id": 280,
+                    "type": "Project"
+                },
+                "content": "Report",
+                "task_assignees": [
+                    {
+                        "id": 970,
+                        "type": SgEntity.HUMANUSER
+                    }
+                ],
+            }
+
+        """
+        is_created = True
+        if data.sg_status_list:
+            valid_values = self.get_valid_values(SgEntity.TASK, "sg_status_list")
+            if data.sg_status_list not in valid_values:
+                raise Exception(f"Invalid {data.sg_status_list} value! Valid values: {valid_values}")
+
+        data_ = data.to_dict()
+
+        try:
+            self.sg.create("Task", data_)
+        except (shotgun_api3.Fault, shotgun_api3.ShotgunError) as e:
+            logger.error(
+                {
+                    "msg": "Fail to create SG task",
+                    "error": e,
+                    "data": data,
+                }
+            )
+            is_created = False
+
+        return is_created
+
+    def bulk_update_sg_task_status(
+            self,
+            task_ids: List[int],
+            status: str,
+    ) -> bool:
         """Bulk Update SG Task Status
 
         Parameters
         ----------
         task_ids : list[int]
             List of Task IDs for bulk update
         status : str
@@ -833,14 +1015,18 @@
 
         Returns
         -------
         bool
             True if bulk update successfully
 
         """
+        valid_values = self.get_valid_values(SgEntity.TASK, "sg_status_list")
+        if status not in valid_values:
+            raise Exception(f"Invalid {status} value! Valid values: {valid_values}")
+
         batch_data = []
         for task_id in task_ids:
             request_data = {
                 "request_type": "update",
                 "entity_id": task_id,
                 "entity_type": SgEntity.TASK,
                 "data": {
@@ -861,14 +1047,60 @@
                     "task ids": task_ids,
                 }
             )
             is_bulk_updated = False
 
         return is_bulk_updated
 
+    def get_sg_versions(
+            self,
+            versions_id: Union[int, Set[int], List[int]],
+            custom_fields: Optional[List[str]] = None,
+    ) -> List[SgVersion]:
+        """Get SG Versions
+
+        Parameters
+        ----------
+        custom_fields: list[str]
+            Optional. List of valid fields for SG Version.
+        versions_id : int | set[int] | list[int]
+            ShotGrid Version ID.
+
+        Returns
+        -------
+        list of SgVersion
+            List of SgVersion or empty list if no results from ShotGrid
+
+        Notes
+        -----
+        If content is 'Idle' or 'Report', the entity value will be None
+
+        """
+        if isinstance(versions_id, int):
+            versions_id = [versions_id]
+
+        if isinstance(versions_id, set):
+            versions_id = list(versions_id)
+
+        filters = [
+            [
+                "id",
+                "in",
+                versions_id
+            ]
+        ]
+        fields = VERSION_FIELDS
+        if custom_fields:
+            fields = custom_fields
+
+        # If content is 'Idle', the entity value will be None
+        versions_: List[dict] = self.sg.find(SgEntity.VERSION, filters, fields)
+        versions = [SgVersion.from_dict(t) for t in versions_]
+        return versions
+
     def get_sg_timelogs(
             self,
             sg_humanuser_id: int,
             custom_fields: Optional[List[str]] = None,
     ) -> List[dict]:
         """Get SG Timelogs
 
@@ -893,21 +1125,15 @@
                     {
                         "id": sg_humanuser_id,
                         "type": SgEntity.HUMANUSER,
                     }
                 ]
             ]
         ]
-        fields = [
-            "date",
-            "description",
-            "duration",
-            "project",
-            "user",
-        ]
+        fields = TIMELOG_FIELDS
         if custom_fields:
             fields = custom_fields
 
         timelogs = self.sg.find(SgEntity.TIMELOG, filters, fields)
         return timelogs
 
     def create_sg_timelog(self, data: SgTimeLog) -> dict:
@@ -1095,57 +1321,7 @@
                     "error": e,
                     "task ids": sg_timelog_ids,
                 }
             )
             is_bulk_delete_timelog_successful = False
 
         return is_bulk_delete_timelog_successful
-
-    def create_sg_task(self, data: dict) -> bool:
-        """Create SG Task
-
-        Create SG Task entity. Refer to the data structure in Examples for
-        the bare minimum key values to successfully create a Task entity.
-
-        Parameters
-        ----------
-        data : dict
-            The SG Task data for create
-
-        Returns
-        -------
-        bool
-            True if created successfully
-
-        Examples
-        --------
-        Content: Valid string format
-            {
-                "project": {
-                    "id": 280,
-                    "type": "Project"
-                },
-                "content": "Report",
-                "task_assignees": [
-                    {
-                        "id": 970,
-                        "type": SgEntity.HUMANUSER
-                    }
-                ],
-            }
-
-        """
-        is_created = True
-
-        try:
-            self.sg.create("Task", data)
-        except (shotgun_api3.Fault, shotgun_api3.ShotgunError) as e:
-            logger.error(
-                {
-                    "msg": "Fail to create SG task",
-                    "error": e,
-                    "data": data,
-                }
-            )
-            is_created = False
-
-        return is_created
```

### Comparing `konbinine-0.1.5/konbinine/enums.py` & `konbinine-0.1.6/konbinine/enums.py`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.5/konbinine/models.py` & `konbinine-0.1.6/konbinine/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import asdict, dataclass, field
 from typing import Any, Dict, List, Optional
 
 from konbinine.enums import SgEntity
 from konbinine.exceptions import (
     InvalidSgDateFormatException,
 )
+from konbinine.types import TSgUploadedMovie
 from konbinine.utils import (
     get_current_utc_dt,
     SG_DATE_FORMAT,
     validate_sg_date_format,
 )
 
 # TODO: Use Python 3.10+ kw_only but that is another headache for maintenance...
@@ -59,31 +60,54 @@
 class SgGenericEntity(SgIdMixin, SgBaseModel):
     name: str = ""
     type: str = ""
 
 
 @dataclass
 class SgNote(SgIdMixin, SgBaseModel):
-    name: str = ""
+    subject: str = ""
+    content: str = ""
+    sg_status_list: str = ""
+    note_links: list[SgGenericEntity] = field(default_factory=list)
     type: str = SgEntity.NOTE
 
+    @classmethod
+    def from_dict(cls, dict_):
+        params = inspect.signature(cls).parameters
+
+        sanitized_dict = {}
+        for k, v in dict_.items():
+            if k == "note_links" and v:
+                v = [SgGenericEntity.from_dict(_v) for _v in v]
+
+            sanitized_dict[k] = v
+
+        return cls(
+            **{
+                k: v for k, v in sanitized_dict.items()
+                if k in params
+            }
+        )
+
 
 @dataclass
 class SgProject(SgIdMixin, SgBaseModel):
     name: str = ""
     type: str = SgEntity.PROJECT
     archived: bool = False
     code: Optional[str] = None
     sg_description: Optional[str] = None
     sg_status: Optional[str] = None
     sg_type: Optional[str] = None
     start_date: Optional[str] = None  # Date uses YYYY-MM-DD format
     end_date: Optional[str] = None
     updated_at: Optional[datetime.datetime] = None  # Example 2023-08-07T06:29:35Z
-    image: Optional[str] = None
+    image: Optional[str] = None  # When retrieve from SG API, should be the URL path
+    filmstrip_image: Optional[str] = None
+    image_upload: Optional[str] = None  # For uploading to SG (str, bytes or os.PathLike object)
     duration: Optional[int] = None  # Number of days
 
     def validate_stale_data(self) -> bool:
         current_dt = get_current_utc_dt()
         return self.updated_at > current_dt
 
 
@@ -98,28 +122,45 @@
 class SgPipelineStep(SgIdMixin, _SgPipelineStep):
     pass
 
 
 @dataclass
 class _SgVersion(SgBaseModel):
     code: str  # Version Name
-    entity: Optional[dict] = None  # Link
-    notes: List[SgNote] = field(default_factory=list)
+    description: Optional[str] = None
+    flagged: bool = False
+    image: Optional[str] = None
+    filmstrip_image: Optional[str] = None
+    entity: Optional[SgGenericEntity] = None  # Link
+    sg_task: Optional[SgGenericEntity] = None
+    sg_uploaded_movie: Optional[TSgUploadedMovie] = None
+    sg_uploaded_movie_mp4: Optional[TSgUploadedMovie] = None
+    sg_uploaded_movie_webm: Optional[TSgUploadedMovie] = None
+    sg_path_to_frames: Optional[str] = None
+    sg_path_to_movie: Optional[str] = None
+    sg_status_list: str = ""
+    uploaded_movie_duration: Optional[str] = None
+    sg_uploaded_movie_frame_rate: Optional[str] = None
+    notes: List[SgGenericEntity] = field(default_factory=list)
     type: str = SgEntity.VERSION
 
     @classmethod
     def from_dict(cls, dict_):
         params = inspect.signature(cls).parameters
 
         sanitized_dict = {}
         for k, v in dict_.items():
             if "." in k:
                 k = k.replace(".", "__")
+            if k == "entity" and v:
+                v = SgGenericEntity.from_dict(v)
+            if k == "sg_task" and v:
+                v = SgGenericEntity.from_dict(v)
             if k == "notes" and v:
-                v = [SgNote.from_dict(_v) for _v in v]
+                v = [SgGenericEntity.from_dict(_v) for _v in v]
 
             sanitized_dict[k] = v
 
         return cls(
             **{
                 k: v for k, v in sanitized_dict.items()
                 if k in params
@@ -131,55 +172,72 @@
 class SgVersion(SgIdMixin, _SgVersion):
     pass
 
 
 @dataclass
 class _SgShot(SgBaseModel):
     code: str  # Shot Code
+    description: Optional[str] = None
+    image: Optional[str] = None
+    filmstrip_image: Optional[str] = None
+    sg_cut_in: Optional[int] = None
+    sg_cut_out: Optional[int] = None
+    sg_cut_duration: Optional[int] = None
+    sg_status_list: str = ""
+    sg_shot_type: str = ""
     type: str = SgEntity.SHOT
 
 
 @dataclass
 class SgShot(SgIdMixin, _SgShot):
     pass
 
 
 @dataclass
 class _SgTask(SgBaseModel):
     name: str
     short_name: str = ""
     content: str = ""
+    sg_status_list: str = ""
     entity: Optional[SgGenericEntity] = None
     project: Optional[SgProject] = None
     type: str = SgEntity.TASK
 
 
 @dataclass
 class SgTask(SgIdMixin, _SgTask):
     pass
 
 
 @dataclass
 class _SgAsset(SgBaseModel):
     code: str  # Shot Code
     tasks: List[SgTask] = field(default_factory=list)
+    notes: list[SgGenericEntity] = field(default_factory=list)
+    image: Optional[str] = None
+    filmstrip_image: Optional[str] = None
+    sg_asset_type: str = ""
+    sg_status_list: str = ""
     type: str = SgEntity.ASSET
 
     @classmethod
     def from_dict(cls, dict_):
         params = inspect.signature(cls).parameters
 
         sanitized_dict = {}
         for k, v in dict_.items():
             if "." in k:
                 k = k.replace(".", "__")
 
             if k == "tasks" and v:
                 v = [SgTask.from_dict(_v) for _v in v]
 
+            if k == "notes" and v:
+                v = [SgGenericEntity.from_dict(_v) for _v in v]
+
             sanitized_dict[k] = v
 
         return cls(
             **{
                 k: v for k, v in sanitized_dict.items()
                 if k in params
             }
@@ -225,14 +283,15 @@
 @dataclass
 class _SgHumanUser(SgBaseModel):
     login: str
     name: str = ""
     firstname: str = ""
     lastname: str = ""
     email: str = ""
+    sg_status_list: str = ""
     file_access: bool = False
     type: str = SgEntity.HUMANUSER
     image: Optional[str] = None
     projects: Optional[List[dict]] = None
     groups: Optional[List[dict]] = None
 
     def to_dict(self) -> Dict[str, Any]:
@@ -253,14 +312,15 @@
 @dataclass
 class _SgBooking(SgBaseModel):
     user: SgHumanUser
     start_date: str
     end_date: str
     vacation: bool = True
     note: str = ""
+    sg_status_list: str = ""
     type: str = SgEntity.BOOKING
 
     @classmethod
     def from_dict(cls, dict_):
         params = inspect.signature(cls).parameters
 
         sanitized_dict = {}
@@ -292,32 +352,32 @@
 
 @dataclass
 class _SgTimeLog(SgBaseModel):
     date: str
     description: str = ""
     duration: float = 0.0
     entity: Optional[SgGenericEntity] = None
-    project: Optional[SgProject] = None
-    user: Optional[SgHumanUser] = None
+    project: Optional[SgGenericEntity] = None
+    user: Optional[SgGenericEntity] = None
     type: str = SgEntity.TIMELOG
 
     @classmethod
     def from_dict(cls, dict_):
         params = inspect.signature(cls).parameters
 
         sanitized_dict = {}
         for k, v in dict_.items():
             if k == "entity" and v:
                 v = SgGenericEntity.from_dict(v)
 
             if k == "project" and v:
-                v = SgProject.from_dict(v)
+                v = SgGenericEntity.from_dict(v)
 
             if k == "user" and v:
-                v = SgHumanUser.from_dict(v)
+                v = SgGenericEntity.from_dict(v)
 
             sanitized_dict[k] = v
 
         return cls(
             **{
                 k: v for k, v in sanitized_dict.items()
                 if k in params
```

### Comparing `konbinine-0.1.5/konbinine/utils.py` & `konbinine-0.1.6/konbinine/utils.py`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.5/konbinine.egg-info/PKG-INFO` & `konbinine-0.1.6/konbinine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.5
+Version: 0.1.6
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
@@ -54,18 +54,19 @@
 because the API usage requirements is 便利じゃないでしょう？
 
 > コンビニね～ As there is an existing PyPI project using **_konbini_** name, this repo project name
 > on PyPI will be **konbinine**.
 
 ## How to Use
 
-> For Python 3.7 and newer! While Autodesk made **shotgun_api3** to be compatible with Python 2 and 3, **konbinine**
-> uses `dataclass` that is only available in Python 3.7 onwards.
+> For Python 3.8 and newer! While Autodesk made **shotgun_api3** to be compatible with Python 2 and 3, **konbinine**
+> uses `dataclass` that is only available in Python 3.7 onwards. Starting with v0.1.6, Python 3.8 will be the minimum
+> version due to the usage of TypedDict.
 
-**konbinine** is designed to be use with web framework (such as Django, Flask, etc) that interacts with ShotGrid. This
+**konbinine** is designed to be used with web framework (such as Django, Flask, etc.) that interacts with ShotGrid. This
 library has not been tested inside Digital Content Creation (DCC) software such as Maya, 3ds Max or Houdini.
 
 Technically it should just work but that is outside the scope of this library.
 
 ### New Project
 
 #### First time setup
@@ -107,7 +108,12 @@
 ```commandline
 pip install -r requirements.txt
 ```
 
 ## Extending konbinine
 
 Coming soon!
+
+## TODO
+
+1. Implement `Sequence` dataclass
+2. Handle Image/Movie upload gracefully (currently for Project entity only)
```

### Comparing `konbinine-0.1.5/pyproject.toml` & `konbinine-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.5/setup.cfg` & `konbinine-0.1.6/setup.cfg`

 * *Files identical despite different names*

