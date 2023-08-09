# Comparing `tmp/nonebot_plugin_jx3-0.5.8.tar.gz` & `tmp/nonebot_plugin_jx3-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_jx3-0.5.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_jx3-0.5.9.tar", max compression
```

## Comparing `nonebot_plugin_jx3-0.5.8.tar` & `nonebot_plugin_jx3-0.5.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-08-08 17:41:12.049341 nonebot_plugin_jx3-0.5.8/LICENSE
--rw-r--r--   0        0        0    13458 2023-07-27 16:21:18.061796 nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/__init__.py
--rw-r--r--   0        0        0     1812 2023-07-27 16:00:09.609228 nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/bind.py
--rw-r--r--   0        0        0      208 2023-07-27 15:47:54.064672 nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/config.py
--rw-r--r--   0        0        0     3645 2023-07-18 11:30:59.000000 nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/subscribe.py
--rw-r--r--   0        0        0     2835 2023-08-09 04:34:31.942844 nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/userdefine.py
--rw-r--r--   0        0        0    11112 2023-07-27 15:49:48.852411 nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/websocket_handler.py
--rw-r--r--   0        0        0      594 2023-08-09 04:34:46.594355 nonebot_plugin_jx3-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2591 2023-08-08 17:52:17.014942 nonebot_plugin_jx3-0.5.8/README.md
--rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 nonebot_plugin_jx3-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-08-08 17:41:12.049341 nonebot_plugin_jx3-0.5.9/LICENSE
+-rw-r--r--   0        0        0    13458 2023-07-27 16:21:18.061796 nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/__init__.py
+-rw-r--r--   0        0        0     1812 2023-07-27 16:00:09.609228 nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/bind.py
+-rw-r--r--   0        0        0      208 2023-07-27 15:47:54.064672 nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/config.py
+-rw-r--r--   0        0        0     3645 2023-07-18 11:30:59.000000 nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/subscribe.py
+-rw-r--r--   0        0        0     2835 2023-08-09 04:34:31.942844 nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/userdefine.py
+-rw-r--r--   0        0        0    11112 2023-07-27 15:49:48.852411 nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/websocket_handler.py
+-rw-r--r--   0        0        0      594 2023-08-09 05:02:19.414210 nonebot_plugin_jx3-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2591 2023-08-08 17:52:17.014942 nonebot_plugin_jx3-0.5.9/README.md
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 nonebot_plugin_jx3-0.5.9/PKG-INFO
```

### Comparing `nonebot_plugin_jx3-0.5.8/LICENSE` & `nonebot_plugin_jx3-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/__init__.py` & `nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/bind.py` & `nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/subscribe.py` & `nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/subscribe.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/userdefine.py` & `nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/userdefine.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.8/nonebot_plugin_jx3/websocket_handler.py` & `nonebot_plugin_jx3-0.5.9/nonebot_plugin_jx3/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.8/pyproject.toml` & `nonebot_plugin_jx3-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-jx3"
-version = "0.5.8"
+version = "0.5.9"
 description = "一个nonebot2的jx3插件"
 authors = ["water <415276785@qq.com>"]
 license ="MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_jx3"}]
 homepage = "https://github.com/fuyang0811/nonebot-plugin-jx3.git"
```

### Comparing `nonebot_plugin_jx3-0.5.8/README.md` & `nonebot_plugin_jx3-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.8/PKG-INFO` & `nonebot_plugin_jx3-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-jx3
-Version: 0.5.8
+Version: 0.5.9
 Summary: 一个nonebot2的jx3插件
 Home-page: https://github.com/fuyang0811/nonebot-plugin-jx3.git
 License: MIT
 Author: water
 Author-email: 415276785@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-jx3 Version: 0.5.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-jx3 Version: 0.5.9 Summary:
 ä¸ä¸ªnonebot2çjx3æä»¶ Home-page: https://github.com/fuyang0811/nonebot-
 plugin-jx3.git License: MIT Author: water Author-email: 415276785@qq.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.7.4,<4.0.0) Requires-
```

