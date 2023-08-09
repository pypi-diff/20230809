# Comparing `tmp/quao-0.4.0.8-py3-none-any.whl.zip` & `tmp/quao-0.4.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 37385 bytes, number of entries: 77
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-26 09:43 __init__.py
--rw-rw-rw-  2.0 fat      148 b- defN 23-Aug-08 10:31 quao/__init__.py
+-rw-rw-rw-  2.0 fat      148 b- defN 23-Aug-08 10:32 quao/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-02 07:11 quao/async_tasks/__init__.py
 -rw-rw-rw-  2.0 fat     2893 b- defN 23-Aug-03 09:28 quao/async_tasks/export_circuit_task.py
 -rw-rw-rw-  2.0 fat     2265 b- defN 23-Aug-08 02:48 quao/async_tasks/post_processing_task.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-02 07:59 quao/component/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-02 08:48 quao/component/backend/__init__.py
 -rw-rw-rw-  2.0 fat     7206 b- defN 23-Aug-08 01:42 quao/component/backend/backend.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-04 04:01 quao/component/callback/__init__.py
@@ -67,13 +67,13 @@
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-02 01:59 quao/util/__init__.py
 -rw-rw-rw-  2.0 fat     1058 b- defN 23-Aug-04 04:10 quao/util/circuit_utils.py
 -rw-rw-rw-  2.0 fat      645 b- defN 23-Aug-08 06:39 quao/util/http_utils.py
 -rw-rw-rw-  2.0 fat      417 b- defN 23-Aug-07 09:11 quao/util/job_status_mapping_utils.py
 -rw-rw-rw-  2.0 fat     2322 b- defN 23-Aug-02 07:11 quao/util/json_parser_utils.py
 -rw-rw-rw-  2.0 fat     1620 b- defN 23-Aug-08 09:40 quao/util/response_utils.py
 -rw-rw-rw-  2.0 fat      890 b- defN 23-Aug-08 04:21 quao/util/status_code_mapping_utils.py
--rw-rw-rw-  2.0 fat     1111 b- defN 23-Aug-08 10:31 quao-0.4.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3342 b- defN 23-Aug-08 10:31 quao-0.4.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-08 10:31 quao-0.4.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Aug-08 10:31 quao-0.4.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6610 b- defN 23-Aug-08 10:31 quao-0.4.0.8.dist-info/RECORD
+-rw-rw-rw-  2.0 fat     1111 b- defN 23-Aug-08 10:33 quao-0.4.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3342 b- defN 23-Aug-08 10:33 quao-0.4.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-08 10:33 quao-0.4.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Aug-08 10:33 quao-0.4.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6610 b- defN 23-Aug-08 10:33 quao-0.4.0.9.dist-info/RECORD
 77 files, 76599 bytes uncompressed, 26763 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -210,23 +210,23 @@
 
 Filename: quao/util/response_utils.py
 Comment: 
 
 Filename: quao/util/status_code_mapping_utils.py
 Comment: 
 
-Filename: quao-0.4.0.8.dist-info/LICENSE
+Filename: quao-0.4.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: quao-0.4.0.8.dist-info/METADATA
+Filename: quao-0.4.0.9.dist-info/METADATA
 Comment: 
 
-Filename: quao-0.4.0.8.dist-info/WHEEL
+Filename: quao-0.4.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: quao-0.4.0.8.dist-info/top_level.txt
+Filename: quao-0.4.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: quao-0.4.0.8.dist-info/RECORD
+Filename: quao-0.4.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quao/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "0.4.0.8"
+__version__ = "0.4.0.9"
 
 from .handler.invocation_handler import InvocationHandler
 from .handler.job_fetching_handler import JobFetchingHandler
```

## Comparing `quao-0.4.0.8.dist-info/LICENSE` & `quao-0.4.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `quao-0.4.0.8.dist-info/METADATA` & `quao-0.4.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.4.0.8
+Version: 0.4.0.9
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

## Comparing `quao-0.4.0.8.dist-info/RECORD` & `quao-0.4.0.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-quao/__init__.py,sha256=kMaXoz4orJ6vxZ3NL3Ogq4trTv6DKPwmK9O0SzP_jOg,148
+quao/__init__.py,sha256=zbvy3yE4YuS7URl4QA3KRF383LjdWtx0_lpwe5_qm_E,148
 quao/async_tasks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 quao/async_tasks/export_circuit_task.py,sha256=h8XmqVVkc4Ew2cvfuuZTDqU6AQVvgTt3H-VOq-_hEBI,2893
 quao/async_tasks/post_processing_task.py,sha256=xjYblYlLJKHS0IZZZIWd-X2kr2QfXNV9TCanyYfeI-g,2265
 quao/component/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 quao/component/backend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 quao/component/backend/backend.py,sha256=vjGjTeAMd5BntcT__MMtsHL9LAbzxKi25linrJ5-O8A,7206
 quao/component/callback/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -66,12 +66,12 @@
 quao/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 quao/util/circuit_utils.py,sha256=ucWtNNDiZesaQaESNUIW8UEVqqoCRvm7xFNxaWATuaQ,1058
 quao/util/http_utils.py,sha256=jwjgcVsE_7sphd8005bCc_6wGOluW9vz7_ohtomF75k,645
 quao/util/job_status_mapping_utils.py,sha256=pGvZUrkejUjc1B-6Cmh7sur6yBAH0Ur2rdDOolyMu9I,417
 quao/util/json_parser_utils.py,sha256=fZG0KoUC64mUZ0QZkIvmdes_xmu1UqfH83cV-jU36j8,2322
 quao/util/response_utils.py,sha256=R2v5-7SQYpYgosA-4qGVrWVu297P9hNWPxx1HsT9DPk,1620
 quao/util/status_code_mapping_utils.py,sha256=DCDg_SaJtC8v623THIDVctM_l1q0FM1ZtG7TkguGkHw,890
-quao-0.4.0.8.dist-info/LICENSE,sha256=4eavVQ3nRUakwGS4-SIlQnewquvbo6fpTU0hE5H3P3I,1111
-quao-0.4.0.8.dist-info/METADATA,sha256=xm6FxqeoiaePcCqXzcbUAg1TZIXVmHPK_MWGod6ZHDA,3342
-quao-0.4.0.8.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
-quao-0.4.0.8.dist-info/top_level.txt,sha256=4Tp4Oqy5GaNvD7KWSQkt1TJ3cm9-3nZxdu_AHJMhQDw,14
-quao-0.4.0.8.dist-info/RECORD,,
+quao-0.4.0.9.dist-info/LICENSE,sha256=4eavVQ3nRUakwGS4-SIlQnewquvbo6fpTU0hE5H3P3I,1111
+quao-0.4.0.9.dist-info/METADATA,sha256=7Wq889qDFxAFIyuzzlR11MtWRqIl__eLle3ri6q5qBI,3342
+quao-0.4.0.9.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+quao-0.4.0.9.dist-info/top_level.txt,sha256=4Tp4Oqy5GaNvD7KWSQkt1TJ3cm9-3nZxdu_AHJMhQDw,14
+quao-0.4.0.9.dist-info/RECORD,,
```

