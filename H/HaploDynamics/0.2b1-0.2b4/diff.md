# Comparing `tmp/HaploDynamics-0.2b1.tar.gz` & `tmp/HaploDynamics-0.2b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaploDynamics-0.2b1.tar", last modified: Mon Aug  7 04:52:07 2023, max compression
+gzip compressed data, was "HaploDynamics-0.2b4.tar", last modified: Wed Aug  9 04:54:42 2023, max compression
```

## Comparing `HaploDynamics-0.2b1.tar` & `HaploDynamics-0.2b4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:52:07.783050 HaploDynamics-0.2b1/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:52:07.783050 HaploDynamics-0.2b1/HaploDynamics/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:52:07.783050 HaploDynamics-0.2b1/HaploDynamics/Framework/
--rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-07 04:51:52.000000 HaploDynamics-0.2b1/HaploDynamics/Framework/__init__.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-07 04:51:52.000000 HaploDynamics-0.2b1/HaploDynamics/Framework/future.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:52:07.783050 HaploDynamics-0.2b1/HaploDynamics/HaploDX/
--rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-07 04:51:52.000000 HaploDynamics-0.2b1/HaploDynamics/HaploDX/HaploDX.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-07 04:51:52.000000 HaploDynamics-0.2b1/HaploDynamics/HaploDX/__init__.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       60 2023-08-07 04:51:52.000000 HaploDynamics-0.2b1/HaploDynamics/__init__.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:52:07.783050 HaploDynamics-0.2b1/HaploDynamics.egg-info/
--rw-rw-r--   0 remy      (1000) remy      (1000)    11082 2023-08-07 04:52:07.000000 HaploDynamics-0.2b1/HaploDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)      383 2023-08-07 04:52:07.000000 HaploDynamics-0.2b1/HaploDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 04:52:07.000000 HaploDynamics-0.2b1/HaploDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-07 04:52:07.000000 HaploDynamics-0.2b1/HaploDynamics.egg-info/requires.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)       14 2023-08-07 04:52:07.000000 HaploDynamics-0.2b1/HaploDynamics.egg-info/top_level.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-07 04:51:52.000000 HaploDynamics-0.2b1/LICENSE
--rw-rw-r--   0 remy      (1000) remy      (1000)    11082 2023-08-07 04:52:07.783050 HaploDynamics-0.2b1/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)    10198 2023-08-07 04:51:52.000000 HaploDynamics-0.2b1/README.md
--rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-07 04:52:07.783050 HaploDynamics-0.2b1/setup.cfg
--rw-rw-r--   0 remy      (1000) remy      (1000)     1257 2023-08-07 04:51:52.000000 HaploDynamics-0.2b1/setup.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-09 04:54:42.770020 HaploDynamics-0.2b4/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-09 04:54:42.770020 HaploDynamics-0.2b4/HaploDynamics/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-09 04:54:42.770020 HaploDynamics-0.2b4/HaploDynamics/Framework/
+-rw-rw-r--   0 remy      (1000) remy      (1000)       25 2023-08-08 20:50:46.000000 HaploDynamics-0.2b4/HaploDynamics/Framework/__init__.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)      648 2023-08-08 21:38:55.000000 HaploDynamics-0.2b4/HaploDynamics/Framework/multiproc.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-09 04:54:42.770020 HaploDynamics-0.2b4/HaploDynamics/HaploDX/
+-rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-08 17:10:32.000000 HaploDynamics-0.2b4/HaploDynamics/HaploDX/HaploDX.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-08 17:10:32.000000 HaploDynamics-0.2b4/HaploDynamics/HaploDX/__init__.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       60 2023-08-08 17:10:32.000000 HaploDynamics-0.2b4/HaploDynamics/__init__.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-09 04:54:42.770020 HaploDynamics-0.2b4/HaploDynamics.egg-info/
+-rw-rw-r--   0 remy      (1000) remy      (1000)    21349 2023-08-09 04:54:42.000000 HaploDynamics-0.2b4/HaploDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)      386 2023-08-09 04:54:42.000000 HaploDynamics-0.2b4/HaploDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-09 04:54:42.000000 HaploDynamics-0.2b4/HaploDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-09 04:54:42.000000 HaploDynamics-0.2b4/HaploDynamics.egg-info/requires.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)       14 2023-08-09 04:54:42.000000 HaploDynamics-0.2b4/HaploDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-08 17:10:32.000000 HaploDynamics-0.2b4/LICENSE
+-rw-rw-r--   0 remy      (1000) remy      (1000)    21349 2023-08-09 04:54:42.770020 HaploDynamics-0.2b4/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)    20465 2023-08-09 04:49:59.000000 HaploDynamics-0.2b4/README.md
+-rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-09 04:54:42.770020 HaploDynamics-0.2b4/setup.cfg
+-rw-rw-r--   0 remy      (1000) remy      (1000)     1257 2023-08-09 04:49:10.000000 HaploDynamics-0.2b4/setup.py
```

### Comparing `HaploDynamics-0.2b1/HaploDynamics/HaploDX/HaploDX.py` & `HaploDynamics-0.2b4/HaploDynamics/HaploDX/HaploDX.py`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.2b1/LICENSE` & `HaploDynamics-0.2b4/LICENSE`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.2b1/setup.py` & `HaploDynamics-0.2b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'HaploDynamics',
   packages=setuptools.find_packages(include=['HaploDynamics','HaploDynamics.HaploDX','HaploDynamics.Framework']),
-  version = 'v0.2-beta.1',
+  version = 'v0.2-beta.4',
   license='gpl-3.0',
   author = 'Remy Tuyeras',
   author_email = 'rtuyeras@gmail.com',
   description = 'A python library to develop genomic data simulators',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = 'https://github.com/remytuyeras/HaploDynamics',
-  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.2-beta.1.tar.gz',
+  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.2-beta.4.tar.gz',
   keywords = ['Simulator', 'Genomics', 'Genomic', 'Microarray','SNP chip','VCF', 'Linkage disequilibrium', 'Hardy-Weinberg equilibrium'],
   install_requires=['scipy'],
   classifiers=[
     'Development Status :: 4 - Beta',  #"3 - Alpha", "4 - Beta" or "5 - Production/Stable"
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
```

