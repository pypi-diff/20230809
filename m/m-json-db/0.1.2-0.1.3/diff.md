# Comparing `tmp/m_json_db-0.1.2.tar.gz` & `tmp/m_json_db-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_json_db-0.1.2.tar", max compression
+gzip compressed data, was "m_json_db-0.1.3.tar", max compression
```

## Comparing `m_json_db-0.1.2.tar` & `m_json_db-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      566 2023-08-08 23:40:15.197203 m_json_db-0.1.2/m_json_db/__init__.py
--rw-r--r--   0        0        0      286 2023-08-08 23:40:31.917124 m_json_db-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      499 2023-08-08 23:40:43.580162 m_json_db-0.1.2/setup.py
--rw-r--r--   0        0        0      346 2023-08-08 23:40:43.580336 m_json_db-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      566 2023-08-08 23:40:15.197203 m_json_db-0.1.3/m_json_db/__init__.py
+-rw-r--r--   0        0        0      286 2023-08-08 23:43:06.608395 m_json_db-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      499 2023-08-08 23:43:31.852112 m_json_db-0.1.3/setup.py
+-rw-r--r--   0        0        0      346 2023-08-08 23:43:31.852271 m_json_db-0.1.3/PKG-INFO
```

### Comparing `m_json_db-0.1.2/m_json_db/__init__.py` & `m_json_db-0.1.3/m_json_db/__init__.py`

 * *Files identical despite different names*

