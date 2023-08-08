# Comparing `tmp/jacktrade-0.1.2.tar.gz` & `tmp/jacktrade-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jacktrade-0.1.2.tar", last modified: Tue Aug  1 08:18:05 2023, max compression
+gzip compressed data, was "jacktrade-0.2.0.tar", last modified: Tue Aug  8 21:33:52 2023, max compression
```

## Comparing `jacktrade-0.1.2.tar` & `jacktrade-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:18:05.206177 jacktrade-0.1.2/
--rw-rw-rw-   0        0        0     1077 2023-02-11 18:38:48.000000 jacktrade-0.1.2/LICENSE.md
--rw-rw-rw-   0        0        0     5258 2023-08-01 08:18:05.205180 jacktrade-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3486 2023-05-24 11:40:26.000000 jacktrade-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 08:18:05.181244 jacktrade-0.1.2/jacktrade/
--rw-rw-rw-   0        0        0        0 2023-02-12 13:53:20.000000 jacktrade-0.1.2/jacktrade/__init__.py
--rw-rw-rw-   0        0        0     2300 2023-04-09 15:05:56.000000 jacktrade-0.1.2/jacktrade/benchmark.py
--rw-rw-rw-   0        0        0     3809 2023-08-01 08:16:47.000000 jacktrade-0.1.2/jacktrade/collections.py
--rw-rw-rw-   0        0        0     2486 2023-04-08 15:30:12.000000 jacktrade-0.1.2/jacktrade/multicore.py
--rw-rw-rw-   0        0        0      662 2023-04-08 16:09:02.000000 jacktrade-0.1.2/jacktrade/pickler.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:18:05.191217 jacktrade-0.1.2/jacktrade.egg-info/
--rw-rw-rw-   0        0        0     5258 2023-08-01 08:18:05.000000 jacktrade-0.1.2/jacktrade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-08-01 08:18:05.000000 jacktrade-0.1.2/jacktrade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:18:05.000000 jacktrade-0.1.2/jacktrade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 08:18:05.000000 jacktrade-0.1.2/jacktrade.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      727 2023-08-01 08:14:05.000000 jacktrade-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 08:18:05.206177 jacktrade-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 08:18:05.203185 jacktrade-0.1.2/tests/
--rw-rw-rw-   0        0        0     1891 2023-04-08 14:04:02.000000 jacktrade-0.1.2/tests/test_benchmark.py
--rw-rw-rw-   0        0        0     4555 2023-08-01 08:17:05.000000 jacktrade-0.1.2/tests/test_collections.py
--rw-rw-rw-   0        0        0     3232 2023-04-09 12:49:59.000000 jacktrade-0.1.2/tests/test_multicore.py
--rw-rw-rw-   0        0        0      608 2023-04-08 16:08:21.000000 jacktrade-0.1.2/tests/test_pickler.py
--rw-rw-rw-   0        0        0      180 2023-04-08 14:13:05.000000 jacktrade-0.1.2/tests/test_template.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:33:52.097062 jacktrade-0.2.0/
+-rw-rw-rw-   0        0        0     1077 2023-02-11 18:38:48.000000 jacktrade-0.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0     5258 2023-08-08 21:33:52.096066 jacktrade-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3486 2023-05-24 11:40:26.000000 jacktrade-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 21:33:52.076119 jacktrade-0.2.0/jacktrade/
+-rw-rw-rw-   0        0        0      320 2023-08-08 21:31:26.000000 jacktrade-0.2.0/jacktrade/__init__.py
+-rw-rw-rw-   0        0        0     2300 2023-04-09 15:05:56.000000 jacktrade-0.2.0/jacktrade/benchmark.py
+-rw-rw-rw-   0        0        0     3200 2023-08-08 16:34:17.000000 jacktrade-0.2.0/jacktrade/buffers.py
+-rw-rw-rw-   0        0        0     3809 2023-08-01 08:16:47.000000 jacktrade-0.2.0/jacktrade/collections.py
+-rw-rw-rw-   0        0        0     2486 2023-04-08 15:30:12.000000 jacktrade-0.2.0/jacktrade/multicore.py
+-rw-rw-rw-   0        0        0      662 2023-04-08 16:09:02.000000 jacktrade-0.2.0/jacktrade/pickler.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:33:52.084097 jacktrade-0.2.0/jacktrade.egg-info/
+-rw-rw-rw-   0        0        0     5258 2023-08-08 21:33:52.000000 jacktrade-0.2.0/jacktrade.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-08-08 21:33:52.000000 jacktrade-0.2.0/jacktrade.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 21:33:52.000000 jacktrade-0.2.0/jacktrade.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 21:33:52.000000 jacktrade-0.2.0/jacktrade.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      727 2023-08-08 21:32:49.000000 jacktrade-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 21:33:52.097062 jacktrade-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 21:33:52.094069 jacktrade-0.2.0/tests/
+-rw-rw-rw-   0        0        0     1881 2023-08-08 21:32:07.000000 jacktrade-0.2.0/tests/test_benchmark.py
+-rw-rw-rw-   0        0        0     3382 2023-08-08 21:32:11.000000 jacktrade-0.2.0/tests/test_buffers.py
+-rw-rw-rw-   0        0        0     4543 2023-08-08 21:32:16.000000 jacktrade-0.2.0/tests/test_collections.py
+-rw-rw-rw-   0        0        0     3222 2023-08-08 21:32:20.000000 jacktrade-0.2.0/tests/test_multicore.py
+-rw-rw-rw-   0        0        0      600 2023-08-08 21:32:25.000000 jacktrade-0.2.0/tests/test_pickler.py
+-rw-rw-rw-   0        0        0      180 2023-04-08 14:13:05.000000 jacktrade-0.2.0/tests/test_template.py
```

### Comparing `jacktrade-0.1.2/LICENSE.md` & `jacktrade-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.2/PKG-INFO` & `jacktrade-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktrade
-Version: 0.1.2
+Version: 0.2.0
 Summary: A collection of commonly used Python utilities.
 Author-email: Mario Zaja <mzaja0@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Mario Zaja
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `jacktrade-0.1.2/README.md` & `jacktrade-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.2/jacktrade/benchmark.py` & `jacktrade-0.2.0/jacktrade/benchmark.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.2/jacktrade/collections.py` & `jacktrade-0.2.0/jacktrade/collections.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.2/jacktrade/multicore.py` & `jacktrade-0.2.0/jacktrade/multicore.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.2/jacktrade/pickler.py` & `jacktrade-0.2.0/jacktrade/pickler.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.2/jacktrade.egg-info/PKG-INFO` & `jacktrade-0.2.0/jacktrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktrade
-Version: 0.1.2
+Version: 0.2.0
 Summary: A collection of commonly used Python utilities.
 Author-email: Mario Zaja <mzaja0@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Mario Zaja
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `jacktrade-0.1.2/pyproject.toml` & `jacktrade-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jacktrade"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Mario Zaja", email="mzaja0@gmail.com" },
 ]
 description = "A collection of commonly used Python utilities."
 readme = "README.md"
 license = { file = "LICENSE.md" }
 requires-python = ">=3.10"
```

### Comparing `jacktrade-0.1.2/tests/test_benchmark.py` & `jacktrade-0.2.0/tests/test_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from unittest import mock
 from time import sleep
 
-from jacktrade.benchmark import CodeTimer
+from jacktrade import CodeTimer
 
 
 class CodeTimerTest(unittest.TestCase):
     """
     Tests the CodeTimer class.
     """
```

### Comparing `jacktrade-0.1.2/tests/test_collections.py` & `jacktrade-0.2.0/tests/test_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from typing import Iterator
 
-from jacktrade.collections import (
+from jacktrade import (
     flatten_dict,
     get_first_dict_item,
     get_first_dict_key,
     get_first_dict_value,
     flatten_list,
     chunkify,
     ichunkify,
```

### Comparing `jacktrade-0.1.2/tests/test_multicore.py` & `jacktrade-0.2.0/tests/test_multicore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from unittest import mock
 from multiprocessing import cpu_count
 
-from jacktrade.multicore import do_multicore_work
+from jacktrade import do_multicore_work
 
 # ---------------------------------------------------------------------------
 # TEST FIXTURES
 # ---------------------------------------------------------------------------
 NUMBERS = [1, 2, 3, 4, 5]
 LETTERS = ["a", "b", "c", "d", "e"]
 COMBINED = list(zip(NUMBERS, LETTERS))
```

### Comparing `jacktrade-0.1.2/tests/test_pickler.py` & `jacktrade-0.2.0/tests/test_pickler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tempfile
 import os.path
 import unittest
 
-from jacktrade.pickler import pickle_object, unpickle_object
+from jacktrade import pickle_object, unpickle_object
 
 
 class PickerTest(unittest.TestCase):
     """
     Tests the convenience pickling functions.
     """
```

