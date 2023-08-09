# Comparing `tmp/wandb-core-alpha-0.0.1a2.tar.gz` & `tmp/wandb-core-alpha-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wandb-core-alpha-0.0.1a2.tar", last modified: Mon Jul 31 12:40:56 2023, max compression
+gzip compressed data, was "wandb-core-alpha-0.0.1a3.tar", last modified: Wed Aug  9 04:49:46 2023, max compression
```

## Comparing `wandb-core-alpha-0.0.1a2.tar` & `wandb-core-alpha-0.0.1a3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-31 12:40:56.158354 wandb-core-alpha-0.0.1a2/
--rw-r--r--   0 jeff       (501) staff       (20)       58 2023-07-18 10:51:23.000000 wandb-core-alpha-0.0.1a2/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)      126 2023-07-31 12:40:56.158208 wandb-core-alpha-0.0.1a2/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)        0 2023-07-21 14:16:15.000000 wandb-core-alpha-0.0.1a2/pyproject.toml
--rw-r--r--   0 jeff       (501) staff       (20)       38 2023-07-31 12:40:56.158402 wandb-core-alpha-0.0.1a2/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)     4095 2023-07-31 12:36:47.000000 wandb-core-alpha-0.0.1a2/setup.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-31 12:40:56.157244 wandb-core-alpha-0.0.1a2/wandb_core/
--rw-r--r--   0 jeff       (501) staff       (20)      308 2023-07-18 10:51:23.000000 wandb-core-alpha-0.0.1a2/wandb_core/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-31 12:40:56.157991 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)      126 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      257 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/not-zip-safe
--rw-r--r--   0 jeff       (501) staff       (20)       11 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-08-09 04:49:46.180261 wandb-core-alpha-0.0.1a3/
+-rw-r--r--   0 jeff       (501) staff       (20)       58 2023-08-09 01:18:39.000000 wandb-core-alpha-0.0.1a3/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)      126 2023-08-09 04:49:46.180111 wandb-core-alpha-0.0.1a3/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2023-08-09 01:18:39.000000 wandb-core-alpha-0.0.1a3/pyproject.toml
+-rw-r--r--   0 jeff       (501) staff       (20)       38 2023-08-09 04:49:46.180315 wandb-core-alpha-0.0.1a3/setup.cfg
+-rw-r--r--   0 jeff       (501) staff       (20)     4094 2023-08-09 04:40:57.000000 wandb-core-alpha-0.0.1a3/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-08-09 04:49:46.178674 wandb-core-alpha-0.0.1a3/wandb_core/
+-rw-r--r--   0 jeff       (501) staff       (20)      309 2023-08-09 04:40:38.000000 wandb-core-alpha-0.0.1a3/wandb_core/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-08-09 04:49:46.179891 wandb-core-alpha-0.0.1a3/wandb_core_alpha.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)      126 2023-08-09 04:49:46.000000 wandb-core-alpha-0.0.1a3/wandb_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      257 2023-08-09 04:49:46.000000 wandb-core-alpha-0.0.1a3/wandb_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-08-09 04:49:46.000000 wandb-core-alpha-0.0.1a3/wandb_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-08-09 04:49:46.000000 wandb-core-alpha-0.0.1a3/wandb_core_alpha.egg-info/not-zip-safe
+-rw-r--r--   0 jeff       (501) staff       (20)       11 2023-08-09 04:49:46.000000 wandb-core-alpha-0.0.1a3/wandb_core_alpha.egg-info/top_level.txt
```

### Comparing `wandb-core-alpha-0.0.1a2/setup.py` & `wandb-core-alpha-0.0.1a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from setuptools import setup
 from setuptools.command.develop import develop
 
 # from distutils.command.bdist import bdist
 from wheel.bdist_wheel import bdist_wheel
 
-
 # Package naming
 # --------------
 #   wandb-core:         Package containing architecture specific code
 #   wandb-core-nightly: Package created every night based on main branch
 #   wandb-core-alpha:   Package used during early development
 _WANDB_CORE_ALPHA_ENV = "WANDB_CORE_ALPHA"
 _is_wandb_core_alpha = bool(os.environ.get(_WANDB_CORE_ALPHA_ENV))
@@ -126,15 +125,15 @@
 
     def run(self):
         bdist_wheel.run(self)
 
 
 setup(
     name="wandb-core" if not _is_wandb_core_alpha else "wandb-core-alpha",
-    version="0.0.1a2",
+    version="0.0.1a3",
     description="Wandb core",
     packages=[PACKAGE],
     zip_safe=False,
     include_package_data=True,
     license="MIT license",
     python_requires=">=3.6",
     cmdclass={
```

