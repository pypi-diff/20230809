# Comparing `tmp/fixreprod-0.0.2.tar.gz` & `tmp/fixreprod-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixreprod-0.0.2.tar", last modified: Wed Aug  9 00:58:20 2023, max compression
+gzip compressed data, was "fixreprod-0.0.3.tar", last modified: Wed Aug  9 01:03:28 2023, max compression
```

## Comparing `fixreprod-0.0.2.tar` & `fixreprod-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 00:58:20.595248 fixreprod-0.0.2/
--rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 00:58:20.593946 fixreprod-0.0.2/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1300 2023-08-02 03:42:28.000000 fixreprod-0.0.2/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-09 00:58:20.595248 fixreprod-0.0.2/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      949 2023-08-09 00:57:45.000000 fixreprod-0.0.2/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 00:58:20.586364 fixreprod-0.0.2/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 00:58:20.592937 fixreprod-0.0.2/src/fixreprod.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      223 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       46 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       10 2023-08-09 00:58:20.000000 fixreprod-0.0.2/src/fixreprod.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1741 2023-08-08 04:41:55.000000 fixreprod-0.0.2/src/fixreprod.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 01:03:28.548337 fixreprod-0.0.3/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 01:03:28.547334 fixreprod-0.0.3/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1300 2023-08-02 03:42:28.000000 fixreprod-0.0.3/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-08-09 01:03:28.548337 fixreprod-0.0.3/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      949 2023-08-09 01:02:18.000000 fixreprod-0.0.3/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 01:03:28.526579 fixreprod-0.0.3/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-08-09 01:03:28.545820 fixreprod-0.0.3/src/fixreprod.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1826 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      223 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       46 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       10 2023-08-09 01:03:28.000000 fixreprod-0.0.3/src/fixreprod.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     1760 2023-08-09 01:01:36.000000 fixreprod-0.0.3/src/fixreprod.py
```

### Comparing `fixreprod-0.0.2/PKG-INFO` & `fixreprod-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixreprod
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for showing all seeds to be fixed
 Home-page: https://github.com/ytakefuji/fixreprod
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/fixreprod
 Platform: UNKNOWN
```

### Comparing `fixreprod-0.0.2/README.md` & `fixreprod-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fixreprod-0.0.2/setup.py` & `fixreprod-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fixreprod",
-    version="0.0.2",
+    version="0.0.3",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for showing all seeds to be fixed",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/fixreprod",
     project_urls={
```

### Comparing `fixreprod-0.0.2/src/fixreprod.egg-info/PKG-INFO` & `fixreprod-0.0.3/src/fixreprod.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixreprod
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for showing all seeds to be fixed
 Home-page: https://github.com/ytakefuji/fixreprod
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/fixreprod
 Platform: UNKNOWN
```

### Comparing `fixreprod-0.0.2/src/fixreprod.py` & `fixreprod-0.0.3/src/fixreprod.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,20 @@
             new_code += f"{library}.{m}.seed({random.randint(0, 1)})\n"
       except ModuleNotFoundError:
         pass
     else:
       new_code += line + "\n"
   return new_code
 
-
-if __name__ == "__main__":
+def main():
   source_code = input("Enter the source code file name: ")
   with open(source_code, "r") as f:
     source_code = f.read()
 
   if check_for_random_numbers(source_code):
     new_code = initialize_seeds(source_code)
     print(new_code)
   else:
     print("The source code does not contain random numbers.")
 
+if __name__ == "__main__":
+ main()
```

