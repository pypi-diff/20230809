# Comparing `tmp/salinic-0.2.4.tar.gz` & `tmp/salinic-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salinic-0.2.4.tar", max compression
+gzip compressed data, was "salinic-0.2.5.tar", max compression
```

## Comparing `salinic-0.2.4.tar` & `salinic-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    10226 2023-08-04 05:46:24.918937 salinic-0.2.4/LICENSE
--rw-r--r--   0        0        0     1695 2023-08-04 05:46:24.918937 salinic-0.2.4/README.md
--rw-r--r--   0        0        0      470 2023-08-04 05:46:24.922937 salinic-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      321 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/__init__.py
--rw-r--r--   0        0        0      344 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/engine.py
--rw-r--r--   0        0        0      285 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/field.py
--rw-r--r--   0        0        0     1250 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/schema.py
--rw-r--r--   0        0        0      228 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/search.py
--rw-r--r--   0        0        0      118 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/search_query.py
--rw-r--r--   0        0        0     3840 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/session.py
--rw-r--r--   0        0        0      601 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/types.py
--rw-r--r--   0        0        0      564 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/utils.py
--rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 salinic-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    10226 2023-08-09 05:04:44.362119 salinic-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1695 2023-08-09 05:04:44.362119 salinic-0.2.5/README.md
+-rw-r--r--   0        0        0      470 2023-08-09 05:04:44.362119 salinic-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/__init__.py
+-rw-r--r--   0        0        0      344 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/engine.py
+-rw-r--r--   0        0        0      285 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/field.py
+-rw-r--r--   0        0        0     4323 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/query.py
+-rw-r--r--   0        0        0     1250 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/schema.py
+-rw-r--r--   0        0        0      221 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/search.py
+-rw-r--r--   0        0        0     4989 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/session.py
+-rw-r--r--   0        0        0      601 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/types.py
+-rw-r--r--   0        0        0      564 2023-08-09 05:04:44.362119 salinic-0.2.5/salinic/utils.py
+-rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 salinic-0.2.5/PKG-INFO
```

### Comparing `salinic-0.2.4/LICENSE` & `salinic-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `salinic-0.2.4/README.md` & `salinic-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `salinic-0.2.4/salinic/schema.py` & `salinic-0.2.5/salinic/schema.py`

 * *Files identical despite different names*

### Comparing `salinic-0.2.4/salinic/session.py` & `salinic-0.2.5/salinic/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import xapian
 from pydantic import BaseModel
 
 from .field import Field, IdField, KeywordField, TextField
-from .search import SearchQuery
+from .query import SearchQuery
 from .utils import first
 
 
 def index_text_field(
     term_generator: xapian.TermGenerator,
     insert_value: str,
     prefix: str,
@@ -42,17 +42,30 @@
 
 def index_keyword_field(
     term_generator: xapian.TermGenerator,
     insert_value: str,
     prefix: str
 ):
     doc = term_generator.get_document()
-    doc.add_boolean_term(
-        prefix + insert_value.lower()
-    )
+    if isinstance(insert_value, str):
+        doc.add_boolean_term(
+            prefix + insert_value
+        )
+        doc.add_boolean_term(
+            prefix + insert_value.lower()
+        )
+
+    if isinstance(insert_value, list):
+        for value in insert_value:
+            doc.add_boolean_term(
+                prefix + value
+            )
+            doc.add_boolean_term(
+                prefix + value.lower()
+            )
 
 
 class Session:
     def __init__(self, engine, language="en"):
         self._engine = engine
         self._termgenerator = xapian.TermGenerator()
         self._termgenerator.set_stemmer(xapian.Stem(language))
@@ -111,19 +124,41 @@
     def remove(self, entity: BaseModel):
         idterm = f"Q{entity.pk}"
         self._engine._db.delete_document(idterm)
         self._engine._db.commit()
 
     def exec(self, sq: SearchQuery):
         results = []
-        for name, field in sq._entity.model_fields.items():
-            self._queryparser.add_prefix(name, name)
 
-        query = self._queryparser.parse_query(sq._query)
+        if str(sq.query.free_text):
+            query = self._queryparser.parse_query(
+                str(sq.query.free_text)
+            )
+        else:
+            query = xapian.Query('')
+
+        for name, field in sq.entity.model_fields.items():
+            self._queryparser.add_prefix(name.upper(), name.upper())
+            filter_queries = sq.query.get_filters_by(name)
+            for qf in filter_queries:
+                xapian_fqueries = [
+                    xapian.Query(qf.name.upper() + filter_value.lower())
+                    for filter_value in qf.values
+                ]
+                # apply AND operator (OR operator) on filter queries
+                xa_fq = xapian.Query(xapian.Query.OP_AND, xapian_fqueries)
+                # combine free text query with filter queries
+                query = xapian.Query(
+                    xapian.Query.OP_FILTER,
+                    query,
+                    xa_fq
+                )
+
         enquire = xapian.Enquire(self._engine._db)
+
         enquire.set_query(query)
 
         for match in enquire.get_mset(0, 10):
             fields = json.loads(match.document.get_data().decode('utf8'))
-            results.append(sq._entity(**fields))
+            results.append(sq.entity(**fields))
 
         return results
```

### Comparing `salinic-0.2.4/salinic/types.py` & `salinic-0.2.5/salinic/types.py`

 * *Files identical despite different names*

### Comparing `salinic-0.2.4/salinic/utils.py` & `salinic-0.2.5/salinic/utils.py`

 * *Files identical despite different names*

### Comparing `salinic-0.2.4/PKG-INFO` & `salinic-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salinic
-Version: 0.2.4
+Version: 0.2.5
 Summary: Search abstraction layer
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

