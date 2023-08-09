# Comparing `tmp/quivr-0.6.1.tar.gz` & `tmp/quivr-0.6.2rc1.tar.gz`

## Comparing `quivr-0.6.1.tar` & `quivr-0.6.2rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/__version__.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/attributes.py
--rw-r--r--   0        0        0    47986 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/columns.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/concat.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/defragment.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/errors.py
--rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/linkage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/py.typed
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/schemagraph.py
--rw-r--r--   0        0        0    40528 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/tables.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.1/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.1/LICENSE
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 quivr-0.6.1/README.md
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 quivr-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/__version__.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/attributes.py
+-rw-r--r--   0        0        0    48027 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/columns.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/concat.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/defragment.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/errors.py
+-rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/linkage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/py.typed
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/schemagraph.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/tables.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/LICENSE
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/README.md
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/pyproject.toml
+-rw-r--r--   0        0        0    10799 2020-02-02 00:00:00.000000 quivr-0.6.2rc1/PKG-INFO
```

### Comparing `quivr-0.6.1/quivr/__init__.py` & `quivr-0.6.2rc1/quivr/__init__.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/quivr/attributes.py` & `quivr-0.6.2rc1/quivr/attributes.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/quivr/columns.py` & `quivr-0.6.2rc1/quivr/columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         if metadata is None:
             metadata = {}
         metadata.update(obj._metadata_for_column(self.name))  # type: ignore
 
         schema = self.schema.with_metadata(metadata)
 
         subtable = pa.Table.from_arrays(array.flatten(), schema=schema)
-        return self.table_type(subtable)
+        return self.table_type.from_pyarrow(subtable, permit_nulls=self.nullable)
 
     def _nulls(self, n: int) -> pa.Array:
         """Return an array of nulls of the appropriate size."""
         # Quite unfortunate: pyarrow doesn't support creating a struct
         # array of nulls; it incorrectly populates all the fields with
         # nulls (including non-nullable ones!) so we need to do this
         # manually.
```

### Comparing `quivr-0.6.1/quivr/concat.py` & `quivr-0.6.2rc1/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/quivr/errors.py` & `quivr-0.6.2rc1/quivr/errors.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/quivr/linkage.py` & `quivr-0.6.2rc1/quivr/linkage.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/quivr/schemagraph.py` & `quivr-0.6.2rc1/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/quivr/tables.py` & `quivr-0.6.2rc1/quivr/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,14 @@
 
     :ivar table: The underlying :class:`pyarrow.Table` for this Table instance.
     :vartype table: pyarrow.Table
     """
 
     schema: ClassVar[pa.Schema]
 
-    #: Instance variable
-    #: does it work?
     table: pa.Table
 
     _quivr_subtables: ClassVar[dict[str, columns.SubTableColumn[Any]]]
     _quivr_attributes: ClassVar[dict[str, attributes.Attribute[Any]]]
     _column_validators: ClassVar[dict[str, validators.Validator]]
 
     def __init_subclass__(cls: Type["Table"], **kwargs: Any):
@@ -142,14 +140,15 @@
             getattr(self, name)
 
     @classmethod
     def from_pyarrow(
         cls,
         table: pa.Table,
         validate: bool = True,
+        permit_nulls: bool = False,
         **kwargs: AttributeValueType,
     ) -> Self:
         """Create a new table from a pyarrow Table.
 
         This is a convenience method which can be used to create a
         Table from a pyarrow Table. It can also accept keyword-style
         arguments to set attributes on the table.
@@ -159,21 +158,36 @@
         metadata to set the attributes on the table if it is
         available. If any attributes are provided as keyword
         arguments, they override any values in the metadata.
 
         :param table: The pyarrow Table to create the table from.
         :param validate: Whether to validate the table against the
             schema, and run any column validators.
+        :param permit_nulls: Whether to permit null values in the
+            table. If True, nulls will be permitted, even in non-nullable
+            fields. This is used when a Table is used as a nullable subtable.
         :param \\**kwargs: Keyword arguments to set attributes on the
             table.
         :type \\**kwargs: :obj:`AttributeValueType`
         :return: A new Table instance.
         """
+        schema = cls.schema
+        if permit_nulls:
+            # Rewrite the schema to permit nulls
+            fields = []
+            for field in schema:
+                if field.nullable:
+                    fields.append(field)
+                else:
+                    fields.append(field.with_nullable(True))
+            schema = pa.schema(fields, metadata=schema.metadata)
+
+        # Absorb metadata from the table
+        schema = schema.with_metadata(table.schema.metadata)
 
-        schema = cls.schema.with_metadata(table.schema.metadata)
         table = table.cast(schema)
         instance = cls(table, **kwargs)
         if validate:
             instance.validate()
         return instance
 
     @classmethod
```

### Comparing `quivr-0.6.1/quivr/validators.py` & `quivr-0.6.2rc1/quivr/validators.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/LICENSE` & `quivr-0.6.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/README.md` & `quivr-0.6.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/pyproject.toml` & `quivr-0.6.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.6.1/PKG-INFO` & `quivr-0.6.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.6.1
+Version: 0.6.2rc1
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
```

