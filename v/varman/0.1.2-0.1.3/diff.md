# Comparing `tmp/varman-0.1.2.tar.gz` & `tmp/varman-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varman-0.1.2.tar", last modified: Fri Aug  4 03:53:50 2023, max compression
+gzip compressed data, was "varman-0.1.3.tar", last modified: Wed Aug  9 03:00:46 2023, max compression
```

## Comparing `varman-0.1.2.tar` & `varman-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 03:53:50.948702 varman-0.1.2/
--rw-rw-rw-   0        0        0     1084 2023-08-03 04:17:23.000000 varman-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3001 2023-08-04 03:53:50.947703 varman-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2578 2023-08-04 02:50:05.000000 varman-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 03:53:50.948702 varman-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-08-04 03:53:39.000000 varman-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 03:53:50.931450 varman-0.1.2/varman/
--rw-rw-rw-   0        0        0     4168 2023-08-04 02:43:45.000000 varman-0.1.2/varman/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 03:53:50.946719 varman-0.1.2/varman.egg-info/
--rw-rw-rw-   0        0        0     3001 2023-08-04 03:53:50.000000 varman-0.1.2/varman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-08-04 03:53:50.000000 varman-0.1.2/varman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 03:53:50.000000 varman-0.1.2/varman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 03:53:50.000000 varman-0.1.2/varman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 03:00:46.674254 varman-0.1.3/
+-rw-rw-rw-   0        0        0     1083 2023-08-09 02:54:16.000000 varman-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3001 2023-08-09 03:00:46.673256 varman-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2578 2023-08-04 02:50:05.000000 varman-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-09 03:00:46.675254 varman-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-08-04 11:36:10.000000 varman-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:00:46.659761 varman-0.1.3/varman/
+-rw-rw-rw-   0        0        0     4352 2023-08-04 11:52:04.000000 varman-0.1.3/varman/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:00:46.672254 varman-0.1.3/varman.egg-info/
+-rw-rw-rw-   0        0        0     3001 2023-08-09 03:00:46.000000 varman-0.1.3/varman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-08-09 03:00:46.000000 varman-0.1.3/varman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 03:00:46.000000 varman-0.1.3/varman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-09 03:00:46.000000 varman-0.1.3/varman.egg-info/top_level.txt
```

### Comparing `varman-0.1.2/LICENSE` & `varman-0.1.3/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 枣狸
+Copyright (c) 2023 zloss
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `varman-0.1.2/PKG-INFO` & `varman-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varman
-Version: 0.1.2
+Version: 0.1.3
 Summary: A dict like variable manager, listen for variable changes.
 Home-page: https://github.com/zlolss/VarMan.py.git
 Author: zloss
 Author-email: zlols@foxmail.com
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `varman-0.1.2/README.md` & `varman-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `varman-0.1.2/setup.py` & `varman-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="varman",
-  version="0.1.2",
+  version="0.1.3",
   python_requires=">=3.6",
   author="zloss",
   author_email="zlols@foxmail.com",
   description="A dict like variable manager, listen for variable changes.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/zlolss/VarMan.py.git",
```

### Comparing `varman-0.1.2/varman/__init__.py` & `varman-0.1.3/varman/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 
 import collections as __collections
 
 class VarMan(__collections.abc.Mapping):
     
+
     '''
 用法：
 var=VarManager()
 modifydset = var.POPMODIFY(tag='default')
 for key in modifydset:
     print(var[key])
 
@@ -35,14 +36,19 @@
             self.__listeners[key] = []
         def onmodify(func):
             self.__listeners[key].append(func)
             # print(f'addlistener:{func}')
             return func
         return onmodify
         
+    def __itemEqual(self, a, b):
+        from typing import Iterable
+        if isinstance(a, Iterable):
+            return id(a) == id(b)
+        return a == b
     
     def REMOVELISTENER(self, key):
         if key in self.__listeners:
             del(self.__listeners[key])
             
     
     def REMOVEANYLISTENER(self):
@@ -111,15 +117,15 @@
     def __setattr__(self, key, value):
         if not self.__isValidVarName(key):
             raise TypeError(f'变量名{key}不合法')
         if key[0] == '_':
             self.__dict__[key] = value
             return 
         
-        if key in self.__vars and self.__vars[key] == value:
+        if key in self.__vars and self.__itemEqual(self.__vars[key], value):
             return
         
         prevalue = self.__vars.get(key, None)
         self.__vars[key] = value
         self.__modify_sequence.append(key)
         
         callbacks = self.__listeners.get(key, None)
```

### Comparing `varman-0.1.2/varman.egg-info/PKG-INFO` & `varman-0.1.3/varman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varman
-Version: 0.1.2
+Version: 0.1.3
 Summary: A dict like variable manager, listen for variable changes.
 Home-page: https://github.com/zlolss/VarMan.py.git
 Author: zloss
 Author-email: zlols@foxmail.com
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

