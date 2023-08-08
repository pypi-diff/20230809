# Comparing `tmp/computing-toolbox-1.0.0.tar.gz` & `tmp/computing-toolbox-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computing-toolbox-1.0.0.tar", last modified: Thu Jul 13 06:32:33 2023, max compression
+gzip compressed data, was "computing-toolbox-1.0.1.tar", last modified: Tue Aug  8 22:06:00 2023, max compression
```

## Comparing `computing-toolbox-1.0.0.tar` & `computing-toolbox-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:33.253126 computing-toolbox-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 06:32:33.253126 computing-toolbox-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:32:33.253126 computing-toolbox-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:33.249126 computing-toolbox-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:33.249126 computing-toolbox-1.0.0/src/computing_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:33.249126 computing-toolbox-1.0.0/src/computing_toolbox/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/algorithms/split_range.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:33.249126 computing-toolbox-1.0.0/src/computing_toolbox/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/gcp/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/gcp/gs_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:33.253126 computing-toolbox-1.0.0/src/computing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/utils/deep_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/utils/es_long_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/utils/http_async_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/utils/http_fake_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/utils/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/utils/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-13 06:32:22.000000 computing-toolbox-1.0.0/src/computing_toolbox/utils/tictoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:32:33.249126 computing-toolbox-1.0.0/src/computing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 06:32:33.000000 computing-toolbox-1.0.0/src/computing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-13 06:32:33.000000 computing-toolbox-1.0.0/src/computing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:32:33.000000 computing-toolbox-1.0.0/src/computing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-13 06:32:33.000000 computing-toolbox-1.0.0/src/computing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 06:32:33.000000 computing-toolbox-1.0.0/src/computing_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:00.518036 computing-toolbox-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 22:06:00.518036 computing-toolbox-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 22:06:00.518036 computing-toolbox-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:00.514036 computing-toolbox-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:00.514036 computing-toolbox-1.0.1/src/computing_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:00.514036 computing-toolbox-1.0.1/src/computing_toolbox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/algorithms/split_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:00.514036 computing-toolbox-1.0.1/src/computing_toolbox/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/gcp/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/gcp/gs_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/gcp/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:00.518036 computing-toolbox-1.0.1/src/computing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/utils/deep_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/utils/es_long_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22366 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/utils/http_async_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/utils/http_fake_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/utils/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/utils/jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-08 22:05:49.000000 computing-toolbox-1.0.1/src/computing_toolbox/utils/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:06:00.514036 computing-toolbox-1.0.1/src/computing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 22:06:00.000000 computing-toolbox-1.0.1/src/computing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-08 22:06:00.000000 computing-toolbox-1.0.1/src/computing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:06:00.000000 computing-toolbox-1.0.1/src/computing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-08 22:06:00.000000 computing-toolbox-1.0.1/src/computing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 22:06:00.000000 computing-toolbox-1.0.1/src/computing_toolbox.egg-info/top_level.txt
```

### Comparing `computing-toolbox-1.0.0/LICENSE` & `computing-toolbox-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/PKG-INFO` & `computing-toolbox-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 1.0.0
+Version: 1.0.1
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-1.0.0/README.md` & `computing-toolbox-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/pyproject.toml` & `computing-toolbox-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "computing-toolbox"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Pedro Mayorga", email="ppmayorga80@gmail.com" },
 ]
 description = "Computing Toolbox for daily computations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/algorithms/split_range.py` & `computing-toolbox-1.0.1/src/computing_toolbox/algorithms/split_range.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/gcp/gs.py` & `computing-toolbox-1.0.1/src/computing_toolbox/gcp/gs.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/gcp/gs_async.py` & `computing-toolbox-1.0.1/src/computing_toolbox/gcp/gs_async.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/gcp/pubsub.py` & `computing-toolbox-1.0.1/src/computing_toolbox/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/gcp/secret_manager.py` & `computing-toolbox-1.0.1/src/computing_toolbox/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/utils/deep_get.py` & `computing-toolbox-1.0.1/src/computing_toolbox/utils/deep_get.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/utils/es_long_search.py` & `computing-toolbox-1.0.1/src/computing_toolbox/utils/es_long_search.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/utils/http_async_request.py` & `computing-toolbox-1.0.1/src/computing_toolbox/utils/http_async_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/utils/http_fake_headers.py` & `computing-toolbox-1.0.1/src/computing_toolbox/utils/http_fake_headers.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/utils/http_request.py` & `computing-toolbox-1.0.1/src/computing_toolbox/utils/http_request.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/utils/jsonl.py` & `computing-toolbox-1.0.1/src/computing_toolbox/utils/jsonl.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 """json line utilities"""
+import multiprocessing
 from itertools import count
 from typing import Any
 
 import jsons
 import smart_open
 from tqdm import tqdm
 
+from computing_toolbox.algorithms.split_range import split_range
+
+
+def _jsonl_read_one_part(args):
+    path_k, k, ak, nk = args
+    tqdm_kwargs = {
+        "desc": f"Read part {k}",
+        "total": nk,
+        "position": k,
+        "leave": False
+    }
+    data_k = Jsonl.read(path=path_k,
+                        offset=ak,
+                        limit=nk,
+                        tqdm_kwargs=tqdm_kwargs)
+    return data_k
+
 
 class Jsonl:
     """class that concentrates common json line operations"""
 
     @classmethod
     def count_lines(cls, path: str, tqdm_kwargs: dict or None = None) -> int:
         """count the number of lines if the path provided
@@ -25,15 +43,15 @@
             },
             **tqdm_kwargs
         } if tqdm_kwargs is not None else tqdm_kwargs
         # 2. open the file
         with smart_open.open(path) as fp:
             # 2.1 define the file iterator
             fp_iterator = tqdm(fp, **
-                               tqdm_kwargs) if tqdm_kwargs is not None else fp
+            tqdm_kwargs) if tqdm_kwargs is not None else fp
             # 2.2 count the number of lines
             n_lines = len([1 for _ in fp_iterator])
         return n_lines
 
     @classmethod
     def read(cls,
              path: str,
@@ -142,7 +160,46 @@
                 # write a new line
                 fp.write(line)
                 # new line should be "\n"
                 nl_prefix = "\n"
 
         # return the number of objects
         return n_data
+
+    @classmethod
+    def parallel_read(cls,
+                      path: str,
+                      mapping_class: Any = None,
+                      offset: int = 0,
+                      limit: int or None = None,
+                      workers: int or None = None,
+                      tqdm_kwargs: dict or None = None) -> list[dict]:
+        """read a jsonl in parallel
+        works better for large files
+        if workers is not defined will use the number of cpus in your
+        computer
+        """
+        workers = workers if workers is not None else multiprocessing.cpu_count()
+        n = Jsonl.count_lines(path, tqdm_kwargs={})
+
+        intervals = split_range(n=n, parts=workers)
+        parameters = [
+            (path, k, ak, bk - ak)
+            for k, (ak, bk) in enumerate(intervals)
+        ]
+
+        with multiprocessing.Pool(workers) as pool:
+            data_in_chunks = pool.map(_jsonl_read_one_part, parameters)
+        print("Parallel read done")
+        print("Flatting data...")
+        flat_data = [
+            xk
+            for x in data_in_chunks
+            for xk in x
+        ]
+        return flat_data
+
+
+if __name__ == "__main__":
+    path = "/Users/pedro/Downloads/divihomes_20230631.jsonl"
+    data = Jsonl.parallel_read(path=path)
+    print("Done", "Lines:", len(data))
```

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox/utils/tictoc.py` & `computing-toolbox-1.0.1/src/computing_toolbox/utils/tictoc.py`

 * *Files identical despite different names*

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox.egg-info/PKG-INFO` & `computing-toolbox-1.0.1/src/computing_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computing-toolbox
-Version: 1.0.0
+Version: 1.0.1
 Summary: Computing Toolbox for daily computations
 Author-email: Pedro Mayorga <ppmayorga80@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `computing-toolbox-1.0.0/src/computing_toolbox.egg-info/SOURCES.txt` & `computing-toolbox-1.0.1/src/computing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

