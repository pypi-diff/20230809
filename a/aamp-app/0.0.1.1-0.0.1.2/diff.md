# Comparing `tmp/aamp_app-0.0.1.1.tar.gz` & `tmp/aamp_app-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aamp_app-0.0.1.1.tar", last modified: Wed Aug  9 00:41:20 2023, max compression
+gzip compressed data, was "aamp_app-0.0.1.2.tar", last modified: Wed Aug  9 00:48:04 2023, max compression
```

## Comparing `aamp_app-0.0.1.1.tar` & `aamp_app-0.0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 pp         (501) staff       (20)        0 2023-08-09 00:41:20.309183 aamp_app-0.0.1.1/
--rw-r--r--   0 pp         (501) staff       (20)      366 2023-08-09 00:41:20.308845 aamp_app-0.0.1.1/PKG-INFO
--rw-r--r--   0 pp         (501) staff       (20)       62 2023-08-08 00:58:12.000000 aamp_app-0.0.1.1/README.md
-drwxr-xr-x   0 pp         (501) staff       (20)        0 2023-08-09 00:41:20.303950 aamp_app-0.0.1.1/aamp_app/
-drwxr-xr-x   0 pp         (501) staff       (20)        0 2023-08-09 00:41:20.306256 aamp_app-0.0.1.1/aamp_app/src/
-drwxr-xr-x   0 pp         (501) staff       (20)        0 2023-08-09 00:41:20.308274 aamp_app-0.0.1.1/aamp_app/src/aamp_app.egg-info/
--rw-r--r--   0 pp         (501) staff       (20)      366 2023-08-09 00:41:20.000000 aamp_app-0.0.1.1/aamp_app/src/aamp_app.egg-info/PKG-INFO
--rw-r--r--   0 pp         (501) staff       (20)      300 2023-08-09 00:41:20.000000 aamp_app-0.0.1.1/aamp_app/src/aamp_app.egg-info/SOURCES.txt
--rw-r--r--   0 pp         (501) staff       (20)        1 2023-08-09 00:41:20.000000 aamp_app-0.0.1.1/aamp_app/src/aamp_app.egg-info/dependency_links.txt
--rw-r--r--   0 pp         (501) staff       (20)      171 2023-08-09 00:41:20.000000 aamp_app-0.0.1.1/aamp_app/src/aamp_app.egg-info/requires.txt
--rw-r--r--   0 pp         (501) staff       (20)       26 2023-08-09 00:41:20.000000 aamp_app-0.0.1.1/aamp_app/src/aamp_app.egg-info/top_level.txt
--rw-r--r--   0 pp         (501) staff       (20)    77964 2023-08-08 01:40:28.000000 aamp_app-0.0.1.1/aamp_app/src/aamp_app.py
--rw-r--r--   0 pp         (501) staff       (20)    26454 2023-07-28 17:35:44.000000 aamp_app-0.0.1.1/aamp_app/src/command_sequence.py
--rw-r--r--   0 pp         (501) staff       (20)       38 2023-08-09 00:41:20.309303 aamp_app-0.0.1.1/setup.cfg
--rw-r--r--   0 pp         (501) staff       (20)     1436 2023-08-09 00:40:44.000000 aamp_app-0.0.1.1/setup.py
+drwxr-xr-x   0 pp         (501) staff       (20)        0 2023-08-09 00:48:04.384276 aamp_app-0.0.1.2/
+-rw-r--r--   0 pp         (501) staff       (20)      366 2023-08-09 00:48:04.383442 aamp_app-0.0.1.2/PKG-INFO
+-rw-r--r--   0 pp         (501) staff       (20)       62 2023-08-08 00:58:12.000000 aamp_app-0.0.1.2/README.md
+drwxr-xr-x   0 pp         (501) staff       (20)        0 2023-08-09 00:48:04.374492 aamp_app-0.0.1.2/aamp_app/
+drwxr-xr-x   0 pp         (501) staff       (20)        0 2023-08-09 00:48:04.379085 aamp_app-0.0.1.2/aamp_app/src/
+drwxr-xr-x   0 pp         (501) staff       (20)        0 2023-08-09 00:48:04.382503 aamp_app-0.0.1.2/aamp_app/src/aamp_app.egg-info/
+-rw-r--r--   0 pp         (501) staff       (20)      366 2023-08-09 00:48:04.000000 aamp_app-0.0.1.2/aamp_app/src/aamp_app.egg-info/PKG-INFO
+-rw-r--r--   0 pp         (501) staff       (20)      332 2023-08-09 00:48:04.000000 aamp_app-0.0.1.2/aamp_app/src/aamp_app.egg-info/SOURCES.txt
+-rw-r--r--   0 pp         (501) staff       (20)        1 2023-08-09 00:48:04.000000 aamp_app-0.0.1.2/aamp_app/src/aamp_app.egg-info/dependency_links.txt
+-rw-r--r--   0 pp         (501) staff       (20)      171 2023-08-09 00:48:04.000000 aamp_app-0.0.1.2/aamp_app/src/aamp_app.egg-info/requires.txt
+-rw-r--r--   0 pp         (501) staff       (20)       59 2023-08-09 00:48:04.000000 aamp_app-0.0.1.2/aamp_app/src/aamp_app.egg-info/top_level.txt
+-rw-r--r--   0 pp         (501) staff       (20)    77964 2023-08-08 01:40:28.000000 aamp_app-0.0.1.2/aamp_app/src/aamp_app.py
+-rw-r--r--   0 pp         (501) staff       (20)    13447 2023-07-28 17:35:44.000000 aamp_app-0.0.1.2/aamp_app/src/command_invoker.py
+-rw-r--r--   0 pp         (501) staff       (20)    26454 2023-07-28 17:35:44.000000 aamp_app-0.0.1.2/aamp_app/src/command_sequence.py
+-rw-r--r--   0 pp         (501) staff       (20)       38 2023-08-09 00:48:04.384542 aamp_app-0.0.1.2/setup.cfg
+-rw-r--r--   0 pp         (501) staff       (20)     1525 2023-08-09 00:46:36.000000 aamp_app-0.0.1.2/setup.py
```

### Comparing `aamp_app-0.0.1.1/aamp_app/src/aamp_app.py` & `aamp_app-0.0.1.2/aamp_app/src/aamp_app.py`

 * *Files identical despite different names*

### Comparing `aamp_app-0.0.1.1/aamp_app/src/command_sequence.py` & `aamp_app-0.0.1.2/aamp_app/src/command_sequence.py`

 * *Files identical despite different names*

### Comparing `aamp_app-0.0.1.1/setup.py` & `aamp_app-0.0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aamp_app",  # This is the name of the package
-    version="0.0.1.1",  # The initial release version
+    version="0.0.1.2",  # The initial release version
     author="Piyush Pahuja",  # Full name of the author
     description="AAMP App",
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],  # Information to filter the project on PyPi website
     python_requires=">=3.6",  # Minimum version requirement of the package
-    py_modules=["aamp_app", "command_sequence"],  # Name of the python package
+    py_modules=[
+        "aamp_app",
+        "command_sequence",
+        "command_invoker",
+        "commands",
+        "devices",
+    ],  # Name of the python package
     package_dir={"": "aamp_app/src"},  # Directory of the source code of the package
     install_requires=[
         "certifi",
         "colorama",
         "dash",
         "dash-ace",
         "dash-bootstrap-components",
```

