# Comparing `tmp/fixreprod-0.0.1.tar.gz` & `tmp/fixreprod-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixreprod-0.0.1.tar", last modified: Wed Aug  2 04:10:14 2023, max compression
+gzip compressed data, was "fixreprod-0.0.2.tar", last modified: Wed Aug  9 00:58:20 2023, max compression
```

## Comparing `fixreprod-0.0.1.tar` & `fixreprod-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-02 04:10:14.426706 fixreprod-0.0.1/
--rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-02 04:10:14.425714 fixreprod-0.0.1/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1300 2023-08-02 03:42:28.000000 fixreprod-0.0.1/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-02 04:10:14.426706 fixreprod-0.0.1/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      949 2023-08-02 03:48:28.000000 fixreprod-0.0.1/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-02 04:10:14.419539 fixreprod-0.0.1/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-02 04:10:14.424688 fixreprod-0.0.1/src/fixreprod.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-02 04:10:14.000000 fixreprod-0.0.1/src/fixreprod.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      223 2023-08-02 04:10:14.000000 fixreprod-0.0.1/src/fixreprod.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-02 04:10:14.000000 fixreprod-0.0.1/src/fixreprod.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       46 2023-08-02 04:10:14.000000 fixreprod-0.0.1/src/fixreprod.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       10 2023-08-02 04:10:14.000000 fixreprod-0.0.1/src/fixreprod.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1354 2023-08-02 04:09:25.000000 fixreprod-0.0.1/src/fixreprod.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 00:58:20.595248 fixreprod-0.0.2/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 00:58:20.593946 fixreprod-0.0.2/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1300 2023-08-02 03:42:28.000000 fixreprod-0.0.2/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-09 00:58:20.595248 fixreprod-0.0.2/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      949 2023-08-09 00:57:45.000000 fixreprod-0.0.2/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 00:58:20.586364 fixreprod-0.0.2/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 00:58:20.592937 fixreprod-0.0.2/src/fixreprod.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      223 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       46 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       10 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     1741 2023-08-08 04:41:55.000000 fixreprod-0.0.2/src/fixreprod.py
```

### Comparing `fixreprod-0.0.1/PKG-INFO` & `fixreprod-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixreprod
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for showing all seeds to be fixed
 Home-page: https://github.com/ytakefuji/fixreprod
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/fixreprod
 Platform: UNKNOWN
```

### Comparing `fixreprod-0.0.1/README.md` & `fixreprod-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fixreprod-0.0.1/setup.py` & `fixreprod-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fixreprod",
-    version="0.0.1",
+    version="0.0.2",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for showing all seeds to be fixed",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/fixreprod",
     project_urls={
```

### Comparing `fixreprod-0.0.1/src/fixreprod.egg-info/PKG-INFO` & `fixreprod-0.0.2/src/fixreprod.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixreprod
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for showing all seeds to be fixed
 Home-page: https://github.com/ytakefuji/fixreprod
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/fixreprod
 Platform: UNKNOWN
```

### Comparing `fixreprod-0.0.1/src/fixreprod.py` & `fixreprod-0.0.2/src/fixreprod.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,63 @@
 import random
 import importlib
 import re
 
 def check_for_random_numbers(source_code):
+  """Checks whether the given source code contains random numbers.
+
+  Args:
+    source_code: The source code to check.
+
+  Returns:
+    True if the source code contains random numbers, False otherwise.
+  """
+
   for line in source_code.splitlines():
     match = re.search("import\s+([a-zA-Z0-9_.]+)\s*", line)
     if match:
       library = match.group(1)
       try:
         for m in importlib.import_module(library).__dict__.keys():
           if hasattr(getattr(importlib.import_module(library), m), "seed"):
             return True
       except ModuleNotFoundError:
         pass
   return False
 
 def initialize_seeds(source_code):
+  """Initializes all seeds for all API libraries in the source code file.
+
+  Args:
+    source_code: The source code to initialize seeds for.
+
+  Returns:
+    A new code with all seeds initialized.
+  """
+
   new_code = ""
   for line in source_code.splitlines():
     match = re.search("import\s+([a-zA-Z0-9_.]+)\s*", line)
     if match:
       library = match.group(1)
       try:
         for m in importlib.import_module(library).__dict__.keys():
           if hasattr(getattr(importlib.import_module(library), m), "seed"):
-            new_code += f"{library}.{m}.seed({random.randint(0, 100000)})\n"
+            new_code += f"{library}.{m}.seed({random.randint(0, 1)})\n"
       except ModuleNotFoundError:
         pass
     else:
       new_code += line + "\n"
   return new_code
 
-def main():
+
+if __name__ == "__main__":
   source_code = input("Enter the source code file name: ")
   with open(source_code, "r") as f:
     source_code = f.read()
 
   if check_for_random_numbers(source_code):
     new_code = initialize_seeds(source_code)
     print(new_code)
   else:
     print("The source code does not contain random numbers.")
 
-if __name__ == "__main__":
- main()
```

