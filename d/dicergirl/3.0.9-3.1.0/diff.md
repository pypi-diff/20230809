# Comparing `tmp/dicergirl-3.0.9.tar.gz` & `tmp/dicergirl-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicergirl-3.0.9.tar", last modified: Mon Jul 31 09:59:35 2023, max compression
+gzip compressed data, was "dicergirl-3.1.0.tar", last modified: Wed Aug  9 05:33:09 2023, max compression
```

## Comparing `dicergirl-3.0.9.tar` & `dicergirl-3.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.772390 dicergirl-3.0.9/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.9/LICENSE
--rw-rw-rw-   0        0        0     9363 2023-07-31 09:59:35.771356 dicergirl-3.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.727379 dicergirl-3.0.9/dicergirl/
--rw-rw-rw-   0        0        0    20079 2023-07-31 09:57:16.000000 dicergirl-3.0.9/dicergirl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.759439 dicergirl-3.0.9/dicergirl/coc/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:17:05.000000 dicergirl-3.0.9/dicergirl/coc/__init__.py
--rw-rw-rw-   0        0        0     4362 2023-07-31 05:29:50.000000 dicergirl-3.0.9/dicergirl/coc/coccards.py
--rw-rw-rw-   0        0        0     9165 2023-07-31 08:22:11.000000 dicergirl-3.0.9/dicergirl/coc/cocutils.py
--rw-rw-rw-   0        0        0     6020 2023-07-30 16:30:57.000000 dicergirl-3.0.9/dicergirl/coc/investigator.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.761910 dicergirl-3.0.9/dicergirl/dnd/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:30:32.000000 dicergirl-3.0.9/dicergirl/dnd/__init__.py
--rw-rw-rw-   0        0        0     2853 2023-07-31 09:32:44.000000 dicergirl-3.0.9/dicergirl/dnd/adventurer.py
--rw-rw-rw-   0        0        0     2831 2023-07-30 14:43:40.000000 dicergirl-3.0.9/dicergirl/dnd/dndcards.py
--rw-rw-rw-   0        0        0     4024 2023-07-31 09:35:10.000000 dicergirl-3.0.9/dicergirl/dnd/dndutils.py
--rw-rw-rw-   0        0        0    17465 2023-07-31 09:30:37.000000 dicergirl-3.0.9/dicergirl/main.py
--rw-rw-rw-   0        0        0     3439 2023-07-30 16:39:51.000000 dicergirl-3.0.9/dicergirl/run.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.764594 dicergirl-3.0.9/dicergirl/scp/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:30:31.000000 dicergirl-3.0.9/dicergirl/scp/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-07-30 16:20:07.000000 dicergirl-3.0.9/dicergirl/scp/agent.py
--rw-rw-rw-   0        0        0     2824 2023-07-31 06:08:08.000000 dicergirl-3.0.9/dicergirl/scp/scpcards.py
--rw-rw-rw-   0        0        0     5188 2023-07-31 09:33:55.000000 dicergirl-3.0.9/dicergirl/scp/scputils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.770191 dicergirl-3.0.9/dicergirl/utils/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.9/dicergirl/utils/__init__.py
--rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.9/dicergirl/utils/chat.py
--rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.9/dicergirl/utils/decorators.py
--rw-rw-rw-   0        0        0     8656 2023-07-31 09:37:09.000000 dicergirl-3.0.9/dicergirl/utils/dicer.py
--rw-rw-rw-   0        0        0    22438 2023-07-31 08:50:24.000000 dicergirl-3.0.9/dicergirl/utils/handlers.py
--rw-rw-rw-   0        0        0    23207 2023-07-31 07:18:19.000000 dicergirl-3.0.9/dicergirl/utils/messages.py
--rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.9/dicergirl/utils/settings.py
--rw-rw-rw-   0        0        0     5839 2023-07-31 09:43:51.000000 dicergirl-3.0.9/dicergirl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:59:35.755176 dicergirl-3.0.9/dicergirl.egg-info/
--rw-rw-rw-   0        0        0     9363 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 09:59:35.000000 dicergirl-3.0.9/dicergirl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 09:59:35.772390 dicergirl-3.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-07-31 07:36:19.000000 dicergirl-3.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 05:33:09.303699 dicergirl-3.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0     9752 2023-08-09 05:33:09.303699 dicergirl-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9155 2023-08-09 03:36:06.000000 dicergirl-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 05:33:09.211250 dicergirl-3.1.0/dicergirl/
+-rw-rw-rw-   0        0        0    19321 2023-08-09 05:27:55.000000 dicergirl-3.1.0/dicergirl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 05:33:09.245550 dicergirl-3.1.0/dicergirl/coc/
+-rw-rw-rw-   0        0        0      134 2023-08-09 05:26:21.000000 dicergirl-3.1.0/dicergirl/coc/__init__.py
+-rw-rw-rw-   0        0        0     3117 2023-08-09 05:28:33.000000 dicergirl-3.1.0/dicergirl/coc/coccards.py
+-rw-rw-rw-   0        0        0     9418 2023-08-09 05:28:39.000000 dicergirl-3.1.0/dicergirl/coc/cocutils.py
+-rw-rw-rw-   0        0        0     6020 2023-07-30 16:30:57.000000 dicergirl-3.1.0/dicergirl/coc/investigator.py
+drwxrwxrwx   0        0        0        0 2023-08-09 05:33:09.261549 dicergirl-3.1.0/dicergirl/dnd/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:30:32.000000 dicergirl-3.1.0/dicergirl/dnd/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-07-31 09:32:44.000000 dicergirl-3.1.0/dicergirl/dnd/adventurer.py
+-rw-rw-rw-   0        0        0     2831 2023-07-30 14:43:40.000000 dicergirl-3.1.0/dicergirl/dnd/dndcards.py
+-rw-rw-rw-   0        0        0     4371 2023-08-09 05:29:14.000000 dicergirl-3.1.0/dicergirl/dnd/dndutils.py
+-rw-rw-rw-   0        0        0    17465 2023-07-31 09:30:37.000000 dicergirl-3.1.0/dicergirl/main.py
+-rw-rw-rw-   0        0        0     3439 2023-07-30 16:39:51.000000 dicergirl-3.1.0/dicergirl/run.py
+drwxrwxrwx   0        0        0        0 2023-08-09 05:33:09.274560 dicergirl-3.1.0/dicergirl/scp/
+-rw-rw-rw-   0        0        0      110 2023-08-09 05:26:28.000000 dicergirl-3.1.0/dicergirl/scp/__init__.py
+-rw-rw-rw-   0        0        0     3285 2023-07-30 16:20:07.000000 dicergirl-3.1.0/dicergirl/scp/agent.py
+-rw-rw-rw-   0        0        0     2948 2023-08-09 05:29:21.000000 dicergirl-3.1.0/dicergirl/scp/scpcards.py
+-rw-rw-rw-   0        0        0     5662 2023-08-09 05:29:05.000000 dicergirl-3.1.0/dicergirl/scp/scputils.py
+drwxrwxrwx   0        0        0        0 2023-08-09 05:33:09.301044 dicergirl-3.1.0/dicergirl/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.1.0/dicergirl/utils/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.1.0/dicergirl/utils/chat.py
+-rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.1.0/dicergirl/utils/decorators.py
+-rw-rw-rw-   0        0        0     8656 2023-07-31 09:37:09.000000 dicergirl-3.1.0/dicergirl/utils/dicer.py
+-rw-rw-rw-   0        0        0    10533 2023-08-09 05:26:03.000000 dicergirl-3.1.0/dicergirl/utils/handlers.py
+-rw-rw-rw-   0        0        0    23207 2023-07-31 07:18:19.000000 dicergirl-3.1.0/dicergirl/utils/messages.py
+-rw-rw-rw-   0        0        0     1270 2023-08-03 02:44:58.000000 dicergirl-3.1.0/dicergirl/utils/settings.py
+-rw-rw-rw-   0        0        0     6124 2023-08-09 05:30:49.000000 dicergirl-3.1.0/dicergirl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-09 05:33:09.241550 dicergirl-3.1.0/dicergirl.egg-info/
+-rw-rw-rw-   0        0        0     9752 2023-08-09 05:33:09.000000 dicergirl-3.1.0/dicergirl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-08-09 05:33:09.000000 dicergirl-3.1.0/dicergirl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 05:33:09.000000 dicergirl-3.1.0/dicergirl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-08-09 05:33:09.000000 dicergirl-3.1.0/dicergirl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-09 05:33:09.000000 dicergirl-3.1.0/dicergirl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 05:33:09.303699 dicergirl-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-08-09 03:31:50.000000 dicergirl-3.1.0/setup.py
```

### Comparing `dicergirl-3.0.9/LICENSE` & `dicergirl-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/PKG-INFO` & `dicergirl-3.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.9
+Version: 3.1.0
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DicerGirl
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicergirl)
+[![PyPI](https://img.shields.io/pypi/v/dicergirl)](https://pypi.org/project/dicergirl/)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/dicergirl)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/dicergirl)](https://pypi.org/project/dicergirl/)
+![PyPI - License](https://img.shields.io/pypi/l/dicergirl)
 
 ## 介绍
 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 
 ## 软件架构
 任何支持 Python3 环境搭建的平台, 建议使用 Python3.10 及以上的 Python 版本, DicerGirl 不支持 Python2.
```

### Comparing `dicergirl-3.0.9/README.md` & `dicergirl-3.1.0/dicergirl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,29 @@
+Metadata-Version: 2.1
+Name: dicergirl
+Version: 3.1.0
+Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
+Home-page: https://gitee.com/unvisitor/dicer
+Author: Night Resurgent <fu050409@163.com>
+Author-email: fu050409@163.com
+License: Apache-2.0
+Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DicerGirl
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicergirl)
+[![PyPI](https://img.shields.io/pypi/v/dicergirl)](https://pypi.org/project/dicergirl/)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/dicergirl)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/dicergirl)](https://pypi.org/project/dicergirl/)
+![PyPI - License](https://img.shields.io/pypi/l/dicergirl)
 
 ## 介绍
 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 
 ## 软件架构
 任何支持 Python3 环境搭建的平台, 建议使用 Python3.10 及以上的 Python 版本, DicerGirl 不支持 Python2.
 
@@ -218,8 +239,8 @@
 注: 以上的 "aDb" 格式(例如10D100)的内容, 表示模拟投掷100面骰子, 投掷10次, 结果小于检定值则检定通过.
 
 欧若可骰娘 版本 3.0.4, 未知访客版权所有.
 Copyright © 2011-2023 Unknown Visitor. All Rights Reserved.
 ```
 
 ## 声明
-此项目由 Apache-2.0 协议开源, 使用代码时, 请注意遵照开源协议.
+此项目由 Apache-2.0 协议开源, 使用代码时, 请注意遵照开源协议.
```

### Comparing `dicergirl-3.0.9/dicergirl/__init__.py` & `dicergirl-3.1.0/dicergirl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from pathlib import Path
 from loguru import logger
-
 from .utils.settings import set_package, get_package
-from .utils.utils import version
 
-import logging
 import nonebot
-import sys
-
-DEBUG = False
-current_dir = Path(__file__).resolve().parent
-mode = "scp"
 
 try:
     driver = nonebot.get_driver()
     set_package("nonebot2")
 except ValueError:
     set_package("qqguild")
 
+from .utils.utils import version
+
+import logging
+import sys
+
+DEBUG = False
+current_dir = Path(__file__).resolve().parent
+mode = "scp"
 package = get_package()
 
 if package == "nonebot2":
     from .coc.investigator import Investigator
-    from .coc.coccards import cards, cache_cards, sa_handler
-    from .coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
+    from .coc.coccards import coc_cards, coc_cache_cards
+    from .coc.cocutils import sc, st, at, coc_dam, en, rd0, ra, ti, li, rb, rp
 
     from .scp.agent import Agent
     from .scp.scpcards import scp_cards, scp_cache_cards
     from .scp.scputils import sra, scp_dam, at as sat
 
     from .dnd.adventurer import Adventurer
     from .dnd.dndcards import dnd_cards, dnd_cache_cards
     from .dnd.dndutils import dra
 
     from .utils.decorators import Commands
     from .utils.messages import help_message, version
-    from .utils.utils import logger, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, get_handlers, get_config, modes
-    from .utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, coc_set_handler, coc_show_handler, coc_del_handler, dnd_set_handler, dnd_show_handler, dnd_del_handler
+    from .utils.utils import logger, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, get_handlers, get_config, modes, get_mentions
+    from .utils.handlers import show_handler, set_handler, scp_del_handler, coc_del_handler, dnd_del_handler
     from .utils.chat import chat
 
     from nonebot.rule import Rule
     from nonebot.matcher import Matcher
     from nonebot.plugin import on_startswith
     from nonebot.adapters import Bot as Bot
     from nonebot.adapters.onebot.v11 import Bot as V11Bot
@@ -69,15 +69,14 @@
     racommand = on_startswith(".ra", priority=2, block=True)
     rhcommand = on_startswith(".rh", priority=2, block=True)
     rhacommand = on_startswith(".rha", priority=1, block=True)
     rcommand = on_startswith(".r", priority=3, block=True)
     ticommand = on_startswith(".ti", priority=2, block=True)
     licommand = on_startswith(".li", priority=2, block=True)
     sccommand = on_startswith(".sc", priority=2, block=True)
-    sacommand = on_startswith(".sa", priority=2, block=True)
     delcommand = on_startswith(".del", priority=2, block=True)# | on_startswith(".delete", priority=2, block=True)
     chatcommand = on_startswith(".chat", priority=2, block=True)
     versioncommand = on_startswith(".version", priority=2, block=True)# | on_startswith(".v", priority=2, block=True)
 
     @driver.on_startup
     async def _():
         global DEBUG
@@ -86,23 +85,19 @@
             logging.getLogger().setLevel(logging.DEBUG)
             logger.remove()
             logger.add(
                 sys.stdout,
                 level = "DEBUG"
             )
             logger.info("DEBUG 模式已启动.")
-        cards.load()
+        init()
+        coc_cards.load()
         scp_cards.load()
         logger.success("欧若可骰娘初始化完毕.")
 
-    def is_group_message() -> Rule:
-        async def _is_group_message(bot: Bot, event: MessageEvent) -> bool:
-            return True if type(event) is GroupMessageEvent else False
-        return Rule(_is_group_message)
-
     @testcommand.handle()
     async def testhandler(matcher: Matcher, event: GroupMessageEvent):
         if not is_super_user(event):
             await matcher.send("[Oracle] 权限不足, 拒绝执行指令.")
             return
         logger.info("发送消息:" + str(event.get_message()))
         logger.info(event.get_message().__repr__())
@@ -226,15 +221,15 @@
             await matcher.send(f'警告: 参数 {args} 不合法, 使用默认值 20 替代.')
             args = 20
 
         inv = Investigator()
         await matcher.send(inv.age_change(args))
 
         if 15 <= args and args < 90:
-            cache_cards.update(event, inv.__dict__, save=False)
+            coc_cache_cards.update(event, inv.__dict__, save=False)
             await matcher.send(str(inv.output()))
 
     @scpcommand.handle()
     async def scp_handler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(event.get_message(), begin=".scp")
         if len(args) > 1:
             logger.info("指令错误, 驳回.")
@@ -285,19 +280,21 @@
             dnd_cache_cards.update(event, adv.__dict__, save=False)
             await matcher.send(str(adv.output()))
         return True
 
     @showcommand.handle()
     async def showhandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(event.get_message(), begin=(".show", ".display"))
+        at = get_mentions(event)
         if not args:
             if mode in modes:
                 try:
-                    sh = eval(f"{mode}_show_handler(event, args)")
-                except:
+                    sh = show_handler(event, args, at, mode=mode)
+                except Exception as error:
+                    logger.exception(error)
                     sh = [f"[Oracle] 错误: 执行指令失败, 疑似该模式不存在该指令."]
             else:
                 await matcher.send("未知的跑团模式.")
                 return True
 
             for msg in sh:
                 await matcher.send(str(msg))
@@ -315,26 +312,20 @@
         for msg in sh:
             await matcher.send(str(msg))
         return
 
     @setcommand.handle()
     async def sethandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(event.get_message(), begin=".set")
-        if not args:
-            args.append(mode)
+        at = get_mentions(event)
 
-        if args[0] in modes:
-            try:
-                now = args[0]
-                args.remove(args[0])
-                sh = eval(f"{now}_set_handler(event, args)")
-            except:
-                sh = [f"[Oracle] 错误: 执行指令失败, 疑似该模式不存在该指令."]
-        else:
-            sh = [f"[Oracle] 错误: 未知的跑团模式."]
+        try:
+            sh = set_handler(event, args, at, mode=mode)
+        except:
+            sh = [f"[Oracle] 错误: 执行指令失败, 疑似模式 {mode} 不存在该指令."]
 
         await matcher.send(sh)
         return
 
 
     @helpcommand.handle()
     async def rdhelphandler(matcher: Matcher, event: GroupMessageEvent):
@@ -348,29 +339,24 @@
 
 
     @modecommand.handle()
     async def modehandler(matcher: Matcher, event: GroupMessageEvent):
         global mode
         args = format_msg(event.get_message(), begin=(".mode", ".m"))
         if args:
-            if args[0] == "coc":
-                mode = "coc"
-                await matcher.send("[Oracle] 已切换到COC跑团模式.")
-                return
-            elif args[0] == "scp":
-                mode = "scp"
-                await matcher.send("[Oracle] 已切换到SCP跑团模式.")
-                return
+            if args[0].lower() in modes:
+                mode = args[0].lower()
+                await matcher.send(f"[Oracle] 已切换到 {mode.upper()} 跑团模式.")
+                return True
             else:
                 await matcher.send("[Oracle] 未知的跑团模式, 忽略.")
                 await matcher.send(help_message("mode"))
-                return
+                return True
         else:
-            await matcher.send(f"[Oracle] 当前的跑团模式为 {mode}.")
-
+            await matcher.send(f"[Oracle] 当前的跑团模式为 {mode.upper()}.")
 
     @stcommand.handle()
     async def stcommandhandler(matcher: Matcher, event: GroupMessageEvent):
         try:
             await matcher.send(st())
         except:
             await matcher.send(help_message("st"))
@@ -387,15 +373,15 @@
 
     @damcommand.handle()
     async def damhandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_msg(event.get_message(), begin=(".dam", ".damage"))
         if mode == "scp":
             sd = scp_dam(args, event)
         elif mode == "coc":
-            sd = dam(args, event)
+            sd = coc_dam(args, event)
         else:
             await matcher.send("未知的跑团模式.")
             return
 
         await matcher.send(sd)
 
 
@@ -471,24 +457,17 @@
 
         if isinstance(scrs, list):
             for scr in scrs:
                 await matcher.send(scr)
         else:
             await matcher.send(scrs)
 
-
-    @sacommand.handle()
-    async def sahandler(matcher: Matcher, event: GroupMessageEvent):
-        args = format_str(event.get_message(), begin=".sa")
-        await matcher.send(sa_handler(event, args))
-
-
     @delcommand.handle()
     async def delhandler(matcher: Matcher, event: GroupMessageEvent):
-        args = format_str(event, begin=(".del", ".delete"))
+        args = format_str(event.get_message(), begin=(".del", ".delete"))
         if mode in modes:
             for msg in eval(f"{mode}_del_handler(event, args)"):
                 await matcher.send(msg)
         return
 
     @chatcommand.handle()
     async def chathandler(matcher: Matcher, event: GroupMessageEvent):
@@ -504,8 +483,8 @@
         args = format_str(event.get_message(), begin=(".version", ".v"))
         await matcher.send(f"欧若可骰娘 版本 {version}, 未知访客版权所有.\nCopyright © 2011-2023 Unknown Visitor. All Rights Reserved.")
         return
 elif package == "qqguild":
     pass
 else:
     logger.critical(f"未知的包模式: {package}!")
-    sys.exit()
+    sys.exit()
```

### Comparing `dicergirl-3.0.9/dicergirl/coc/coccards.py` & `dicergirl-3.1.0/dicergirl/coc/coccards.py`

 * *Files 27% similar despite different names*

```diff
@@ -61,16 +61,16 @@
             if data["skills"].get(skill_name):
                 data["skills"].pop(skill_name)
                 self.update(message, data, qid=qid, save=save)
                 return True
         return False
 
 
-cards = Cards()
-cache_cards = Cards()
+coc_cards = Cards()
+coc_cache_cards = Cards()
 attrs_dict: Dict[str, List[str]] = {
     "名字": ["name", "名字", "名称", "姓名"],
     "性别": ["sex", "性别"],
     "年龄": ["age", "年龄"],
     "力量": ["str", "力量", "攻击", "攻击力"],
     "体质": ["con", "体质"],
     "体型": ["siz", "体型"],
@@ -78,45 +78,8 @@
     "外貌": ["app", "外貌"],
     "智力": ["int", "智力", "灵感"],
     "意志": ["pow", "意志", "精神"],
     "教育": ["edu", "教育"],
     "幸运": ["luc", "幸运"],
     "理智": ["san", "理智", "精神状态", "san值"],
     "生命": ["hp", "生命"]
-}
-
-def sa_handler(message, args: str):
-    args = args.split(" ")
-    args = list(filter(None, args))
-    if args:
-        args = args[0]
-    else:
-        args = None
-    if not args:
-        return help_messages.sa
-    elif not cards.get(message):
-        return "[Oracle] 请先使用`.set`指令保存人物卡后再使用快速检定功能."
-    for attr, alias in attrs_dict.items():
-        if args in alias:
-            arg = alias[0]
-            break
-        else:
-            arg = None
-    if not arg:
-        return f"[Oracle] 错误: 目标参数不在 {attrs_dict} 之内."
-    card_data = cards.get(message)
-    dices = Dice()
-    try:
-        data = card_data[arg]
-        if arg != "名字":
-            val = int(data)
-        else:
-            val = None
-    except KeyError:
-        return f"[Oracle] 致命错误: 存储的数据 {data} 转化为数字的时候出现错误."
-    if not isinstance(val, int):
-        return f"[Oracle] 错误: 参数 {arg} 不可以进行快速检定, 即便它在合法指令中, 因为它没有数值.\n\
-            如果你确信这是一个错误, 请尝试重新车卡或联系管理员."
-    return expr(dices, val)
-
-if __name__ == "__main__":
-    pass
+}
```

### Comparing `dicergirl-3.0.9/dicergirl/coc/cocutils.py` & `dicergirl-3.1.0/dicergirl/coc/cocutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Optional
 try:
     from ..utils.messages import help_messages, temporary_madness, madness_end, phobias, manias, help_message
     from ..utils.dicer import Dice, expr
     from ..utils.utils import _log
-    from .coccards import cards, attrs_dict
+    from .coccards import coc_cards, attrs_dict
     from .investigator import Investigator
 except ImportError:
     from dicergirl.utils.messages import help_messages, temporary_madness, madness_end, phobias, manias, help_message
     from dicergirl.utils.dicer import Dice, expr
     from dicergirl.utils.utils import _log
-    from dicergirl.coc.coccards import cards, attrs_dict
+    from dicergirl.coc.coccards import coc_cards, attrs_dict
     from dicergirl.coc.investigator import Investigator
 
 import random
 import re
 
 def sc(arg, event):
     reply = []
@@ -29,15 +29,15 @@
         failure.roll()
         failure = failure.calc()
         if len(args) > 1:
             card = {"san": int(args[1]), "name": "未指定调查员"}
             reply.append("[Oracle] 用户指定了应当检定的 SAN 值, 这会使得本次检定不会被记录.")
             using_card = False
         else:
-            card = cards.get(event)
+            card = coc_cards.get(event)
             using_card = True
         r = Dice().roll().calc()
         s = f"[Oracle] 调查员: {card['name']}\n"
         s += f"检定精神状态: {card['san']}\n"
         s += f"理智检定值: {r}, "
         if r <= card["san"]:
             down = success
@@ -56,15 +56,15 @@
             s += "未受到严重影响.\n"
         card["san"] -= down
         if card["san"] <= 0:
             card["san"] = 0
         s += f"当前 {card['name']} 的 SAN 值为: {card['san']}"
         reply.append(s)
         if using_card:
-            cards.update(event, card)
+            coc_cards.update(event, card)
         return reply
     except:
         return help_messages.sc
 
 def st():
     result = random.randint(1, 20)
     if result < 4:
@@ -80,51 +80,61 @@
     elif result < 20:
         rstr = "左臂"
     elif result < 21:
         rstr = "头部"
     return "D20=%d: 命中了%s" % (result, rstr)
 
 def at(args, event):
-    inv = Investigator().load(cards.get(event))
+    inv = Investigator().load(coc_cards.get(event))
+    method = "+"
 
     if args:
         d = Dice().parse(args).roll()
     else:
         d = Dice().parse("1d6").roll()
-    db = Dice(inv.db()).roll()
 
-    return f"[Oracle] 投掷 {d.db}+{db.db}=({d.total}+{db.total})\n造成了 {d.total+db.total}点 伤害."
+    if "d" in inv.db():
+        db = Dice(inv.db()).roll()
+        dbtotal = db.total
+        db = db.db
+    else:
+        db = int(inv.db())
+        dbtotal = db
+        if db < 0:
+            method = ""
+
+    return f"[Oracle] 投掷 {d.db}{method}{db}=({d.total}+{dbtotal})\n造成了 {d.total+dbtotal}点 伤害."
 
-def dam(args, message):
-    card = cards.get(message)
+def coc_dam(args, message):
+    card = coc_cards.get(message)
     if not card:
         return "[Oracle] 未找到缓存数据, 请先使用`.coc`指令进行车卡生成角色卡并`.set`进行保存."
     max_hp = card["con"] + card["siz"]
     try:
         arg = int(args[0])
         card["hp"] -= arg
         r = f"[Orcale] {card['name']} 失去了 {arg}点 生命"
     except:
         d = Dice().parse("1d6").roll()
         card["hp"] -= d.total
         r = "[Oracle] 投掷 1D6={d}\n受到了 {d}点 伤害".format(d=d.calc())
     if card["hp"] <= 0:
         card["hp"] = 0
         r += f", 调查员 {card['name']} 已死亡."
-    elif max_hp * 0.8 <= card["hp"] and card["hp"] < max_hp:
+    elif (max_hp * 0.8) <= card["hp"] and (card["hp"] < max_hp):
         r += f", 调查员 {card['name']} 具有轻微伤."
-    elif max_hp * 0.6 <= card["hp"] and card["hp"] <= max_hp * 0.8:
+    elif (max_hp * 0.6 <= card["hp"]) and (card["hp"] <= max_hp * 0.8):
         r += f", 调查员 {card['name']} 进入轻伤状态."
-    elif max_hp * 0.2 <= card["hp"] and card["hp"] <= max_hp * 0.6:
+    elif (max_hp * 0.2 <= card["hp"]) and (card["hp"] <= max_hp * 0.6):
         r += f", 调查员 {card['name']} 身负重伤."
     elif max_hp * 0.2 >= card["hp"]:
         r += f", 调查员 {card['name']} 濒死."
     else:
         r += "."
-    cards.update(message, card)
+    coc_cards.update(message, card)
     return r
 
 def rd0(arg: str) -> str:
     args = arg.lower().split(" ")
     d_str = args.pop(0).split("#")
     try:
         parse = d_str.pop(0)
@@ -152,15 +162,15 @@
 
 def ra(args, event):
     if len(args) == 0:
         return help_message("ra")
     if len(args) > 2:
         return "[Oracle] 错误: 参数过多(2需要 %d给予)." % len(args)
 
-    card_data = cards.get(event)
+    card_data = coc_cards.get(event)
     if not card_data:
         return "[Oracle] 在执行参数检定前, 请先执行`.coc`车卡并执行`.set`保存."
     inv = Investigator().load(card_data)
     is_base = False
     for _, alias in attrs_dict.items():
         if args[0] in alias:
             v = int(eval("inv.{prop}".format(prop=alias[0])))
```

### Comparing `dicergirl-3.0.9/dicergirl/coc/investigator.py` & `dicergirl-3.1.0/dicergirl/coc/investigator.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/dnd/adventurer.py` & `dicergirl-3.1.0/dicergirl/dnd/adventurer.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/dnd/dndcards.py` & `dicergirl-3.1.0/dicergirl/dnd/dndcards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/dnd/dndutils.py` & `dicergirl-3.1.0/dicergirl/dnd/dndutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,34 @@
         rstr = "右臂"
     elif result < 20:
         rstr = "左臂"
     elif result < 21:
         rstr = "头部"
     return "[Oracle] 命中了%s" % (rstr)
 
-def at(args):
+def at(args, event):
+    inv = Adventurer().load(dnd_cards.get(event))
+    method = "+"
+
     if args:
         d = Dice().parse(args).roll()
     else:
         d = Dice().parse("1d6").roll()
-    return f"[Oracle] 投掷 {d.db}={d.total}\n造成了 {d.total}点 伤害."
+
+    if "d" in inv.db():
+        db = Dice(inv.db()).roll()
+        dbtotal = db.total
+        db = db.db
+    else:
+        db = int(inv.db())
+        dbtotal = db
+        if db < 0:
+            method = ""
+
+    return f"[Oracle] 投掷 {d.db}{method}{db}=({d.total}+{dbtotal})={d.total+dbtotal}\n造成了 {d.total+dbtotal}点 伤害."
 
 def dnd_dam(args, message):
     card = dnd_cards.get(message)
     if not card:
         return "[Oracle] 未找到缓存数据, 请先使用`.dnd`指令进行车卡生成角色卡并`.set`进行保存."
     max_hp = card["hp_max"]
     if len(args) == 1:
```

### Comparing `dicergirl-3.0.9/dicergirl/main.py` & `dicergirl-3.1.0/dicergirl/main.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/run.py` & `dicergirl-3.1.0/dicergirl/run.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/scp/agent.py` & `dicergirl-3.1.0/dicergirl/scp/agent.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/scp/scpcards.py` & `dicergirl-3.1.0/dicergirl/scp/scpcards.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,17 @@
 
 scp_cards = Cards()
 scp_cache_cards = Cards()
 scp_attrs_dict: Dict[str, List[str]] = {
     "名字": ["name", "名字", "名称", "姓名"],
     "性别": ["sex", "性别"],
     "年龄": ["age", "年龄"],
-    "强度": ["str", "力量", "攻击", "强度"],
-    "灵巧": ["dex", "灵巧"],
-    "健康": ["hth", "健康"],
-    "命运": ["fte", "命运"],
-    "魅力": ["chr", "魅力"],
-    "情报": ["int", "情报"],
-    "意志": ["wil", "意志", "精神"],
+    "强度": ["str", "强度", "力量", "攻击"],
+    "感知": ["per", "感知", "灵感"],
+    "灵巧": ["dex", "灵巧", "敏捷"],
+    "健康": ["hth", "健康", "体质"],
+    "命运": ["fte", "命运", "幸运", "气运", "运气"],
+    "魅力": ["chr", "魅力", "外貌"],
+    "情报": ["int", "情报", "侦查"],
+    "意志": ["wil", "意志", "精神", "理智"],
     "生命": ["hp", "生命"]
 }
```

### Comparing `dicergirl-3.0.9/dicergirl/scp/scputils.py` & `dicergirl-3.1.0/dicergirl/scp/scputils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from ..utils.messages import help_messages, help_message
-    from ..utils.dicer import Dice, scp_doc
+    from ..utils.dicer import Dice, scp_doc, expr
     from .scpcards import scp_cards, scp_attrs_dict as attrs_dict
     from .agent import Agent
 except ImportError:
     from dicergirl.utils.messages import help_messages, help_message
-    from dicergirl.utils.dicer import Dice, scp_doc
+    from dicergirl.utils.dicer import Dice, scp_doc, expr
     from dicergirl.scp.scpcards import scp_cards, scp_attrs_dict as attrs_dict
     from dicergirl.scp.agent import Agent
 
 import random
 
 def st():
     result = random.randint(1, 20)
@@ -25,26 +25,43 @@
         rstr = "右臂"
     elif result < 20:
         rstr = "左臂"
     elif result < 21:
         rstr = "头部"
     return "[Oracle] 命中了%s" % (rstr)
 
-def at(args):
+def at(args, event):
+    inv = Agent().load(scp_cards.get(event))
+    method = "+"
+
     if args:
         d = Dice().parse(args).roll()
     else:
         d = Dice().parse("1d6").roll()
-    return f"[Oracle] 投掷 {d.db}={d.total}\n造成了 {d.total}点 伤害."
+
+    if "d" in inv.db():
+        db = Dice(inv.db()).roll()
+        dbtotal = db.total
+        db = db.db
+    else:
+        db = int(inv.db())
+        dbtotal = db
+        if db < 0:
+            method = ""
+
+    return f"[Oracle] 投掷 {d.db}{method}{db}=({d.total}+{dbtotal})={d.total+dbtotal}\n造成了 {d.total+dbtotal}点 伤害."
 
 def scp_dam(args, message):
     card = scp_cards.get(message)
+
     if not card:
         return "[Oracle] 未找到缓存数据, 请先使用`.scp`指令进行车卡生成角色卡并`.set`进行保存."
+
     max_hp = card["hp_max"]
+
     if len(args) == 1:
         if not args[0] in ["check", "c"]:
             arg = int(args[0])
             card["hp"] -= arg
             r = f"[Orcale] {card['name']} 失去了 {arg}点 生命"
         else:
             r = "检查特工状态"
@@ -55,14 +72,15 @@
     elif len(args) == 3:
         if args[1] != "d":
             r = "[Oracle] 未知的指令格式."
         else:
             d = Dice().parse(f"{args[0]}{args[1]}{args[2]}").roll()
             card["hp"] -= d.total
             r = f"[Oracle] 投掷 {args[0]}D{args[2]}={d.calc()}\n受到了 {d.calc()}点 伤害"
+
     if card["hp"] <= 0:
         card["hp"] = 0
         r += f", 特工 {card['name']} 已死亡."
     elif (max_hp * 0.8 <= card["hp"]) and (card["hp"] < max_hp):
         r += f", 特工 {card['name']} 具有轻微伤势."
     elif (max_hp * 0.6 <= card["hp"]) and (card['hp'] <= max_hp * 0.8):
         r += f", 特工 {card['name']} 具有轻微伤."
@@ -70,65 +88,78 @@
         r += f", 特工 {card['name']} 具有轻伤."
     elif (max_hp * 0.2 <= card["hp"]) and (card["hp"] <= max_hp * 0.4):
         r += f", 特工 {card['name']} 身负重伤."
     elif max_hp * 0.2 >= card["hp"]:
         r += f", 特工 {card['name']} 濒死."
     else:
         r += "."
+
     scp_cards.update(message, card)
     return r
 
 def sra(args, event):
     if len(args) == 0:
         return help_message("sra")
+
     if len(args) > 2:
         return "[Oracle] 错误: 参数过多(最多2需要但%d给予)." % len(args)
     
     if len(args) == 2:
         difficulty = int(args[1])
     else:
         difficulty = 12
 
     card_data = scp_cards.get(event)
+
     if not card_data:
         return "[Oracle] 在执行参数检定前, 请先执行`.scp`车卡并执行`.set`保存."
+
     inv = Agent().load(card_data)
+
     is_base = False
     for _, alias in attrs_dict.items():
         if args[0] in alias:
             dices: list = eval("inv.dices['{prop}']".format(prop=alias[0]))
             is_base = True
             break
+
     is_skill = False
     if not is_base:
         for skill in inv.skills:
             if args[0] == skill:
                 v = inv.skills[skill]
                 break
+
     if not is_base and not is_skill:
         return "[Oracle] 错误: 没有这个数据或技能."
     
+    if not is_base and is_skill:
+        result = Dice()
+        return expr(result, int(v))
+
     all_dices = []
+
     if len(dices) > 4:
         while True:
             if len(all_dices) == 4:
                 break
             choice = random.choice(dices)
             all_dices.append(choice)
             dices.remove(choice)
     elif len(dices) <= 4:
         all_dices = dices
-    
+
     results = []
     great = False
     for dice in all_dices:
         dice = Dice("1"+dice.lower()).roll()
         results.append(dice.total)
         if dice.great == True:
             great = True
+
     result = max(results)
     results.remove(result)
     result += max(results)
     r = scp_doc(result, difficulty, agent=inv.name, great=great)
     return r
```

### Comparing `dicergirl-3.0.9/dicergirl/utils/chat.py` & `dicergirl-3.1.0/dicergirl/utils/chat.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/utils/decorators.py` & `dicergirl-3.1.0/dicergirl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/utils/dicer.py` & `dicergirl-3.1.0/dicergirl/utils/dicer.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/utils/messages.py` & `dicergirl-3.1.0/dicergirl/utils/messages.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/dicergirl/utils/settings.py` & `dicergirl-3.1.0/dicergirl/utils/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from loguru import logger
 from pathlib import Path
 
 import sys
 import yaml
 
-package = "qqguild"
+package = None
 allowed_packages = ["nonebot2", "qqguild"]
 
 def set_package(pkg: str):
     global package
     pkg = pkg.lower()
 
     if pkg in allowed_packages:
```

### Comparing `dicergirl-3.0.9/dicergirl/utils/utils.py` & `dicergirl-3.1.0/dicergirl/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 from typing import Union
 
 import json
 import sys
 import uuid
 import re
 import inspect
+import json
 
 try:
     from dicergirl.utils.decorators import translate_punctuation
     from dicergirl.utils.settings import get_package, setconfig, getconfig
     from dicergirl import coc, scp, dnd
 except ImportError:
     from .decorators import translate_punctuation
     from .settings import get_package, setconfig, getconfig
-    from . import coc, scp, dnd
+    from .. import coc, scp, dnd
 
 package = get_package()
 
 if package == "nonebot2":
     class Message:
         pass
     try:
@@ -38,15 +39,15 @@
     try:
         from botpy.message import Message
     except ModuleNotFoundError:
         logger.warning("未找到依赖`qq-botpy`, 请检查你的配置.")
         class Message:
             pass
 
-version = "3.0.9"
+version = "3.1.0"
 current_dir = Path(__file__).resolve().parent
 dicer_girl_dir = Path.home() / ".dicergirl"
 data_dir = dicer_girl_dir / "data"
 _coc_cachepath = data_dir / "coc_cards.json"
 _scp_cachepath = data_dir / "scp_cards.json"
 _dnd_cachepath = data_dir / "dnd_cards.json"
 _super_user = data_dir / "super_user.json"
@@ -84,37 +85,47 @@
 def get_config() -> dict:
     return getconfig(path=dicer_girl_dir, filename="config.yaml")
 
 def format_msg(message, begin=None):
     msg = format_str(message, begin=begin).split(" ")
     outer = []
     for m in msg:
-        m = re.split(r'(\d+)|([a-zA-Z]+)|([\u4e00-\u9fa5]+)', m)
+        m = re.split(r'(\d+)|([a-zA-Z\u4e00-\u9fa5]+)', m)
         m = list(filter(None, m))
         outer += m
     msg = outer
     msg = list(filter(None, msg))
     _log.debug(msg)
     return msg
 
 def format_str(message: Union[Message, str], begin=None):
-    regex = "[<](.*?)[>]"
+    regex = r"[<\[](.*?)[\]>]"
     content = message.content if isinstance(message, Message) else message
     msg = re.sub("\s+", " ", re.sub(regex, "", str(content).lower())).strip(" ")
     msg = translate_punctuation(msg)
     _log.debug(msg)
     if begin:
         if isinstance(begin, list) or isinstance(begin, tuple):
             for b in begin:
                 msg = msg.replace(b, "").lstrip(" ")
         else:
             msg = msg.replace(begin, "").lstrip(" ")
     _log.debug(msg)
     return msg
 
+def get_mentions(event: GroupMessageEvent):
+    mentions = []
+    message = json.loads(event.json())["message"]
+
+    for mention in message:
+        if mention["type"] == "at":
+            mentions.append(mention["data"]["qq"])
+
+    return mentions
+
 def get_handlers(main):
     commands_functions = []
 
     for _, obj in vars(main).items():
         if inspect.isfunction(obj) and hasattr(obj, '__annotations__'):
             annotations = obj.__annotations__
             if annotations.get('message') is Message:
@@ -132,15 +143,15 @@
         logger.warning(f"超出预计的 package: {package}, 将 Group ID 设置为 0.")
         return "0"
 
 def get_user_id(event):
     try:
         if package == "qqguild":
             return eval(str(event.author))["id"]
-        elif package:
+        elif package == "nonebot2":
             return str(event.get_user_id())
     except:
         logger.warning(f"超出预计的 package: {package}, 将 User ID 设置为 0.")
         return "0"
 
 def add_super_user(message):
     with open(_super_user, "w+") as _su:
@@ -175,8 +186,8 @@
             sudos = {}
         else:
             sudos = json.loads(sr)
     for sudo in sudos.keys():
         if get_user_id(message) == sudo:
             su = True
             break
-    return su
+    return su
```

### Comparing `dicergirl-3.0.9/dicergirl.egg-info/PKG-INFO` & `dicergirl-3.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.1
-Name: dicergirl
-Version: 3.0.9
-Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
-Home-page: https://gitee.com/unvisitor/dicer
-Author: Night Resurgent <fu050409@163.com>
-Author-email: fu050409@163.com
-License: Apache-2.0
-Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DicerGirl
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dicergirl)
+[![PyPI](https://img.shields.io/pypi/v/dicergirl)](https://pypi.org/project/dicergirl/)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/dicergirl)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/dicergirl)](https://pypi.org/project/dicergirl/)
+![PyPI - License](https://img.shields.io/pypi/l/dicergirl)
 
 ## 介绍
 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 
 ## 软件架构
 任何支持 Python3 环境搭建的平台, 建议使用 Python3.10 及以上的 Python 版本, DicerGirl 不支持 Python2.
 
@@ -234,8 +223,8 @@
 注: 以上的 "aDb" 格式(例如10D100)的内容, 表示模拟投掷100面骰子, 投掷10次, 结果小于检定值则检定通过.
 
 欧若可骰娘 版本 3.0.4, 未知访客版权所有.
 Copyright © 2011-2023 Unknown Visitor. All Rights Reserved.
 ```
 
 ## 声明
-此项目由 Apache-2.0 协议开源, 使用代码时, 请注意遵照开源协议.
+此项目由 Apache-2.0 协议开源, 使用代码时, 请注意遵照开源协议.
```

### Comparing `dicergirl-3.0.9/dicergirl.egg-info/SOURCES.txt` & `dicergirl-3.1.0/dicergirl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.9/setup.py` & `dicergirl-3.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     license = "Apache-2.0",
     packages = setuptools.find_packages(),
     install_requires = [
-        'nb-cli',
         'nonebot2',
         'qq-botpy',
         'watchdog',
         'loguru',
         'pyyaml',
         'openai'
     ],
```

