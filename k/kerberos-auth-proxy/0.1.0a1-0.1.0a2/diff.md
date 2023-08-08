# Comparing `tmp/kerberos_auth_proxy-0.1.0a1.tar.gz` & `tmp/kerberos_auth_proxy-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerberos_auth_proxy-0.1.0a1.tar", max compression
+gzip compressed data, was "kerberos_auth_proxy-0.1.0a2.tar", max compression
```

## Comparing `kerberos_auth_proxy-0.1.0a1.tar` & `kerberos_auth_proxy-0.1.0a2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1075 2023-07-01 17:16:05.974247 kerberos_auth_proxy-0.1.0a1/LICENSE
--rw-r--r--   0        0        0       68 2023-07-01 17:13:15.814927 kerberos_auth_proxy-0.1.0a1/README.md
--rw-r--r--   0        0        0        0 2023-07-01 17:13:15.814927 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 19:42:12.010594 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/__init__.py
--rw-r--r--   0        0        0     2963 2023-07-06 10:40:39.368152 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/addon.py
--rw-r--r--   0        0        0     1520 2023-07-06 10:44:52.213364 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/auth.py
--rw-r--r--   0        0        0        0 2023-07-03 22:09:06.654893 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/__init__.py
--rw-r--r--   0        0        0      760 2023-07-03 22:15:14.534627 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/base.py
--rw-r--r--   0        0        0     3805 2023-07-05 16:18:00.380638 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/hosts.py
--rw-r--r--   0        0        0     5807 2023-07-05 09:09:36.660046 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/kerberos.py
--rw-r--r--   0        0        0     8478 2023-07-05 16:19:25.493892 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/hostutils.py
--rw-r--r--   0        0        0     1385 2023-07-04 16:06:59.191830 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/utils.py
--rw-r--r--   0        0        0      747 2023-07-31 13:30:39.429283 kerberos_auth_proxy-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 kerberos_auth_proxy-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-01 17:16:05.974247 kerberos_auth_proxy-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0       68 2023-07-01 17:13:15.814927 kerberos_auth_proxy-0.1.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 17:13:15.814927 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 19:42:12.010594 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/__init__.py
+-rw-r--r--   0        0        0     2963 2023-07-06 10:40:39.368152 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/addon.py
+-rw-r--r--   0        0        0     1520 2023-07-06 10:44:52.213364 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/auth.py
+-rw-r--r--   0        0        0        0 2023-07-03 22:09:06.654893 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/filters/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-03 22:15:14.534627 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/filters/base.py
+-rw-r--r--   0        0        0     3805 2023-07-05 16:18:00.380638 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/filters/hosts.py
+-rw-r--r--   0        0        0     5807 2023-07-05 09:09:36.660046 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/filters/kerberos.py
+-rw-r--r--   0        0        0     8478 2023-07-05 16:19:25.493892 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/hostutils.py
+-rw-r--r--   0        0        0     1385 2023-07-04 16:06:59.191830 kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/utils.py
+-rw-r--r--   0        0        0      747 2023-08-08 22:28:35.289397 kerberos_auth_proxy-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 kerberos_auth_proxy-0.1.0a2/PKG-INFO
```

### Comparing `kerberos_auth_proxy-0.1.0a1/LICENSE` & `kerberos_auth_proxy-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/addon.py` & `kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/addon.py`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/auth.py` & `kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/auth.py`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/base.py` & `kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/filters/base.py`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/hosts.py` & `kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/filters/hosts.py`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/kerberos.py` & `kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/filters/kerberos.py`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/hostutils.py` & `kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/mitm/hostutils.py`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/utils.py` & `kerberos_auth_proxy-0.1.0a2/kerberos_auth_proxy/utils.py`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a1/pyproject.toml` & `kerberos_auth_proxy-0.1.0a2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "kerberos-auth-proxy"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Proxy requests to Kerberos-enabled endpoints"
 authors = ["Diógenes Oliveira <diogenes1oliveira@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "kerberos_auth_proxy" }]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.6"
 mitmproxy = "^9.0"
 requests-gssapi = "^1.2"
 flask = "^2.2"
 aiohttp = "^3.8"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.1"
```

