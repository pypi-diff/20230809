# Comparing `tmp/rabbit-client-3.0.1.tar.gz` & `tmp/rabbit-client-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbit-client-3.0.1.tar", last modified: Thu Mar  9 23:24:17 2023, max compression
+gzip compressed data, was "rabbit-client-3.0.2.tar", last modified: Wed Aug  9 05:38:10 2023, max compression
```

## Comparing `rabbit-client-3.0.1.tar` & `rabbit-client-3.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-03-09 23:24:17.826044 rabbit-client-3.0.1/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)    11356 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/LICENSE
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       78 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/MANIFEST.in
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3179 2023-03-09 23:24:17.826044 rabbit-client-3.0.1/PKG-INFO
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1758 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/README.md
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       98 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/pyproject.toml
-drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-03-09 23:24:17.826044 rabbit-client-3.0.1/rabbit/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      475 2023-03-09 23:23:26.000000 rabbit-client-3.0.1/rabbit/__init__.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       65 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/rabbit/__main__.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1883 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/rabbit/_wait.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1554 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/rabbit/background_tasks.py
-drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-03-09 23:24:17.826044 rabbit-client-3.0.1/rabbit/cli/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     6770 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/rabbit/cli/__init__.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1886 2023-03-09 23:23:26.000000 rabbit-client-3.0.1/rabbit/cli/consumer.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1033 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/rabbit/cli/publisher.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     4440 2023-03-09 23:23:26.000000 rabbit-client-3.0.1/rabbit/client.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     4271 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/rabbit/dlx.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      458 2023-03-09 23:23:26.000000 rabbit-client-3.0.1/rabbit/exceptions.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      356 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/rabbit/exchange.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      785 2023-03-09 23:23:26.000000 rabbit-client-3.0.1/rabbit/job.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      101 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/rabbit/logger.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2387 2023-03-09 23:23:26.000000 rabbit-client-3.0.1/rabbit/publish.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      290 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/rabbit/queue.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     6400 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/rabbit/subscribe.py
-drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-03-09 23:24:17.826044 rabbit-client-3.0.1/rabbit_client.egg-info/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3179 2023-03-09 23:24:17.000000 rabbit-client-3.0.1/rabbit_client.egg-info/PKG-INFO
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      882 2023-03-09 23:24:17.000000 rabbit-client-3.0.1/rabbit_client.egg-info/SOURCES.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)        1 2023-03-09 23:24:17.000000 rabbit-client-3.0.1/rabbit_client.egg-info/dependency_links.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       47 2023-03-09 23:24:17.000000 rabbit-client-3.0.1/rabbit_client.egg-info/entry_points.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       96 2023-03-09 23:24:17.000000 rabbit-client-3.0.1/rabbit_client.egg-info/requires.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       13 2023-03-09 23:24:17.000000 rabbit-client-3.0.1/rabbit_client.egg-info/top_level.txt
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2507 2023-03-09 23:24:17.826044 rabbit-client-3.0.1/setup.cfg
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)       38 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/setup.py
-drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-03-09 23:24:17.826044 rabbit-client-3.0.1/tests/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/tests/__init__.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     4385 2023-03-09 21:48:33.000000 rabbit-client-3.0.1/tests/conftest.py
-drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-03-09 23:24:17.826044 rabbit-client-3.0.1/tests/unit/
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/tests/unit/__init__.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      876 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/tests/unit/test_cli.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1276 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/tests/unit/test_client.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      642 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/tests/unit/test_dlx.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      183 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/tests/unit/test_exchange.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      181 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/tests/unit/test_jobs.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      663 2023-03-09 23:23:26.000000 rabbit-client-3.0.1/tests/unit/test_publish.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      152 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/tests/unit/test_queue.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)      675 2023-03-09 18:16:48.000000 rabbit-client-3.0.1/tests/unit/test_subscribe.py
--rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2190 2023-03-07 03:24:58.000000 rabbit-client-3.0.1/tests/unit/test_wait.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-08-09 05:38:10.985770 rabbit-client-3.0.2/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)    11356 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/LICENSE
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       78 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/MANIFEST.in
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3179 2023-08-09 05:38:10.985770 rabbit-client-3.0.2/PKG-INFO
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1758 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/README.md
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       98 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/pyproject.toml
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-08-09 05:38:10.985770 rabbit-client-3.0.2/rabbit/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      475 2023-08-09 05:37:45.000000 rabbit-client-3.0.2/rabbit/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       65 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/rabbit/__main__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1883 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/rabbit/_wait.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1554 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/rabbit/background_tasks.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-08-09 05:38:10.985770 rabbit-client-3.0.2/rabbit/cli/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     6770 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/rabbit/cli/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1886 2023-03-09 23:23:26.000000 rabbit-client-3.0.2/rabbit/cli/consumer.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1033 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/rabbit/cli/publisher.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     4440 2023-03-09 23:23:26.000000 rabbit-client-3.0.2/rabbit/client.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     4503 2023-08-09 05:37:45.000000 rabbit-client-3.0.2/rabbit/dlx.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      458 2023-03-09 23:23:26.000000 rabbit-client-3.0.2/rabbit/exceptions.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      356 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/rabbit/exchange.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      785 2023-03-09 23:23:26.000000 rabbit-client-3.0.2/rabbit/job.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      101 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/rabbit/logger.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2387 2023-03-09 23:23:26.000000 rabbit-client-3.0.2/rabbit/publish.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      290 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/rabbit/queue.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     6400 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/rabbit/subscribe.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-08-09 05:38:10.985770 rabbit-client-3.0.2/rabbit_client.egg-info/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     3179 2023-08-09 05:38:10.000000 rabbit-client-3.0.2/rabbit_client.egg-info/PKG-INFO
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      882 2023-08-09 05:38:10.000000 rabbit-client-3.0.2/rabbit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)        1 2023-08-09 05:38:10.000000 rabbit-client-3.0.2/rabbit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       47 2023-08-09 05:38:10.000000 rabbit-client-3.0.2/rabbit_client.egg-info/entry_points.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       96 2023-08-09 05:38:10.000000 rabbit-client-3.0.2/rabbit_client.egg-info/requires.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       13 2023-08-09 05:38:10.000000 rabbit-client-3.0.2/rabbit_client.egg-info/top_level.txt
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2508 2023-08-09 05:38:10.989771 rabbit-client-3.0.2/setup.cfg
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)       38 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/setup.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-08-09 05:38:10.985770 rabbit-client-3.0.2/tests/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/tests/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     4385 2023-03-09 21:48:33.000000 rabbit-client-3.0.2/tests/conftest.py
+drwxr-xr-x   0 amenezes  (1000) amenezes  (1000)        0 2023-08-09 05:38:10.985770 rabbit-client-3.0.2/tests/unit/
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)        0 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/tests/unit/__init__.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      876 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/tests/unit/test_cli.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     1276 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/tests/unit/test_client.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      642 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/tests/unit/test_dlx.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      183 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/tests/unit/test_exchange.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      181 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/tests/unit/test_jobs.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      663 2023-03-09 23:23:26.000000 rabbit-client-3.0.2/tests/unit/test_publish.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      152 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/tests/unit/test_queue.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)      675 2023-03-09 18:16:48.000000 rabbit-client-3.0.2/tests/unit/test_subscribe.py
+-rw-r--r--   0 amenezes  (1000) amenezes  (1000)     2190 2023-03-07 03:24:58.000000 rabbit-client-3.0.2/tests/unit/test_wait.py
```

### Comparing `rabbit-client-3.0.1/LICENSE` & `rabbit-client-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/PKG-INFO` & `rabbit-client-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbit-client
-Version: 3.0.1
+Version: 3.0.2
 Summary: async rabbit client
 Home-page: https://github.com/amenezes/rabbit-client
 Author: alexandre menezes
 Author-email: alexandre.fmenezes@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://rabbit-client.amenezes.net
 Project-URL: Code, https://github.com/amenezes/rabbit-client
```

### Comparing `rabbit-client-3.0.1/README.md` & `rabbit-client-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/_wait.py` & `rabbit-client-3.0.2/rabbit/_wait.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/background_tasks.py` & `rabbit-client-3.0.2/rabbit/background_tasks.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/cli/__init__.py` & `rabbit-client-3.0.2/rabbit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/cli/consumer.py` & `rabbit-client-3.0.2/rabbit/cli/consumer.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/cli/publisher.py` & `rabbit-client-3.0.2/rabbit/cli/publisher.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/client.py` & `rabbit-client-3.0.2/rabbit/client.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/dlx.py` & `rabbit-client-3.0.2/rabbit/dlx.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,32 +93,39 @@
         return value
 
     async def send_event(
         self, cause: Exception, body: bytes, envelope: Envelope, properties: Properties
     ) -> None:
         """Sent event message to DLX/DLQ."""
         timeout = self.delay_strategy(properties.headers)
-        properties = await self._get_properties(timeout, cause, envelope)
+        properties = await self._get_properties(timeout, cause, envelope, properties)
 
         logger.debug(
             f"Send event to dlq: [exchange: {self.exchange.name}"
             f" | routing_key: {self.queue.name} | properties: {properties}]"
         )
         try:
             await self._channel.publish(
                 body, self.exchange.name, self.queue.name, properties
             )
         except AttributeError:
             raise OperationError("Ensure that instance was connected ")
 
     async def _get_properties(
-        self, timeout: int, exception_message: Exception, envelope: Envelope
+        self,
+        timeout: int,
+        exception_message: Exception,
+        envelope: Envelope,
+        properties: Properties,
     ) -> dict:
-        return {
+        custom_properties: dict = {
             "expiration": f"{timeout}",
             "headers": {
                 "x-delay": f"{timeout}",
                 "x-exception-message": f"{exception_message}",
                 "x-original-exchange": f"{envelope.exchange_name}",
                 "x-original-routingKey": f"{envelope.routing_key}",
             },
         }
+        if properties.headers is not None:
+            custom_properties["headers"].update(properties.headers)
+        return custom_properties
```

### Comparing `rabbit-client-3.0.1/rabbit/job.py` & `rabbit-client-3.0.2/rabbit/job.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/publish.py` & `rabbit-client-3.0.2/rabbit/publish.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit/subscribe.py` & `rabbit-client-3.0.2/rabbit/subscribe.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/rabbit_client.egg-info/PKG-INFO` & `rabbit-client-3.0.2/rabbit_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbit-client
-Version: 3.0.1
+Version: 3.0.2
 Summary: async rabbit client
 Home-page: https://github.com/amenezes/rabbit-client
 Author: alexandre menezes
 Author-email: alexandre.fmenezes@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://rabbit-client.amenezes.net
 Project-URL: Code, https://github.com/amenezes/rabbit-client
```

### Comparing `rabbit-client-3.0.1/rabbit_client.egg-info/SOURCES.txt` & `rabbit-client-3.0.2/rabbit_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/setup.cfg` & `rabbit-client-3.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 version = attr:  rabbit.__version__
 author = alexandre menezes
 author_email = alexandre.fmenezes@gmail.com
 description = async rabbit client
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache-2.0
-license_file = LICENSE
+license_files = LICENSE
 url = https://github.com/amenezes/rabbit-client
 project_urls = 
 	Documentation = https://rabbit-client.amenezes.net
 	Code = https://github.com/amenezes/rabbit-client
 	Issue tracker = https://github.com/amenezes/rabbit-client/issues
 	Changes = https://github.com/amenezes/rabbit-client/releases
 classifiers =
```

### Comparing `rabbit-client-3.0.1/tests/conftest.py` & `rabbit-client-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/tests/unit/test_cli.py` & `rabbit-client-3.0.2/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/tests/unit/test_client.py` & `rabbit-client-3.0.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/tests/unit/test_dlx.py` & `rabbit-client-3.0.2/tests/unit/test_dlx.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/tests/unit/test_publish.py` & `rabbit-client-3.0.2/tests/unit/test_publish.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/tests/unit/test_subscribe.py` & `rabbit-client-3.0.2/tests/unit/test_subscribe.py`

 * *Files identical despite different names*

### Comparing `rabbit-client-3.0.1/tests/unit/test_wait.py` & `rabbit-client-3.0.2/tests/unit/test_wait.py`

 * *Files identical despite different names*

