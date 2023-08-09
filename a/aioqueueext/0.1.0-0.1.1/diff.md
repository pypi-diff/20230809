# Comparing `tmp/aioqueueext-0.1.0.tar.gz` & `tmp/aioqueueext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqueueext-0.1.0.tar", last modified: Tue Aug  8 05:42:56 2023, max compression
+gzip compressed data, was "aioqueueext-0.1.1.tar", last modified: Wed Aug  9 04:56:56 2023, max compression
```

## Comparing `aioqueueext-0.1.0.tar` & `aioqueueext-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-08 05:42:56.512402 aioqueueext-0.1.0/
--rw-r--r--   0 deuser    (1000) deuser    (1000)     1107 2023-08-06 14:28:28.000000 aioqueueext-0.1.0/LICENSE
--rw-r--r--   0 deuser    (1000) deuser    (1000)     1172 2023-08-08 05:42:56.512402 aioqueueext-0.1.0/PKG-INFO
--rw-r--r--   0 deuser    (1000) deuser    (1000)      612 2023-08-06 15:04:23.000000 aioqueueext-0.1.0/README.md
--rw-r--r--   0 deuser    (1000) deuser    (1000)      635 2023-08-08 04:41:05.000000 aioqueueext-0.1.0/pyproject.toml
--rw-r--r--   0 deuser    (1000) deuser    (1000)       38 2023-08-08 05:42:56.512402 aioqueueext-0.1.0/setup.cfg
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-08 05:42:56.508401 aioqueueext-0.1.0/src/
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-08 05:42:56.508401 aioqueueext-0.1.0/src/aioqueueext/
--rw-r--r--   0 deuser    (1000) deuser    (1000)       83 2023-08-08 04:28:50.000000 aioqueueext-0.1.0/src/aioqueueext/__init__.py
--rw-r--r--   0 deuser    (1000) deuser    (1000)     4935 2023-08-06 15:26:24.000000 aioqueueext-0.1.0/src/aioqueueext/base.py
--rw-r--r--   0 deuser    (1000) deuser    (1000)     1498 2023-08-06 09:44:44.000000 aioqueueext-0.1.0/src/aioqueueext/one_queue.py
--rw-r--r--   0 deuser    (1000) deuser    (1000)     1778 2023-08-06 15:30:41.000000 aioqueueext-0.1.0/src/aioqueueext/queue.py
--rw-r--r--   0 deuser    (1000) deuser    (1000)      715 2023-08-08 04:17:04.000000 aioqueueext-0.1.0/src/aioqueueext/util.py
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-08 05:42:56.512402 aioqueueext-0.1.0/src/aioqueueext.egg-info/
--rw-r--r--   0 deuser    (1000) deuser    (1000)     1172 2023-08-08 05:42:56.000000 aioqueueext-0.1.0/src/aioqueueext.egg-info/PKG-INFO
--rw-r--r--   0 deuser    (1000) deuser    (1000)      337 2023-08-08 05:42:56.000000 aioqueueext-0.1.0/src/aioqueueext.egg-info/SOURCES.txt
--rw-r--r--   0 deuser    (1000) deuser    (1000)        1 2023-08-08 05:42:56.000000 aioqueueext-0.1.0/src/aioqueueext.egg-info/dependency_links.txt
--rw-r--r--   0 deuser    (1000) deuser    (1000)       12 2023-08-08 05:42:56.000000 aioqueueext-0.1.0/src/aioqueueext.egg-info/top_level.txt
-drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-08 05:42:56.512402 aioqueueext-0.1.0/tests/
--rw-r--r--   0 deuser    (1000) deuser    (1000)     6976 2023-08-08 05:42:23.000000 aioqueueext-0.1.0/tests/test_base.py
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:56:56.182780 aioqueueext-0.1.1/
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     1107 2023-08-06 14:28:28.000000 aioqueueext-0.1.1/LICENSE
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     1273 2023-08-09 04:56:56.182780 aioqueueext-0.1.1/PKG-INFO
+-rw-r--r--   0 deuser    (1000) deuser    (1000)      612 2023-08-06 15:04:23.000000 aioqueueext-0.1.1/README.md
+-rw-r--r--   0 deuser    (1000) deuser    (1000)      734 2023-08-09 04:48:40.000000 aioqueueext-0.1.1/pyproject.toml
+-rw-r--r--   0 deuser    (1000) deuser    (1000)       38 2023-08-09 04:56:56.182780 aioqueueext-0.1.1/setup.cfg
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:56:56.182780 aioqueueext-0.1.1/src/
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:56:56.182780 aioqueueext-0.1.1/src/aioqueueext/
+-rw-r--r--   0 deuser    (1000) deuser    (1000)       83 2023-08-08 04:28:50.000000 aioqueueext-0.1.1/src/aioqueueext/__init__.py
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     4935 2023-08-06 15:26:24.000000 aioqueueext-0.1.1/src/aioqueueext/base.py
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     1498 2023-08-06 09:44:44.000000 aioqueueext-0.1.1/src/aioqueueext/one_queue.py
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     1778 2023-08-06 15:30:41.000000 aioqueueext-0.1.1/src/aioqueueext/queue.py
+-rw-r--r--   0 deuser    (1000) deuser    (1000)      715 2023-08-08 04:17:04.000000 aioqueueext-0.1.1/src/aioqueueext/util.py
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:56:56.182780 aioqueueext-0.1.1/src/aioqueueext.egg-info/
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     1273 2023-08-09 04:56:56.000000 aioqueueext-0.1.1/src/aioqueueext.egg-info/PKG-INFO
+-rw-r--r--   0 deuser    (1000) deuser    (1000)      337 2023-08-09 04:56:56.000000 aioqueueext-0.1.1/src/aioqueueext.egg-info/SOURCES.txt
+-rw-r--r--   0 deuser    (1000) deuser    (1000)        1 2023-08-09 04:56:56.000000 aioqueueext-0.1.1/src/aioqueueext.egg-info/dependency_links.txt
+-rw-r--r--   0 deuser    (1000) deuser    (1000)       12 2023-08-09 04:56:56.000000 aioqueueext-0.1.1/src/aioqueueext.egg-info/top_level.txt
+drwxr-xr-x   0 deuser    (1000) deuser    (1000)        0 2023-08-09 04:56:56.182780 aioqueueext-0.1.1/tests/
+-rw-r--r--   0 deuser    (1000) deuser    (1000)     8069 2023-08-08 05:53:12.000000 aioqueueext-0.1.1/tests/test_base.py
```

### Comparing `aioqueueext-0.1.0/LICENSE` & `aioqueueext-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioqueueext-0.1.0/PKG-INFO` & `aioqueueext-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: aioqueueext
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extended asyncio queues, implements peeking, setting put and get callbacks.
 Author-email: darkhaniop <darkhaniop@google.com>
 Project-URL: Homepage, https://github.com/gw-tools/aioqueueext
 Project-URL: Bug Tracker, https://github.com/gw-tools/aioqueueext/issues
+Keywords: asyncio,queue
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: AsyncIO
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aioqueueext
 
 A package that provides asyncio Queues with additional functionality.
```

### Comparing `aioqueueext-0.1.0/README.md` & `aioqueueext-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aioqueueext-0.1.0/src/aioqueueext/base.py` & `aioqueueext-0.1.1/src/aioqueueext/base.py`

 * *Files identical despite different names*

### Comparing `aioqueueext-0.1.0/src/aioqueueext/one_queue.py` & `aioqueueext-0.1.1/src/aioqueueext/one_queue.py`

 * *Files identical despite different names*

### Comparing `aioqueueext-0.1.0/src/aioqueueext/queue.py` & `aioqueueext-0.1.1/src/aioqueueext/queue.py`

 * *Files identical despite different names*

### Comparing `aioqueueext-0.1.0/src/aioqueueext/util.py` & `aioqueueext-0.1.1/src/aioqueueext/util.py`

 * *Files identical despite different names*

### Comparing `aioqueueext-0.1.0/src/aioqueueext.egg-info/PKG-INFO` & `aioqueueext-0.1.1/src/aioqueueext.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: aioqueueext
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extended asyncio queues, implements peeking, setting put and get callbacks.
 Author-email: darkhaniop <darkhaniop@google.com>
 Project-URL: Homepage, https://github.com/gw-tools/aioqueueext
 Project-URL: Bug Tracker, https://github.com/gw-tools/aioqueueext/issues
+Keywords: asyncio,queue
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Framework :: AsyncIO
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aioqueueext
 
 A package that provides asyncio Queues with additional functionality.
```

### Comparing `aioqueueext-0.1.0/tests/test_base.py` & `aioqueueext-0.1.1/tests/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -211,10 +211,45 @@
             "on_get_callback(item) call with incorrect arguments",
         )
         self.assertTrue(
             cb_items[n_calls] is item2_copy,
             "value passed to on_get_callback(item) and the one returned by get_nowait() must be the same",
         )
 
+    async def _test_peek_and_get_00_sync(self) -> None:
+        # on_get_callback uses peek_nowait() which is not implemented in this
+        # class, using a dummy implementation.
+        queue = QueueWithDummyPeek()
+        l = []
+
+        def my_decider_func(item: t.Any) -> bool:
+            decision = False
+            l.append({"item": item, "decision": decision})
+            return decision
+
+        item1 = object()
+        item2 = object()
+
+        await queue.put(item1)
+        queue.put_nowait(item2)
+        self.assertTrue(len(l) == 0, "on_get_callback was called")
+
+    async def _test_peek_and_get_01_async(self) -> None:
+        queue = QueueWithDummyPeek()
+        l = []
+
+        def my_decider_func(item: t.Any) -> bool:
+            decision = False
+            l.append({"item": item, "decision": decision})
+            return decision
+
+        item1 = object()
+        item2 = object()
+
+        queue.set_on_get_callback(my_decider_func)
+        await queue.put(item1)
+        queue.put_nowait(item2)
+        self.assertTrue(len(l) == 0, "on_get_callback was called")
+
 
 if __name__ == "__main__":
     unittest.main()
```

