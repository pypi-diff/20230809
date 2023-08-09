# Comparing `tmp/nonebot_plugin_jx3-0.5.6.tar.gz` & `tmp/nonebot_plugin_jx3-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_jx3-0.5.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_jx3-0.5.7.tar", max compression
```

## Comparing `nonebot_plugin_jx3-0.5.6.tar` & `nonebot_plugin_jx3-0.5.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-08-08 17:41:12.049341 nonebot_plugin_jx3-0.5.6/LICENSE
--rw-r--r--   0        0        0    13458 2023-07-27 16:21:18.061796 nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/__init__.py
--rw-r--r--   0        0        0     1812 2023-07-27 16:00:09.609228 nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/bind.py
--rw-r--r--   0        0        0      208 2023-07-27 15:47:54.064672 nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/config.py
--rw-r--r--   0        0        0     3645 2023-07-18 11:30:59.000000 nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/subscribe.py
--rw-r--r--   0        0        0     2829 2023-07-18 11:30:59.000000 nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/userdefine.py
--rw-r--r--   0        0        0    11112 2023-07-27 15:49:48.852411 nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/websocket_handler.py
--rw-r--r--   0        0        0      559 2023-08-09 04:24:45.591585 nonebot_plugin_jx3-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     2591 2023-08-08 17:52:17.014942 nonebot_plugin_jx3-0.5.6/README.md
--rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 nonebot_plugin_jx3-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-08-08 17:41:12.049341 nonebot_plugin_jx3-0.5.7/LICENSE
+-rw-r--r--   0        0        0    13458 2023-07-27 16:21:18.061796 nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/__init__.py
+-rw-r--r--   0        0        0     1812 2023-07-27 16:00:09.609228 nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/bind.py
+-rw-r--r--   0        0        0      208 2023-07-27 15:47:54.064672 nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/config.py
+-rw-r--r--   0        0        0     3645 2023-07-18 11:30:59.000000 nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/subscribe.py
+-rw-r--r--   0        0        0     2829 2023-07-18 11:30:59.000000 nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/userdefine.py
+-rw-r--r--   0        0        0    11112 2023-07-27 15:49:48.852411 nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/websocket_handler.py
+-rw-r--r--   0        0        0      594 2023-08-09 04:28:38.791573 nonebot_plugin_jx3-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     2591 2023-08-08 17:52:17.014942 nonebot_plugin_jx3-0.5.7/README.md
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 nonebot_plugin_jx3-0.5.7/PKG-INFO
```

### Comparing `nonebot_plugin_jx3-0.5.6/LICENSE` & `nonebot_plugin_jx3-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/__init__.py` & `nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/bind.py` & `nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/subscribe.py` & `nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/subscribe.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/userdefine.py` & `nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/userdefine.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.6/nonebot_plugin_jx3/websocket_handler.py` & `nonebot_plugin_jx3-0.5.7/nonebot_plugin_jx3/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.6/pyproject.toml` & `nonebot_plugin_jx3-0.5.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nonebot-plugin-jx3"
-version = "0.5.6"
+version = "0.5.7"
 description = "一个nonebot2的jx3插件"
 authors = ["water <415276785@qq.com>"]
 license ="MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_jx3"}]
 homepage = "https://github.com/fuyang0811/nonebot-plugin-jx3.git"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0rc1"
 nonebot-adapter-onebot = "^2.0.0"
 httpx= "^0.19.0"
 tinydb= "^4.5.1"
 aiohttp= "^3.7.4"
-
+nonebot_plugin_apscheduler="^0.3.0"
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_jx3-0.5.6/README.md` & `nonebot_plugin_jx3-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_jx3-0.5.6/PKG-INFO` & `nonebot_plugin_jx3-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-jx3
-Version: 0.5.6
+Version: 0.5.7
 Summary: 一个nonebot2的jx3插件
 Home-page: https://github.com/fuyang0811/nonebot-plugin-jx3.git
 License: MIT
 Author: water
 Author-email: 415276785@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: httpx (>=0.19.0,<0.20.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.3.0,<0.4.0)
 Requires-Dist: tinydb (>=4.5.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-jx3 Version: 0.5.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-jx3 Version: 0.5.7 Summary:
 ä¸ä¸ªnonebot2çjx3æä»¶ Home-page: https://github.com/fuyang0811/nonebot-
 plugin-jx3.git License: MIT Author: water Author-email: 415276785@qq.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.7.4,<4.0.0) Requires-
 Dist: httpx (>=0.19.0,<0.20.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.0.0,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Requires-Dist:
-tinydb (>=4.5.1,<5.0.0) Description-Content-Type: text/markdown
+nonebot_plugin_apscheduler (>=0.3.0,<0.4.0) Requires-Dist: tinydb
+(>=4.5.1,<5.0.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                # nonebot-plugin-jx3 _è¿æ¯ä¸ä¸ªä½¿ç¨ NoneBot
 æ¡æ¶ç¼åçæä»¶ï¼æä¾å¤ç§åè½å¦æ¥å¸¸æ¥è¯¢ï¼é¢æµï¼éä»·æ¥è¯¢ï¼é²è±ï¼å¬åï¼æ²çï¼jjcï¼é»å¸ï¼éªè¯ï¼å¥éï¼æåä»¥åå¤ç§æ¶æ¯æ¨éåè½ã_
                            [license] [pypi] [python]
 ## ð ä»ç» nonebot-plugin-jx3 æ¯ä¸ä¸ªä½¿ç¨ NoneBot
 æ¡æ¶ç¼åçæä»¶ï¼å®æä¾äºå¤ç§åè½ï¼ä¾å¦æ¥å¸¸æ¥è¯¢ï¼é¢æµï¼éä»·æ¥è¯¢ï¼é²è±ï¼å¬åï¼æ²çï¼jjcï¼é»å¸ï¼éªè¯ï¼å¥éï¼æåä»¥åå¤ç§æ¶æ¯æ¨éåè½ï¼ä¾å¦"818",
```

