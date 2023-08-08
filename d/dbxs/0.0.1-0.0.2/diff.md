# Comparing `tmp/dbxs-0.0.1.tar.gz` & `tmp/dbxs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxs-0.0.1.tar", last modified: Fri Jun  2 06:35:36 2023, max compression
+gzip compressed data, was "dbxs-0.0.2.tar", last modified: Tue Aug  8 23:08:30 2023, max compression
```

## Comparing `dbxs-0.0.1.tar` & `dbxs-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,42 @@
-drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-06-02 06:35:36.529223 dbxs-0.0.1/
--rw-r--r--   0 glyph      (501) staff       (20)      170 2023-06-02 06:35:36.529119 dbxs-0.0.1/PKG-INFO
-drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-06-02 06:35:36.528987 dbxs-0.0.1/dbxs.egg-info/
--rw-r--r--   0 glyph      (501) staff       (20)      170 2023-06-02 06:35:36.000000 dbxs-0.0.1/dbxs.egg-info/PKG-INFO
--rw-r--r--   0 glyph      (501) staff       (20)      120 2023-06-02 06:35:36.000000 dbxs-0.0.1/dbxs.egg-info/SOURCES.txt
--rw-r--r--   0 glyph      (501) staff       (20)        1 2023-06-02 06:35:36.000000 dbxs-0.0.1/dbxs.egg-info/dependency_links.txt
--rw-r--r--   0 glyph      (501) staff       (20)        1 2023-06-02 06:35:36.000000 dbxs-0.0.1/dbxs.egg-info/top_level.txt
--rw-r--r--   0 glyph      (501) staff       (20)       38 2023-06-02 06:35:36.529254 dbxs-0.0.1/setup.cfg
--rw-r--r--   0 glyph      (501) staff       (20)      272 2023-06-02 06:35:02.000000 dbxs-0.0.1/setup.py
+-rw-r--r--   0        0        0      276 2023-08-08 06:36:49.893389 dbxs-0.0.2/.coveragerc
+-rw-r--r--   0        0        0     1852 2023-08-08 07:24:45.936231 dbxs-0.0.2/.flake8
+-rw-r--r--   0        0        0      431 2023-08-08 07:27:04.041532 dbxs-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     8242 2023-08-08 07:32:56.766360 dbxs-0.0.2/.github/workflows/cicd.yml
+-rw-r--r--   0        0        0      122 2023-08-08 07:13:13.071351 dbxs-0.0.2/.gitignore
+-rw-r--r--   0        0        0      428 2023-08-08 07:07:24.579066 dbxs-0.0.2/.isort.cfg
+-rw-r--r--   0        0        0     2721 2023-08-08 07:09:12.395270 dbxs-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      825 2023-08-08 19:59:25.652036 dbxs-0.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1098 2023-08-08 06:33:16.482723 dbxs-0.0.2/LICENSE
+-rw-r--r--   0        0        0       38 2023-08-08 07:03:40.836668 dbxs-0.0.2/README.md
+-rw-r--r--   0        0        0      634 2023-08-08 07:06:45.051470 dbxs-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0      925 2023-08-08 07:07:56.727571 dbxs-0.0.2/docs/conf.py
+-rw-r--r--   0        0        0      426 2023-08-08 07:21:18.314151 dbxs-0.0.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-08-08 07:06:45.052283 dbxs-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0     1416 2023-08-08 07:12:11.964813 dbxs-0.0.2/mypy.ini
+-rw-r--r--   0        0        0      453 2023-08-08 06:57:24.104765 dbxs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-08-08 06:24:04.578247 dbxs-0.0.2/requirements/black.txt
+-rw-r--r--   0        0        0       16 2023-08-08 06:24:04.578540 dbxs-0.0.2/requirements/coverage.txt
+-rw-r--r--   0        0        0       28 2023-08-08 06:24:04.578723 dbxs-0.0.2/requirements/docs-auto.txt
+-rw-r--r--   0        0        0       69 2023-08-08 19:59:52.300245 dbxs-0.0.2/requirements/mypy.txt
+-rw-r--r--   0        0        0       35 2023-08-08 06:24:04.579073 dbxs-0.0.2/requirements/packaging.txt
+-rw-r--r--   0        0        0       18 2023-08-08 06:24:04.579229 dbxs-0.0.2/requirements/pre-commit.txt
+-rw-r--r--   0        0        0       18 2023-08-08 06:24:04.579435 dbxs-0.0.2/requirements/pyupgrade.txt
+-rw-r--r--   0        0        0       74 2023-08-08 06:24:04.579622 dbxs-0.0.2/requirements/release.txt
+-rw-r--r--   0        0        0       38 2023-08-08 06:24:04.579777 dbxs-0.0.2/requirements/sphinx.txt
+-rw-r--r--   0        0        0      156 2023-08-08 06:36:08.178130 dbxs-0.0.2/requirements/tox-pin-base.txt
+-rw-r--r--   0        0        0       23 2023-08-08 06:24:04.580110 dbxs-0.0.2/requirements/tox-tests.txt
+-rw-r--r--   0        0        0      664 2023-08-08 23:06:56.616359 dbxs-0.0.2/src/dbxs/__init__.py
+-rw-r--r--   0        0        0     8429 2023-08-08 07:07:58.541586 dbxs-0.0.2/src/dbxs/_access.py
+-rw-r--r--   0        0        0     2277 2023-08-08 07:07:58.542475 dbxs-0.0.2/src/dbxs/_dbapi_async_protocols.py
+-rw-r--r--   0        0        0    11118 2023-08-08 07:07:58.544837 dbxs-0.0.2/src/dbxs/_dbapi_async_twisted.py
+-rw-r--r--   0        0        0     1371 2023-08-08 07:07:58.545384 dbxs-0.0.2/src/dbxs/_dbapi_types.py
+-rw-r--r--   0        0        0     4277 2023-08-08 06:38:58.373868 dbxs-0.0.2/src/dbxs/_testing.py
+-rw-r--r--   0        0        0      917 2023-08-08 07:07:58.548082 dbxs-0.0.2/src/dbxs/_typing_compat.py
+-rw-r--r--   0        0        0      433 2023-08-08 07:07:58.548936 dbxs-0.0.2/src/dbxs/dbapi_async.py
+-rw-r--r--   0        0        0      224 2023-08-08 07:07:58.549526 dbxs-0.0.2/src/dbxs/dbapi_sync.py
+-rw-r--r--   0        0        0        0 2023-08-08 06:17:21.310283 dbxs-0.0.2/src/dbxs/test/__init__.py
+-rw-r--r--   0        0        0     6587 2023-08-08 07:07:58.551326 dbxs-0.0.2/src/dbxs/test/test_access.py
+-rw-r--r--   0        0        0    18465 2023-08-08 07:07:58.554928 dbxs-0.0.2/src/dbxs/test/test_sync_adapter.py
+-rw-r--r--   0        0        0      295 2023-08-08 07:07:58.555662 dbxs-0.0.2/src/dbxs/testing.py
+-rw-r--r--   0        0        0     5103 2023-08-08 06:56:09.064167 dbxs-0.0.2/tox.ini
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 dbxs-0.0.2/PKG-INFO
```

