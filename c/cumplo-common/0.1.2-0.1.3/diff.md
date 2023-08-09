# Comparing `tmp/cumplo_common-0.1.2.tar.gz` & `tmp/cumplo_common-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumplo_common-0.1.2.tar", max compression
+gzip compressed data, was "cumplo_common-0.1.3.tar", max compression
```

## Comparing `cumplo_common-0.1.2.tar` & `cumplo_common-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-08-04 22:48:00.735339 cumplo_common-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-08-04 22:49:44.133087 cumplo_common-0.1.2/README.md
--rw-r--r--   0        0        0      105 2023-08-08 23:46:37.127497 cumplo_common-0.1.2/cumplo_common/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 21:08:12.823188 cumplo_common-0.1.2/cumplo_common/database/__init__.py
--rw-r--r--   0        0        0     5389 2023-08-05 21:18:50.983861 cumplo_common-0.1.2/cumplo_common/database/firestore.py
--rw-r--r--   0        0        0     1504 2023-08-05 21:24:45.780295 cumplo_common-0.1.2/cumplo_common/integrations/cloud_tasks.py
--rw-r--r--   0        0        0      694 2023-08-07 22:56:57.754118 cumplo_common-0.1.2/cumplo_common/middlewares/authentication.py
--rw-r--r--   0        0        0      372 2023-08-05 21:26:47.630268 cumplo_common-0.1.2/cumplo_common/middlewares/authorization.py
--rw-r--r--   0        0        0        0 2023-08-05 21:08:18.258596 cumplo_common-0.1.2/cumplo_common/models/__init__.py
--rw-r--r--   0        0        0     1669 2023-08-04 23:07:25.517655 cumplo_common-0.1.2/cumplo_common/models/configuration.py
--rw-r--r--   0        0        0      402 2023-08-04 23:11:28.896994 cumplo_common-0.1.2/cumplo_common/models/notification.py
--rw-r--r--   0        0        0      517 2023-08-04 23:09:27.965311 cumplo_common-0.1.2/cumplo_common/models/user.py
--rw-r--r--   0        0        0        0 2023-08-08 23:44:08.032473 cumplo_common-0.1.2/cumplo_common/py.typed
--rw-r--r--   0        0        0        0 2023-08-05 21:08:31.777792 cumplo_common-0.1.2/cumplo_common/utils/__init__.py
--rw-r--r--   0        0        0      369 2023-08-05 21:24:15.107625 cumplo_common-0.1.2/cumplo_common/utils/constants.py
--rw-r--r--   0        0        0      189 2023-08-05 20:59:13.277955 cumplo_common-0.1.2/cumplo_common/utils/currency.py
--rw-r--r--   0        0        0      701 2023-08-05 20:58:12.453196 cumplo_common-0.1.2/cumplo_common/utils/text.py
--rw-r--r--   0        0        0      677 2023-08-08 23:48:24.693382 cumplo_common-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 cumplo_common-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-08-04 22:48:00.735339 cumplo_common-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-08-04 22:49:44.133087 cumplo_common-0.1.3/README.md
+-rw-r--r--   0        0        0      105 2023-08-09 00:27:46.789766 cumplo_common-0.1.3/cumplo_common/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:08:12.823188 cumplo_common-0.1.3/cumplo_common/database/__init__.py
+-rw-r--r--   0        0        0     6425 2023-08-09 00:15:06.589694 cumplo_common-0.1.3/cumplo_common/database/firestore.py
+-rw-r--r--   0        0        0     2113 2023-08-09 00:06:35.811417 cumplo_common-0.1.3/cumplo_common/integrations/cloud_tasks.py
+-rw-r--r--   0        0        0      962 2023-08-09 00:12:02.984407 cumplo_common-0.1.3/cumplo_common/middlewares/authentication.py
+-rw-r--r--   0        0        0      501 2023-08-09 00:12:31.866674 cumplo_common-0.1.3/cumplo_common/middlewares/authorization.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:08:18.258596 cumplo_common-0.1.3/cumplo_common/models/__init__.py
+-rw-r--r--   0        0        0     1903 2023-08-09 00:15:07.872851 cumplo_common-0.1.3/cumplo_common/models/configuration.py
+-rw-r--r--   0        0        0       84 2023-08-09 00:21:37.135260 cumplo_common-0.1.3/cumplo_common/models/currency.py
+-rw-r--r--   0        0        0      592 2023-08-09 00:15:53.054284 cumplo_common-0.1.3/cumplo_common/models/notification.py
+-rw-r--r--   0        0        0      517 2023-08-04 23:09:27.965311 cumplo_common-0.1.3/cumplo_common/models/user.py
+-rw-r--r--   0        0        0        0 2023-08-08 23:44:08.032473 cumplo_common-0.1.3/cumplo_common/py.typed
+-rw-r--r--   0        0        0        0 2023-08-05 21:08:31.777792 cumplo_common-0.1.3/cumplo_common/utils/__init__.py
+-rw-r--r--   0        0        0      394 2023-08-09 00:16:25.895180 cumplo_common-0.1.3/cumplo_common/utils/constants.py
+-rw-r--r--   0        0        0      505 2023-08-09 00:22:01.892991 cumplo_common-0.1.3/cumplo_common/utils/currency.py
+-rw-r--r--   0        0        0      930 2023-08-09 00:25:04.452398 cumplo_common-0.1.3/cumplo_common/utils/text.py
+-rw-r--r--   0        0        0      677 2023-08-09 00:27:54.114001 cumplo_common-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 cumplo_common-0.1.3/PKG-INFO
```

### Comparing `cumplo_common-0.1.2/LICENSE` & `cumplo_common-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cumplo_common-0.1.2/cumplo_common/database/firestore.py` & `cumplo_common-0.1.3/cumplo_common/database/firestore.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,23 +25,36 @@
         firebase_credentials = credentials.ApplicationDefault()
         initialize_app(firebase_credentials, {"projectId": PROJECT_ID})
         self.client = firestore.client()
 
     def get_users(self) -> Generator[User, None, None]:
         """
         Gets all the users data
+
+        Yields:
+            Generator[User, None, None]: Iterable of User objects
         """
         logger.info("Getting all users from Firestore")
         user_stream = self.client.collection(USERS_COLLECTION).stream()
         for user in user_stream:
             yield User(id=user.id, **user.to_dict())
 
     def get_user(self, api_key: str) -> User:
         """
-        Gets the user data
+        Gets the user data for a given API key
+
+        Args:
+            api_key (str): User API key
+
+        Raises:
+            KeyError: When the user does not exist
+            ValueError: When the user data is empty
+
+        Returns:
+            User: A User object containing the user data
         """
         logger.info(f"Getting user with API key {secure_key(api_key)} from Firestore")
         filter_ = FieldFilter("api_key", "==", api_key)
         user_stream = self.client.collection(USERS_COLLECTION).where(filter=filter_).stream()
 
         if not (user := next(user_stream, None)):
             raise KeyError(f"User with API key {secure_key(api_key)} does not exist")
@@ -51,39 +64,55 @@
 
         configurations = self._get_user_configurations(user.id)
         notifications = self._get_user_notifications(user.id)
         return User(id=user.id, configurations=configurations, notifications=notifications, **user_data)
 
     def update_notification(self, id_user: str, id_funding_request: int) -> None:
         """
-        Updates the notification for a given user
+        Updates the notification for a given user and funding request
+
+        Args:
+            id_user (str): A user ID which owns the notification
+            id_funding_request (int): A funding request ID
         """
         logger.info(f"Updating notification for funding request {id_funding_request} at Firestore")
         notification = self._get_notification_document(id_user, id_funding_request)
         notification.set({"date": arrow.utcnow().datetime})
 
     def update_configuration(self, id_user: str, configuration: Configuration) -> None:
         """
         Updates a configuration of a given user
+
+        Args:
+            id_user (str): A user ID which owns the configuration
+            configuration (Configuration): A Configuration object containing the new configuration data to be updated
         """
         logger.info(f"Updating configuration {configuration.id} of user {id_user} at Firestore")
         configuration_reference = self._get_configuration_document(id_user, configuration.id)
-        configuration_reference.set(configuration.serialize(to_firestore=True))
+        configuration_reference.set(configuration.serialize(for_firestore=True))
 
     def delete_notification(self, id_user: str, id_funding_request: int) -> None:
         """
         Deletes a notification of a funding request for a given user
+
+        Args:
+            id_user (str): A user ID which owns the notification
+            id_funding_request (int): A funding request ID to be deleted
         """
         logger.info(f"Deleting notification {id_funding_request} from Firestore")
         notification = self._get_notification_document(id_user, id_funding_request)
         notification.delete()
 
     def delete_configuration(self, id_user: str, id_configuration: int) -> None:
         """
-        Deletes a configuration for a given user
+        Deletes a configuration for a given user and configuration ID
+
+        Args:
+            id_user (str): A user ID which owns the configuration
+            id_configuration (int): A configuration ID to be deleted
         """
         logger.info(f"Deleting configuration {id_configuration} from Firestore")
         configuration = self._get_configuration_document(id_user, id_configuration)
         configuration.delete()
 
     def _get_user_document(self, id_user: str) -> DocumentReference:
         """Gets a user document reference"""
```

### Comparing `cumplo_common-0.1.2/cumplo_common/integrations/cloud_tasks.py` & `cumplo_common-0.1.3/cumplo_common/integrations/cloud_tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from datetime import datetime
 from typing import Annotated
 
+import arrow
 from google.cloud.tasks_v2 import CloudTasksClient, CreateTaskRequest, HttpMethod, HttpRequest, Task
 from google.protobuf.duration_pb2 import Duration
 from google.protobuf.timestamp_pb2 import Timestamp
 
 from cumplo_common.utils.constants import LOCATION, PROJECT_ID
 
 
@@ -16,16 +17,30 @@
     task_id: str,
     dispatch_deadline: int | None = None,
     schedule_time: datetime | None = None,
     http_method: Annotated[int, HttpMethod] = HttpMethod.POST,
 ) -> Task:
     """
     Create an HTTP POST task with a JSON payload.
+
+    Args:
+        url (str): Destination URL
+        queue (str): Queue name
+        payload (dict): Request JSON payload
+        task_id (str): Task identifier
+        dispatch_deadline (int | None, optional): Seconds until the task is dispatched. Defaults to None.
+        schedule_time (datetime | None, optional): Time at which the task will be scheduled. Defaults to None.
+        http_method (Annotated[int, HttpMethod], optional): HTTP method to use. Defaults to HttpMethod.POST.
+
+    Returns:
+        Task: A unit of scheduled work
     """
     client = CloudTasksClient()
+
+    task_id = f"{task_id}-{arrow.utcnow().timestamp}"
     name = client.task_path(PROJECT_ID, LOCATION, queue, task_id)
 
     http_request = HttpRequest(
         url=url,
         http_method=http_method,
         body=json.dumps(payload).encode(),
         headers={"Content-type": "application/json"},
```

### Comparing `cumplo_common-0.1.2/cumplo_common/middlewares/authentication.py` & `cumplo_common-0.1.3/cumplo_common/middlewares/authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 from fastapi.requests import Request
 
 from cumplo_common.database.firestore import firestore_client
 
 
 async def authenticate(request: Request, x_api_key: Annotated[str | None, Header] = None) -> None:
     """
-    Authenticates a request.
+    Authenticates a request using the X-API-KEY header
+
+    Args:
+        request (Request): The request to authenticate
+        x_api_key (Annotated[str  |  None, Header], optional): API key header. Defaults to None.
+
+    Raises:
+        HTTPException: When the API key is not present or invalid
     """
     if not x_api_key:
         raise HTTPException(status_code=HTTPStatus.UNAUTHORIZED)
 
     try:
         user = firestore_client.get_user(x_api_key)
     except (KeyError, ValueError):
```

### Comparing `cumplo_common-0.1.2/cumplo_common/models/configuration.py` & `cumplo_common-0.1.3/cumplo_common/models/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,25 @@
     def __hash__(self) -> int:
         exclude = {"id", "name", "expiration_minutes"}
         return hash(self.model_dump_json(exclude=exclude, exclude_defaults=True, exclude_none=True))
 
     def __eq__(self, other: Any) -> bool:
         return self.__hash__() == other.__hash__()
 
-    def serialize(self, to_firestore: bool = False) -> dict[str, Any]:
-        """Serializes a configuration"""
-        if to_firestore:
+    def serialize(self, for_firestore: bool = False) -> dict[str, Any]:
+        """
+        Serializes the configuration
+
+        Args:
+            for_firestore (bool, optional): Whether to serialize for Firestore or not. Defaults to False.
+
+        Returns:
+            dict[str, Any]: The serialized configuration as a dictionary
+        """
+        if for_firestore:
             content = self.model_dump(exclude_none=True, exclude={"id"})
             for key, value in content.items():
                 if isinstance(value, Decimal):
                     content[key] = float(value)
             return content
 
         return self.model_dump(exclude_none=True)
```

### Comparing `cumplo_common-0.1.2/cumplo_common/models/user.py` & `cumplo_common-0.1.3/cumplo_common/models/user.py`

 * *Files identical despite different names*

### Comparing `cumplo_common-0.1.2/cumplo_common/utils/text.py` & `cumplo_common-0.1.3/cumplo_common/utils/text.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 SEPARATORS = ["_", "-"]
 
 
 def clean_text(error: str) -> str:
     """
     Cleans a text by removing punctuation and normalizing unicode characters
+
+    Args:
+        error (str): The text to be cleaned
+
+    Returns:
+        str: The cleaned text
     """
     for separator in SEPARATORS:
         error = " ".join(error.split(separator))
 
     return " ".join(
         unicodedata.normalize("NFD", error)
         .encode("ASCII", "ignore")
@@ -21,10 +27,16 @@
         .upper()
         .split()
     )
 
 
 def secure_key(key: str) -> str:
     """
-    Returns a secure version of a key
+    Returns a secure version of a key for logging purposes
+
+    Args:
+        key (str): The key to be secured
+
+    Returns:
+        str: A loggable version of the key
     """
     return f"{key[:5]}{'*' * (len(key) - 15)}{key[-10:]}"
```

### Comparing `cumplo_common-0.1.2/pyproject.toml` & `cumplo_common-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cumplo-common"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python library that contains all common logic throughout Cumplo API project"
 authors = ["Cristobal Sfeir <cnsfeir@uc.cl>"]
 readme = "README.md"
 packages = [{ include = "cumplo_common" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `cumplo_common-0.1.2/PKG-INFO` & `cumplo_common-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumplo-common
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library that contains all common logic throughout Cumplo API project
 Author: Cristobal Sfeir
 Author-email: cnsfeir@uc.cl
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
```

