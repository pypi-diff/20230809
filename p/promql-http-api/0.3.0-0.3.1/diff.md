# Comparing `tmp/promql_http_api-0.3.0.tar.gz` & `tmp/promql_http_api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promql_http_api-0.3.0.tar", max compression
+gzip compressed data, was "promql_http_api-0.3.1.tar", max compression
```

## Comparing `promql_http_api-0.3.0.tar` & `promql_http_api-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    10764 2023-01-27 09:07:19.549411 promql_http_api-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     7248 2023-08-08 03:23:49.919661 promql_http_api-0.3.0/README.md
--rw-r--r--   0        0        0      746 2023-01-27 09:07:19.565408 promql_http_api-0.3.0/promql_http_api/__init__.py
--rw-r--r--   0        0        0     1049 2023-01-27 09:07:19.816418 promql_http_api-0.3.0/promql_http_api/alerts.py
--rw-r--r--   0        0        0     1070 2023-01-27 09:07:19.833422 promql_http_api-0.3.0/promql_http_api/alertsmanagers.py
--rw-r--r--   0        0        0     3555 2023-07-11 00:34:11.623046 promql_http_api-0.3.0/promql_http_api/api.py
--rw-r--r--   0        0        0     1724 2023-01-27 09:07:19.827419 promql_http_api-0.3.0/promql_http_api/api_endpoint.py
--rw-r--r--   0        0        0     4527 2023-03-31 07:15:17.659745 promql_http_api-0.3.0/promql_http_api/api_response.py
--rw-r--r--   0        0        0     1065 2023-01-27 09:07:19.831419 promql_http_api-0.3.0/promql_http_api/buildinfo.py
--rw-r--r--   0        0        0     1056 2023-01-27 09:07:19.829418 promql_http_api-0.3.0/promql_http_api/config.py
--rw-r--r--   0        0        0     1053 2023-01-27 09:07:19.850430 promql_http_api-0.3.0/promql_http_api/flags.py
--rw-r--r--   0        0        0     1190 2023-01-27 09:07:19.812420 promql_http_api-0.3.0/promql_http_api/format_query.py
--rw-r--r--   0        0        0       44 2023-07-08 03:05:34.339332 promql_http_api-0.3.0/promql_http_api/http_config.py
--rw-r--r--   0        0        0     1344 2023-01-27 09:37:30.210288 promql_http_api-0.3.0/promql_http_api/label_values.py
--rw-r--r--   0        0        0     1068 2023-01-27 09:37:38.611318 promql_http_api-0.3.0/promql_http_api/labels.py
--rw-r--r--   0        0        0     7417 2023-08-07 20:29:26.630663 promql_http_api-0.3.0/promql_http_api/query.py
--rw-r--r--   0        0        0     1246 2023-01-27 09:07:19.818421 promql_http_api-0.3.0/promql_http_api/rules.py
--rw-r--r--   0        0        0     1071 2023-01-27 09:07:19.840413 promql_http_api-0.3.0/promql_http_api/runtimeinfo.py
--rw-r--r--   0        0        0     1497 2023-01-27 09:33:47.634307 promql_http_api-0.3.0/promql_http_api/series.py
--rw-r--r--   0        0        0     1257 2023-01-27 09:07:19.825417 promql_http_api-0.3.0/promql_http_api/targets.py
--rw-r--r--   0        0        0     1209 2023-08-08 03:25:26.738878 promql_http_api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8394 1970-01-01 00:00:00.000000 promql_http_api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10764 2023-01-27 09:07:19.549411 promql_http_api-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     7248 2023-08-08 03:23:49.919661 promql_http_api-0.3.1/README.md
+-rw-r--r--   0        0        0      746 2023-01-27 09:07:19.565408 promql_http_api-0.3.1/promql_http_api/__init__.py
+-rw-r--r--   0        0        0     1049 2023-01-27 09:07:19.816418 promql_http_api-0.3.1/promql_http_api/alerts.py
+-rw-r--r--   0        0        0     1070 2023-01-27 09:07:19.833422 promql_http_api-0.3.1/promql_http_api/alertsmanagers.py
+-rw-r--r--   0        0        0     3555 2023-07-11 00:34:11.623046 promql_http_api-0.3.1/promql_http_api/api.py
+-rw-r--r--   0        0        0     1724 2023-01-27 09:07:19.827419 promql_http_api-0.3.1/promql_http_api/api_endpoint.py
+-rw-r--r--   0        0        0     4527 2023-03-31 07:15:17.659745 promql_http_api-0.3.1/promql_http_api/api_response.py
+-rw-r--r--   0        0        0     1065 2023-01-27 09:07:19.831419 promql_http_api-0.3.1/promql_http_api/buildinfo.py
+-rw-r--r--   0        0        0     1056 2023-01-27 09:07:19.829418 promql_http_api-0.3.1/promql_http_api/config.py
+-rw-r--r--   0        0        0     1053 2023-01-27 09:07:19.850430 promql_http_api-0.3.1/promql_http_api/flags.py
+-rw-r--r--   0        0        0     1190 2023-01-27 09:07:19.812420 promql_http_api-0.3.1/promql_http_api/format_query.py
+-rw-r--r--   0        0        0       44 2023-07-08 03:05:34.339332 promql_http_api-0.3.1/promql_http_api/http_config.py
+-rw-r--r--   0        0        0     1344 2023-01-27 09:37:30.210288 promql_http_api-0.3.1/promql_http_api/label_values.py
+-rw-r--r--   0        0        0     1068 2023-01-27 09:37:38.611318 promql_http_api-0.3.1/promql_http_api/labels.py
+-rw-r--r--   0        0        0     7417 2023-08-07 20:29:26.630663 promql_http_api-0.3.1/promql_http_api/query.py
+-rw-r--r--   0        0        0     1246 2023-01-27 09:07:19.818421 promql_http_api-0.3.1/promql_http_api/rules.py
+-rw-r--r--   0        0        0     1071 2023-01-27 09:07:19.840413 promql_http_api-0.3.1/promql_http_api/runtimeinfo.py
+-rw-r--r--   0        0        0     1497 2023-01-27 09:33:47.634307 promql_http_api-0.3.1/promql_http_api/series.py
+-rw-r--r--   0        0        0     1257 2023-01-27 09:07:19.825417 promql_http_api-0.3.1/promql_http_api/targets.py
+-rw-r--r--   0        0        0     1209 2023-08-09 02:17:37.113843 promql_http_api-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8394 1970-01-01 00:00:00.000000 promql_http_api-0.3.1/PKG-INFO
```

### Comparing `promql_http_api-0.3.0/LICENSE.md` & `promql_http_api-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/README.md` & `promql_http_api-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/__init__.py` & `promql_http_api-0.3.1/promql_http_api/__init__.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/alerts.py` & `promql_http_api-0.3.1/promql_http_api/alerts.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/alertsmanagers.py` & `promql_http_api-0.3.1/promql_http_api/alertsmanagers.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/api.py` & `promql_http_api-0.3.1/promql_http_api/api.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/api_endpoint.py` & `promql_http_api-0.3.1/promql_http_api/api_endpoint.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/api_response.py` & `promql_http_api-0.3.1/promql_http_api/api_response.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/buildinfo.py` & `promql_http_api-0.3.1/promql_http_api/buildinfo.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/config.py` & `promql_http_api-0.3.1/promql_http_api/config.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/flags.py` & `promql_http_api-0.3.1/promql_http_api/flags.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/format_query.py` & `promql_http_api-0.3.1/promql_http_api/format_query.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/label_values.py` & `promql_http_api-0.3.1/promql_http_api/label_values.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/labels.py` & `promql_http_api-0.3.1/promql_http_api/labels.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/query.py` & `promql_http_api-0.3.1/promql_http_api/query.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/rules.py` & `promql_http_api-0.3.1/promql_http_api/rules.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/runtimeinfo.py` & `promql_http_api-0.3.1/promql_http_api/runtimeinfo.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/series.py` & `promql_http_api-0.3.1/promql_http_api/series.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/promql_http_api/targets.py` & `promql_http_api-0.3.1/promql_http_api/targets.py`

 * *Files identical despite different names*

### Comparing `promql_http_api-0.3.0/pyproject.toml` & `promql_http_api-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promql-http-api"
-version = "0.3.0"
+version = "0.3.1"
 description = "Query a Prometheus server and get a Pandas DataFrame"
 homepage = "https://github.com/nir-arad/promql-http-api"
 repository = "https://github.com/nir-arad/promql-http-api"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["prometheus", "promql", "pandas", "dataframe"]
 authors = ["Nir Arad"]
```

### Comparing `promql_http_api-0.3.0/PKG-INFO` & `promql_http_api-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promql-http-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Query a Prometheus server and get a Pandas DataFrame
 Home-page: https://github.com/nir-arad/promql-http-api
 License: Apache-2.0
 Keywords: prometheus,promql,pandas,dataframe
 Author: Nir Arad
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

