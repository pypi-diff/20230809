# Comparing `tmp/quivr-0.6.0rc2.tar.gz` & `tmp/quivr-0.6.1.tar.gz`

## Comparing `quivr-0.6.0rc2.tar` & `quivr-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/__version__.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/attributes.py
--rw-r--r--   0        0        0    46076 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/columns.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/concat.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/defragment.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/errors.py
--rw-r--r--   0        0        0    18327 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/linkage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/py.typed
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/schemagraph.py
--rw-r--r--   0        0        0    39757 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/tables.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/quivr/validators.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/LICENSE
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/README.md
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/pyproject.toml
--rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 quivr-0.6.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/__version__.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/attributes.py
+-rw-r--r--   0        0        0    47986 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/columns.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/concat.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/defragment.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/errors.py
+-rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/linkage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/py.typed
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/schemagraph.py
+-rw-r--r--   0        0        0    40528 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/tables.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 quivr-0.6.1/quivr/validators.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 quivr-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.6.1/LICENSE
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 quivr-0.6.1/README.md
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 quivr-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 quivr-0.6.1/PKG-INFO
```

### Comparing `quivr-0.6.0rc2/quivr/__init__.py` & `quivr-0.6.1/quivr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,30 @@
     UInt32Column,
     UInt64Column,
 )
 from .concat import concatenate
 from .defragment import defragment
 from .errors import (
     AttributeImmutableError,
+    InvalidColumnDataError,
+    InvalidColumnDefault,
     InvariantViolatedError,
     LinkageCombinationError,
     TableFragmentedError,
     TablesNotCompatibleError,
     ValidationError,
 )
 from .linkage import Linkage, MultiKeyLinkage, combine_linkages, combine_multilinkages
-from .tables import AnyTable, AttributeValueType, DataSourceType, Table
+from .tables import (
+    AnyTable,
+    ArrowArrayProvider,
+    AttributeValueType,
+    DataSourceType,
+    Table,
+)
 from .validators import Validator, and_, eq, ge, gt, is_in, le, lt
 
 __all__ = [
     "AnyTable",
     "AttributeImmutableError",
     "AttributeValueType",
     "BinaryColumn",
@@ -76,14 +84,15 @@
     "Float64Column",
     "FloatAttribute",
     "Int16Column",
     "Int32Column",
     "Int64Column",
     "Int8Column",
     "IntAttribute",
+    "InvalidColumnDefault",
     "InvariantViolatedError",
     "LargeBinaryColumn",
     "LargeListColumn",
     "LargeStringColumn",
     "Linkage",
     "LinkageCombinationError",
     "ListColumn",
@@ -117,8 +126,10 @@
     "defragment",
     "eq",
     "ge",
     "gt",
     "is_in",
     "le",
     "lt",
+    "InvalidColumnDataError",
+    "ArrowArrayProvider",
 ]
```

### Comparing `quivr-0.6.0rc2/quivr/attributes.py` & `quivr-0.6.1/quivr/attributes.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc2/quivr/columns.py` & `quivr-0.6.1/quivr/columns.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     :ivar validator: A validator to use when setting the column.
     :ivar default: A default value to use when setting the column.
     """
 
     def __init__(
         self,
         dtype: pa.DataType,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], Any], Any] = None,
     ):
         self.dtype = dtype
         self.nullable = nullable
         self.metadata = metadata
@@ -128,28 +128,64 @@
 
     def pyarrow_field(self) -> pa.Field:
         """
         Returns a pyarrow Field object for this column.
         """
         return pa.field(self.name, self.dtype, self.nullable, self.metadata)
 
+    def _load(
+        self,
+        data: Union[tables.DataSourceType, None],
+        size_hint: Optional[int],
+    ) -> Optional[pa.Array]:
+        """Load a data source as a pyarrow Array of data which
+        matches the column's schema. Defaults are not poulated.
+
+        size_hint is an optional expected size of the input data. If provided:
+         - For input of None, an array of nulls is returned.
+         - For all other inputs, the input's length is checked.
+
+        If the column is nullable and the input value is None, then
+        this returns None.  Otherwise, it will either return a pyarrow
+        Array, or raise an error.
+        """
+        if data is None:
+            if not self.nullable and self.default is None:
+                raise errors.InvalidColumnDataError(
+                    self, "received no data, but field is not nullable and has no default"
+                )
+
+            # Either it's nullable, or has a default; either way, we can proceed.
+            if size_hint is None:
+                # We can't even make a null array of the appropriate
+                # size, so we're forced to return None.
+                return None
+
+            return self._nulls(size_hint)
+
+        return pa.array(data, type=self.dtype)
+
+    def _nulls(self, n: int) -> pa.Array:
+        """Return an array of nulls of the appropriate size."""
+        return pa.nulls(n, type=self.dtype)
+
 
 T = TypeVar("T", bound=tables.Table)
 
 
 class SubTableColumn(Column, Generic[T]):
     """
-    A column which represents an embedded Quivr table.
+    A column which represents an embedded quivr table.
 
     :param table_type: The type of the table to embed.
     :param nullable: Whether the column can contain null values.
     :param metadata: A dictionary of metadata to attach to the column.
     """
 
-    def __init__(self, table_type: type[T], nullable: bool = True, metadata: Optional[MetadataDict] = None):
+    def __init__(self, table_type: type[T], nullable: bool = False, metadata: Optional[MetadataDict] = None):
         self.table_type = table_type
         self.schema = table_type.schema
         dtype = pa.struct(table_type.schema)
         super().__init__(dtype, nullable=nullable, metadata=metadata)
 
     def __set__(self, obj: tables.Table, value: T) -> None:
         # Propagate the value's metadata through to the parent
@@ -182,25 +218,35 @@
         metadata.update(obj._metadata_for_column(self.name))  # type: ignore
 
         schema = self.schema.with_metadata(metadata)
 
         subtable = pa.Table.from_arrays(array.flatten(), schema=schema)
         return self.table_type(subtable)
 
+    def _nulls(self, n: int) -> pa.Array:
+        """Return an array of nulls of the appropriate size."""
+        # Quite unfortunate: pyarrow doesn't support creating a struct
+        # array of nulls; it incorrectly populates all the fields with
+        # nulls (including non-nullable ones!) so we need to do this
+        # manually.
+        #
+        # See: https://github.com/apache/arrow/issues/37072
+        return pa.array([None] * n, type=self.dtype)
+
 
 class Int8Column(Column):
     """
     A column for storing 8-bit integers.
     """
 
     primitive_dtype = pa.int8()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.int8(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -224,15 +270,15 @@
     A column for storing 16-bit integers.
     """
 
     primitive_dtype = pa.int16()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.int16(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -256,15 +302,15 @@
     A column for storing 32-bit integers.
     """
 
     primitive_dtype = pa.int32()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.int32(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -288,15 +334,15 @@
     A column for storing 64-bit integers.
     """
 
     primitive_dtype = pa.int64()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.int64(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -320,15 +366,15 @@
     A column for storing 8-bit unsigned integers.
     """
 
     primitive_dtype = pa.uint8()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.uint8(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -352,15 +398,15 @@
     A column for storing 16-bit unsigned integers.
     """
 
     primitive_dtype = pa.uint16()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.uint16(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -384,15 +430,15 @@
     A column for storing 32-bit unsigned integers.
     """
 
     primitive_dtype = pa.uint32()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.uint32(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -416,15 +462,15 @@
     A column for storing 64-bit unsigned integers.
     """
 
     primitive_dtype = pa.uint64()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], int], int] = None,
     ):
         super().__init__(
             pa.uint64(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -459,15 +505,15 @@
       not supported by Arrow's compute functions).
     """
 
     primitive_dtype = pa.float16()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.float16(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
@@ -488,15 +534,15 @@
     A column for storing 32-bit floating point numbers.
     """
 
     primitive_dtype = pa.float32()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], float], float] = None,
     ):
         super().__init__(
             pa.float32(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -520,15 +566,15 @@
     A column for storing 64-bit floating point numbers.
     """
 
     primitive_dtype = pa.float64()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], float], float] = None,
     ):
         super().__init__(
             pa.float64(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -550,15 +596,15 @@
 class BooleanColumn(Column):
     """A column for storing booleans."""
 
     primitive_dtype = pa.bool_()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, Callable[[], bool], bool] = None,
     ):
         super().__init__(
             pa.bool_(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -586,15 +632,15 @@
 
     """
 
     primitive_dtype = pa.string()
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, str, Callable[[], str]] = None,
     ):
         super().__init__(
             pa.string(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -617,15 +663,15 @@
     r"""
     A column for storing large binary objects (over 2\ :sup:`31` bytes long). Large binary data is stored in
     variable-length chunks.
     """
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, bytes, Callable[[], bytes]] = None,
     ):
         super().__init__(
             pa.large_binary(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -648,15 +694,15 @@
     r"""
     A column for storing large strings (over 2\ :sup:`31` bytes long). Large string data is stored in
     variable-length chunks.
     """
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, str, Callable[[], str]] = None,
     ):
         super().__init__(
             pa.large_string(), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -681,15 +727,15 @@
     Internally, this column stores dates as 32-bit integers which
     represent time since the UNIX epoch.
 
     """
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.date32(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
@@ -711,15 +757,15 @@
     Internally, this column stores dates as 64-bit integers which
     represent time since the UNIX epoch in milliseconds, where the
     values are evenly divisible by 86,400,000.
     """
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.date64(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
@@ -761,15 +807,15 @@
         can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         unit: str,
         tz: Optional[str] = None,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, datetime.datetime, Callable[[], datetime.datetime]] = None,
     ):
         super().__init__(
             pa.timestamp(unit, tz), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -805,15 +851,15 @@
     :param default: An optional default value for the column. This
         can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         unit: str,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, datetime.time, Callable[[], datetime.time]] = None,
     ):
         super().__init__(
             pa.time32(unit), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -849,15 +895,15 @@
     :param default: An optional default value for the column. This
         can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         unit: str,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, datetime.time, Callable[[], datetime.time]] = None,
     ):
         super().__init__(
             pa.time64(unit), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -886,15 +932,15 @@
     :param metadata: Optional metadata to associate with the column.
     :param validator: An optional validator to apply to the column.
     """
 
     def __init__(
         self,
         unit: str,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.duration(unit), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
@@ -920,15 +966,15 @@
 
     Leap seconds are ignored.
 
     """
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(
             pa.month_day_nano_interval(), nullable=nullable, metadata=metadata, validator=validator
         )
 
@@ -949,15 +995,15 @@
 
 
 class BinaryColumn(Column):
     """A column for storing opaque binary data."""
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, bytes, Callable[[], bytes]] = None,
     ):
         super().__init__(
             pa.binary(-1), nullable=nullable, metadata=metadata, validator=validator, default=default
         )
@@ -986,15 +1032,15 @@
     :param default: An optional default value for the column. This
         can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         byte_width: int,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
         default: Union[None, bytes, Callable[[], bytes]] = None,
     ):
         self.byte_width = byte_width
         super().__init__(
             pa.binary(byte_width), nullable=nullable, metadata=metadata, validator=validator, default=default
@@ -1042,15 +1088,15 @@
         can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         precision: int,
         scale: int,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         default: Union[None, decimal.Decimal, Callable[[], decimal.Decimal]] = None,
     ):
         super().__init__(
             pa.decimal128(precision, scale), nullable=nullable, metadata=metadata, default=default
         )
 
@@ -1086,15 +1132,15 @@
         can be a scalar value or a callable that takes no arguments.
     """
 
     def __init__(
         self,
         precision: int,
         scale: int,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         default: Union[None, decimal.Decimal, Callable[[], decimal.Decimal]] = None,
     ):
         super().__init__(
             pa.decimal256(precision, scale), nullable=nullable, metadata=metadata, default=default
         )
 
@@ -1118,15 +1164,15 @@
     Nulls are represented as a single bit, and do not take up any
     memory space.
 
     """
 
     def __init__(
         self,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.null(), nullable=nullable, metadata=metadata, validator=validator)
 
     @overload
     def __get__(self, obj: None, objtype: type) -> Self:
@@ -1146,27 +1192,28 @@
 
 
 class ListColumn(Column):
     """A column for storing variably-sized lists of values.
 
     The values in the list can be of any type.
 
-    Note that all quivr tables.Tables are storing lists of values, so this
+    Note that all quivr Tables are storing lists of values, so this
     column type is only useful for storing lists of lists.
 
     :param value_type: The type of the values in the list.
     :param nullable: Whether the list can contain null values.
     :param metadata: A dictionary of metadata to attach to the column.
     :param validator: A validator to run against the column's values.
+
     """
 
     def __init__(
         self,
         value_type: Union[pa.DataType, pa.Field, Column],
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(pa.list_(value_type, -1), nullable=nullable, metadata=metadata, validator=validator)
 
@@ -1199,15 +1246,15 @@
     :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         value_type: Union[pa.DataType, pa.Field, Column],
         list_size: int,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         if list_size <= 0:
             raise ValueError("list_size must be greater than 0")
         if isinstance(value_type, Column):
             value_type = value_type.dtype
@@ -1245,15 +1292,15 @@
     :param metadata: A dictionary of metadata to attach to the column.
     :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         value_type: Union[pa.DataType, pa.Field, Column],
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         if isinstance(value_type, Column):
             value_type = value_type.dtype
         super().__init__(pa.large_list(value_type), nullable=nullable, metadata=metadata, validator=validator)
 
@@ -1284,15 +1331,15 @@
     :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         key_type: Union[pa.DataType, pa.Field, Column],
         item_type: Union[pa.DataType, pa.Field, Column],
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         if isinstance(key_type, Column):
             key_type = key_type.dtype
         if isinstance(item_type, Column):
             item_type = item_type.dtype
@@ -1329,15 +1376,15 @@
     """
 
     def __init__(
         self,
         index_type: pa.DataType,
         value_type: Union[pa.DataType, pa.Field, Column],
         ordered: bool = False,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         if isinstance(index_type, Column):
             index_type = index_type.dtype
         if isinstance(value_type, Column):
             value_type = value_type.dtype
@@ -1374,15 +1421,15 @@
     :param validator: A validator to run against the column's values.
 
     """
 
     def __init__(
         self,
         fields: list[pa.Field],
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(pa.struct(fields), nullable=nullable, metadata=metadata, validator=validator)
 
 
 class RunEndEncodedColumn(Column):
@@ -1408,15 +1455,15 @@
     :param validator: A validator to run against the column's values.
     """
 
     def __init__(
         self,
         run_end_type: pa.DataType,
         value_type: pa.DataType,
-        nullable: bool = True,
+        nullable: bool = False,
         metadata: Optional[MetadataDict] = None,
         validator: Optional[validators.Validator] = None,
     ):
         super().__init__(
             pa.run_end_encoded(run_end_type, value_type),
             nullable=nullable,
             metadata=metadata,
```

### Comparing `quivr-0.6.0rc2/quivr/concat.py` & `quivr-0.6.1/quivr/concat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Iterator
 
 import pyarrow as pa
 
-from . import errors, tables
-from .defragment import defragment
+from . import defragment, errors, tables
 
 
 def concatenate(values: Iterator[tables.AnyTable], defrag: bool = True) -> tables.AnyTable:
     """Concatenate a collection of Tables into a single Table.
 
     All input Tables be of the same class, and have the same attribute
     values (if any).
@@ -40,9 +39,9 @@
                 )
 
     if len(batches) == 0:
         raise ValueError("No values to concatenate")
     table = pa.Table.from_batches(batches)
     result = first_cls.from_pyarrow(table=table)
     if defrag:
-        result = defragment(result)
+        result = defragment.defragment(result)
     return result
```

### Comparing `quivr-0.6.0rc2/quivr/errors.py` & `quivr-0.6.1/quivr/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Any, Optional
 
 import pyarrow
 
+from . import columns
+
 
 class InvariantViolatedError(RuntimeError):
     """
     Exception raised when an invariant expectation is violated.
     """
 
     ...
@@ -72,7 +74,18 @@
 
 class AttributeImmutableError(RuntimeError):
     """Exception raised when an attempt is made to modify an immutable
     attribute.
     """
 
     ...
+
+
+class InvalidColumnDataError(Exception):
+    """
+    Exception raised when invalid data is provided to populate a particular column
+    """
+
+    def __init__(self, column: columns.Column, msg: str):
+        self.column = column
+        msg = f"Invalid data provided for column {column.name}: {msg}"
+        super().__init__(msg)
```

### Comparing `quivr-0.6.0rc2/quivr/linkage.py` & `quivr-0.6.1/quivr/linkage.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,56 +193,54 @@
 
     The dictionaries must have the same keys, and the arrays must:
       - be identically typed under the same keys
       - have no null values
       - be the same length as the associated table
 
     Example:
-        >>> from quivr import *
-        >>> class Positions(Table):
-        ...     x = Float32Column()
-        ...     y = Float32Column()
-        ...     time = TimestampColumn(unit="s")
-        ...     id = UInt32Column()
+        >>> import quivr as qv
+        >>> class Positions(qv.Table):
+        ...     x = qv.Float32Column()
+        ...     y = qv.Float32Column()
+        ...     time = qv.TimestampColumn(unit="s")
+        ...     id = qv.UInt32Column()
         ...
-        >>> class Velocities(tables.Table):
-        ...     vx = Float32Column()
-        ...     vy = Float32Column()
-        ...     time = TimestampColumn(unit="s")
-        ...     id = UInt32Column()
+        >>> class Velocities(qv.Table):
+        ...     vx = qv.Float32Column()
+        ...     vy = qv.Float32Column()
+        ...     time = qv.TimestampColumn(unit="s")
+        ...     id = qv.UInt32Column()
         ...
-        >>> positions = Positions.from_data(
+        >>> positions = Positions.from_kwargs(
         ...     x=[0.0, 1.0, 2.0, 3.0, 4.0],
         ...     y=[0.0, 1.0, 2.0, 3.0, 4.0],
         ...     time=[0, 1, 2, 3, 4],
         ...     id=[0, 1, 1, 2, 2],
         ... )
-        >>> velocities = Velocities.from_data(
+        >>> velocities = Velocities.from_kwargs(
         ...     vx=[0.0, 1.0, 2.0, 3.0, 4.0],
         ...     vy=[0.0, 1.0, 2.0, 3.0, 4.0],
         ...     time=[0, 1, 2, 3, 4],
         ...     id=[0, 1, 1, 2, 2],
         ... )
-        >>> linkage = MultiKeyLinkage(
+        >>> linkage = qv.MultiKeyLinkage(
         ...     positions,
         ...     velocities,
         ...     {"id": positions.id, "time": positions.time},
         ...     {"id": velocities.id, "time": velocities.time},
         ... )
         >>> for val, left, right in sorted(linkage, key=lambda x: (x[0][1].as_py())):
         ...     print(val, left, right)
         [('id', 0), ('time', datetime.datetime(1970, 1, 1, 0, 0))] Positions(size=1) Velocities(size=1)
         [('id', 1), ('time', datetime.datetime(1970, 1, 1, 0, 0, 1))] Positions(size=1) Velocities(size=1)
         [('id', 1), ('time', datetime.datetime(1970, 1, 1, 0, 0, 2))] Positions(size=1) Velocities(size=1)
         [('id', 2), ('time', datetime.datetime(1970, 1, 1, 0, 0, 3))] Positions(size=1) Velocities(size=1)
         [('id', 2), ('time', datetime.datetime(1970, 1, 1, 0, 0, 4))] Positions(size=1) Velocities(size=1)
 
 
-
-
     :param left_table: The left table to link.
     :param right_table: The right table to link.
     :param left_keys: A dictionary of key names to arrays of values. The arrays
         must be the same length as the left table, and must not contain null
         values. The key names must be the same as the right keys.
     :param right_keys: A dictionary of key names to arrays of values. The
         arrays must be the same length as the right table, and must not contain
@@ -319,40 +317,40 @@
         return self
 
     def key(self, **kwargs: Any) -> pa.Scalar:
         """
         Returns a composite key scalar for the given values.
 
         Example:
-            >>> from quivr import *
-            >>> class Positions(Table):
-            ...     x = Float32Column()
-            ...     y = Float32Column()
-            ...     time = TimestampColumn(unit="s")
-            ...     id = UInt32Column()
+            >>> import quivr as qv
+            >>> class Positions(qv.Table):
+            ...     x = qv.Float32Column()
+            ...     y = qv.Float32Column()
+            ...     time = qv.TimestampColumn(unit="s")
+            ...     id = qv.UInt32Column()
             ...
-            >>> class Velocities(tables.Table):
-            ...     vx = Float32Column()
-            ...     vy = Float32Column()
-            ...     time = TimestampColumn(unit="s")
-            ...     id = UInt32Column()
+            >>> class Velocities(qv.Table):
+            ...     vx = qv.Float32Column()
+            ...     vy = qv.Float32Column()
+            ...     time = qv.TimestampColumn(unit="s")
+            ...     id = qv.UInt32Column()
             ...
-            >>> positions = Positions.from_data(
+            >>> positions = Positions.from_kwargs(
             ...     x=[0.0, 1.0, 2.0, 3.0, 4.0],
             ...     y=[0.0, 1.0, 2.0, 3.0, 4.0],
             ...     time=[0, 1, 2, 3, 4],
             ...     id=[0, 1, 1, 2, 2],
             ... )
-            >>> velocities = Velocities.from_data(
+            >>> velocities = Velocities.from_kwargs(
             ...     vx=[0.0, 1.0, 2.0, 3.0, 4.0],
             ...     vy=[0.0, 1.0, 2.0, 3.0, 4.0],
             ...     time=[0, 1, 2, 3, 4],
             ...     id=[0, 1, 1, 2, 2],
             ... )
-            >>> linkage = MultiKeyLinkage(
+            >>> linkage = qv.MultiKeyLinkage(
             ...     positions,
             ...     velocities,
             ...     {"time": positions.time, "id": positions.id},
             ...     {"time": velocities.time, "id": velocities.id},
             ... )
             >>> key = linkage.key(time=1, id=1)
             >>> key
```

### Comparing `quivr-0.6.0rc2/quivr/schemagraph.py` & `quivr-0.6.1/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc2/quivr/tables.py` & `quivr-0.6.1/quivr/tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import os
 import sys
+import warnings
 from io import IOBase
 
 if sys.version_info < (3, 11):
     from typing_extensions import Self
 else:
     from typing import Self
 
 from typing import (
     Any,
     ClassVar,
     Iterator,
+    List,
     Optional,
+    Protocol,
     Type,
     TypeAlias,
     TypeVar,
     Union,
     cast,
 )
 
@@ -26,24 +29,42 @@
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.csv
 import pyarrow.feather
 import pyarrow.parquet
 
-from . import columns
-from .attributes import Attribute
-from .errors import TableFragmentedError, ValidationError
-from .schemagraph import _walk_schema
-from .validators import Validator
+from . import attributes, columns, errors, schemagraph, validators
+
+
+class ArrowArrayProvider(Protocol):
+    """
+    A Protocol which describes objects that support the Arrow custom array extension protocol.
+    """
+
+    def __arrow_array__(self, type: Optional[pa.DataType] = None) -> pa.Array:
+        ...
+
 
 AttributeValueType: TypeAlias = Union[int, float, str]
-DataSourceType: TypeAlias = Union[pa.Array, list[Any], "Table", pd.Series, npt.NDArray[Any]]
+DataSourceType: TypeAlias = Union[
+    pa.Array, list[Any], "Table", pd.Series, npt.NDArray[Any], ArrowArrayProvider
+]
 AnyTable = TypeVar("AnyTable", bound="Table")
 
+# If a table uses any of the following names, it will break quivr
+# internals entirely, so they must be rejected.
+_FORBIDDEN_COLUMN_NAMES = {
+    "table",
+    "schema",
+    "_quivr_subtables",
+    "_quivr_attributes",
+    "_column_validators",
+}
+
 
 class Table:
     """Table is the primary data structure in quivr.
 
     Tables are used to represent tabular data with a fixed schema. The
     schema is defined by subclassing Table, providing Column objects
     as class attributes. The Table class will then generate a pyarrow
@@ -62,44 +83,51 @@
     :vartype schema: pyarrow.Schema
 
     :ivar table: The underlying :class:`pyarrow.Table` for this Table instance.
     :vartype table: pyarrow.Table
     """
 
     schema: ClassVar[pa.Schema]
+
+    #: Instance variable
+    #: does it work?
     table: pa.Table
 
     _quivr_subtables: ClassVar[dict[str, columns.SubTableColumn[Any]]]
-    _quivr_attributes: ClassVar[dict[str, Attribute[Any]]]
-    _column_validators: ClassVar[dict[str, Validator]]
+    _quivr_attributes: ClassVar[dict[str, attributes.Attribute[Any]]]
+    _column_validators: ClassVar[dict[str, validators.Validator]]
 
     def __init_subclass__(cls: Type["Table"], **kwargs: Any):
         fields = []
         column_validators = {}
         subtables = {}
-        attributes = {}
+        attrs = {}
         for name, obj in cls.__dict__.items():
+            if name in _FORBIDDEN_COLUMN_NAMES:
+                raise AttributeError(
+                    f"Invalid column name {name} in {cls.__name__}: {name} is a reserved name"
+                )
             if isinstance(obj, columns.Column):
                 fields.append(obj.pyarrow_field())
                 if obj.validator is not None:
                     column_validators[name] = obj.validator
                 if isinstance(obj, columns.SubTableColumn):
                     subtables[name] = obj
-            elif isinstance(obj, Attribute):
-                attributes[name] = obj
+            elif isinstance(obj, attributes.Attribute):
+                attrs[name] = obj
 
         # Generate a pyarrow schema
         schema = pa.schema(fields)
         cls.schema = schema
 
         # Keep track of subtables
         cls._quivr_subtables = subtables
 
         # Add attributes
-        cls._quivr_attributes = attributes
+        cls._quivr_attributes = attrs
 
         # Add validators
         cls._column_validators = column_validators
 
         super().__init_subclass__(**kwargs)
 
     def __init__(self, table: pa.Table, **kwargs: AttributeValueType):
@@ -164,42 +192,18 @@
         precise constructors (from_arrays, from_pylist, etc) should be
         preferred.
 
         If the validate argument is True, the data will be validated
         against the table's schema. If validation fails, a
         :class:`ValidationError` will be raised.
 
-        For example:
-
-            >>> import quivr
-            >>> class MyTable(quivr.Table):
-            ...     a = quivr.StringColumn()
-            ...     b = quivr.Int64Column()
-            ...
-            >>> # All of these are equivalent:
-            >>> MyTable.from_data({"a": ["a", "b"], "b": [1, 2]})
-            MyTable(size=2)
-            >>> MyTable.from_data([{"a": "a", "b": 1}, {"a": "b", "b": 2}])
-            MyTable(size=2)
-            >>> MyTable.from_data(a=["a", "b"], b=[1, 2])
-            MyTable(size=2)
-            >>> import numpy as np
-            >>> MyTable.from_data(a=np.array(["a", "b"]), b=np.array([1, 2]))
-            MyTable(size=2)
-
-        :param data: The data to populate the table with.
-        :param validate: Whether to validate the data against the table's schema.
-        :param \\**kwargs: More data in keyword argument form. The keys
-          can be column names or attribute names. The values should be
-          arrays, lists, or pyarrow Arrays.
-        :type \\**kwargs: Union[:obj:`AttributeValueType`, :obj:`DataSourceType`]
-
         """
+        warnings.warn(DeprecationWarning("Table.from_data will be removed in quivr version 0.7"))
         if data is None:
-            instance = cls.from_kwargs(**kwargs)
+            instance = cls.from_kwargs(validate=validate, **kwargs)
         else:
             attrib_kwargs = cls._attribute_kwargs_from_kwargs(kwargs)
             if isinstance(data, pa.Table):
                 instance = cls.from_pyarrow(data, False, **attrib_kwargs)
             elif isinstance(data, dict):
                 instance = cls.from_pydict(data, **attrib_kwargs)
             elif isinstance(data, list):
@@ -208,15 +212,15 @@
                 elif isinstance(data[0], dict):
                     instance = cls.from_rows(data, **attrib_kwargs)
                 elif isinstance(data[0], list):
                     instance = cls.from_lists(data, **attrib_kwargs)
                 else:
                     raise TypeError(f"Unsupported type: {type(data[0])}")
             elif isinstance(data, pd.DataFrame):
-                instance = cls.from_dataframe(data, **attrib_kwargs)
+                instance = cls.from_dataframe(data, validate, **attrib_kwargs)
             else:
                 raise TypeError(f"Unsupported type: {type(data)}")
 
         if validate:
             instance.validate()
         return instance
 
@@ -249,100 +253,101 @@
 
         :param metadata: Metadata to attach to the column.
 
         """
         return columns.SubTableColumn(cls, nullable=nullable, metadata=metadata)
 
     @classmethod
-    def from_kwargs(cls, **kwargs: Union[DataSourceType, AttributeValueType]) -> Self:
+    def from_kwargs(cls, validate: bool = True, **kwargs: Union[DataSourceType, AttributeValueType]) -> Self:
         """Create a Table instance from keyword arguments.
 
         Each keyword argument corresponds to a column in the Table.
 
         The keys should correspond to column names or attribute names.
 
         For columns, the values should be arrays, lists, or pyarrow Arrays.
 
         For attributes, the values should be the appropriate type for that attribute.
 
+        :param validate: If (the default), run column validators on all input data.
         :param \\**kwargs: The data to populate the table with.
         :type \\**kwargs: Union[:obj:`AttributeValueType`, :obj:`DataSourceType`]
 
         """
         arrays: list[Union[None, pa.Array]] = []
         size = None
+        size_col = ""
 
         # We don't know the size of the table until we've found a
         # field in the schema which corresponds to a kwarg with data.
         # Therefore, we need to keep track of which columns are empty
         # *before* we've discovered the size of the table so we can
         # populate them with nulls later.
         empty_columns = []
 
         metadata: dict[bytes, bytes] = {}
         for i, field in enumerate(cls.schema):
             column_name = field.name
-            value = kwargs.pop(column_name, None)
+            column = getattr(cls, column_name)
 
-            if value is None:
-                if not field.nullable:
-                    column = getattr(cls, column_name)
-                    if column.default is None:
-                        raise ValueError(f"Missing non-nullable column {column_name}")
-                if size is not None:
-                    value = pa.nulls(size, type=cls.schema[i].type)
-                    arrays.append(value)
-                else:
-                    # We'll have to wait until we get to a non-None column
-                    # to figure out the size.
-                    empty_columns.append(i)
-                    arrays.append(None)
+            value = kwargs.pop(column_name, None)
+            array = column._load(value, size)
+            if array is None:
+                # We'll have to wait until we get to a non-None column
+                # to figure out the size.
+                empty_columns.append(i)
+                arrays.append(None)
                 continue
 
             if size is None:
-                size = len(value)  # type: ignore
-            elif len(value) != size:
-                raise ValueError(
-                    f"Column {column_name} has wrong length {len(value)} (first column has length {size})"
+                size = len(array)
+                size_col = column_name
+            elif len(array) != size:
+                raise errors.InvalidColumnDataError(
+                    column,
+                    f"wrong length {len(value)} (expected {size} based on column {size_col})",
                 )
 
+            arrays.append(array)
+
             if isinstance(value, Table):
                 field_meta = value.table.schema.metadata
                 if field_meta is not None:
                     for key, val in field_meta.items():
                         key = (field.name + "." + key.decode("utf-8")).encode("utf-8")
                         metadata[key] = val
-                arrays.append(value.to_structarray())
-            elif isinstance(value, pa.Array):
-                arrays.append(value)
-            elif isinstance(value, np.ndarray):
-                arrays.append(pa.array(value, type=field.type))
-            elif isinstance(value, list):
-                arrays.append(pa.array(value, type=field.type))
-            elif isinstance(value, pd.Series):
-                arrays.append(pa.array(value, type=field.type))
-            else:
-                raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
 
         if size is None:
             raise ValueError("No data provided")
 
         for idx in empty_columns:
-            arrays[idx] = pa.nulls(size, type=cls.schema[idx].type)
+            column = getattr(cls, cls.schema[idx].name)
+            arrays[idx] = column._nulls(size)
 
         # Inform the type checker that we've filled all Nones
         arrays = cast(list[pa.Array], arrays)
 
         for i, array in enumerate(arrays):
             if array.null_count > 0:
                 column = getattr(cls, cls.schema[i].name)
                 arrays[i] = column.fill_default(array)
 
+        pyarrow_table = cls._build_arrow_table(arrays, metadata)
         attrib_kwargs = cls._attribute_kwargs_from_kwargs(kwargs)
-        return cls.from_arrays(arrays, metadata=metadata, **attrib_kwargs)
+        return cls.from_pyarrow(table=pyarrow_table, validate=validate, **attrib_kwargs)
+
+    @classmethod
+    def _build_arrow_table(cls, arrays: List[pa.Array], metadata: dict[bytes, bytes]) -> pa.Table:
+        """
+        Construct a pyarrow Table which will back cls from a list of arrays. The
+        Table's schema comes from cls.schema.
+        """
+        schema = cls.schema.with_metadata(metadata)
+        table = pa.Table.from_arrays(arrays, schema=schema)
+        return table
 
     @classmethod
     def from_arrays(
         cls,
         arrays: list[pa.Array],
         metadata: Optional[dict[bytes, bytes]] = None,
         **kwargs: AttributeValueType,
@@ -352,50 +357,39 @@
 
         :param arrays: A list of pyarrow.Array objects.
         :param metadata: An optional dictionary of metadata to attach to the Table.
         :param \\**kwargs: Additional keyword arguments for any Table attributes.
         :type \\**kwargs: :obj:`AttributeValueType`
         :return: A Table object.
         """
+        warnings.warn(DeprecationWarning("Table.from_arrays will be removed in quivr version 0.7"))
         if metadata is None:
             metadata = {}
-        schema = cls.schema.with_metadata(metadata)
-        table = pa.Table.from_arrays(arrays, schema=schema)
+        table = cls._build_arrow_table(arrays, metadata)
         return cls.from_pyarrow(table=table, validate=False, **kwargs)
 
     @classmethod
     def from_pydict(
         cls, d: dict[str, Union[pa.array, list[Any], npt.NDArray[Any]]], **kwargs: AttributeValueType
     ) -> Self:
+        warnings.warn(DeprecationWarning("Table.from_pydict will be removed in quivr version 0.7"))
         table = pa.Table.from_pydict(d, schema=cls.schema)
         return cls.from_pyarrow(table=table, validate=False, **kwargs)
 
     @classmethod
     def from_rows(cls, rows: list[dict[str, Any]], **kwargs: AttributeValueType) -> Self:
         """
         Create a Table object from a list of dictionaries.
 
         :param rows: A list of values. Each value corresponds to a row in the table.
         :param \\**kwargs: Additional keyword arguments for any Table attributes.
         :type \\**kwargs: :obj:`AttributeValueType`
         :returns: A Table object.
-
-        Examples:
-            >>> import quivr
-            >>> class Inner(quivr.Table):
-            ...     a = quivr.StringColumn()
-            ...
-            >>> class Outer(quivr.Table):
-            ...     z = quivr.StringColumn()
-            ...     i = Inner.as_column()
-            ...
-            >>> data = [{"z": "v1", "i": {"a": "v1_in"}}, {"z": "v2", "i": {"a": "v2_in"}}]
-            >>> Outer.from_rows(data)
-            Outer(size=2)
         """
+        warnings.warn(DeprecationWarning("Table.from_rows will be removed in quivr version 0.7"))
         table = pa.Table.from_pylist(rows, schema=cls.schema)
         return cls(table=table, **kwargs)
 
     @classmethod
     def from_lists(cls, lists: list[list[Any]], **kwargs: AttributeValueType) -> Self:
         """Create a Table object from a list of lists.
 
@@ -405,37 +399,40 @@
 
         :param lists: A list of lists. Each inner list corresponds to a column in the table.
         :param \\**kwargs: Additional keyword arguments for any Table attributes.
         :type \\**kwargs: :obj:`AttributeValueType`
         :returns: A Table object.
 
         """
-        table = pa.Table.from_arrays(list(map(pa.array, lists)), schema=cls.schema)
-        return cls(table=table, **kwargs)
+        warnings.warn(DeprecationWarning("Table.from_lists will be removed in quivr version 0.7"))
+        arrays = list(map(pa.array, lists))
+        table = cls._build_arrow_table(arrays, {})
+        return cls.from_pyarrow(table=table, validate=False, **kwargs)
 
     @classmethod
-    def from_dataframe(cls, df: pd.DataFrame, **kwargs: AttributeValueType) -> Self:
+    def from_dataframe(cls, df: pd.DataFrame, validate: bool = True, **kwargs: AttributeValueType) -> Self:
         """Load a DataFrame into the Table.
 
         If the DataFrame is missing any of the Table's columns, an
         error is raised. If the DataFrame has extra columns, they are
         ignored.
 
         This function cannot load "flattened" dataframes. This only
         matters for nested Tables which contain other Table
         definitions as columns. For that use case, either load an
         unflattened DataFrame, or use from_flat_dataframe.
 
         :param df: A pandas DataFrame containing the data to load.
+        :param validate: Whether to validate the data after loading.
         :param \\**kwargs: Additional keyword arguments for any Table attributes.
         :type \\**kwargs: :obj:`AttributeValueType`
         """
 
         table = pa.Table.from_pandas(df, schema=cls.schema)
-        return cls.from_pyarrow(table=table, validate=False, **kwargs)
+        return cls.from_pyarrow(table=table, validate=validate, **kwargs)
 
     @classmethod
     def _unflatten_table(cls, table: pa.Table) -> pa.Table:
         """Unflatten a Table.
 
         This is used when loading a flattened CSV into a nested
         Table. It takes a Table with a flat schema, and returns a
@@ -468,32 +465,36 @@
                 child_arrays.append(struct_array_for(field, []))
             else:
                 child_arrays.append(table.column(field.name).combine_chunks())
 
         return pa.Table.from_arrays(child_arrays, schema=cls.schema)
 
     @classmethod
-    def from_flat_dataframe(cls, df: pd.DataFrame, **kwargs: AttributeValueType) -> Self:
+    def from_flat_dataframe(
+        cls, df: pd.DataFrame, validate: bool = True, **kwargs: AttributeValueType
+    ) -> Self:
         """Load a flattened DataFrame into the Table.
 
         .. caution::
           Known bug: Doesn't correctly interpret fixed-length lists.
 
         :param df: A pandas DataFrame containing the data to load.
+        :param validate: Whether to validate the data after loading.
         :param \\**kwargs: Additional keyword arguments for any Table attributes.
         :type \\**kwargs: :obj:`AttributeValueType`
 
         """
         struct_fields = []
         for field in cls.schema:
             if pa.types.is_struct(field.type):
                 struct_fields.append(field)
 
         if len(struct_fields) == 0:
-            return cls(table=pa.Table.from_pandas(df, schema=cls.schema), **kwargs)
+            table = pa.Table.from_pandas(df, schema=cls.schema)
+            return cls.from_pyarrow(table=table, validate=validate, **kwargs)
 
         root = pa.field("", pa.struct(cls.schema))
 
         # Walk the schema, and build a StructArray for each embedded
         # type. These are stored in a dictionary, keyed by their
         # dot-separated path. For example, if the schema is:
         #
@@ -543,25 +544,25 @@
                     arrays.append(field_df[subfield.name])
             sa = pa.StructArray.from_arrays(arrays, fields=list(field.type))
             struct_arrays[df_key] = sa
 
             # Clean the fields out
             df = df.drop(field_columns, axis="columns")
 
-        _walk_schema(root, visitor, None)
+        schemagraph._walk_schema(root, visitor, None)
         # Now build a table back up. Grab the root-level struct array.
         sa = struct_arrays[""]
 
         table_arrays = []
         for subfield in cls.schema:
             # Pull out the fields of that root-level struct array.
             table_arrays.append(sa.field(subfield.name))
 
         table = pa.Table.from_arrays(table_arrays, schema=cls.schema)
-        return cls(table=table, **kwargs)
+        return cls.from_pyarrow(table, validate=validate, **kwargs)
 
     def flattened_table(self) -> pa.Table:
         """Completely flatten the Table's underlying Arrow table,
         taking into account any nested structure, and return the data
         table itself.
         """
 
@@ -618,15 +619,15 @@
 
         This only works if self is not fragmented. Call table =
         defragment(table) if table.fragmented() is True.
 
         :raises TableFragmentedError: if the table is fragmented.
         """
         if self.fragmented():
-            raise TableFragmentedError(
+            raise errors.TableFragmentedError(
                 "Tables cannot be converted to StructArrays while fragmented; call defragment(table) first."
             )
         arrays = [chunked_array.chunks[0] for chunked_array in self.table.columns]
         return pa.StructArray.from_arrays(arrays, fields=list(self.schema))
 
     def to_dataframe(self, flatten: bool = True) -> pd.DataFrame:
         """Returns self as a pandas DataFrame.
@@ -748,14 +749,15 @@
     def from_parquet(
         cls,
         path: str,
         memory_map: bool = False,
         pq_buffer_size: int = 0,
         filters: Optional[pc.Expression] = None,
         column_name_map: Optional[dict[str, str]] = None,
+        validate: bool = True,
         **kwargs: AttributeValueType,
     ) -> Self:
         """Read a table from a Parquet file.
 
         :param path: The path to the Parquet file.
         :param memory_map: If True, memory-map the file, otherwise read it into memory.
 
@@ -767,37 +769,43 @@
                 removed from scanned data. For more information, see
                 the PyArrow documentation on
                 pyarrow.parquet.read_table and its filter parameter.
         :param column_name_map: An optional dictionary mapping column names in the Parquet file to
                 column names in the resulting Table. This is useful if the Parquet file contains
                 column names that are not valid Python identifiers, or if you want to rename
                 columns for any other reason.
+        :param validate: Whether to run column validation on the resulting Table.
         :param \\**kwargs: Additional keyword arguments to pass to Self's __init__ method.
 
         """
         table = cls._load_parquet_table(
             path=path,
             memory_map=memory_map,
             pq_buffer_size=pq_buffer_size,
             filters=filters,
             column_name_map=column_name_map,
         )
-        return cls.from_pyarrow(table=table, validate=True, **kwargs)
+        return cls.from_pyarrow(table=table, validate=validate, **kwargs)
 
     @classmethod
     def _load_parquet_table(
         cls,
         path: str,
         memory_map: bool,
         pq_buffer_size: int,
         filters: Optional[pc.Expression],
         column_name_map: Optional[dict[str, str]],
     ) -> pa.Table:
         if column_name_map is not None:
-            inverted_map = {v: k for k, v in column_name_map.items()} if column_name_map else {}
+            for value in column_name_map.values():
+                if value not in cls.schema.names:
+                    raise ValueError(
+                        f"Column name {value} does not exist for {cls.__name__}, so cannot rename to it"
+                    )
+            inverted_map = {v: k for k, v in column_name_map.items()}
             column_names = [inverted_map.get(field.name, field.name) for field in cls.schema]
             schema = pa.schema(
                 [pa.field(inverted_map.get(field.name, field.name), field.type) for field in cls.schema]
             )
         else:
             column_names = [field.name for field in cls.schema]
             schema = cls.schema
@@ -824,21 +832,23 @@
 
         :param path: The path to write the Feather file to.
         :param kwargs: Additional arguments to pass to pyarrow.feather.write_feather.
         """
         pyarrow.feather.write_feather(self.table, path, **kwargs)
 
     @classmethod
-    def from_feather(cls, path: str, **kwargs: AttributeValueType) -> Self:
+    def from_feather(cls, path: str, validate: bool = True, **kwargs: AttributeValueType) -> Self:
         """Read a table from a Feather file.
 
         :param path: The path to the Feather file.
+        :param validate: Whether to run column validators on the table after loading it.
         :param \\**kwargs: Additional keyword arguments to pass to Self's __init__ method.
         """
-        return cls(table=pyarrow.feather.read_table(path), **kwargs)
+        table = pyarrow.feather.read_table(path)
+        return cls.from_pyarrow(table=table, validate=validate, **kwargs)
 
     def to_csv(self, path: str, attribute_columns: bool = True) -> None:
         """Write the table to a CSV file. Any nested structure is flattened.
 
         :param path: The path to write the CSV file to.
         :param attribute_columns: If True, store any Attributes defined for the table
             (or its subtable columns) as columns in the CSV file. If False, do not store
@@ -851,15 +861,18 @@
                     name,
                     pa.repeat(val, len(table)),
                 )
         pyarrow.csv.write_csv(table, path)
 
     @classmethod
     def from_csv(
-        cls, input_file: Union[str, os.PathLike, IOBase], **kwargs: AttributeValueType  # type: ignore
+        cls,
+        input_file: Union[str, os.PathLike, IOBase],  # type: ignore
+        validate: bool = True,
+        **kwargs: AttributeValueType,
     ) -> Self:
         """
         Read a table from a CSV file.
 
         :param input_file: The path to the CSV file, or a file-like object.
         :param \\**kwargs: Additional keyword arguments to set the Table's attributes.
         """
@@ -881,40 +894,40 @@
 
         attribute_meta = cls._unpack_string_metadata(attributes)
 
         table = cls._unflatten_table(flat_table)
         metadata = table.schema.metadata or {}
         metadata.update(attribute_meta)
         table = table.replace_schema_metadata(metadata)
-        return cls(table, **kwargs)
+        return cls.from_pyarrow(table=table, validate=validate, **kwargs)
 
     def is_valid(self) -> bool:
         """Validate the table against the schema."""
         for name, validator in self._column_validators.items():
             if not validator.valid(self.table.column(name)):
                 return False
         return True
 
     def validate(self) -> None:
         """Validate the table against the schema, raising an exception if invalid."""
         for name, validator in self._column_validators.items():
             try:
                 validator.validate(self.table.column(name))
-            except ValidationError as e:
-                raise ValidationError(f"Column {name} failed validation: {str(e)}", e.failures) from e
+            except errors.ValidationError as e:
+                raise errors.ValidationError(f"Column {name} failed validation: {str(e)}", e.failures) from e
 
     @classmethod
     def empty(cls, **kwargs: AttributeValueType) -> Self:
         """Create an empty instance of the table.
 
         :param \\**kwargs: Additional keyword arguments to set the Table's attributes.
         """
         data = [[] for _ in range(len(cls.schema))]  # type: ignore
         empty_table = pa.table(data, schema=cls.schema)
-        return cls(table=empty_table, **kwargs)
+        return cls.from_pyarrow(table=empty_table, validate=False, **kwargs)
 
     def attributes(self) -> dict[str, Any]:
         """Return a dictionary of the table's attributes."""
         return {name: getattr(self, name) for name in self._quivr_attributes}
 
     def _string_attributes(self) -> dict[str, str]:
         """Return a dictionary of the table's attributes.
@@ -1000,20 +1013,29 @@
         Return a new table with rows filtered to match an expression.
 
         The expression must be a pyarrow Expression that evaluates to a boolean array.
 
         :param expr: A pyarrow Expression to apply to the table.
 
         Examples:
-            >>> from quivr import Table, Int64Column
+            >>> import quivr as qv
             >>> import pyarrow.compute as pc
-            >>> class MyTable(Table):
-            ...     x = Int64Column()
-            ...     y = Int64Column()
-            >>> t = MyTable.from_data(x=[1, 2, 3], y=[4, 5, 6])
+            >>> class MyTable(qv.Table):
+            ...     x = qv.Int64Column()
+            ...     y = qv.Int64Column()
+            >>> t = MyTable.from_kwargs(x=[1, 2, 3], y=[4, 5, 6])
             >>> filtered = t.where(pc.field("x") > 1)
             >>> print(filtered.x.to_pylist())
             [2, 3]
             >>> print(filtered.y.to_pylist())
             [5, 6]
         """
         return self.__class__(self.table.filter(expr))
+
+    def __arrow_array__(self, type: Optional[pa.DataType] = None) -> pa.StructArray:
+        """
+        Implements the Arrow array protocol by returning as StructArray.
+        """
+        array = self.to_structarray()
+        if type is None:
+            return array
+        return array.cast(type)
```

### Comparing `quivr-0.6.0rc2/quivr/validators.py` & `quivr-0.6.1/quivr/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 
 import pyarrow
 import pyarrow.compute as pc
 
-from .errors import ValidationError
+from . import errors
 
 
 class Validator:
     """A Validator is a tool to validate that data in a
     :class:`pyarrow.Array` matches a predicate expression.
 
     :ivar func: The predicate function to use for validation. This
@@ -60,30 +60,30 @@
         """
         Raises a :class:`ValidationError` if the given array is not valid.
 
         :param array: The array to validate.
         """
         if not self.valid(array):
             if self.func.kind == "scalar_aggregate":
-                raise ValidationError(f"array did not pass validator '{self.label}'")
+                raise errors.ValidationError(f"array did not pass validator '{self.label}'")
             indices, failures = self.failures(array)
             if len(failures) == 1:
                 index = indices[0].as_py()
                 value = failures[0].as_py()
                 msg = f"val={value}, index={index} failed validator '{self.label}'"
-                raise ValidationError(msg, failures)
+                raise errors.ValidationError(msg, failures)
             else:
                 n_failed = len(failures)
                 index = indices[0].as_py()
                 value = failures[0].as_py()
                 msg = (
                     f"validator '{self.label}' failed on {n_failed} values, "
                     + f"first failure: val={value}, index={index}"
                 )
-                raise ValidationError(msg, failures)
+                raise errors.ValidationError(msg, failures)
 
     def failures(self, array: pyarrow.Array) -> tuple[pyarrow.Array, pyarrow.Array]:
         """
         Returns a tuple of two arrays, the first containing the indices of the invalid values,
         and the second containing the invalid values themselves.
 
         If the validator is a scalar aggregate function, raises a TypeError.
```

### Comparing `quivr-0.6.0rc2/LICENSE` & `quivr-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc2/README.md` & `quivr-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,32 +45,32 @@
 
 Your main entrypoint to Quivr is through defining classes which
 represent your tables. You write a subclass of quivr.Table, annotating
 it with Columns that describe the data you're working with, and quivr
 will handle the rest.
 
 ```python
-from quivr import Table, Float64Column
+import quivr as qv
 import pyarrow as pa
 
 
-class Coordinates(Table):
-	x = Float64Column()
-	y = Float64Column()
-	z = Float64Column()
-	vx = Float64Column()
-	vy = Float64Column()
-	vz = Float64Column()
+class Coordinates(qv.Table):
+	x = qv.Float64Column()
+	y = qv.Float64Column()
+	z = qv.Float64Column()
+	vx = qv.Float64Column()
+	vy = qv.Float64Column()
+	vz = qv.Float64Column()
 ```
 
 Then, you can construct tables from data:
 
 ```python
 
-coords = Coordinates.from_data(
+coords = Coordinates.from_kwargs(
     x=np.array([ 1.00760887, -2.06203093,  1.24360546, -1.00131722]),
     y=np.array([-2.7227298 ,  0.70239707,  2.23125432,  0.37269832]),
     z=np.array([-0.27148738, -0.31768623, -0.2180482 , -0.02528401]),
     vx=np.array([ 0.00920172, -0.00570486, -0.00877929, -0.00809866]),
     vy=np.array([ 0.00297888, -0.00914301,  0.00525891, -0.01119134]),
     vz=np.array([-0.00160217,  0.00677584,  0.00091095, -0.00140548])
 )
@@ -90,23 +90,23 @@
 
 ### Embedded definitions and nullable columns
 
 You can embed one table's definition within another, and you can make columns nullable:
 
 ```python
 
-class AsteroidOrbit(Table):
-	designation = StringColumn()
-	mass = Float64Column(nullable=True)
-	radius = Float64Column(nullable=True)
+class AsteroidOrbit(qv.Table):
+	designation = qv.StringColumn()
+	mass = qv.Float64Column(nullable=True)
+	radius = qv.Float64Column(nullable=True)
 	coords = Coordinates.as_column()
 
 # You can construct embedded columns from Arrow StructArrays, which you can get from
 # other Quivr tables using the to_structarray() method with zero copy.
-orbits = AsteroidOrbit.from_data(
+orbits = AsteroidOrbit.from_kwargs(
     designation=np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
     mass=np.array([9.393e20, 2.06e21, 2.59e20, None]),
     radius=np.array([4.6e6, 2.7e6, 2.6e6, None]),
     coords=coords.to_structarray(),
 )
 ```
 
@@ -146,41 +146,41 @@
 Because Quivr tables are just Python classes, you can customize the
 behavior of your tables by adding or overriding methods. For example, if you want to add a
 method to compute the total mass of the asteroids in the table, you
 can do so like this:
 
 ```python
 
-class AsteroidOrbit(Table):
-	designation = StringColumn()
-	mass = Float64Column(nullable=True)
-	radius = Float64Column(nullable=True)
+class AsteroidOrbit(qv.Table):
+	designation = qv.StringColumn()
+	mass = qv.Float64Column(nullable=True)
+	radius = qv.Float64Column(nullable=True)
 	coords = Coordinates.as_column()
 
     def total_mass(self):
         return pc.sum(self.mass)
 
 ```
 
 You can also use this to add "meta-columns" which are combinations of other columns. For example:
 
 ```python
-class CoordinateCovariance(Table):
-	matrix_values = ListColumn(pa.float64(), 36)
+class CoordinateCovariance(qv.Table):
+	matrix_values = qv.ListColumn(pa.float64(), 36)
 
     @property
     def matrix(self):
         # This is a numpy array of shape (n, 6, 6)
         return self.matrix_values.to_numpy().reshape(-1, 6, 6)
 
 
-class AsteroidOrbit(Table):
-	designation = StringColumn()
-	mass = Float64Column(nullable=True)
-	radius = Float64Column(nullable=True)
+class AsteroidOrbit(qv.Table):
+	designation = qv.StringColumn()
+	mass = qv.Float64Column(nullable=True)
+	radius = qv.Float64Column(nullable=True)
 	coords = Coordinates.as_column()
 	covariance = CoordinateCovariance.as_column()
 
 orbits = load_orbits() # Analogous to the example above
 
 # Compute the determinant of the covariance matrix for each asteroid
 determinants = np.linalg.det(orbits.covariance.matrix)
@@ -195,24 +195,24 @@
 if you do this, there are a few rules:
 
  1. Your `__init__` method must have an attribute called `table`, with
     type `pyarrow.Table`, and you must pass this to Table's `__init__`
     (via `super().__init__(table)`).
  2. You must implement a `with_table(self, table: pa.Table) -> Self`
     method which returns a **new** instance with the provided table,
-    bringing along the current values of all instance attributes.
+    bringingalong the current values of all instance attributes.
 
 For example:
 
 ```python
 from typing import Self
 
-class AsteroidOrbit(Table):
-    designation = StringColumn()
-	mass = Float64Column(nullable=True)
+class AsteroidOrbit(qv.Table):
+    designation = qv.StringColumn()
+	mass = qv.Float64Column(nullable=True)
 	
 	def __init__(self, table: pa.Table, mu: float):
 	    super().__init__(table)
 		self.mu = mu
 		
 	def with_table(self, table: pa.Table) -> Self:
         return AsteroidOrbit(table, self.mu)
@@ -235,32 +235,32 @@
 mostly for numeric checks, but as use cases emerge, more will be
 added.
 
 To add data validation, use the `validator=` keyword inside
 columns. For example:
 
 ```python
-from quivr import Table, Int64Column, Float64Column, StringColumn
+import quivr as qv
 from quivr.validators import gt, ge, le, and_, is_in
 
-class Observation(Table):
-    id = Int64Column(validator=gt(0))
-    ra = Float64Column(validator=and_(ge(0), le(360))
-    dataset_id = StringColumn(validator=is_in(["ztf", "nsc", "skymapper"])))
-    unvalidated = Int64Column()
+class Observation(qv.Table):
+    id = qv.Int64Column(validator=gt(0))
+    ra = qv.Float64Column(validator=and_(ge(0), le(360))
+    dataset_id = qv.StringColumn(validator=is_in(["ztf", "nsc", "skymapper"])))
+    unvalidated = qv.Int64Column()
 ```
 
 This `Observation` table has validators that
 - the `id` column's values are greater than 0
 - the `ra` column's values are between 0 and 360, inclusive
 - the `dataset_id` column only has strings in the set `{"ztf", "nsc", "skymapper"}`
 
-When an `Observation` instance is created using the `from_data`
+When an `Observation` instance is created using the `from_kwargs`
 method, these validation checks will be run, by default. This can be
-disabled by calling `Observation.from_data(..., validate=False)`.
+disabled by calling `Observation.from_kwargs(..., validate=False)`.
 
 In addition, an instance can be explicitly validated by calling the
 `.validate()` method, which will raise a `quivr.ValidationError` if
 there are any failures.
 
 Also, tables have a `.is_valid()` method which returns a boolean to
 indicate whether they pass validation.
@@ -281,34 +281,14 @@
 "select" method on the Table:
 
 ```python
 # Get the orbit of Ceres
 ceres_orbit = orbits.select("designation", "Ceres")
 ```
 
-#### Indexes for Fast Lookups
-
-If you're going to be doing a lot of lookups on a particular column,
-it can be useful to create an index for that column. You can do using
-the `quivr.StringIndex` class to build an index for string values:
-
-```python
-# Build an index for the designation column
-designation_index = quivr.StringIndex(orbits, "designation")
-
-# Get the orbit of Ceres
-ceres_orbit = designation_index.lookup("Ceres")
-```
-
-The `lookup` method on the StringIndex returns Quivr Tables, or None
-if there is no match. Keep in mind that the returned tables might have
-multiple rows if there are multiple matches.
-
-_TODO: Add numeric and time-based indexes._
-
 ### Serialization
 
 #### Feather
 Feather is a fast, zero-copy serialization format for Arrow tables. It
 can be used for interprocess communication, or for working with data
 on disk via memory mapping.
```

### Comparing `quivr-0.6.0rc2/pyproject.toml` & `quivr-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.6.0rc2/PKG-INFO` & `quivr-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quivr
-Version: 0.6.0rc2
+Version: 0.6.1
 Summary: Container library for working with tabular Arrow data
 Project-URL: Source, https://github.com/spenczar/quivr
 Author-email: Spencer Nelson <spencer@spencerwnelson.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: mmh3
 Requires-Dist: numpy
@@ -66,32 +66,32 @@
 
 Your main entrypoint to Quivr is through defining classes which
 represent your tables. You write a subclass of quivr.Table, annotating
 it with Columns that describe the data you're working with, and quivr
 will handle the rest.
 
 ```python
-from quivr import Table, Float64Column
+import quivr as qv
 import pyarrow as pa
 
 
-class Coordinates(Table):
-	x = Float64Column()
-	y = Float64Column()
-	z = Float64Column()
-	vx = Float64Column()
-	vy = Float64Column()
-	vz = Float64Column()
+class Coordinates(qv.Table):
+	x = qv.Float64Column()
+	y = qv.Float64Column()
+	z = qv.Float64Column()
+	vx = qv.Float64Column()
+	vy = qv.Float64Column()
+	vz = qv.Float64Column()
 ```
 
 Then, you can construct tables from data:
 
 ```python
 
-coords = Coordinates.from_data(
+coords = Coordinates.from_kwargs(
     x=np.array([ 1.00760887, -2.06203093,  1.24360546, -1.00131722]),
     y=np.array([-2.7227298 ,  0.70239707,  2.23125432,  0.37269832]),
     z=np.array([-0.27148738, -0.31768623, -0.2180482 , -0.02528401]),
     vx=np.array([ 0.00920172, -0.00570486, -0.00877929, -0.00809866]),
     vy=np.array([ 0.00297888, -0.00914301,  0.00525891, -0.01119134]),
     vz=np.array([-0.00160217,  0.00677584,  0.00091095, -0.00140548])
 )
@@ -111,23 +111,23 @@
 
 ### Embedded definitions and nullable columns
 
 You can embed one table's definition within another, and you can make columns nullable:
 
 ```python
 
-class AsteroidOrbit(Table):
-	designation = StringColumn()
-	mass = Float64Column(nullable=True)
-	radius = Float64Column(nullable=True)
+class AsteroidOrbit(qv.Table):
+	designation = qv.StringColumn()
+	mass = qv.Float64Column(nullable=True)
+	radius = qv.Float64Column(nullable=True)
 	coords = Coordinates.as_column()
 
 # You can construct embedded columns from Arrow StructArrays, which you can get from
 # other Quivr tables using the to_structarray() method with zero copy.
-orbits = AsteroidOrbit.from_data(
+orbits = AsteroidOrbit.from_kwargs(
     designation=np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
     mass=np.array([9.393e20, 2.06e21, 2.59e20, None]),
     radius=np.array([4.6e6, 2.7e6, 2.6e6, None]),
     coords=coords.to_structarray(),
 )
 ```
 
@@ -167,41 +167,41 @@
 Because Quivr tables are just Python classes, you can customize the
 behavior of your tables by adding or overriding methods. For example, if you want to add a
 method to compute the total mass of the asteroids in the table, you
 can do so like this:
 
 ```python
 
-class AsteroidOrbit(Table):
-	designation = StringColumn()
-	mass = Float64Column(nullable=True)
-	radius = Float64Column(nullable=True)
+class AsteroidOrbit(qv.Table):
+	designation = qv.StringColumn()
+	mass = qv.Float64Column(nullable=True)
+	radius = qv.Float64Column(nullable=True)
 	coords = Coordinates.as_column()
 
     def total_mass(self):
         return pc.sum(self.mass)
 
 ```
 
 You can also use this to add "meta-columns" which are combinations of other columns. For example:
 
 ```python
-class CoordinateCovariance(Table):
-	matrix_values = ListColumn(pa.float64(), 36)
+class CoordinateCovariance(qv.Table):
+	matrix_values = qv.ListColumn(pa.float64(), 36)
 
     @property
     def matrix(self):
         # This is a numpy array of shape (n, 6, 6)
         return self.matrix_values.to_numpy().reshape(-1, 6, 6)
 
 
-class AsteroidOrbit(Table):
-	designation = StringColumn()
-	mass = Float64Column(nullable=True)
-	radius = Float64Column(nullable=True)
+class AsteroidOrbit(qv.Table):
+	designation = qv.StringColumn()
+	mass = qv.Float64Column(nullable=True)
+	radius = qv.Float64Column(nullable=True)
 	coords = Coordinates.as_column()
 	covariance = CoordinateCovariance.as_column()
 
 orbits = load_orbits() # Analogous to the example above
 
 # Compute the determinant of the covariance matrix for each asteroid
 determinants = np.linalg.det(orbits.covariance.matrix)
@@ -216,24 +216,24 @@
 if you do this, there are a few rules:
 
  1. Your `__init__` method must have an attribute called `table`, with
     type `pyarrow.Table`, and you must pass this to Table's `__init__`
     (via `super().__init__(table)`).
  2. You must implement a `with_table(self, table: pa.Table) -> Self`
     method which returns a **new** instance with the provided table,
-    bringing along the current values of all instance attributes.
+    bringingalong the current values of all instance attributes.
 
 For example:
 
 ```python
 from typing import Self
 
-class AsteroidOrbit(Table):
-    designation = StringColumn()
-	mass = Float64Column(nullable=True)
+class AsteroidOrbit(qv.Table):
+    designation = qv.StringColumn()
+	mass = qv.Float64Column(nullable=True)
 	
 	def __init__(self, table: pa.Table, mu: float):
 	    super().__init__(table)
 		self.mu = mu
 		
 	def with_table(self, table: pa.Table) -> Self:
         return AsteroidOrbit(table, self.mu)
@@ -256,32 +256,32 @@
 mostly for numeric checks, but as use cases emerge, more will be
 added.
 
 To add data validation, use the `validator=` keyword inside
 columns. For example:
 
 ```python
-from quivr import Table, Int64Column, Float64Column, StringColumn
+import quivr as qv
 from quivr.validators import gt, ge, le, and_, is_in
 
-class Observation(Table):
-    id = Int64Column(validator=gt(0))
-    ra = Float64Column(validator=and_(ge(0), le(360))
-    dataset_id = StringColumn(validator=is_in(["ztf", "nsc", "skymapper"])))
-    unvalidated = Int64Column()
+class Observation(qv.Table):
+    id = qv.Int64Column(validator=gt(0))
+    ra = qv.Float64Column(validator=and_(ge(0), le(360))
+    dataset_id = qv.StringColumn(validator=is_in(["ztf", "nsc", "skymapper"])))
+    unvalidated = qv.Int64Column()
 ```
 
 This `Observation` table has validators that
 - the `id` column's values are greater than 0
 - the `ra` column's values are between 0 and 360, inclusive
 - the `dataset_id` column only has strings in the set `{"ztf", "nsc", "skymapper"}`
 
-When an `Observation` instance is created using the `from_data`
+When an `Observation` instance is created using the `from_kwargs`
 method, these validation checks will be run, by default. This can be
-disabled by calling `Observation.from_data(..., validate=False)`.
+disabled by calling `Observation.from_kwargs(..., validate=False)`.
 
 In addition, an instance can be explicitly validated by calling the
 `.validate()` method, which will raise a `quivr.ValidationError` if
 there are any failures.
 
 Also, tables have a `.is_valid()` method which returns a boolean to
 indicate whether they pass validation.
@@ -302,34 +302,14 @@
 "select" method on the Table:
 
 ```python
 # Get the orbit of Ceres
 ceres_orbit = orbits.select("designation", "Ceres")
 ```
 
-#### Indexes for Fast Lookups
-
-If you're going to be doing a lot of lookups on a particular column,
-it can be useful to create an index for that column. You can do using
-the `quivr.StringIndex` class to build an index for string values:
-
-```python
-# Build an index for the designation column
-designation_index = quivr.StringIndex(orbits, "designation")
-
-# Get the orbit of Ceres
-ceres_orbit = designation_index.lookup("Ceres")
-```
-
-The `lookup` method on the StringIndex returns Quivr Tables, or None
-if there is no match. Keep in mind that the returned tables might have
-multiple rows if there are multiple matches.
-
-_TODO: Add numeric and time-based indexes._
-
 ### Serialization
 
 #### Feather
 Feather is a fast, zero-copy serialization format for Arrow tables. It
 can be used for interprocess communication, or for working with data
 on disk via memory mapping.
```

