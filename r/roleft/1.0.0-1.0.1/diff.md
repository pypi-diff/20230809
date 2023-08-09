# Comparing `tmp/roleft-1.0.0.tar.gz` & `tmp/roleft-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\roleft-1.0.0.tar", last modified: Tue May 15 07:20:06 2018, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `roleft-1.0.0.tar` & `roleft-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,25 @@
-drwxrwxrwx   0        0        0        0 2018-05-15 07:20:06.000000 roleft-1.0.0/
--rw-rw-rw-   0        0        0      287 2018-05-15 07:20:06.000000 roleft-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2018-05-15 07:20:06.000000 roleft-1.0.0/roleft.egg-info/
--rw-rw-rw-   0        0        0        1 2018-05-15 07:20:03.000000 roleft-1.0.0/roleft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      287 2018-05-15 07:20:03.000000 roleft-1.0.0/roleft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       20 2018-05-15 07:20:03.000000 roleft-1.0.0/roleft.egg-info/requires.txt
--rw-rw-rw-   0        0        0      157 2018-05-15 07:20:03.000000 roleft-1.0.0/roleft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2018-05-15 07:20:03.000000 roleft-1.0.0/roleft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2018-05-15 07:20:06.000000 roleft-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      470 2018-05-15 07:15:48.000000 roleft-1.0.0/setup.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 roleft-1.0.1/main.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 roleft-1.0.1/setup.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 roleft-1.0.1/test_1.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 roleft-1.0.1/test_2.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 roleft-1.0.1/test_2copy.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 roleft-1.0.1/test_3.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 roleft-1.0.1/test_4.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 roleft-1.0.1/test_5.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 roleft-1.0.1/test_6.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 roleft-1.0.1/test_7.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 roleft-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 roleft-1.0.1/KeyText/__init__.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 roleft-1.0.1/Modules/__init__.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 roleft-1.0.1/Utilities/AU.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 roleft-1.0.1/Utilities/CU.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 roleft-1.0.1/Utilities/HU.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 roleft-1.0.1/Utilities/ListU.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 roleft-1.0.1/Utilities/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 roleft-1.0.1/roleft/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 roleft-1.0.1/roleft/entry.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 roleft-1.0.1/xDictDefs/__init__.py
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 roleft-1.0.1/xListDefs/__init__.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 roleft-1.0.1/.gitignore
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 roleft-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 roleft-1.0.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

