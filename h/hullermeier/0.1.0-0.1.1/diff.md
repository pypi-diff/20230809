# Comparing `tmp/hullermeier-0.1.0.tar.gz` & `tmp/hullermeier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hullermeier-0.1.0.tar", max compression
+gzip compressed data, was "hullermeier-0.1.1.tar", max compression
```

## Comparing `hullermeier-0.1.0.tar` & `hullermeier-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2023-07-16 20:05:10.484807 hullermeier-0.1.0/LICENSE
--rw-r--r--   0        0        0       41 2023-07-16 20:30:27.274826 hullermeier-0.1.0/README.md
--rw-r--r--   0        0        0      436 2023-07-16 20:11:12.095325 hullermeier-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      530 2023-07-16 20:34:07.443727 hullermeier-0.1.0/src/hullermeier.py
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 hullermeier-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-16 20:05:10.484807 hullermeier-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1313 2023-08-08 01:50:50.389477 hullermeier-0.1.1/README.md
+-rw-r--r--   0        0        0      436 2023-08-08 01:51:24.259238 hullermeier-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      530 2023-07-16 20:34:07.443727 hullermeier-0.1.1/src/hullermeier.py
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 hullermeier-0.1.1/PKG-INFO
```

### Comparing `hullermeier-0.1.0/LICENSE` & `hullermeier-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hullermeier-0.1.0/src/hullermeier.py` & `hullermeier-0.1.1/src/hullermeier.py`

 * *Files identical despite different names*

