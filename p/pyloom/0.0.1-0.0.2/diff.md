# Comparing `tmp/pyloom-0.0.1.tar.gz` & `tmp/pyloom-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloom-0.0.1.tar", max compression
+gzip compressed data, was "pyloom-0.0.2.tar", max compression
```

## Comparing `pyloom-0.0.1.tar` & `pyloom-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0       22 2023-07-23 17:04:15.217706 pyloom-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-23 16:25:55.886743 pyloom-0.0.1/pyloom/__init__.py
--rw-r--r--   0        0        0       57 2023-07-23 16:29:08.939817 pyloom-0.0.1/pyloom/hello.py
--rw-r--r--   0        0        0      265 2023-07-23 17:25:49.839803 pyloom-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 pyloom-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-09 02:49:52.650371 pyloom-0.0.2/LICENSE
+-rw-r--r--   0        0        0       13 2023-08-09 02:49:52.650649 pyloom-0.0.2/README.md
+-rw-r--r--   0        0        0       89 2023-08-09 02:13:36.489300 pyloom-0.0.2/pyloom/__init__.py
+-rw-r--r--   0        0        0      695 2023-08-09 01:47:31.306731 pyloom-0.0.2/pyloom/class_resolver.py
+-rw-r--r--   0        0        0    22506 2023-08-09 02:15:01.010925 pyloom-0.0.2/pyloom/thread.py
+-rw-r--r--   0        0        0     4357 2023-08-09 02:12:19.620972 pyloom-0.0.2/pyloom/tree.py
+-rw-r--r--   0        0        0      435 2023-08-09 03:00:26.392259 pyloom-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 pyloom-0.0.2/PKG-INFO
```

