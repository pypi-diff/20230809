# Comparing `tmp/quivr-0.6.2rc2.tar.gz` & `tmp/quivr-0.6.2rc3.tar.gz`

## Comparing `quivr-0.6.2rc2.tar` & `quivr-0.6.2rc3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/__version__.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/attributes.py
--rw-r--r--   0        0        0    48466 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/columns.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/concat.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/defragment.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/errors.py
--rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/linkage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/py.typed
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/schemagraph.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/tables.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/LICENSE
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/README.md
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/pyproject.toml
--rw-r--r--   0        0        0    10799 2020-02-02 00:00:00.000000 quivr-0.6.2rc2/PKG-INFO
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/__version__.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/attributes.py
+-rw-r--r--   0        0        0    48900 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/columns.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/concat.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/defragment.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/errors.py
+-rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/linkage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/py.typed
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/schemagraph.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/tables.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/LICENSE
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/README.md
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/pyproject.toml
+-rw-r--r--   0        0        0    10799 2020-02-02 00:00:00.000000 quivr-0.6.2rc3/PKG-INFO
```

### Comparing `quivr-0.6.2rc2/quivr/__init__.py` & `quivr-0.6.2rc3/quivr/__init__.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/quivr/attributes.py` & `quivr-0.6.2rc3/quivr/attributes.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/quivr/columns.py` & `quivr-0.6.2rc3/quivr/columns.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,17 +204,27 @@
         # Propagate the value's metadata through to the parent
         metadata = obj.table.schema.metadata
         value_meta = value.table.schema.metadata
         if value_meta is not None:
             for key, val in value_meta.items():
                 key = (self.name + "." + key.decode("utf-8")).encode("utf-8")
                 metadata[key] = val
+
         idx = obj.table.schema.get_field_index(self.name)
         obj.table = obj.table.replace_schema_metadata(metadata)
-        obj.table = obj.table.set_column(idx, self.pyarrow_field(), [value.to_structarray()])
+        data = value.to_structarray()
+        if self.nullable:
+            # rewrite the structarray's type to make all fields
+            # nullable. This is necessary for the case where the
+            # field is not-nullable, but the table is nullable.
+            fields = []
+            for field in data.type:
+                fields.append(field.with_nullable(True))
+            data = pa.StructArray.from_arrays(data.flatten(), fields=fields)
+        obj.table = obj.table.set_column(idx, self.pyarrow_field(), [data])
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
         ...
 
     @overload
     def __get__(self, obj: tables.Table, objtype: type) -> T:
```

### Comparing `quivr-0.6.2rc2/quivr/concat.py` & `quivr-0.6.2rc3/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/quivr/errors.py` & `quivr-0.6.2rc3/quivr/errors.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/quivr/linkage.py` & `quivr-0.6.2rc3/quivr/linkage.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/quivr/schemagraph.py` & `quivr-0.6.2rc3/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/quivr/tables.py` & `quivr-0.6.2rc3/quivr/tables.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/quivr/validators.py` & `quivr-0.6.2rc3/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/LICENSE` & `quivr-0.6.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/README.md` & `quivr-0.6.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/pyproject.toml` & `quivr-0.6.2rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.6.2rc2/PKG-INFO` & `quivr-0.6.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.6.2rc2
+Version: 0.6.2rc3
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

