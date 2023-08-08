# Comparing `tmp/pybet-0.7.0.tar.gz` & `tmp/pybet-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybet-0.7.0.tar", max compression
+gzip compressed data, was "pybet-0.7.1.tar", max compression
```

## Comparing `pybet-0.7.0.tar` & `pybet-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.7.0/LICENSE
--rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.7.0/pybet/__init__.py
--rw-r--r--   0        0        0    10336 2023-08-08 21:26:36.954848 pybet-0.7.0/pybet/market.py
--rw-r--r--   0        0        0    11717 2023-06-12 22:15:51.544566 pybet-0.7.0/pybet/odds.py
--rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.7.0/pybet/staking/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-29 12:08:45.277280 pybet-0.7.0/pybet/staking/kelly.py
--rw-r--r--   0        0        0     1015 2023-08-08 21:26:36.954848 pybet-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.7.0/README.md
--rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.7.1/LICENSE
+-rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.7.1/pybet/__init__.py
+-rw-r--r--   0        0        0    10336 2023-08-08 21:26:36.954848 pybet-0.7.1/pybet/market.py
+-rw-r--r--   0        0        0    11717 2023-06-12 22:15:51.544566 pybet-0.7.1/pybet/odds.py
+-rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.7.1/pybet/staking/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-29 12:08:45.277280 pybet-0.7.1/pybet/staking/kelly.py
+-rw-r--r--   0        0        0     1023 2023-08-08 22:17:27.163206 pybet-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.7.1/README.md
+-rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.7.1/PKG-INFO
```

### Comparing `pybet-0.7.0/LICENSE` & `pybet-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybet-0.7.0/pybet/market.py` & `pybet-0.7.1/pybet/market.py`

 * *Files identical despite different names*

### Comparing `pybet-0.7.0/pybet/odds.py` & `pybet-0.7.1/pybet/odds.py`

 * *Files identical despite different names*

### Comparing `pybet-0.7.0/pybet/staking/kelly.py` & `pybet-0.7.1/pybet/staking/kelly.py`

 * *Files identical despite different names*

### Comparing `pybet-0.7.0/pyproject.toml` & `pybet-0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybet"
-version = "0.7.0"
+version = "0.7.1"
 description = "A library of betting utilities to assist with calculation of bets, stakes and markets"
 license = "GPL-3.0-only"
 authors = ["Robert Peacock <robertjamespeacock@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/peaky76/pybet"
 documentation = "https://pybet.readthedocs.io/"
 keywords = ["betting", "gambling"]
@@ -25,13 +25,13 @@
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 ruff = ">=0.0.265,<0.0.283"
 sphinx = ">=6.1.3,<8.0.0"
 sphinx-rtd-theme = "^1.2.0"
 
 [tool.ruff]
-ignore = ["E501", "F821"]
+ignore = ["E501", "E731", "F821"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pybet-0.7.0/README.md` & `pybet-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pybet-0.7.0/PKG-INFO` & `pybet-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybet
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library of betting utilities to assist with calculation of bets, stakes and markets
 Home-page: https://github.com/peaky76/pybet
 License: GPL-3.0-only
 Keywords: betting,gambling
 Author: Robert Peacock
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
```

