# Comparing `tmp/python-dotenv-vault-0.6.2.tar.gz` & `tmp/python-dotenv-vault-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dotenv-vault-0.6.2.tar", last modified: Mon Aug  7 04:39:54 2023, max compression
+gzip compressed data, was "python-dotenv-vault-0.6.3.tar", last modified: Wed Aug  9 00:41:40 2023, max compression
```

## Comparing `python-dotenv-vault-0.6.2.tar` & `python-dotenv-vault-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:39:54.595458 python-dotenv-vault-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-08-07 04:39:54.591458 python-dotenv-vault-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 04:39:54.595458 python-dotenv-vault-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:39:54.591458 python-dotenv-vault-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:39:54.591458 python-dotenv-vault-0.6.2/src/dotenv_vault/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/src/dotenv_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/src/dotenv_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/src/dotenv_vault/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-07 04:39:36.000000 python-dotenv-vault-0.6.2/src/dotenv_vault/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:39:54.591458 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 04:39:54.000000 python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:41:40.805733 python-dotenv-vault-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-08-09 00:41:40.805733 python-dotenv-vault-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 00:41:40.805733 python-dotenv-vault-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:41:40.801732 python-dotenv-vault-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:41:40.805733 python-dotenv-vault-0.6.3/src/dotenv_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/src/dotenv_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/src/dotenv_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/src/dotenv_vault/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-09 00:41:14.000000 python-dotenv-vault-0.6.3/src/dotenv_vault/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:41:40.805733 python-dotenv-vault-0.6.3/src/python_dotenv_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-08-09 00:41:40.000000 python-dotenv-vault-0.6.3/src/python_dotenv_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-09 00:41:40.000000 python-dotenv-vault-0.6.3/src/python_dotenv_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:41:40.000000 python-dotenv-vault-0.6.3/src/python_dotenv_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-09 00:41:40.000000 python-dotenv-vault-0.6.3/src/python_dotenv_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-09 00:41:40.000000 python-dotenv-vault-0.6.3/src/python_dotenv_vault.egg-info/top_level.txt
```

### Comparing `python-dotenv-vault-0.6.2/CHANGELOG.md` & `python-dotenv-vault-0.6.3/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.3
+
+### Changed
+
+- Fixed a bug where it was looking up .env instead of .env.vault [#18](https://github.com/dotenv-org/python-dotenv-vault/pull/18)
+
 ## 0.6.2
 
 ### Changed
 
 - Look for .env.vault file at same location as .env file. Finds .env file anywhere in app (just like original python lib) [#13](https://github.com/dotenv-org/python-dotenv-vault/pull/13)
 
 ## 0.6.1
```

### Comparing `python-dotenv-vault-0.6.2/LICENSE` & `python-dotenv-vault-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.2/PKG-INFO` & `python-dotenv-vault-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.6.2
+Version: 0.6.3
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
@@ -172,14 +172,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.3
+
+### Changed
+
+- Fixed a bug where it was looking up .env instead of .env.vault [#18](https://github.com/dotenv-org/python-dotenv-vault/pull/18)
+
 ## 0.6.2
 
 ### Changed
 
 - Look for .env.vault file at same location as .env file. Finds .env file anywhere in app (just like original python lib) [#13](https://github.com/dotenv-org/python-dotenv-vault/pull/13)
 
 ## 0.6.1
```

### Comparing `python-dotenv-vault-0.6.2/README.md` & `python-dotenv-vault-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.2/setup.py` & `python-dotenv-vault-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.2/src/dotenv_vault/main.py` & `python-dotenv-vault-0.6.3/src/dotenv_vault/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 from cryptography.exceptions import InvalidTag
 import dotenv.main as dotenv
 
 logger = logging.getLogger(__name__)
 
 def load_dotenv_vault() -> str:
-    path = dotenv.find_dotenv()
+    path = dotenv.find_dotenv(filename=".env.vault", usecwd=True)
     if not path:
         return path
     path = os.path.dirname(path)
     if '.env.vault' not in os.listdir(path):
         # we fall back to .env
         logger.warning(f"You set DOTENV_KEY but you are missing a .env.vault file at {path}. Did you forget to build it?")
         return f"{path}/.env"
```

### Comparing `python-dotenv-vault-0.6.2/src/dotenv_vault/test_vault.py` & `python-dotenv-vault-0.6.3/src/dotenv_vault/test_vault.py`

 * *Files identical despite different names*

### Comparing `python-dotenv-vault-0.6.2/src/python_dotenv_vault.egg-info/PKG-INFO` & `python-dotenv-vault-0.6.3/src/python_dotenv_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dotenv-vault
-Version: 0.6.2
+Version: 0.6.3
 Summary: Decrypt .env.vault file.
 Home-page: https://github.com/dotenv-org/python-dotenv-vault
 Author: dotenv
 Author-email: mot@dotenv.org
 License: MIT
 Keywords: environment,environment variables,deployments,settings,env,dotenv,configurations,python,dotenv-vault
 Description-Content-Type: text/markdown
@@ -172,14 +172,20 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
 ## [Unreleased](https://github.com/dotenv-org/python-dotenv-vault/compare/v0.5.1...master)
 
+## 0.6.3
+
+### Changed
+
+- Fixed a bug where it was looking up .env instead of .env.vault [#18](https://github.com/dotenv-org/python-dotenv-vault/pull/18)
+
 ## 0.6.2
 
 ### Changed
 
 - Look for .env.vault file at same location as .env file. Finds .env file anywhere in app (just like original python lib) [#13](https://github.com/dotenv-org/python-dotenv-vault/pull/13)
 
 ## 0.6.1
```

