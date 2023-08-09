# Comparing `tmp/myipmacpackage-1.0.2.tar.gz` & `tmp/myipmacpackage-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myipmacpackage-1.0.2.tar", last modified: Tue Aug  8 13:59:10 2023, max compression
+gzip compressed data, was "myipmacpackage-1.0.3.tar", last modified: Wed Aug  9 05:33:03 2023, max compression
```

## Comparing `myipmacpackage-1.0.2.tar` & `myipmacpackage-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 13:59:10.071746 myipmacpackage-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      385 2023-08-08 13:59:10.071746 myipmacpackage-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-08 13:31:39.000000 myipmacpackage-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 13:59:10.071746 myipmacpackage-1.0.2/myipmac/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 13:32:46.000000 myipmacpackage-1.0.2/myipmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-08-08 13:32:46.000000 myipmacpackage-1.0.2/myipmac/fetcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 13:59:10.071746 myipmacpackage-1.0.2/myipmacpackage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      385 2023-08-08 13:59:10.000000 myipmacpackage-1.0.2/myipmacpackage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2023-08-08 13:59:10.000000 myipmacpackage-1.0.2/myipmacpackage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 13:59:10.000000 myipmacpackage-1.0.2/myipmacpackage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-08-08 13:59:10.000000 myipmacpackage-1.0.2/myipmacpackage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-08 13:59:10.000000 myipmacpackage-1.0.2/myipmacpackage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 13:59:10.071746 myipmacpackage-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      762 2023-08-08 13:55:46.000000 myipmacpackage-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:33:03.743238 myipmacpackage-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      385 2023-08-09 05:33:03.743238 myipmacpackage-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-08 13:31:39.000000 myipmacpackage-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:33:03.743238 myipmacpackage-1.0.3/myipmac/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 13:32:46.000000 myipmacpackage-1.0.3/myipmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-08-08 13:32:46.000000 myipmacpackage-1.0.3/myipmac/fetcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:33:03.743238 myipmacpackage-1.0.3/myipmacpackage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      385 2023-08-09 05:33:03.000000 myipmacpackage-1.0.3/myipmacpackage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2023-08-09 05:33:03.000000 myipmacpackage-1.0.3/myipmacpackage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 05:33:03.000000 myipmacpackage-1.0.3/myipmacpackage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-09 05:33:03.000000 myipmacpackage-1.0.3/myipmacpackage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-09 05:33:03.000000 myipmacpackage-1.0.3/myipmacpackage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-09 05:33:03.743238 myipmacpackage-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      763 2023-08-09 05:32:30.000000 myipmacpackage-1.0.3/setup.py
```

### Comparing `myipmacpackage-1.0.2/myipmac/fetcher.py` & `myipmacpackage-1.0.3/myipmac/fetcher.py`

 * *Files identical despite different names*

### Comparing `myipmacpackage-1.0.2/setup.py` & `myipmacpackage-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import subprocess
 
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
-        subprocess.run(["python", "post_install.py"])
+        subprocess.run(["python3", "post_install.py"])
 
 setup(
     name="myipmacpackage",
-    version="1.0.2",
+    version="1.0.3",
     description="Fetch and store IP and MAC addresses in a database",
     author="Muneer",
     author_email="Muneer.moosa@electrifex.com",
     packages=find_packages(),
     install_requires=[
         "mysql-connector-python"
     ],
```

