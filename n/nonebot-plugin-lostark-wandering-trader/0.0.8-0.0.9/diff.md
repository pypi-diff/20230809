# Comparing `tmp/nonebot_plugin_lostark_wandering_trader-0.0.8.tar.gz` & `tmp/nonebot_plugin_lostark_wandering_trader-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot_plugin_lostark_wandering_trader-0.0.8.tar", last modified: Mon Aug  7 09:55:28 2023, max compression
+gzip compressed data, was "dist/nonebot_plugin_lostark_wandering_trader-0.0.9.tar", last modified: Wed Aug  9 00:21:14 2023, max compression
```

## Comparing `nonebot_plugin_lostark_wandering_trader-0.0.8.tar` & `nonebot_plugin_lostark_wandering_trader-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-07 09:55:28.583213 nonebot_plugin_lostark_wandering_trader-0.0.8/
--rw-r--r--   0 gongmin    (501) staff       (20)     1064 2023-08-02 03:29:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/LICENSE
--rw-r--r--   0 gongmin    (501) staff       (20)     5974 2023-08-07 09:55:28.582724 nonebot_plugin_lostark_wandering_trader-0.0.8/PKG-INFO
--rw-r--r--   0 gongmin    (501) staff       (20)     4034 2023-08-07 00:58:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/README.md
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-07 09:55:28.578671 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader/
--rw-r--r--   0 gongmin    (501) staff       (20)    10912 2023-08-07 09:53:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader/__init__.py
--rw-r--r--   0 gongmin    (501) staff       (20)      273 2023-08-07 00:58:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader/config.py
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-07 09:55:28.581719 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader.egg-info/
--rw-r--r--   0 gongmin    (501) staff       (20)     5974 2023-08-07 09:55:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
--rw-r--r--   0 gongmin    (501) staff       (20)      457 2023-08-07 09:55:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
--rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-07 09:55:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
--rw-r--r--   0 gongmin    (501) staff       (20)      110 2023-08-07 09:55:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
--rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-07 09:55:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
--rw-r--r--   0 gongmin    (501) staff       (20)      630 2023-08-07 09:54:47.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/pyproject.toml
--rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-07 09:55:28.583400 nonebot_plugin_lostark_wandering_trader-0.0.8/setup.cfg
--rw-r--r--   0 gongmin    (501) staff       (20)     1304 2023-08-07 09:54:51.000000 nonebot_plugin_lostark_wandering_trader-0.0.8/setup.py
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-09 00:21:14.659503 nonebot_plugin_lostark_wandering_trader-0.0.9/
+-rw-r--r--   0 gongmin    (501) staff       (20)     1064 2023-08-02 03:29:04.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/LICENSE
+-rw-r--r--   0 gongmin    (501) staff       (20)     6106 2023-08-09 00:21:14.659052 nonebot_plugin_lostark_wandering_trader-0.0.9/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)     4166 2023-08-09 00:20:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/README.md
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-09 00:21:14.655154 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader/
+-rw-r--r--   0 gongmin    (501) staff       (20)    11341 2023-08-08 13:50:18.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader/__init__.py
+-rw-r--r--   0 gongmin    (501) staff       (20)      273 2023-08-07 00:58:36.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader/config.py
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-09 00:21:14.658224 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader.egg-info/
+-rw-r--r--   0 gongmin    (501) staff       (20)     6106 2023-08-09 00:21:14.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)      457 2023-08-09 00:21:14.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-09 00:21:14.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      110 2023-08-09 00:21:14.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-09 00:21:14.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      630 2023-08-09 00:20:43.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/pyproject.toml
+-rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-09 00:21:14.659657 nonebot_plugin_lostark_wandering_trader-0.0.9/setup.cfg
+-rw-r--r--   0 gongmin    (501) staff       (20)     1304 2023-08-09 00:20:47.000000 nonebot_plugin_lostark_wandering_trader-0.0.9/setup.py
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.8/LICENSE` & `nonebot_plugin_lostark_wandering_trader-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.8/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_lostark_wandering_trader
-Version: 0.0.8
+Version: 0.0.9
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: EmiyaGm <464723943@qq.com>
 License: MIT License
         
         Copyright (c) 2023 EmiyaGm
@@ -61,14 +61,17 @@
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-lostark-wandering-trader">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-lostark-wandering-trader.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 </p>
 
+## 重要提示
+因为国服更新了韩服最近的流浪商人机制，已经不再需要提示了，所以本插件暂停更新
+
 ## 安装
 
 ```bash
 nb plugin install nonebot_plugin_lostark_wandering_trader
 ```
 或者
 ```bash
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot_plugin_lostark_wandering_trader Version:
-0.0.8 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.9 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: EmiyaGm <464723943@qq.com> License: MIT License Copyright (c)
 2023 EmiyaGm Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -23,14 +23,16 @@
 Independent Requires-Python: >=3.8,<4.0 Description-Content-Type: text/markdown
 License-File: LICENSE
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
             èªå¨æ­æ¥ç¨æåå¶ä»¥ä¸å¡çå·æ° æä»¶ â¨_
                            [license] [pypi] [python]
+## éè¦æç¤º
+å ä¸ºå½ææ´æ°äºé©ææè¿çæµæµªåäººæºå¶ï¼å·²ç»ä¸åéè¦æç¤ºäºï¼æä»¥æ¬æä»¶æåæ´æ°
 ## å®è£ ```bash nb plugin install nonebot_plugin_lostark_wandering_trader ```
 æè ```bash pip install nonebot-plugin-lostark-wandering-trader ``` ##
 æ´æ° ```bash nb plugin update nonebot_plugin_lostark_wandering_trader ```
 æè ```bash pip install nonebot-plugin-lostark-wandering-trader -U ``` ###
 å¯¼å¥æä»¶ - å¨`pyproject.toml`éç`[tool.nonebot]`ä¸­æ·»å `plugins =
 ["nonebot_plugin_lostark_wandering_trader"]`
 **æ³¨**ï¼å¦æä½ ä½¿ç¨`nb`å®è£æä»¶ï¼åä¸éè¦è®¾ç½®æ­¤é¡¹ ##
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.8/README.md` & `nonebot_plugin_lostark_wandering_trader-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,17 @@
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-lostark-wandering-trader">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-lostark-wandering-trader.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 </p>
 
+## 重要提示
+因为国服更新了韩服最近的流浪商人机制，已经不再需要提示了，所以本插件暂停更新
+
 ## 安装
 
 ```bash
 nb plugin install nonebot_plugin_lostark_wandering_trader
 ```
 或者
 ```bash
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
             èªå¨æ­æ¥ç¨æåå¶ä»¥ä¸å¡çå·æ° æä»¶ â¨_
                            [license] [pypi] [python]
+## éè¦æç¤º
+å ä¸ºå½ææ´æ°äºé©ææè¿çæµæµªåäººæºå¶ï¼å·²ç»ä¸åéè¦æç¤ºäºï¼æä»¥æ¬æä»¶æåæ´æ°
 ## å®è£ ```bash nb plugin install nonebot_plugin_lostark_wandering_trader ```
 æè ```bash pip install nonebot-plugin-lostark-wandering-trader ``` ##
 æ´æ° ```bash nb plugin update nonebot_plugin_lostark_wandering_trader ```
 æè ```bash pip install nonebot-plugin-lostark-wandering-trader -U ``` ###
 å¯¼å¥æä»¶ - å¨`pyproject.toml`éç`[tool.nonebot]`ä¸­æ·»å `plugins =
 ["nonebot_plugin_lostark_wandering_trader"]`
 **æ³¨**ï¼å¦æä½ ä½¿ç¨`nb`å®è£æä»¶ï¼åä¸éè¦è®¾ç½®æ­¤é¡¹ ##
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader/__init__.py` & `nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,77 +65,83 @@
                         nid = notice.get('locationId', '')
                         id = item.get('locationId', '')
                         if nid == id:
                             can_notice = False
                     if can_notice:
                         card = item.get('_card', {})
                         rapport = item.get('_rapport', {})
-                        rarity = card.get('rarity', '')
                         rarity_array = []
                         send_type_array = []
                         if len(plugin_config.get('send_type')) == 0:
                             send_type_array = ['Card', 'Rapport']
                         else:
                             send_type_array = plugin_config.get('send_type')
                         if len(plugin_config.get('rarity')) == 0:
                             rarity_array = ['Epic', 'Legendary', 'Rare']
                         else:
                             rarity_array = plugin_config.get('rarity')
-                        confirm = False
-                        for rItem in rarity_array:
-                            if rItem == rarity and "Card" in send_type_array:
-                                confirm = True
                         location = item.get('_location', {})
                         image = location.get('snapshot', '')
                         lname = location.get('name', '')
                         member = item.get('_member', {})
                         username = member.get('username', '未知人士')
-                        if confirm:
-                            cname = card.get('name', '')
-                            response = lname + f' 出{cname}了！' + f'稀有度为{rarity}' + f' 提报人: {username}'
-                            try:
-                                for qq in plugin_config.get('user_ids'):
-                                    await bot.call_api('send_private_msg', **{
-                                        'user_id': qq,
-                                        'message': response
-                                    })
-                            except:
-                                pass
-                            try:
-                                for group in plugin_config.get('group_ids'):
-                                    await bot.call_api('send_group_msg', **{
-                                        'group_id': group,
-                                        'message': response
-                                    })
-                            except:
-                                pass
-                            time.sleep(1)
+                        if card is None:
+                            confirm = False
+                        else:
+                            rarity = card.get('rarity', '')
+                            confirm = False
+                            for rItem in rarity_array:
+                                if rItem == rarity and "Card" in send_type_array:
+                                    confirm = True
+                            if confirm:
+                                cname = card.get('name', '')
+                                response = lname + f' 出{cname}了！' + f'稀有度为{rarity}' + f' 提报人: {username}'
+                                try:
+                                    for qq in plugin_config.get('user_ids'):
+                                        await bot.call_api('send_private_msg', **{
+                                            'user_id': qq,
+                                            'message': response
+                                        })
+                                except:
+                                    pass
+                                try:
+                                    for group in plugin_config.get('group_ids'):
+                                        await bot.call_api('send_group_msg', **{
+                                            'group_id': group,
+                                            'message': response
+                                        })
+                                except:
+                                    pass
+                                time.sleep(1)
                         rapport_confirm = False
-                        if rapport.get('rarity') == 'Legendary' and "Rapport" in send_type_array:
-                            rapport_confirm = True
-                        if rapport_confirm:
-                            rname = rapport.get('name', '')
-                            response = lname + f' 出{rname}了！' + '稀有度为传说' + f' 提报人: {username}'
-                            try:
-                                for qq in plugin_config.get('user_ids'):
-                                    await bot.call_api('send_private_msg', **{
-                                        'user_id': qq,
-                                        'message': response
-                                    })
-                            except:
-                                pass
-                            try:
-                                for group in plugin_config.get('group_ids'):
-                                    await bot.call_api('send_group_msg', **{
-                                        'group_id': group,
-                                        'message': response
-                                    })
-                            except:
-                                pass
-                            time.sleep(1)
+                        if rapport is None:
+                            rapport_confirm = False
+                        else:
+                            if rapport.get('rarity') == 'Legendary' and "Rapport" in send_type_array:
+                                rapport_confirm = True
+                            if rapport_confirm:
+                                rname = rapport.get('name', '')
+                                response = lname + f' 出{rname}了！' + '稀有度为传说' + f' 提报人: {username}'
+                                try:
+                                    for qq in plugin_config.get('user_ids'):
+                                        await bot.call_api('send_private_msg', **{
+                                            'user_id': qq,
+                                            'message': response
+                                        })
+                                except:
+                                    pass
+                                try:
+                                    for group in plugin_config.get('group_ids'):
+                                        await bot.call_api('send_group_msg', **{
+                                            'group_id': group,
+                                            'message': response
+                                        })
+                                except:
+                                    pass
+                                time.sleep(1)
                         if confirm or rapport_confirm:
                             try:
                                 for qq in plugin_config.get('user_ids'):
                                     await bot.call_api('send_private_msg', **{
                                         'user_id': qq,
                                         'message': MessageSegment.image(f"https://www.emrpg.com/{image}")
                                     })
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.8/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.9/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-lostark-wandering-trader
-Version: 0.0.8
+Version: 0.0.9
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: EmiyaGm <464723943@qq.com>
 License: MIT License
         
         Copyright (c) 2023 EmiyaGm
@@ -61,14 +61,17 @@
   </a>
   <a href="https://pypi.python.org/pypi/nonebot-plugin-lostark-wandering-trader">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-lostark-wandering-trader.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 </p>
 
+## 重要提示
+因为国服更新了韩服最近的流浪商人机制，已经不再需要提示了，所以本插件暂停更新
+
 ## 安装
 
 ```bash
 nb plugin install nonebot_plugin_lostark_wandering_trader
 ```
 或者
 ```bash
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot-plugin-lostark-wandering-trader Version:
-0.0.8 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.9 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: EmiyaGm <464723943@qq.com> License: MIT License Copyright (c)
 2023 EmiyaGm Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -23,14 +23,16 @@
 Independent Requires-Python: >=3.8,<4.0 Description-Content-Type: text/markdown
 License-File: LICENSE
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
             èªå¨æ­æ¥ç¨æåå¶ä»¥ä¸å¡çå·æ° æä»¶ â¨_
                            [license] [pypi] [python]
+## éè¦æç¤º
+å ä¸ºå½ææ´æ°äºé©ææè¿çæµæµªåäººæºå¶ï¼å·²ç»ä¸åéè¦æç¤ºäºï¼æä»¥æ¬æä»¶æåæ´æ°
 ## å®è£ ```bash nb plugin install nonebot_plugin_lostark_wandering_trader ```
 æè ```bash pip install nonebot-plugin-lostark-wandering-trader ``` ##
 æ´æ° ```bash nb plugin update nonebot_plugin_lostark_wandering_trader ```
 æè ```bash pip install nonebot-plugin-lostark-wandering-trader -U ``` ###
 å¯¼å¥æä»¶ - å¨`pyproject.toml`éç`[tool.nonebot]`ä¸­æ·»å `plugins =
 ["nonebot_plugin_lostark_wandering_trader"]`
 **æ³¨**ï¼å¦æä½ ä½¿ç¨`nb`å®è£æä»¶ï¼åä¸éè¦è®¾ç½®æ­¤é¡¹ ##
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.8/pyproject.toml` & `nonebot_plugin_lostark_wandering_trader-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot_plugin_lostark_wandering_trader"
-version = "0.0.8"
+version = "0.0.9"
 description = "NoneBot lostark cn wandering trader plugin"
 authors = [
     {name = "EmiyaGm", email = "464723943@qq.com"},
 ]
 dependencies = [
     "httpx<1.0.0,>=0.18.0",
     "nonebot_plugin_apscheduler>=0.3.0",
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.8/setup.py` & `nonebot_plugin_lostark_wandering_trader-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = "NoneBot lostark cn wandering trader plugin"
 
 setuptools.setup(
     name="nonebot_plugin_lostark_wandering_trader",
-    version="0.0.8",
+    version="0.0.9",
     license='MIT',
     author="EmiyaGm",
     author_email="464723943@qq.com",
     description="NoneBot lostark cn wandering trader plugin",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader",
```

