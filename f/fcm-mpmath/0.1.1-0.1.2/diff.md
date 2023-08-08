# Comparing `tmp/fcm_mpmath-0.1.1.tar.gz` & `tmp/fcm_mpmath-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcm_mpmath-0.1.1.tar", max compression
+gzip compressed data, was "fcm_mpmath-0.1.2.tar", max compression
```

## Comparing `fcm_mpmath-0.1.1.tar` & `fcm_mpmath-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2023-07-16 20:04:58.492673 fcm_mpmath-0.1.1/LICENSE
--rw-r--r--   0        0        0       27 2023-07-16 20:56:20.100495 fcm_mpmath-0.1.1/README.md
--rw-r--r--   0        0        0      396 2023-07-16 20:57:20.095017 fcm_mpmath-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5007 2023-07-16 20:34:11.755746 fcm_mpmath-0.1.1/src/fcm_mpmath.py
--rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 fcm_mpmath-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-16 20:04:58.492673 fcm_mpmath-0.1.2/LICENSE
+-rw-r--r--   0        0        0      942 2023-08-08 01:41:53.213008 fcm_mpmath-0.1.2/README.md
+-rw-r--r--   0        0        0      396 2023-08-08 01:42:39.722365 fcm_mpmath-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5007 2023-07-16 20:34:11.755746 fcm_mpmath-0.1.2/src/fcm_mpmath.py
+-rw-r--r--   0        0        0     1412 1970-01-01 00:00:00.000000 fcm_mpmath-0.1.2/PKG-INFO
```

### Comparing `fcm_mpmath-0.1.1/LICENSE` & `fcm_mpmath-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fcm_mpmath-0.1.1/src/fcm_mpmath.py` & `fcm_mpmath-0.1.2/src/fcm_mpmath.py`

 * *Files identical despite different names*

