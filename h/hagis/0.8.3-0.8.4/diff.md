# Comparing `tmp/hagis-0.8.3.tar.gz` & `tmp/hagis-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.8.3.tar", last modified: Fri Jun 16 13:39:28 2023, max compression
+gzip compressed data, was "hagis-0.8.4.tar", last modified: Wed Aug  9 00:47:03 2023, max compression
```

## Comparing `hagis-0.8.3.tar` & `hagis-0.8.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 13:39:28.603144 hagis-0.8.3/
--rw-rw-rw-   0        0        0      963 2023-06-16 13:39:28.601144 hagis-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0      479 2023-05-26 01:17:16.000000 hagis-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 13:39:28.599145 hagis-0.8.3/hagis.egg-info/
--rw-rw-rw-   0        0        0      963 2023-06-16 13:39:28.000000 hagis-0.8.3/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-06-16 13:39:28.000000 hagis-0.8.3/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 13:39:28.000000 hagis-0.8.3/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 13:39:28.000000 hagis-0.8.3/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    27548 2023-06-16 13:36:01.000000 hagis-0.8.3/hagis.py
--rw-rw-rw-   0        0        0      589 2023-06-16 13:37:37.000000 hagis-0.8.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 13:39:28.603144 hagis-0.8.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-09 00:47:03.328409 hagis-0.8.4/
+-rw-rw-rw-   0        0        0      963 2023-08-09 00:47:03.327396 hagis-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-08-09 00:44:03.000000 hagis-0.8.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 00:47:03.325422 hagis-0.8.4/hagis.egg-info/
+-rw-rw-rw-   0        0        0      963 2023-08-09 00:47:03.000000 hagis-0.8.4/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-08-09 00:47:03.000000 hagis-0.8.4/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 00:47:03.000000 hagis-0.8.4/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-09 00:47:03.000000 hagis-0.8.4/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    27495 2023-08-09 00:44:03.000000 hagis-0.8.4/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-08-09 00:44:03.000000 hagis-0.8.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-09 00:47:03.328409 hagis-0.8.4/setup.cfg
```

### Comparing `hagis-0.8.3/PKG-INFO` & `hagis-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.8.3
+Version: 0.8.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.8.3/hagis.egg-info/PKG-INFO` & `hagis-0.8.4/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.8.3
+Version: 0.8.4
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.8.3/hagis.py` & `hagis-0.8.4/hagis.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,19 +203,19 @@
             where_clause = "1=1"
         elif isinstance(where_clause, Callable):
             where_clause = self._to_sql(where_clause)
 
         obj = self._call("query", where=where_clause, returnCountOnly=True)
         return obj.count
 
-    def find(self, oid: int, **kwargs: Any) -> Optional[T]:
+    def find(self, oid: Union[int, str, UUID], **kwargs: Any) -> Optional[T]:
         """ Finds the item by Object ID.
 
         Args:
-            oid (int): Object ID.
+            oid (Union[int, str, UUID]): Object ID or Global ID.
 
         Returns:
             Optional[T]: Item if found (otherwise None).
         """
         where_clause = self.generate_where_clause(oid)
         items = list(self.query(where_clause, **kwargs))
         return items[0] if items else None
@@ -294,18 +294,14 @@
             id_set = set(map(str, ids))
         else:
             field_name = id_field if id_field else "globalid"
             id_set = set((f"'{_id}'" for _id in ids))
 
         return f"({field_name} IN ({','.join(id_set)}))"
 
-    def __iter__(self) -> Iterator[T]:
-        self._iterator = self.query()
-        return self
-
     def __next__(self) -> T:
         if not self._iterator:
             self._iterator = self.query()
         return self._iterator.__next__()
 
     def _to_dict(self, item: T) -> Dict[str, Any]:
         dictionary: Dict[str, Any] = {}
```

### Comparing `hagis-0.8.3/pyproject.toml` & `hagis-0.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

