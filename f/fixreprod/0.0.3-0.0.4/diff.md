# Comparing `tmp/fixreprod-0.0.3.tar.gz` & `tmp/fixreprod-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixreprod-0.0.3.tar", last modified: Wed Aug  9 01:03:28 2023, max compression
+gzip compressed data, was "fixreprod-0.0.4.tar", last modified: Wed Aug  9 04:26:46 2023, max compression
```

## Comparing `fixreprod-0.0.3.tar` & `fixreprod-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 01:03:28.548337 fixreprod-0.0.3/
--rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 01:03:28.547334 fixreprod-0.0.3/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1300 2023-08-02 03:42:28.000000 fixreprod-0.0.3/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-09 01:03:28.548337 fixreprod-0.0.3/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      949 2023-08-09 01:02:18.000000 fixreprod-0.0.3/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 01:03:28.526579 fixreprod-0.0.3/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 01:03:28.545820 fixreprod-0.0.3/src/fixreprod.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      223 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       46 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       10 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1760 2023-08-09 01:01:36.000000 fixreprod-0.0.3/src/fixreprod.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 04:26:46.758237 fixreprod-0.0.4/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 04:26:46.757236 fixreprod-0.0.4/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1300 2023-08-02 03:42:28.000000 fixreprod-0.0.4/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-09 04:26:46.758237 fixreprod-0.0.4/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      949 2023-08-09 04:25:14.000000 fixreprod-0.0.4/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 04:26:46.750144 fixreprod-0.0.4/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 04:26:46.756237 fixreprod-0.0.4/src/fixreprod.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 04:26:46.000000 fixreprod-0.0.4/src/fixreprod.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      223 2023-08-09 04:26:46.000000 fixreprod-0.0.4/src/fixreprod.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-09 04:26:46.000000 fixreprod-0.0.4/src/fixreprod.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       46 2023-08-09 04:26:46.000000 fixreprod-0.0.4/src/fixreprod.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       10 2023-08-09 04:26:46.000000 fixreprod-0.0.4/src/fixreprod.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     2826 2023-08-09 04:00:01.000000 fixreprod-0.0.4/src/fixreprod.py
```

### Comparing `fixreprod-0.0.3/PKG-INFO` & `fixreprod-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixreprod
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for showing all seeds to be fixed
 Home-page: https://github.com/ytakefuji/fixreprod
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/fixreprod
 Platform: UNKNOWN
```

### Comparing `fixreprod-0.0.3/README.md` & `fixreprod-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fixreprod-0.0.3/setup.py` & `fixreprod-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fixreprod",
-    version="0.0.3",
+    version="0.0.4",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for showing all seeds to be fixed",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/fixreprod",
     project_urls={
```

### Comparing `fixreprod-0.0.3/src/fixreprod.egg-info/PKG-INFO` & `fixreprod-0.0.4/src/fixreprod.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixreprod
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for showing all seeds to be fixed
 Home-page: https://github.com/ytakefuji/fixreprod
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/fixreprod
 Platform: UNKNOWN
```

### Comparing `fixreprod-0.0.3/src/fixreprod.py` & `fixreprod-0.0.4/src/fixreprod.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     source_code: The source code to check.
 
   Returns:
     True if the source code contains random numbers, False otherwise.
   """
 
   for line in source_code.splitlines():
-    match = re.search("import\s+([a-zA-Z0-9_.]+)\s*", line)
+    match = re.search(r"import\s+([a-zA-Z0-9_.]+)(?:\s+as\s+([a-zA-Z0-9_]+))?\s*", line)
     if match:
       library = match.group(1)
+      alias = match.group(2) or library
       try:
         for m in importlib.import_module(library).__dict__.keys():
           if hasattr(getattr(importlib.import_module(library), m), "seed"):
             return True
       except ModuleNotFoundError:
         pass
   return False
@@ -32,21 +33,40 @@
 
   Returns:
     A new code with all seeds initialized.
   """
 
   new_code = ""
   for line in source_code.splitlines():
-    match = re.search("import\s+([a-zA-Z0-9_.]+)\s*", line)
+    match = re.search(r"import\s+([a-zA-Z0-9_.]+)(?:\s+as\s+([a-zA-Z0-9_]+))?\s*", line)
     if match:
       library = match.group(1)
+      alias = match.group(2) or library
       try:
         for m in importlib.import_module(library).__dict__.keys():
           if hasattr(getattr(importlib.import_module(library), m), "seed"):
-            new_code += f"{library}.{m}.seed({random.randint(0, 1)})\n"
+            if library == "gym":
+              new_code += f"{alias}.Space().seed({random.randint(0, 1)})\n"
+            elif library == "torch":
+              if m == "Generator":
+                new_code += f"{alias}.{m}().seed({random.randint(0, 1)})\n"
+              elif m == "manual_seed":
+                new_code += f"{alias}.{m}({random.randint(0, 1)})\n"
+              elif m == "initial_seed":
+                new_code += f"{alias}.{m}()\n"
+              elif m == "cuda":
+                new_code += f"{alias}.{m}.manual_seed({random.randint(0, 1)})\n"
+                new_code += f"{alias}.{m}.manual_seed_all({random.randint(0, 1)})\n"
+              elif m == "use_deterministic_algorithms":
+                new_code += f"{alias}.{m}(True)\n"
+            elif library == "tensorflow":
+              if m == "set_seed":
+                new_code += f"{alias}.random.{m}({random.randint(0, 1)})\n"
+            else:
+              new_code += f"{alias}.{m}.seed({random.randint(0, 1)})\n"
       except ModuleNotFoundError:
         pass
     else:
       new_code += line + "\n"
   return new_code
 
 def main():
@@ -58,7 +78,8 @@
     new_code = initialize_seeds(source_code)
     print(new_code)
   else:
     print("The source code does not contain random numbers.")
 
 if __name__ == "__main__":
  main()
+
```

