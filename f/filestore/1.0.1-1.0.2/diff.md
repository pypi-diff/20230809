# Comparing `tmp/filestore-1.0.1.tar.gz` & `tmp/filestore-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filestore-1.0.1.tar", last modified: Sun Aug  6 11:29:35 2023, max compression
+gzip compressed data, was "filestore-1.0.2.tar", last modified: Tue Aug  8 22:13:45 2023, max compression
```

## Comparing `filestore-1.0.1.tar` & `filestore-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 11:29:35.936185 filestore-1.0.1/
--rw-rw-rw-   0        0        0     1092 2023-07-20 04:55:35.000000 filestore-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    11030 2023-08-06 11:29:35.932187 filestore-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10399 2023-08-06 11:10:38.000000 filestore-1.0.1/README.md
--rw-rw-rw-   0        0        0      845 2023-08-06 11:10:38.000000 filestore-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 11:29:35.937188 filestore-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 11:29:35.582189 filestore-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 11:29:35.780969 filestore-1.0.1/src/filestore/
--rw-rw-rw-   0        0        0      257 2023-08-05 22:07:21.000000 filestore-1.0.1/src/filestore/__init__.py
--rw-rw-rw-   0        0        0     3745 2023-08-06 11:10:38.000000 filestore-1.0.1/src/filestore/localstorage.py
--rw-rw-rw-   0        0        0    14124 2023-08-06 11:04:44.000000 filestore-1.0.1/src/filestore/main.py
--rw-rw-rw-   0        0        0     1333 2023-07-30 14:58:06.000000 filestore-1.0.1/src/filestore/memorystorage.py
--rw-rw-rw-   0        0        0     4675 2023-08-06 11:10:38.000000 filestore-1.0.1/src/filestore/s3.py
--rw-rw-rw-   0        0        0      894 2023-08-05 21:46:09.000000 filestore-1.0.1/src/filestore/util.py
-drwxrwxrwx   0        0        0        0 2023-08-06 11:29:35.923183 filestore-1.0.1/src/filestore.egg-info/
--rw-rw-rw-   0        0        0    11030 2023-08-06 11:29:35.000000 filestore-1.0.1/src/filestore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-08-06 11:29:35.000000 filestore-1.0.1/src/filestore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 11:29:35.000000 filestore-1.0.1/src/filestore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-08-06 11:29:35.000000 filestore-1.0.1/src/filestore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 11:29:35.000000 filestore-1.0.1/src/filestore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-06 11:29:35.928186 filestore-1.0.1/tests/
--rw-rw-rw-   0        0        0     3360 2023-08-06 11:10:38.000000 filestore-1.0.1/tests/test_fast_store.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:13:45.509750 filestore-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-20 04:55:35.000000 filestore-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    11281 2023-08-08 22:13:45.507756 filestore-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10650 2023-08-08 21:45:17.000000 filestore-1.0.2/README.md
+-rw-rw-rw-   0        0        0      845 2023-08-08 22:12:30.000000 filestore-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 22:13:45.509750 filestore-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 22:13:45.052751 filestore-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 22:13:45.374755 filestore-1.0.2/src/filestore/
+-rw-rw-rw-   0        0        0      257 2023-08-05 22:07:21.000000 filestore-1.0.2/src/filestore/__init__.py
+-rw-rw-rw-   0        0        0     3745 2023-08-06 11:10:38.000000 filestore-1.0.2/src/filestore/localstorage.py
+-rw-rw-rw-   0        0        0    14187 2023-08-08 21:47:18.000000 filestore-1.0.2/src/filestore/main.py
+-rw-rw-rw-   0        0        0     1333 2023-07-30 14:58:06.000000 filestore-1.0.2/src/filestore/memorystorage.py
+-rw-rw-rw-   0        0        0     4675 2023-08-06 11:10:38.000000 filestore-1.0.2/src/filestore/s3.py
+-rw-rw-rw-   0        0        0      894 2023-08-05 21:46:09.000000 filestore-1.0.2/src/filestore/util.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:13:45.469748 filestore-1.0.2/src/filestore.egg-info/
+-rw-rw-rw-   0        0        0    11281 2023-08-08 22:13:45.000000 filestore-1.0.2/src/filestore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-08-08 22:13:45.000000 filestore-1.0.2/src/filestore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 22:13:45.000000 filestore-1.0.2/src/filestore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-08-08 22:13:45.000000 filestore-1.0.2/src/filestore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 22:13:45.000000 filestore-1.0.2/src/filestore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 22:13:45.502761 filestore-1.0.2/tests/
+-rw-rw-rw-   0        0        0     3360 2023-08-06 11:10:38.000000 filestore-1.0.2/tests/test_fast_store.py
```

### Comparing `filestore-1.0.1/LICENSE` & `filestore-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `filestore-1.0.1/PKG-INFO` & `filestore-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,13 @@
-Metadata-Version: 2.1
-Name: filestore
-Version: 1.0.1
-Summary: Storage Engine Package for FastAPI
-Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
-Project-URL: Homepage, https://github.com/Ichinga-Samuel/faststore
-Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/faststore/issues
-Keywords: fastapi,filestorage,cloudstorage,storageengine,faststore
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: s3
-License-File: LICENSE
-
 # FileStore
+![GitHub](https://img.shields.io/github/license/ichinga-samuel/faststore?style=plastic)
+![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/faststore?style=plastic)
+![PyPI](https://img.shields.io/pypi/v/filestore)
 
+## Introduction
 Simple file storage dependency for FastAPI. Makes use of FastAPI's dependency injection system to provide a simple way
 to store files. Inspired by Multer it allows both single and multiple file uploads through different fields with a 
 simple interface. Comes with a default implementation for local file storage, simple in-memory storage and AWS S3
 storage but can be easily extended to support other storage systems.
 
 ## Installation
 
@@ -131,44 +119,44 @@
 
 ### Filename and Destination Function. 
 You can specify a filename and destination function for customizing a filename and specifying a storage location for the saved file.
 The filename function should modify the filename attribute of the file and return the modified file while the destination function should return a path or string object. This functions have access to the request object, the form, the form field and the file objects.
 
 #### A destination function
 ```python
-def local_destination(req: Request, form: Form, field: str, file: UploadFile) -> Path:
+def local_destination(req: Request, form: FormData, field: str, file: UploadFile) -> Path:
     """
     Local storage destination function.
     Pass this function to the LocalStorage config parameter 'destination' to create a destination for the file.
     Creates a directory named after the field inside the test_data/uploads folder if it doesn't exist.
 
     Returns:
         Path: Path to the stored file.
     """
     path = Path.cwd() / f'test_data/uploads/{field}'
     path.mkdir(parents=True, exist_ok=True) if not path.exists() else ...
     return path / f'{file.filename}'
 ```
 #### A filename function
 ```python
-def local_filename(req: Request, form: Form, field: str, file: UploadFile) -> UploadFile:
+def local_filename(req: Request, form: FormData, field: str, file: UploadFile) -> UploadFile:
     """
     Local storage filename function. Appends 'local_' to the filename.
 
     Returns:
         UploadFile: The file with the new filename.
     """
     file.filename = f'local_{file.filename}'
     return file
 ```
 
 ### Filtering
 Set this to a function to control which files should be uploaded and which should be skipped. The function should look like this:
 ```python
-def local_filter(req: Request, form: Form, field: str, file: UploadFile) -> bool:
+def local_filter(req: Request, form: FormData, field: str, file: UploadFile) -> bool:
     """
     Local storage filter function.
     Returns:
         bool: True if the file is a text file, False otherwise.
     """
     return file.filename and file.filename.endswith('.txt')
 ```
@@ -226,13 +214,7 @@
 ### Background Tasks
 You can run the file storage operation as a background task by setting the background config parameter to True.
 
 ### Build your own storage class
 You can build your own storage class by inheriting from the FastStore class and implementing the **upload** and 
 **multiple_upload** methods. Just make sure you properly set the private **_result** attribute with the result of the file 
 storage operation.
-
-
-
-
-
-
```

### Comparing `filestore-1.0.1/README.md` & `filestore-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,29 @@
+Metadata-Version: 2.1
+Name: filestore
+Version: 1.0.2
+Summary: Storage Engine Package for FastAPI
+Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
+Project-URL: Homepage, https://github.com/Ichinga-Samuel/faststore
+Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/faststore/issues
+Keywords: fastapi,filestorage,cloudstorage,storageengine,faststore
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: s3
+License-File: LICENSE
+
 # FileStore
+![GitHub](https://img.shields.io/github/license/ichinga-samuel/faststore?style=plastic)
+![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/faststore?style=plastic)
+![PyPI](https://img.shields.io/pypi/v/filestore)
 
+## Introduction
 Simple file storage dependency for FastAPI. Makes use of FastAPI's dependency injection system to provide a simple way
 to store files. Inspired by Multer it allows both single and multiple file uploads through different fields with a 
 simple interface. Comes with a default implementation for local file storage, simple in-memory storage and AWS S3
 storage but can be easily extended to support other storage systems.
 
 ## Installation
 
@@ -115,44 +135,44 @@
 
 ### Filename and Destination Function. 
 You can specify a filename and destination function for customizing a filename and specifying a storage location for the saved file.
 The filename function should modify the filename attribute of the file and return the modified file while the destination function should return a path or string object. This functions have access to the request object, the form, the form field and the file objects.
 
 #### A destination function
 ```python
-def local_destination(req: Request, form: Form, field: str, file: UploadFile) -> Path:
+def local_destination(req: Request, form: FormData, field: str, file: UploadFile) -> Path:
     """
     Local storage destination function.
     Pass this function to the LocalStorage config parameter 'destination' to create a destination for the file.
     Creates a directory named after the field inside the test_data/uploads folder if it doesn't exist.
 
     Returns:
         Path: Path to the stored file.
     """
     path = Path.cwd() / f'test_data/uploads/{field}'
     path.mkdir(parents=True, exist_ok=True) if not path.exists() else ...
     return path / f'{file.filename}'
 ```
 #### A filename function
 ```python
-def local_filename(req: Request, form: Form, field: str, file: UploadFile) -> UploadFile:
+def local_filename(req: Request, form: FormData, field: str, file: UploadFile) -> UploadFile:
     """
     Local storage filename function. Appends 'local_' to the filename.
 
     Returns:
         UploadFile: The file with the new filename.
     """
     file.filename = f'local_{file.filename}'
     return file
 ```
 
 ### Filtering
 Set this to a function to control which files should be uploaded and which should be skipped. The function should look like this:
 ```python
-def local_filter(req: Request, form: Form, field: str, file: UploadFile) -> bool:
+def local_filter(req: Request, form: FormData, field: str, file: UploadFile) -> bool:
     """
     Local storage filter function.
     Returns:
         bool: True if the file is a text file, False otherwise.
     """
     return file.filename and file.filename.endswith('.txt')
 ```
@@ -210,13 +230,7 @@
 ### Background Tasks
 You can run the file storage operation as a background task by setting the background config parameter to True.
 
 ### Build your own storage class
 You can build your own storage class by inheriting from the FastStore class and implementing the **upload** and 
 **multiple_upload** methods. Just make sure you properly set the private **_result** attribute with the result of the file 
 storage operation.
-
-
-
-
-
-
```

### Comparing `filestore-1.0.1/pyproject.toml` & `filestore-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "filestore"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `filestore-1.0.1/src/filestore/localstorage.py` & `filestore-1.0.2/src/filestore/localstorage.py`

 * *Files identical despite different names*

### Comparing `filestore-1.0.1/src/filestore/main.py` & `filestore-1.0.2/src/filestore/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import Any, Type, cast, TypedDict, TypeVar, NotRequired, Callable
 from abc import abstractmethod
 from pathlib import Path
 from logging import getLogger
 from functools import cache
 from random import randint
 
-from starlette.datastructures import UploadFile as StarletteUploadFile
+from starlette.datastructures import UploadFile as StarletteUploadFile, FormData
 from fastapi import Request, UploadFile as UF, Form, BackgroundTasks
 from pydantic import BaseModel, create_model, Field
 
 from .util import FormModel
 
 Fields = TypedDict('Fields', {'name': str, 'max_count': NotRequired[int], 'required': NotRequired[bool]})
 
@@ -48,35 +48,35 @@
         return cast(UploadFile, __input_value)
 
 
 def _file_filter(file):
     return isinstance(file, StarletteUploadFile)
 
 
-def file_filter(req: Request, form: Form, field: str, file: UploadFile) -> bool:
+def file_filter(req: Request, form: FormData, field: str, file: UploadFile) -> bool:
     """
     The default filter function for the FastStore class.
     Args:
         req (Request): The request object.
-        form (Form): The form object.
+        form (FormData): The form data object.
         field (Field): The name of the field.
         file (UploadFile): The file object.
 
     Returns (bool): True if the file is valid, False otherwise.
     """
     return isinstance(file, StarletteUploadFile) and file.filename
 
 
-def filename(req: Request, form: Form, field: str, file: UploadFile) -> UploadFile:
+def filename(req: Request, form: FormData, field: str, file: UploadFile) -> UploadFile:
     """
     Update the filename of the file object.
 
     Args:
         req (Request): The request object.
-        form (Form): The form object.
+        form (FormData): The form data object.
         field (Field): The name of the field.
         file (UploadFile): The file object.
 
     Returns (UploadFile): The file object with the updated filename.
     """
     return file
 
@@ -157,15 +157,15 @@
     This class is used to upload files to a storage service.
     It is an abstract class and must be inherited from.
     The upload and multi_upload methods must be implemented in a child class.
 
     Attributes:
         fields (list[Fields]): The fields to expect from the form.
         request (Request): The request object.
-        form (Form): The form object.
+        form (FormData): The form data object.
         config (dict): The configuration for the storage service.
         _result (Result): The result of the file storage operation.
         result (Result): Property to access and set the result of the file storage operation.
         max_count (int): The maximum number of files to accept for all fields.
         background_tasks (BackgroundTasks): The background tasks object for running tasks in the background.
 
     Methods:
@@ -176,32 +176,32 @@
     Config:
         max_files (int): The maximum number of files to accept in a single request. Defaults to 1000.
 
         max_fields (int): The maximum number of fields to accept in a single request. Defaults to 1000.
 
         dest (str | Path): Destination to save the file to in the storage service defaults to 'uploads'.
 
-        filename (Callable[[Request, Form, str, UploadFile], UploadFile): A function that takes in the request,
+        filename (Callable[[Request, FormData, str, UploadFile], UploadFile): A function that takes in the request,
             form and file, filename modifies the filename attribute of the file and returns the file.
 
-        destination (Callable[[Request, Form, str, UploadFile], str | Path]): A function that takes in the request,
+        destination (Callable[[Request, FormData, str, UploadFile], str | Path]): A function that takes in the request,
             form and file and returns a path to save the file to in the storage service.
 
-        filter (Callable[[Request, Form, str, UploadFile], bool]): A function that takes in the request, form and file
-            and returns a boolean.
+        filter (Callable[[Request, FormData, str, UploadFile], bool]): A function that takes in the request,
+            form and file and returns a boolean.
 
         background (bool): A boolean to indicate if the file storage operation should be run in the background.
 
         extra_args (dict): Extra arguments to pass to the storage service.
 
         bucket (str): The name of the bucket to upload the file to in the cloud storage service.
     """
     fields: list[Fields]
     config: Config
-    form: Form
+    form: FormData
     request: Request
     result: Result
     background_tasks: BackgroundTasks
     max_count: int
     _result: Result
 
     def __init__(self, name: str = '', count: int = 1, required=False, fields: list[Fields] | None = None,
@@ -298,15 +298,15 @@
 
     @abstractmethod
     async def multi_upload(self, *, field_files: list[tuple[str, UploadFile]]):
         """
         Upload multiple files to a storage service.
 
         Args:
-            field_files (list[tuple[str, UploadFile]]): A list of tuples containing the name of the file field and the
+            field_files (list[tuple[str, UploadFile]]): A list of tuples containing the field names and files to upload.
         """
 
     @property
     def result(self) -> Result:
         """
         Returns the result of the file storage.
```

### Comparing `filestore-1.0.1/src/filestore/memorystorage.py` & `filestore-1.0.2/src/filestore/memorystorage.py`

 * *Files identical despite different names*

### Comparing `filestore-1.0.1/src/filestore/s3.py` & `filestore-1.0.2/src/filestore/s3.py`

 * *Files identical despite different names*

### Comparing `filestore-1.0.1/src/filestore/util.py` & `filestore-1.0.2/src/filestore/util.py`

 * *Files identical despite different names*

### Comparing `filestore-1.0.1/src/filestore.egg-info/PKG-INFO` & `filestore-1.0.2/src/filestore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: filestore
-Version: 1.0.1
+Version: 1.0.2
 Summary: Storage Engine Package for FastAPI
 Author-email: Ichinga Samuel <ichingasamuel@gmail.com>
 Project-URL: Homepage, https://github.com/Ichinga-Samuel/faststore
 Project-URL: Bug Tracker, https://github.com/Ichinga-Samuel/faststore/issues
 Keywords: fastapi,filestorage,cloudstorage,storageengine,faststore
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: s3
 License-File: LICENSE
 
 # FileStore
+![GitHub](https://img.shields.io/github/license/ichinga-samuel/faststore?style=plastic)
+![GitHub issues](https://img.shields.io/github/issues/ichinga-samuel/faststore?style=plastic)
+![PyPI](https://img.shields.io/pypi/v/filestore)
 
+## Introduction
 Simple file storage dependency for FastAPI. Makes use of FastAPI's dependency injection system to provide a simple way
 to store files. Inspired by Multer it allows both single and multiple file uploads through different fields with a 
 simple interface. Comes with a default implementation for local file storage, simple in-memory storage and AWS S3
 storage but can be easily extended to support other storage systems.
 
 ## Installation
 
@@ -131,44 +135,44 @@
 
 ### Filename and Destination Function. 
 You can specify a filename and destination function for customizing a filename and specifying a storage location for the saved file.
 The filename function should modify the filename attribute of the file and return the modified file while the destination function should return a path or string object. This functions have access to the request object, the form, the form field and the file objects.
 
 #### A destination function
 ```python
-def local_destination(req: Request, form: Form, field: str, file: UploadFile) -> Path:
+def local_destination(req: Request, form: FormData, field: str, file: UploadFile) -> Path:
     """
     Local storage destination function.
     Pass this function to the LocalStorage config parameter 'destination' to create a destination for the file.
     Creates a directory named after the field inside the test_data/uploads folder if it doesn't exist.
 
     Returns:
         Path: Path to the stored file.
     """
     path = Path.cwd() / f'test_data/uploads/{field}'
     path.mkdir(parents=True, exist_ok=True) if not path.exists() else ...
     return path / f'{file.filename}'
 ```
 #### A filename function
 ```python
-def local_filename(req: Request, form: Form, field: str, file: UploadFile) -> UploadFile:
+def local_filename(req: Request, form: FormData, field: str, file: UploadFile) -> UploadFile:
     """
     Local storage filename function. Appends 'local_' to the filename.
 
     Returns:
         UploadFile: The file with the new filename.
     """
     file.filename = f'local_{file.filename}'
     return file
 ```
 
 ### Filtering
 Set this to a function to control which files should be uploaded and which should be skipped. The function should look like this:
 ```python
-def local_filter(req: Request, form: Form, field: str, file: UploadFile) -> bool:
+def local_filter(req: Request, form: FormData, field: str, file: UploadFile) -> bool:
     """
     Local storage filter function.
     Returns:
         bool: True if the file is a text file, False otherwise.
     """
     return file.filename and file.filename.endswith('.txt')
 ```
@@ -226,13 +230,7 @@
 ### Background Tasks
 You can run the file storage operation as a background task by setting the background config parameter to True.
 
 ### Build your own storage class
 You can build your own storage class by inheriting from the FastStore class and implementing the **upload** and 
 **multiple_upload** methods. Just make sure you properly set the private **_result** attribute with the result of the file 
 storage operation.
-
-
-
-
-
-
```

### Comparing `filestore-1.0.1/tests/test_fast_store.py` & `filestore-1.0.2/tests/test_fast_store.py`

 * *Files identical despite different names*

