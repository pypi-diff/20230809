# Comparing `tmp/fileformats-0.8.5.tar.gz` & `tmp/fileformats-0.8.6.tar.gz`

## Comparing `fileformats-0.8.5.tar` & `fileformats-0.8.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/archive/__init__.py
--rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/_version.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/converter.py
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/datatype.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/field.py
--rw-r--r--   0        0        0    46547 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/fileset.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/mark.py
--rw-r--r--   0        0        0    27183 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/mixin.py
--rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/utils.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_test_extras.py
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/document/__init__.py
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/base.py
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/notclassifiedyet.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/vector.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/misc/medical.py
--rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/misc/unclassified.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/model/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/testing/classifiers.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/testing/headers.py
--rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/text/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.5/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.5/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.5/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.5/LICENSE
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.5/README.rst
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.5/pyproject.toml
--rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/converter.py
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/datatype.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/field.py
+-rw-r--r--   0        0        0    46550 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/mark.py
+-rw-r--r--   0        0        0    27183 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/mixin.py
+-rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/utils.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_test_extras.py
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/image/base.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/image/notclassifiedyet.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/image/vector.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/misc/medical.py
+-rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/misc/unclassified.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/model/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/testing/headers.py
+-rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/text/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.6/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.6/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.6/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.6/LICENSE
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.6/README.rst
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.6/PKG-INFO
```

### Comparing `fileformats-0.8.5/fileformats/archive/__init__.py` & `fileformats-0.8.6/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/audio/__init__.py` & `fileformats-0.8.6/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/converter.py` & `fileformats-0.8.6/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/datatype.py` & `fileformats-0.8.6/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/exceptions.py` & `fileformats-0.8.6/fileformats/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/field.py` & `fileformats-0.8.6/fileformats/core/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     @property
     def metadata(self):
         """Empty metadata dict for duck-typing with file-sets"""
         return {}
 
     @classproperty
-    def all_fields(cls) -> list[ty.Type[Field]]:  # pylint: disable=no-self-argument
+    def all_fields(cls) -> ty.List[ty.Type[Field]]:  # pylint: disable=no-self-argument
         """Iterate over all field formats in fileformats.* namespaces"""
         import fileformats.field  # noqa
 
         return [f for f in Field.subclasses() if f.primitive is not None]
 
     @classmethod
     def from_primitive(cls, dtype: type):
```

### Comparing `fileformats-0.8.5/fileformats/core/fileset.py` & `fileformats-0.8.6/fileformats/core/fileset.py`

 * *Files 1% similar despite different names*

```diff
@@ -722,15 +722,15 @@
         crytpo_obj = crypto()
         for path, bytes_iter in self.byte_chunks(**kwargs):
             crytpo_obj.update(path.encode())
             for bytes_str in bytes_iter:
                 crytpo_obj.update(bytes_str)
         return crytpo_obj.hexdigest()
 
-    def hash_files(self, crypto=None, **kwargs) -> dict[str, bytes]:
+    def hash_files(self, crypto=None, **kwargs) -> ty.Dict[str, bytes]:
         """Calculate hashes for all files in the file-set based on the relative paths and
         contents of its constituent files
 
         Parameters
         ----------
         crypto : function, optional
             the cryptography method used to hash the files, by default hashlib.sha256
```

### Comparing `fileformats-0.8.5/fileformats/core/mark.py` & `fileformats-0.8.6/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/mixin.py` & `fileformats-0.8.6/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/utils.py` & `fileformats-0.8.6/fileformats/core/utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_classifiers.py` & `fileformats-0.8.6/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_converter.py` & `fileformats-0.8.6/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_detection.py` & `fileformats-0.8.6/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_general.py` & `fileformats-0.8.6/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_mime.py` & `fileformats-0.8.6/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_mixin.py` & `fileformats-0.8.6/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_subpackages.py` & `fileformats-0.8.6/fileformats/core/tests/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_test_extras.py` & `fileformats-0.8.6/fileformats/core/tests/test_test_extras.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/core/tests/test_utils.py` & `fileformats-0.8.6/fileformats/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/document/__init__.py` & `fileformats-0.8.6/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/field/__init__.py` & `fileformats-0.8.6/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/field/tests/test_fields.py` & `fileformats-0.8.6/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.8.6/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/generic/__init__.py` & `fileformats-0.8.6/fileformats/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/image/__init__.py` & `fileformats-0.8.6/fileformats/image/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/image/notclassifiedyet.py` & `fileformats-0.8.6/fileformats/image/notclassifiedyet.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/image/raster.py` & `fileformats-0.8.6/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/image/tests/test_image_raster.py` & `fileformats-0.8.6/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/misc/__init__.py` & `fileformats-0.8.6/fileformats/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/misc/unclassified.py` & `fileformats-0.8.6/fileformats/misc/unclassified.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/model/__init__.py` & `fileformats-0.8.6/fileformats/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/serialization/__init__.py` & `fileformats-0.8.6/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/testing/classifiers.py` & `fileformats-0.8.6/fileformats/testing/classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/testing/headers.py` & `fileformats-0.8.6/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/text/__init__.py` & `fileformats-0.8.6/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/fileformats/video/__init__.py` & `fileformats-0.8.6/fileformats/video/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/LICENSE` & `fileformats-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/README.rst` & `fileformats-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/pyproject.toml` & `fileformats-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.5/PKG-INFO` & `fileformats-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.8.5
+Version: 0.8.6
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

