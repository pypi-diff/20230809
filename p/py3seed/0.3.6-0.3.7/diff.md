# Comparing `tmp/py3seed-0.3.6.tar.gz` & `tmp/py3seed-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.3.6.tar", last modified: Tue Aug  8 12:57:59 2023, max compression
+gzip compressed data, was "py3seed-0.3.7.tar", last modified: Wed Aug  9 03:46:03 2023, max compression
```

## Comparing `py3seed-0.3.6.tar` & `py3seed-0.3.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.417404 py3seed-0.3.6/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.6/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-08 12:57:59.417533 py3seed-0.3.6/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.6/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.6/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-08 12:57:59.418160 py3seed-0.3.6/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.6/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.391421 py3seed-0.3.6/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.406749 py3seed-0.3.6/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.6/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.6/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.6/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     8042 2023-08-08 12:56:48.000000 py3seed-0.3.6/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.412673 py3seed-0.3.6/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.6/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    22814 2023-08-05 06:24:39.000000 py3seed-0.3.6/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.6/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.6/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.6/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.6/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.3.6/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.6/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    15080 2023-08-05 08:05:06.000000 py3seed-0.3.6/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.6/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.411718 py3seed-0.3.6/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-08 12:57:59.000000 py3seed-0.3.6/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-08 12:57:59.416819 py3seed-0.3.6/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4144 2023-08-08 12:56:48.000000 py3seed-0.3.6/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-08-05 08:10:59.000000 py3seed-0.3.6/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.6/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.3.6/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.6/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-09 03:46:03.622624 py3seed-0.3.7/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.3.7/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-09 03:46:03.622784 py3seed-0.3.7/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.3.7/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.3.7/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-08-09 03:46:03.623620 py3seed-0.3.7/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.3.7/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-09 03:46:03.598360 py3seed-0.3.7/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-09 03:46:03.612089 py3seed-0.3.7/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.3.7/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.3.7/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.3.7/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     8042 2023-08-08 12:56:48.000000 py3seed-0.3.7/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-09 03:46:03.615955 py3seed-0.3.7/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.3.7/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    22834 2023-08-09 02:28:20.000000 py3seed-0.3.7/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.3.7/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.3.7/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.3.7/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.3.7/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57275 2023-08-08 14:15:51.000000 py3seed-0.3.7/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.3.7/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    15792 2023-08-09 03:36:41.000000 py3seed-0.3.7/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.3.7/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-09 03:46:03.614906 py3seed-0.3.7/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-08-09 03:46:03.000000 py3seed-0.3.7/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-08-09 03:46:03.000000 py3seed-0.3.7/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-08-09 03:46:03.000000 py3seed-0.3.7/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-08-09 03:46:03.000000 py3seed-0.3.7/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-08-09 03:46:03.000000 py3seed-0.3.7/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-08-09 03:46:03.000000 py3seed-0.3.7/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-08-09 03:46:03.621789 py3seed-0.3.7/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4144 2023-08-08 12:56:48.000000 py3seed-0.3.7/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7133 2023-08-09 03:45:42.000000 py3seed-0.3.7/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.3.7/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5165 2023-08-09 02:24:09.000000 py3seed-0.3.7/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.3.7/tests/test_mongosupport.py
```

### Comparing `py3seed-0.3.6/LICENSE` & `py3seed-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/PKG-INFO` & `py3seed-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.3.6
+Version: 0.3.7
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.3.6/setup.cfg` & `py3seed-0.3.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.3.6
+version = 0.3.7
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.3.6/src/py3seed/__init__.py` & `py3seed-0.3.7/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/__main__.py` & `py3seed-0.3.7/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/admin.py` & `py3seed-0.3.7/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/cachesupport.py` & `py3seed-0.3.7/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/commands/gen.py` & `py3seed-0.3.7/src/py3seed/commands/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,18 +120,18 @@
         #
         for v in values:
             if matcher.match(v):
                 return v
         # If no matching, return nothing
         return None
 
-    def fields(layout_or_schema, matcher=None):
+    def fields(layout_or_schema, matcher=None, **kwargs):
         """ Get the matched fields from layout or schema. """
         if isinstance(layout_or_schema, list):  # layout is [[{}, ...], ...]
-            _fields = list(get_layout_fields(layout_or_schema))
+            _fields = list(get_layout_fields(layout_or_schema, **kwargs))
         elif isinstance(layout_or_schema, dict):  # schema is dict {type: 'object', properties: {name, type, ... }}
             _fields = list(layout_or_schema['properties'].keys())
         else:
             raise ValueError(f'Unsupported type to calculate fields: {type(layout_or_schema)}')
         #
         if matcher:
             # NOTE: in jinja2, you need to escape regex str, e.g, \w -> \\w
```

### Comparing `py3seed-0.3.6/src/py3seed/error.py` & `py3seed-0.3.7/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/inflection.py` & `py3seed-0.3.7/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/log.py` & `py3seed-0.3.7/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/merge3.py` & `py3seed-0.3.7/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/model.py` & `py3seed-0.3.7/src/py3seed/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,14 +692,16 @@
     # The id field name
     __id_name__ = None
     __id_type__ = None
     #
     __icon__ = None
     __title__ = None
     __description__ = None
+    # When doing some logic that list models, e.g, drawing a table of users, we can use these columns to draw by default.
+    __columns__ = []
     # Views for this model, should be a dict
     # i.e,
     # {
     #   view_name: {                    # View name should be unique, in blueprint/view format, if blueprint is not specified, use default public by default
     #     domains: ['www'],             # Domains that this view can be generated, should always be application's name
     #     layout: '''action?param=1     # Layout of this view, we use this layout to generate corresponding view and template source code
     #       field_string, field_select
@@ -1133,15 +1135,15 @@
 
     @classmethod
     def find(cls, *args, **kwargs):
         """ abstract method, use it to fetch many related models. """
         return []
 
     @classmethod
-    def schema(cls, layouts={}):
+    def schema(cls):
         """ To json schema dict.
 
         NOTE:
         Return json schema is a subset of Object Schema from OAS 3.0.
         In order to keep all the things simple, we do not use complex keywords such as oneOf, $ref, patternProperties, additionalProperties, etc.
         https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#schemaObject
         https://swagger.io/docs/specification/data-models/
@@ -1273,14 +1275,15 @@
                         relations[f_type.__name__] += [f_n]
                     #
                     properties[f_n] = field_schema
                 #
                 obj = {
                     'type': 'object',
                     'properties': properties,
+                    'columns': type_.__columns__,
                     'requires': requires,
                     'editable': True,
                     'py_type': type_.__name__,
                     'icon': type_.__icon__ if type_.__icon__ else None,
                     'title': type_.__title__ if type_.__title__ else type_.__name__.upper(),
                     'description': type_.__description__ if type_.__description__ else None,
                     # searchables, [field__comparator|field]
@@ -1289,26 +1292,14 @@
                     # sortables, [(field_name, 1/-1)]
                     'sortables': sortables,
                     'relations': [k for k in relations.keys() if k != type_.__name__],  # skip self
                     # id_name & id_type, used for relation inputs
                     'id_name': type_.__id_name__,
                     'id_type': type_.__id_type__.__name__ if type_.__id_type__ else None,
                 }
-                # Inject layouts into schema
-                if layouts:
-                    layout = layouts.get(type_.__name__, {})
-                    if not layout.get('columns'):
-                        layout['columns'] = obj['requires']
-                    if not layout.get('read'):
-                        # Each field is a row
-                        layout['read'] = [[{'name': f, 'params': {}}] for f in obj['properties'].keys()]
-                    if not layout.get('form'):
-                        layout['form'] = layout['read']
-                    #
-                    obj.update(layout)
                 #
                 return obj
             elif type_ is str:
                 return {'type': 'string', 'format': Format.TEXT, 'py_type': 'str'}
             elif type_ is int:
                 return {'type': 'integer', 'format': Format.INT, 'py_type': 'int'}
             elif type_ is float:
```

### Comparing `py3seed-0.3.6/src/py3seed/mongosupport.py` & `py3seed-0.3.7/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed/utils.py` & `py3seed-0.3.7/src/py3seed/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,23 +233,30 @@
                     # Some formats are used for display only, i.e, summary, so we do not need to validate the fields under a summary group
                     if col_name not in _schema['properties']:  # type of _schema is always a object
                         raise LayoutError(f'Field {col_name} not found in schema')
                     #
                     column_schema = _schema['properties'][col_name]
                     column_type = column_schema['type']
                     inner_schema = None
+                    # If inner layout does not exist, we should create a default one
                     if column_type == 'object':
                         inner_schema = column_schema
+                        # default layout for object is each row with one column
+                        if not col_lines:
+                            col_lines = [inner_schema['columns'] if inner_schema['columns'] else inner_schema['properties'].keys()]
+                            logger.debug(f'{leading}Set default layout')
                     elif column_type == 'array':
                         inner_schema = column_schema['items'] if column_schema['items']['type'] == 'object' else None
+                        # default layout for object array is one row with columns
+                        if inner_schema and not col_lines:
+                            col_lines = [', '.join(inner_schema['columns'] if inner_schema['columns'] else inner_schema['properties'].keys())]
+                            logger.debug(f'{leading}Set default layout')
                     #
                     if inner_schema:
-                        # Inner layout is optional for inner object
-                        if col_lines:
-                            column['rows'] = _parse_lines(level + 1, col_lines, inner_schema, _action)  # Schema passing recursively should always be an object
+                        column['rows'] = _parse_lines(level + 1, col_lines, inner_schema, _action)  # Schema passing recursively should always be an object
                     else:
                         if col_lines:
                             raise LayoutError(f'{column_type.capitalize()} field {col_name} can not have inner layout')
                     #
                     column.pop('lines', None)
             #
             _rows.append(columns)
@@ -332,27 +339,27 @@
     return {
         'action': action,
         'params': params,
         'rows': rows
     }
 
 
-def get_layout_fields(layout):
+def get_layout_fields(layout, exclude_formats=(Format.SUMMARY,)):
     """ Do not recursively parse inner object/array, only return current level field names. """
     if not layout:
         return []
     #
     for row in layout:
         for col in row:
             col_name = col['name']
             # NOTE: Ignore the groups with summary format, because they are used for reference only
             # e.g,
             # - 1#summary4 is used to display a summary card of current object
-            # - project#summary4 is used to display a summary card of a related object or inner object
-            if col['format'] == Format.SUMMARY:
+            # - project#summaget_layout_fieldsry4 is used to display a summary card of a related object or inner object
+            if col['format'] in exclude_formats:
                 continue
             # Blank column
             if not col_name:
                 pass
             # Hyphen column
             elif col_name == '-':
                 pass
```

### Comparing `py3seed-0.3.6/src/py3seed/websupport.py` & `py3seed-0.3.7/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.3.7/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.3.6
+Version: 0.3.7
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.3.6/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.3.7/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/tests/test_cachesupport.py` & `py3seed-0.3.7/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/tests/test_gen.py` & `py3seed-0.3.7/tests/test_gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,35 +16,36 @@
 from py3seed.utils import parse_layout, get_layout_fields
 from py3seed.commands.gen import _gen
 from .core.models import User, Team
 
 
 def test_layout_parsing():
     """ Test layout parsing. """
-    # User profile
+    # Testing layouts
+    # NOTE: Below layouts just for layout parse tests, not for gen test cases
     user_profile_layout = '''#!form?title=User
         1#summary4,    2#8                                           
           avatar         name  
           name           phone                                                  
           status         intro                                                 
           roles          avatar                                                
           email          point#4,
           phone
           create_time
     '''
-    user_schema = User.schema()
-    # Team members
     team_members_layout = '''#!read?title=Members
         1#summary,     members#8                                                  
           logo           avatar, name, status, roles, email, phone, team_join_time
           name         
           phone                                                                
           members                                                                   
           create_time  
     '''
+    # Schemas
+    user_schema = User.schema()
     team_schema = Team.schema()
 
     #
     # Validation
     #
 
     # Validate invalid indent
@@ -126,14 +127,17 @@
 <body>
     <h1 class="base">Members</h1>
     <h2>read</h2>
     <div class="row">
         <div class="column">1</div>
         <div class="column">members</div>
     </div>
+    <div class="row">
+        <div class="column">members</div>
+    </div>
 </body>
 </html>'''
     #
     with open('www/templates/public/team-members.html.1', 'w', encoding='utf-8') as f:
         f.write(base)
     #
     this = '''<html>
@@ -143,14 +147,17 @@
 <body>
     <h1 class="this">Members</h1>
     <h2>read</h2>
     <div class="row">
         <div class="column">1</div>
         <div class="column">members</div>
     </div>
+    <div class="row">
+        <div class="column">members</div>
+    </div>
 </body>
 </html>'''
     with open('www/templates/public/team-members.html', 'w', encoding='utf-8') as f:
         f.write(this)
     #
     # Generate
     #
@@ -206,14 +213,17 @@
     <h1 class="this">Members</h1>
 >>>>>>> THIS
     <h2>read</h2>
     <div class="row">
         <div class="column">1</div>
         <div class="column">members</div>
     </div>
+    <div class="row">
+        <div class="column">members</div>
+    </div>
 </body>
 </html>'''
     # enum.js should be rendered every time
     enums_js = open('www/static/js/enums.js', encoding='utf-8').read()
     assert enums_js == '''//
 // Enums
 //
```

### Comparing `py3seed-0.3.6/tests/test_merge3.py` & `py3seed-0.3.7/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.3.6/tests/test_model.py` & `py3seed-0.3.7/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,17 @@
     assert schema['properties']['posts']['items']['properties']['title']['type'] == 'string'
     assert schema['properties']['posts']['items']['properties']['comments']['items']['properties']['date'][
                'type'] == 'date'
     assert 'ip' in schema['properties']['last_login']['properties']
     assert 'ip' in schema['properties']['logins']['items']['properties']
     assert 'title' in schema['properties']['posts']['items']['properties']
     assert schema['searchables'] == ['name__like', 'status']
-    #
     assert schema['properties']['team']['icon'] == 'users'
+    #
+    assert schema['columns'] == User.__columns__
     # Relation schema
     assert schema['relations'] == ['Team']
     assert 'is_out_relation' not in schema['properties']['sibling']
     assert schema['properties']['team']['is_out_relation']
     assert schema['properties']['team']['properties']['name']['type'] == 'string'
     assert schema['properties']['team']['properties']['_id']['py_type'] == 'ObjectId'
     assert schema['properties']['team_id']['py_type'] == 'ObjectId'
```

### Comparing `py3seed-0.3.6/tests/test_mongosupport.py` & `py3seed-0.3.7/tests/test_mongosupport.py`

 * *Files identical despite different names*

