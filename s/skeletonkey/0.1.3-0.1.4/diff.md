# Comparing `tmp/skeletonkey-0.1.3.tar.gz` & `tmp/skeletonkey-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.1.3.tar", last modified: Tue Aug  1 22:12:10 2023, max compression
+gzip compressed data, was "skeletonkey-0.1.4.tar", last modified: Tue Aug  8 23:57:09 2023, max compression
```

## Comparing `skeletonkey-0.1.3.tar` & `skeletonkey-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-01 22:12:10.302878 skeletonkey-0.1.3/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.3/LICENSE
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-08-01 22:12:10.290877 skeletonkey-0.1.3/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.3/README.md
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-08-01 22:12:10.322878 skeletonkey-0.1.3/setup.cfg
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      758 2023-08-01 22:12:04.000000 skeletonkey-0.1.3/setup.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-01 22:12:09.830856 skeletonkey-0.1.3/skeletonkey/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      598 2023-08-01 22:00:42.000000 skeletonkey-0.1.3/skeletonkey/__init__.py
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)    11332 2023-08-01 22:00:42.000000 skeletonkey-0.1.3/skeletonkey/config.py
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     6133 2023-08-01 22:00:42.000000 skeletonkey-0.1.3/skeletonkey/core.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-01 22:12:10.214873 skeletonkey-0.1.3/skeletonkey.egg-info/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      266 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       14 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/requires.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-08 23:57:09.422968 skeletonkey-0.1.4/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.4/LICENSE
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-08-08 23:57:09.398967 skeletonkey-0.1.4/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.4/README.md
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-08-08 23:57:09.450970 skeletonkey-0.1.4/setup.cfg
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      758 2023-08-08 23:55:06.000000 skeletonkey-0.1.4/setup.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-08 23:57:08.798939 skeletonkey-0.1.4/skeletonkey/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      598 2023-08-01 22:00:42.000000 skeletonkey-0.1.4/skeletonkey/__init__.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)    11332 2023-08-01 22:00:42.000000 skeletonkey-0.1.4/skeletonkey/config.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     6208 2023-08-08 23:54:23.000000 skeletonkey-0.1.4/skeletonkey/core.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-08 23:57:09.298963 skeletonkey-0.1.4/skeletonkey.egg-info/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-08-08 23:57:07.000000 skeletonkey-0.1.4/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      266 2023-08-08 23:57:08.000000 skeletonkey-0.1.4/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-08-08 23:57:07.000000 skeletonkey-0.1.4/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       14 2023-08-08 23:57:07.000000 skeletonkey-0.1.4/skeletonkey.egg-info/requires.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-08-08 23:57:07.000000 skeletonkey-0.1.4/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.1.3/LICENSE` & `skeletonkey-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.3/PKG-INFO` & `skeletonkey-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.1.3
+Version: 0.1.4
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skeletonkey-0.1.3/README.md` & `skeletonkey-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.3/setup.py` & `skeletonkey-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version="0.1.3",
+    version="0.1.4",
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
```

### Comparing `skeletonkey-0.1.3/skeletonkey/__init__.py` & `skeletonkey-0.1.4/skeletonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.3/skeletonkey/config.py` & `skeletonkey-0.1.4/skeletonkey/config.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.3/skeletonkey/core.py` & `skeletonkey-0.1.4/skeletonkey/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,18 @@
     target_keyword = "_target_"
     class_obj = import_class(obj_kwargs[target_keyword])
     del obj_kwargs[target_keyword]
 
     obj_kwargs.update(kwargs)
 
     obj_parameters = inspect.signature(class_obj).parameters
-    required_parameters = [param_name for param_name, param in obj_parameters.items() if param.default == param.empty]
+    required_parameters = [
+        param_name for param_name, param in obj_parameters.items()
+        if param.default == param.empty and param.kind != inspect.Parameter.VAR_KEYWORD
+    ]
     valid_parameters = {k: v for k, v in obj_kwargs.items() if k in required_parameters}
     missing_parameters = [k for k in required_parameters if k not in valid_parameters.keys()]
 
     if len(missing_parameters) != 0:
         raise TypeError(
             f"missing {len(missing_parameters)} required positional(s) argument: {', '.join(missing_parameters)}."
             + "Add it to your config or as a keyword argument to skeletonkey.instantiate()."
@@ -163,8 +166,8 @@
 
         if not hasattr(obj_namespace, "_target_"):
             raise ValueError(f"subconfig ({obj_key}) in collection does not have '_target_' key at the top level.")
         
         obj = instantiate(obj_namespace, **kwargs)
         objects.append(obj)
     
-    return tuple(objects)
+    return tuple(objects)
```

### Comparing `skeletonkey-0.1.3/skeletonkey.egg-info/PKG-INFO` & `skeletonkey-0.1.4/skeletonkey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.1.3
+Version: 0.1.4
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

