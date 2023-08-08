# Comparing `tmp/smart_app_framework-2.3.0rc2-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.3.0rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 306834 bytes, number of entries: 334
+Zip file size: 306833 bytes, number of entries: 334
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6902 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -326,11 +326,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     3946 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3322 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10824 b- defN 80-Jan-01 00:00 smart_app_framework-2.3.0rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.3.0rc2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32355 b- defN 16-Jan-01 00:00 smart_app_framework-2.3.0rc2.dist-info/RECORD
-334 files, 987932 bytes uncompressed, 254088 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10824 b- defN 80-Jan-01 00:00 smart_app_framework-2.3.0rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.3.0rc3.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32355 b- defN 16-Jan-01 00:00 smart_app_framework-2.3.0rc3.dist-info/RECORD
+334 files, 987932 bytes uncompressed, 254087 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -987,17 +987,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.3.0rc2.dist-info/METADATA
+Filename: smart_app_framework-2.3.0rc3.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.3.0rc2.dist-info/WHEEL
+Filename: smart_app_framework-2.3.0rc3.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.3.0rc2.dist-info/RECORD
+Filename: smart_app_framework-2.3.0rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `smart_app_framework-2.3.0rc2.dist-info/METADATA` & `smart_app_framework-2.3.0rc3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.3.0rc2
+Version: 2.3.0rc3
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

## Comparing `smart_app_framework-2.3.0rc2.dist-info/RECORD` & `smart_app_framework-2.3.0rc3.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -325,10 +325,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=UP2Zmp0VW4YZpDPe_lGQ-5L_wF5wd7J4B33kXyUINmQ,3946
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=n5N4FHjXyeZAASjVB2zhoOMsbnWiixI0OQsk4KkcDFg,3322
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.3.0rc2.dist-info/METADATA,sha256=k4pGN3AunVkSe5euOFnJc5BlRHRyMk3gM_Qc6KyvaqU,10824
-smart_app_framework-2.3.0rc2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-smart_app_framework-2.3.0rc2.dist-info/RECORD,,
+smart_app_framework-2.3.0rc3.dist-info/METADATA,sha256=m2o1b1mK-6lJYpg9XrV2X_KOCt_XIr7KdvLJmywWEao,10824
+smart_app_framework-2.3.0rc3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.3.0rc3.dist-info/RECORD,,
```

