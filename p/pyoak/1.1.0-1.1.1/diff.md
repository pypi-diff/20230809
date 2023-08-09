# Comparing `tmp/pyoak-1.1.0.tar.gz` & `tmp/pyoak-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoak-1.1.0.tar", max compression
+gzip compressed data, was "pyoak-1.1.1.tar", max compression
```

## Comparing `pyoak-1.1.0.tar` & `pyoak-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1068 2023-08-08 21:27:53.621445 pyoak-1.1.0/LICENSE
--rw-r--r--   0        0        0    20693 2023-08-08 21:27:53.621445 pyoak-1.1.0/README.md
--rw-r--r--   0        0        0     2690 2023-08-08 21:27:53.625445 pyoak-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      122 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/__init__.py
--rw-r--r--   0        0        0     5606 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/error.py
--rw-r--r--   0        0        0     1189 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/file.py
--rw-r--r--   0        0        0     6409 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/helpers.py
--rw-r--r--   0        0        0        0 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/__init__.py
--rw-r--r--   0        0        0      726 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/error.py
--rw-r--r--   0        0        0     1110 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/grammar.py
--rw-r--r--   0        0        0     1612 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/helpers.py
--rw-r--r--   0        0        0    37790 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/pattern.py
--rw-r--r--   0        0        0     6036 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/match/xpath.py
--rw-r--r--   0        0        0    70095 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/node.py
--rw-r--r--   0        0        0    22983 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/origin.py
--rw-r--r--   0        0        0        0 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/py.typed
--rw-r--r--   0        0        0    13537 2023-08-08 21:27:53.625445 pyoak-1.1.0/src/pyoak/serialize.py
--rw-r--r--   0        0        0    21611 1970-01-01 00:00:00.000000 pyoak-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-09 00:27:06.456030 pyoak-1.1.1/LICENSE
+-rw-r--r--   0        0        0    20693 2023-08-09 00:27:06.456030 pyoak-1.1.1/README.md
+-rw-r--r--   0        0        0     2690 2023-08-09 00:27:06.460030 pyoak-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/__init__.py
+-rw-r--r--   0        0        0     5606 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/error.py
+-rw-r--r--   0        0        0     1189 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/file.py
+-rw-r--r--   0        0        0     6409 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/match/__init__.py
+-rw-r--r--   0        0        0      726 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/match/error.py
+-rw-r--r--   0        0        0     1110 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/match/grammar.py
+-rw-r--r--   0        0        0     1612 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/match/helpers.py
+-rw-r--r--   0        0        0    37790 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/match/pattern.py
+-rw-r--r--   0        0        0     6036 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/match/xpath.py
+-rw-r--r--   0        0        0    70095 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/node.py
+-rw-r--r--   0        0        0    23164 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/origin.py
+-rw-r--r--   0        0        0        0 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/py.typed
+-rw-r--r--   0        0        0    13537 2023-08-09 00:27:06.460030 pyoak-1.1.1/src/pyoak/serialize.py
+-rw-r--r--   0        0        0    21611 1970-01-01 00:00:00.000000 pyoak-1.1.1/PKG-INFO
```

### Comparing `pyoak-1.1.0/LICENSE` & `pyoak-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/README.md` & `pyoak-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/pyproject.toml` & `pyoak-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyoak"
-version = "1.1.0"
+version = "1.1.1"
 homepage = "https://github.com/mishamsk/pyoak"
 description = "Library for building and working with arbitrary ASTs on top dataclasses"
 authors = ["Mike Perlov <mishamsk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
```

### Comparing `pyoak-1.1.0/src/pyoak/error.py` & `pyoak-1.1.1/src/pyoak/error.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/file.py` & `pyoak-1.1.1/src/pyoak/file.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/helpers.py` & `pyoak-1.1.1/src/pyoak/helpers.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/match/error.py` & `pyoak-1.1.1/src/pyoak/match/error.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/match/grammar.py` & `pyoak-1.1.1/src/pyoak/match/grammar.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/match/helpers.py` & `pyoak-1.1.1/src/pyoak/match/helpers.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/match/pattern.py` & `pyoak-1.1.1/src/pyoak/match/pattern.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/match/xpath.py` & `pyoak-1.1.1/src/pyoak/match/xpath.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/node.py` & `pyoak-1.1.1/src/pyoak/node.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/src/pyoak/origin.py` & `pyoak-1.1.1/src/pyoak/origin.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing as t
 import zipfile
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from pathlib import Path
 
 from .file import read_text_unknown_encoding
-from .serialize import DataClassSerializeMixin
+from .serialize import TYPE_KEY, DataClassSerializeMixin
 
 if t.TYPE_CHECKING:
     from mashumaro.dialect import Dialect
 
 logger = logging.getLogger(__name__)
 
 URI_DELIM = "::"
@@ -87,15 +87,15 @@
     def _serialize(self) -> dict[str, t.Any]:
         if self._get_serialization_options().get(SOURCE_OPTIMIZED_SERIALIZATION_KEY, False):
             return {"idx": Source._sources[self]}
         return super()._serialize()
 
     @classmethod
     def _deserialize(cls, data: dict[str, t.Any]) -> Source:
-        if data == {}:
+        if data == {} or (TYPE_KEY in data and data[TYPE_KEY] == "NoSource"):
             return NoSource()
 
         # Try to deserialize as optimized serialization
         idx = data.get("idx")
 
         if idx is None:
             # This may return not the object in the registry, but a new instance
@@ -181,15 +181,15 @@
 
 
 class Position(DataClassSerializeMixin, FQN):
     """Base class for all position types."""
 
     @classmethod
     def _deserialize(cls, value: dict[str, t.Any]) -> Position:
-        if value == {}:
+        if value == {} or (TYPE_KEY in value and value[TYPE_KEY] == "NoPosition"):
             return NO_POSITION
 
         return super()._deserialize(value)
 
 
 @dataclass(frozen=True)
 class Origin(DataClassSerializeMixin, FQN):
@@ -203,15 +203,15 @@
             raise TypeError(f"Expected Source, got {type(self.source)}")
 
         if not isinstance(self.position, Position):
             raise TypeError(f"Expected Position, got {type(self.position)}")
 
     @classmethod
     def _deserialize(cls, value: dict[str, t.Any]) -> Origin:
-        if value == {}:
+        if value == {} or (TYPE_KEY in value and value[TYPE_KEY] == "NoOrigin"):
             return NO_ORIGIN
 
         return super()._deserialize(value)
 
     def __str__(self) -> str:
         return f"{self.source.source_type}@{self.fqn}"
```

### Comparing `pyoak-1.1.0/src/pyoak/serialize.py` & `pyoak-1.1.1/src/pyoak/serialize.py`

 * *Files identical despite different names*

### Comparing `pyoak-1.1.0/PKG-INFO` & `pyoak-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoak
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library for building and working with arbitrary ASTs on top dataclasses
 Home-page: https://github.com/mishamsk/pyoak
 License: MIT
 Author: Mike Perlov
 Author-email: mishamsk@gmail.com
 Requires-Python: >=3.10
 Classifier: Development Status :: 5 - Production/Stable
```

