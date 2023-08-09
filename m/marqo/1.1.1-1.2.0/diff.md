# Comparing `tmp/marqo-1.1.1.tar.gz` & `tmp/marqo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-1.1.1.tar", last modified: Fri Jul 28 06:39:55 2023, max compression
+gzip compressed data, was "marqo-1.2.0.tar", last modified: Wed Aug  9 05:09:04 2023, max compression
```

## Comparing `marqo-1.1.1.tar` & `marqo-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:39:55.546959 marqo-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-28 06:39:44.000000 marqo-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-28 06:39:55.546959 marqo-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-28 06:39:44.000000 marqo-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-28 06:39:44.000000 marqo-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 06:39:55.546959 marqo-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 06:39:44.000000 marqo-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:39:55.542959 marqo-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:39:55.542959 marqo-1.1.1/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25718 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/marqo_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/marqo_url_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 06:39:44.000000 marqo-1.1.1/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 06:39:55.546959 marqo-1.1.1/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 06:39:55.000000 marqo-1.1.1/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:09:04.896136 marqo-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-09 05:08:50.000000 marqo-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-08-09 05:09:04.896136 marqo-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-08-09 05:08:50.000000 marqo-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-09 05:08:50.000000 marqo-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 05:09:04.896136 marqo-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-09 05:08:50.000000 marqo-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:09:04.892136 marqo-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:09:04.896136 marqo-1.2.0/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/cloud_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/default_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29748 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/marqo_cloud_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/marqo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-09 05:08:50.000000 marqo-1.2.0/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:09:04.896136 marqo-1.2.0/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-08-09 05:09:04.000000 marqo-1.2.0/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-09 05:09:04.000000 marqo-1.2.0/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 05:09:04.000000 marqo-1.2.0/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-09 05:09:04.000000 marqo-1.2.0/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-09 05:09:04.000000 marqo-1.2.0/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-1.1.1/LICENSE` & `marqo-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-1.1.1/PKG-INFO` & `marqo-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 1.1.1
+Version: 1.2.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 1.1.1 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 1.2.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
```

### Comparing `marqo-1.1.1/README.md` & `marqo-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `marqo-1.1.1/setup.py` & `marqo-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         "packaging"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="1.1.1",
+    version="1.2.0",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-1.1.1/src/marqo/_httprequests.py` & `marqo-1.2.0/src/marqo/_httprequests.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,19 @@
         if method not in ALLOWED_OPERATIONS:
             raise ValueError("{} not an allowed operation {}".format(method, ALLOWED_OPERATIONS))
 
         return OPERATION_MAPPING[method]
 
     def _construct_path(self, path: str, index_name="") -> str:
         """Augment the URL request path based if telemetry is required."""
-        url = f"{self.config.get_url(index_name=index_name)}/{path}"
+        base_url = self.config.instance_mapping.get_index_base_url(index_name=index_name) if index_name \
+            else self.config.instance_mapping.get_control_base_url()
+        url = f"{base_url}/{path}"
         if self.config.use_telemetry:
-            delimeter= "?" if "?" not in f"{self.config.url}/{path}" else "&"
+            delimeter= "?" if "?" not in f"{base_url}/{path}" else "&"
             return url + f"{delimeter}telemetry=True"
         return url
 
     def send_request(
         self,
         http_operation: HTTP_OPERATIONS,
         path: str,
```

### Comparing `marqo-1.1.1/src/marqo/client.py` & `marqo-1.2.0/src/marqo/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,77 @@
 import base64
+import os
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import error_wrappers
 from requests.exceptions import RequestException
+from typing_extensions import deprecated
 
+from marqo.cloud_helpers import cloud_wait_for_index_status
+from marqo.default_instance_mappings import DefaultInstanceMappings
 from marqo.index import Index
 from marqo.config import Config
+from marqo.instance_mappings import InstanceMappings
+from marqo.marqo_cloud_instance_mappings import MarqoCloudInstanceMappings
 from marqo.models import BulkSearchBody, BulkSearchQuery
 from marqo._httprequests import HttpRequests
 from marqo import utils, enums
 from marqo import errors
-from marqo.version import minimum_supported_marqo_version
 from marqo.marqo_logging import mq_logger
 from marqo.errors import MarqoWebError
 # we want to avoid name conflicts with marqo.version
-from packaging import version as versioning_helpers
 from json import JSONDecodeError
 
 # A dictionary to cache the marqo url and version for compatibility check
-marqo_url_and_version_cache = {}
 
 
 class Client:
     """
     A client for the marqo API
 
     A client instance is needed for every marqo API method to know the location of
     marqo and its permissions.
     """
 
     def __init__(
-            self, url: str = "http://localhost:8882",
+            self, url: Optional[str] = "http://localhost:8882",
+            instance_mappings: Optional[InstanceMappings] = None,
             main_user: str = None, main_password: str = None,
             return_telemetry: bool = False,
             api_key: str = None
     ) -> None:
         """
         Parameters
         ----------
         url:
-            The url to the S2Search API (ex: http://localhost:8882)
+            The url to the Marqo API (ex: http://localhost:8882) If MARQO_CLOUD_URL environment variable is set, when
+            matching url is passed, the client will use the Marqo Cloud instance mappings.
+        instance_mappings:
+            An instance of InstanceMappings that maps index names to urls
+        api_key:
+            The api key to use for authentication with the Marqo API
         """
-        self.main_user = main_user
-        self.main_password = main_password
-        if (main_user is not None) and (main_password is not None):
-            self.url = utils.construct_authorized_url(url_base=url, username=main_user, password=main_password)
-        else:
-            self.url = url
-        self.config = Config(self.url, use_telemetry=return_telemetry, api_key=api_key)
+        if url is not None and instance_mappings is not None:
+            raise ValueError("Cannot specify both url and instance_mappings")
+
+        is_marqo_cloud = False
+        if url is not None:
+            if url.lower().startswith(os.environ.get("MARQO_CLOUD_URL", "https://api.marqo.ai")):
+                instance_mappings = MarqoCloudInstanceMappings(control_base_url=url, api_key=api_key)
+                is_marqo_cloud = True
+            else:
+                instance_mappings = DefaultInstanceMappings(url, main_user, main_password)
+
+        self.config = Config(
+            instance_mappings=instance_mappings,
+            is_marqo_cloud=is_marqo_cloud,
+            use_telemetry=return_telemetry,
+            api_key=api_key
+        )
         self.http = HttpRequests(self.config)
-        self._marqo_minimum_supported_version_check()
 
     def create_index(
             self, index_name: str,
             treat_urls_and_pointers_as_images=False, model=None,
             normalize_embeddings=True,
             sentences_per_chunk=2,
             sentence_overlap=0,
@@ -104,14 +122,15 @@
             index_name: name of the index
 
         Returns:
             response body about the result of the delete request
         """
         try:
             res = self.http.delete(path=f"indexes/{index_name}")
+            cloud_wait_for_index_status(self.http, index_name, enums.IndexStatus.DELETED)
         except errors.MarqoWebError as e:
             return e.message
 
     def get_index(self, index_name: str) -> Index:
         """Get the index.
         This index should already exist.
 
@@ -157,23 +176,14 @@
                 config=self.config,
                 index_name=index_info["index_name"],
             )
             for index_info in response["results"]
         ]
         return response
 
-    def enrich(self, documents: List[Dict], enrichment: Dict, device: str = None, ):
-        """Enrich documents"""
-        translated = utils.translate_device_string_for_url(device)
-        response = self.http.post(path=f'enrichment?device={translated}', body={
-            "documents": documents,
-            "enrichment": enrichment
-        })
-        return response
-
     def bulk_search(self, queries: List[Dict[str, Any]], device: Optional[str] = None) -> Dict[str, Any]:
         try:
             parsed_queries = [BulkSearchBody(**q) for q in queries]
         except error_wrappers.ValidationError as e:
             raise errors.InvalidArgError(f"some parameters in search query(s) are invalid. Errors are: {e.errors()}")
 
         translated_device_param = f"{f'?&device={utils.translate_device_string_for_url(device)}' if device is not None else ''}"
@@ -184,68 +194,81 @@
 
     @staticmethod
     def _base64url_encode(
             data: bytes
     ) -> str:
         return base64.urlsafe_b64encode(data).decode('utf-8').replace('=', '')
 
+    @deprecated(
+        "This method is deprecated and will be removed in Marqo 2.0.0. "
+        "Please use `mq.index(index_name).get_marqo()` instead. "
+        "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details."
+    )
     def get_marqo(self):
+        if self.config.is_marqo_cloud:
+            self.raise_error_for_cloud("get_marqo")
         return self.http.get(path="")
 
+    @deprecated(
+        "This method is deprecated and will be removed in Marqo 2.0.0. "
+        "Please use `mq.index(index_name).health()` instead. "
+        "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details."
+    )
     def health(self):
-        mq_logger.warning('The `client.health()` API has been deprecated and will be removed in '
-                          'Marqo 2.0.0. Use `client.index(index_name).health()` instead. '
-                          'Check `https://docs.marqo.ai/latest/API-Reference/indexes/` for more details.')
+        if self.config.is_marqo_cloud:
+            self.raise_error_for_cloud("health")
         try:
             return self.http.get(path="health")
         except (MarqoWebError, RequestException, TypeError, KeyError) as e:
             raise errors.BadRequestError("Marqo encountered an error trying to check the health of the Marqo instance. "
                                          "If you are trying to check the health on Marqo Cloud, please note that "
                                          "the `client.health()` API is not supported on Marqo Cloud and will be removed in "
                                          "Marqo 2.0.0. Please Use `client.index('your-index-name').health()` instead. "
                                          "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details.")
 
+    @deprecated(
+        "This method is deprecated and will be removed in Marqo 2.0.0. "
+        "Please use 'mq.index(index_name).eject_model() instead. "
+        "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details."
+    )
     def eject_model(self, model_name: str, model_device: str):
+        if self.config.is_marqo_cloud:
+            self.raise_error_for_cloud("eject_model")
         return self.http.delete(path=f"models?model_name={model_name}&model_device={model_device}")
 
+    @deprecated(
+        "This method is deprecated and will be removed in Marqo 2.0.0. "
+        "Please use 'mq.index(index_name).get_loaded_models() instead. "
+        "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details."
+    )
     def get_loaded_models(self):
+        if self.config.is_marqo_cloud:
+            self.raise_error_for_cloud("get_loaded_models")
         return self.http.get(path="models")
 
+    @deprecated(
+        "This method is deprecated and will be removed in Marqo 2.0.0. "
+        "Please use 'mq.index(index_name).get_cuda_info() instead. "
+        "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details."
+    )
     def get_cuda_info(self):
+        if self.config.is_marqo_cloud:
+            self.raise_error_for_cloud("get_cuda_info")
         return self.http.get(path="device/cuda")
 
+    @deprecated(
+        "This method is deprecated and will be removed in Marqo 2.0.0. "
+        "Please use 'mq.index(index_name).get_cpu_info() instead. "
+        "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details."
+    )
     def get_cpu_info(self):
+        if self.config.is_marqo_cloud:
+            self.raise_error_for_cloud("get_cpu_info")
         return self.http.get(path="device/cpu")
 
-    def _marqo_minimum_supported_version_check(self):
-        min_ver = minimum_supported_marqo_version()
-        skip_warning_message = (
-            f"Marqo encountered a problem trying to check the Marqo version found at `{self.url}`. "
-            f"The minimum supported Marqo version for this client is {min_ver}. "
-            f"If you are sure your Marqo version is compatible with this client, you can ignore this message. ")
-
-        # Skip the check if the url is previously labelled as "_skipped"
-        if self.url in marqo_url_and_version_cache and marqo_url_and_version_cache[self.url] == "_skipped":
-            mq_logger.warning(skip_warning_message)
-            return
-
-        # Skip the check for Marqo CloudV2 APIs right now
-        skip_version_check_url = ["https://api.marqo.ai", "https://cloud.marqo.ai"]
-        if self.url in skip_version_check_url:
-            marqo_url_and_version_cache[self.url] = "_skipped"
-            mq_logger.warning(skip_warning_message)
-            return
+    @staticmethod
+    def raise_error_for_cloud(function_name: str = None):
+        raise errors.BadRequestError(
+            f"The `mq.{function_name}()` API is not supported on Marqo Cloud. "
+            f"Please Use `mq.index('your-index-name').{function_name}()` instead. "
+            "Check `https://docs.marqo.ai/1.1.0/API-Reference/indexes/` for more details.")
 
-        # Do version check
-        try:
-            if self.url not in marqo_url_and_version_cache:
-                marqo_url_and_version_cache[self.url] = self.get_marqo()["version"]
-            marqo_version = marqo_url_and_version_cache[self.url]
-            if versioning_helpers.parse(marqo_version) < versioning_helpers.parse(min_ver):
-                mq_logger.warning(f"Your Marqo Python client requires a minimum Marqo version of "
-                                  f"{minimum_supported_marqo_version()} to function properly, but your Marqo version is {marqo_version}. "
-                                  f"Please upgrade your Marqo instance to avoid potential errors. "
-                                  f"If you have already changed your Marqo instance but still get this warning, please restart your Marqo client Python interpreter.")
-        except (MarqoWebError, RequestException, TypeError, KeyError) as e:
-            mq_logger.warning(skip_warning_message)
-            marqo_url_and_version_cache[self.url] = "_skipped"
-        return
```

### Comparing `marqo-1.1.1/src/marqo/defaults.py` & `marqo-1.2.0/src/marqo/defaults.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.1/src/marqo/errors.py` & `marqo-1.2.0/src/marqo/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,18 @@
 
     def __init__(self, message: str):
         self.message = message
 
     error_type = "invalid_request"
 
 
+class UnsupportedOperationError(__InvalidRequestError):
+    code = "unsupported_operation"
+
+
 class IndexAlreadyExistsError(__InvalidRequestError):
     code = "index_already_exists"
     status_code = HTTPStatus.CONFLICT
 
 
 class IndexNotFoundError(__InvalidRequestError):
     code = "index_not_found"
```

### Comparing `marqo-1.1.1/src/marqo/index.py` & `marqo-1.2.0/src/marqo/index.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import functools
 import json
-import logging
 import pprint
 import time
 
+from requests import RequestException
+
 from marqo import defaults
+from marqo.cloud_helpers import cloud_wait_for_index_status
+from marqo.enums import IndexStatus
 import typing
 from urllib import parse
 from datetime import datetime
 from timeit import default_timer as timer
 from typing import Any, Dict, Generator, List, Optional, Union
 from marqo._httprequests import HttpRequests
 from marqo.config import Config
 from marqo.enums import SearchMethods, Devices
 from marqo import errors, utils
+from marqo.errors import MarqoWebError, UnsupportedOperationError
 from marqo.marqo_logging import mq_logger
+from marqo.version import minimum_supported_marqo_version
+from packaging import version as versioning_helpers
+
+marqo_url_and_version_cache: Dict[str, str] = {}
 
 
 class Index:
     """
     Wraps the /indexes/ endpoint
     """
 
@@ -38,19 +46,37 @@
             updated_at:
         """
         self.config = config
         self.http = HttpRequests(config)
         self.index_name = index_name
         self.created_at = self._maybe_datetime(created_at)
         self.updated_at = self._maybe_datetime(updated_at)
+        skip_version_check = False
+        if config.is_marqo_cloud:
+            try:
+                if self.get_status()["index_status"] != IndexStatus.CREATED:
+                    mq_logger.warning(f"Index {index_name} is not ready. Status: {self.get_status()}. Common operations, "
+                                    f"such as search and add_documents, may fail until the index is ready. "
+                                    f"Please check `mq.index('{index_name}').get_status()` for the index's status. "
+                                    f"Skipping version check.")
+                    skip_version_check = True
+            except (MarqoWebError, TypeError, KeyError) as e:
+                skip_version_check = True
+                mq_logger.warning(f"Failed to get index status for index {index_name}. Skipping version check. Error: {e}")
+        if not skip_version_check:
+            self._marqo_minimum_supported_version_check()
 
     def delete(self) -> Dict[str, Any]:
         """Delete the index.
         """
-        return self.http.delete(path=f"indexes/{self.index_name}")
+        response = self.http.delete(path=f"indexes/{self.index_name}")
+        if self.config.is_marqo_cloud:
+            cloud_wait_for_index_status(self.http, self.index_name, IndexStatus.DELETED)
+        return response
+
 
     @staticmethod
     def create(config: Config, index_name: str,
                treat_urls_and_pointers_as_images=False,
                model=None,
                normalize_embeddings=True,
                sentences_per_chunk=2,
@@ -84,43 +110,43 @@
             replicas_count: number of replicas for the index
         Returns:
             Response body, containing information about index creation result
         """
         req = HttpRequests(config)
 
         if settings_dict is not None and settings_dict:
-            return req.post(f"indexes/{index_name}", body=settings_dict)
+            response = req.post(f"indexes/{index_name}", body=settings_dict)
+            if config.is_marqo_cloud:
+                cloud_wait_for_index_status(req, index_name, IndexStatus.CREATED)
+            return response
 
         if config.api_key is not None:
             # making the keyword settings params override the default cloud
             #  settings
             cl_settings = defaults.get_cloud_default_index_settings()
             cl_ix_defaults = cl_settings['index_defaults']
             cl_ix_defaults['treat_urls_and_pointers_as_images'] = treat_urls_and_pointers_as_images
-            cl_ix_defaults['model'] = model
+            if model is not None:
+                cl_ix_defaults['model'] = model
             cl_ix_defaults['normalize_embeddings'] = normalize_embeddings
             cl_text_preprocessing = cl_ix_defaults['text_preprocessing']
             cl_text_preprocessing['split_overlap'] = sentence_overlap
             cl_text_preprocessing['split_length'] = sentences_per_chunk
             cl_img_preprocessing = cl_ix_defaults['image_preprocessing']
-            cl_img_preprocessing['patch_method'] = image_preprocessing_method
-            if not config.cluster_is_marqo:
+            if image_preprocessing_method is not None:
+                cl_img_preprocessing['patch_method'] = image_preprocessing_method
+            if not config.is_marqo_cloud:
                 return req.post(f"indexes/{index_name}", body=cl_settings)
             cl_settings['inference_type'] = inference_node_type
             cl_settings['storage_class'] = storage_node_type
             cl_settings['number_of_inferences'] = inference_node_count
             cl_settings['number_of_replicas'] = replicas_count
             cl_settings['number_of_shards'] = storage_node_count
             response = req.post(f"indexes/{index_name}", body=cl_settings)
-            index = Index(config, index_name)
-            creation = index.get_status()
-            while creation['index_status'] != 'READY':
-                time.sleep(10)
-                creation = index.get_status()
-                mq_logger.info(f"Index creation status: {creation['index_status']}")
+            cloud_wait_for_index_status(req, index_name, IndexStatus.CREATED)
             return response
 
         return req.post(f"indexes/{index_name}", body={
             "index_defaults": {
                 "treat_urls_and_pointers_as_images": treat_urls_and_pointers_as_images,
                 "model": model,
                 "normalize_embeddings": normalize_embeddings,
@@ -137,15 +163,18 @@
 
     def refresh(self):
         """refreshes the index"""
         return self.http.post(path=F"indexes/{self.index_name}/refresh", index_name=self.index_name,)
 
     def get_status(self):
         """gets the status of the index"""
-        return self.http.get(path=F"indexes/{self.index_name}/status")
+        if self.config.is_marqo_cloud:
+            return self.http.get(path=F"indexes/{self.index_name}/status")
+        else:
+            raise UnsupportedOperationError("This operation is only supported for Marqo Cloud")
 
     def search(self, q: Union[str, dict], searchable_attributes: Optional[List[str]] = None,
                limit: int = 10, offset: int = 0, search_method: Union[SearchMethods.TENSOR, str] = SearchMethods.TENSOR,
                highlights=None, device: Optional[str] = None, filter_string: str = None,
                show_highlights=True, reranker=None, image_download_headers: Optional[Dict] = None,
                attributes_to_retrieve: Optional[List[str]] = None, boost: Optional[Dict[str,List[Union[float, int]]]] = None,
                context: Optional[dict] = None, score_modifiers: Optional[dict] = None, model_auth: Optional[dict] = None
@@ -405,15 +434,14 @@
             errors_detected = False
 
             if 'processingTimeMs' in res:       # Only outputs log if response is non-empty
                 mq_logger.debug(f"add_documents Marqo index: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} "
                                 f"docs (server unbatched), for an average of {(res['processingTimeMs'] / (1000 * num_docs)):.3f}s per doc.")
             if 'errors' in res and res['errors']:
                 mq_logger.info(error_detected_message)
-
             if errors_detected:
                 mq_logger.info(error_detected_message)
         total_add_docs_time = timer() - t0
         mq_logger.debug(f"add_documents completed. total time taken: {(total_add_docs_time):.3f}s.")
         return res
 
     def delete_documents(self, ids: List[str], auto_refresh: bool = None) -> Dict[str, int]:
@@ -546,7 +574,53 @@
     def get_settings(self) -> dict:
         """Get all settings of the index"""
         return self.http.get(path=f"indexes/{self.index_name}/settings", index_name=self.index_name,)
 
     def health(self) -> dict:
         """Check the health of an index"""
         return self.http.get(path=f"indexes/{self.index_name}/health", index_name=self.index_name)
+
+    def get_loaded_models(self):
+        return self.http.get(path="models", index_name=self.index_name)
+
+    def get_cuda_info(self):
+        return self.http.get(path="device/cuda", index_name=self.index_name)
+
+    def get_cpu_info(self):
+        return self.http.get(path="device/cpu", index_name=self.index_name)
+
+    def get_marqo(self):
+        return self.http.get(path="", index_name=self.index_name)
+
+    def eject_model(self, model_name: str, model_device: str):
+        return self.http.delete(
+            path=f"models?model_name={model_name}&model_device={model_device}", index_name=self.index_name
+        )
+
+    def _marqo_minimum_supported_version_check(self):
+        min_ver = minimum_supported_marqo_version()
+        url = self.config.instance_mapping.get_index_base_url(self.index_name)
+        skip_warning_message = (
+            f"Marqo encountered a problem trying to check the Marqo version found at `{url}`. "
+            f"The minimum supported Marqo version for this client is {min_ver}. "
+            f"If you are sure your Marqo version is compatible with this client, you can ignore this message. ")
+
+        # Skip the check if the url is previously labelled as "_skipped"
+        if url in marqo_url_and_version_cache and marqo_url_and_version_cache[url] == "_skipped":
+            mq_logger.warning(skip_warning_message)
+            return
+
+        # Do version check
+        try:
+            if url not in marqo_url_and_version_cache:
+                marqo_url_and_version_cache[url] = self.get_marqo()["version"]
+            marqo_version = marqo_url_and_version_cache[url]
+            if versioning_helpers.parse(marqo_version) < versioning_helpers.parse(min_ver):
+                mq_logger.warning(f"Your Marqo Python client requires a minimum Marqo version of "
+                                  f"{minimum_supported_marqo_version()} to function properly, but your Marqo version is {marqo_version}. "
+                                  f"Please upgrade your Marqo instance to avoid potential errors. "
+                                  f"If you have already changed your Marqo instance but still get this warning, please restart your Marqo client Python interpreter.")
+        except (MarqoWebError, RequestException, TypeError, KeyError) as e:
+            mq_logger.warning(skip_warning_message)
+            marqo_url_and_version_cache[url] = "_skipped"
+        return
+
```

### Comparing `marqo-1.1.1/src/marqo/marqo_url_resolver.py` & `marqo-1.2.0/src/marqo/marqo_cloud_instance_mappings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 import time
-from marqo.marqo_logging import mq_logger
+from typing import Optional
+
 import requests
 from requests.exceptions import Timeout
+
 from marqo.errors import (
     MarqoCloudIndexNotFoundError,
     MarqoCloudIndexNotReadyError,
 )
+from marqo.instance_mappings import InstanceMappings
+from marqo.marqo_logging import mq_logger
 
 
-class MarqoUrlResolver:
-    def __init__(self, api_key=None, expiration_time: int = 15):
-        """ URL Resolver is a cache for urls that are resolved to their respective indices only for marqo cloud. """
-        self.timestamp = time.time() - expiration_time
+class MarqoCloudInstanceMappings(InstanceMappings):
+    def __init__(self, control_base_url, api_key=None, url_cache_duration: int = 15):
+        self.latest_index_mappings_refresh_timestamp = time.time() - url_cache_duration
         self._urls_mapping = {"READY": {}, "CREATING": {}}
         self.api_key = api_key
-        self.expiration_time = expiration_time
+        self.url_cache_duration = url_cache_duration
+        self._control_base_url = control_base_url
+
+    def get_control_base_url(self) -> str:
+        return f"{self._control_base_url}/api"
 
-    def refresh_urls_if_needed(self, index_name):
-        if index_name not in self._urls_mapping['READY'] and time.time() - self.timestamp > self.expiration_time:
+    def get_index_base_url(self, index_name: str) -> str:
+        self._refresh_urls_if_needed(index_name)
+        if index_name in self._urls_mapping['READY']:
+            return self._urls_mapping['READY'][index_name]
+        if index_name in self._urls_mapping['CREATING']:
+            raise MarqoCloudIndexNotReadyError(index_name)
+        raise MarqoCloudIndexNotFoundError(index_name)
+
+    def is_remote(self):
+        return True
+
+    def _refresh_urls_if_needed(self, index_name):
+        if index_name not in self._urls_mapping['READY'] and \
+                time.time() - self.latest_index_mappings_refresh_timestamp > self.url_cache_duration:
             # fast refresh to catch if index was created
             self._refresh_urls()
-        if index_name in self._urls_mapping['READY'] and time.time() - self.timestamp > 360:
+        if index_name in self._urls_mapping['READY'] and \
+                time.time() - self.latest_index_mappings_refresh_timestamp > 360:
             # slow refresh in case index was deleted
             self._refresh_urls(timeout=3)
 
-    def __getitem__(self, item):
-        self.refresh_urls_if_needed(item)
-        if item in self._urls_mapping['READY']:
-            return self._urls_mapping['READY'][item]
-        if item in self._urls_mapping['CREATING']:
-            raise MarqoCloudIndexNotReadyError(item)
-        raise MarqoCloudIndexNotFoundError(item)
-
     def _refresh_urls(self, timeout=None):
         try:
-            response = requests.get('https://api.marqo.ai/api/indexes',
+            response = requests.get(f'{self.get_control_base_url()}/indexes',
                                     headers={"x-api-key": self.api_key}, timeout=timeout)
         except Timeout:
             mq_logger.warning(
                 f"Timeout getting and caching URLs for Marqo Cloud indexes from the"
                 f" /api/indexes/ endpoint. Please contact marqo support at support@marqo.ai if this message"
                 f" persists."
             )
@@ -47,8 +59,8 @@
         if not response.ok:
             mq_logger.warning(response.text)
         response_json = response.json()
         for index in response_json['results']:
             if index.get('index_status') in ["READY", "CREATING"]:
                 self._urls_mapping[index['index_status']][index['index_name']] = index.get('endpoint')
         if self._urls_mapping:
-            self.timestamp = time.time()
+            self.latest_index_mappings_refresh_timestamp = time.time()
```

### Comparing `marqo-1.1.1/src/marqo/models.py` & `marqo-1.2.0/src/marqo/models.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.1/src/marqo/utils.py` & `marqo-1.2.0/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-1.1.1/src/marqo/version.py` & `marqo-1.2.0/src/marqo/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__marqo_version__ = "1.0.0"
+__marqo_version__ = "1.1.0"
 __marqo_release_page__ = f"https://github.com/marqo-ai/marqo/releases/tag/{__marqo_version__}"
 
 __minimum_supported_marqo_version__ = "1.0.0"
 
 
 def supported_marqo_version() -> str:
     return f"This Marqo Python client is built for Marqo release ({__marqo_version__}) \n" \
```

### Comparing `marqo-1.1.1/src/marqo.egg-info/PKG-INFO` & `marqo-1.2.0/src/marqo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 1.1.1
+Version: 1.2.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 1.1.1 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 1.2.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
```

