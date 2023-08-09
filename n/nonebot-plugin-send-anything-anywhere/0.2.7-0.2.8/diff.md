# Comparing `tmp/nonebot_plugin_send_anything_anywhere-0.2.7.tar.gz` & `tmp/nonebot_plugin_send_anything_anywhere-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.2.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_send_anything_anywhere-0.2.8.tar", max compression
```

## Comparing `nonebot_plugin_send_anything_anywhere-0.2.7.tar` & `nonebot_plugin_send_anything_anywhere-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1066 2023-06-07 18:09:50.279991 nonebot_plugin_send_anything_anywhere-0.2.7/LICENSE
--rw-r--r--   0        0        0     5946 2023-06-07 18:09:50.279991 nonebot_plugin_send_anything_anywhere-0.2.7/README.md
--rw-r--r--   0        0        0     1486 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/__init__.py
--rw-r--r--   0        0        0      181 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/__init__.py
--rw-r--r--   0        0        0     5355 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/kaiheila.py
--rw-r--r--   0        0        0     5537 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/onebot_v11.py
--rw-r--r--   0        0        0     8274 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/onebot_v12.py
--rw-r--r--   0        0        0     5923 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/qqguild.py
--rw-r--r--   0        0        0     5150 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/telegram.py
--rw-r--r--   0        0        0      189 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/types/__init__.py
--rw-r--r--   0        0        0     1972 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/types/common_message_segment.py
--rw-r--r--   0        0        0     1148 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/types/custom_message_segment.py
--rw-r--r--   0        0        0     1847 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/__init__.py
--rw-r--r--   0        0        0     2084 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/auto_select_bot.py
--rw-r--r--   0        0        0      707 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/const.py
--rw-r--r--   0        0        0      492 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/exceptions.py
--rw-r--r--   0        0        0      429 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/helpers.py
--rw-r--r--   0        0        0     6271 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/platform_send_target.py
--rw-r--r--   0        0        0    16654 2023-06-07 18:09:50.283991 nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/types.py
--rw-r--r--   0        0        0     1756 2023-06-07 18:09:50.287991 nonebot_plugin_send_anything_anywhere-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.7/setup.py
--rw-r--r--   0        0        0     7047 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-09 03:09:27.622110 nonebot_plugin_send_anything_anywhere-0.2.8/LICENSE
+-rw-r--r--   0        0        0     5937 2023-08-09 03:09:27.622110 nonebot_plugin_send_anything_anywhere-0.2.8/README.md
+-rw-r--r--   0        0        0     1790 2023-08-09 03:09:27.622110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/__init__.py
+-rw-r--r--   0        0        0      212 2023-08-09 03:09:27.622110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/__init__.py
+-rw-r--r--   0        0        0     4943 2023-08-09 03:09:27.622110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/feishu.py
+-rw-r--r--   0        0        0     5355 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/kaiheila.py
+-rw-r--r--   0        0        0     8161 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/onebot_v11.py
+-rw-r--r--   0        0        0    12544 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     6929 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/qqguild.py
+-rw-r--r--   0        0        0     5150 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/telegram.py
+-rw-r--r--   0        0        0      259 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/types/__init__.py
+-rw-r--r--   0        0        0     1972 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/types/common_message_segment.py
+-rw-r--r--   0        0        0     1148 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/types/custom_message_segment.py
+-rw-r--r--   0        0        0     2571 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/__init__.py
+-rw-r--r--   0        0        0     2090 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/auto_select_bot.py
+-rw-r--r--   0        0        0      801 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/const.py
+-rw-r--r--   0        0        0      492 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/exceptions.py
+-rw-r--r--   0        0        0      429 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/helpers.py
+-rw-r--r--   0        0        0     7931 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/platform_send_target.py
+-rw-r--r--   0        0        0    16658 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/types.py
+-rw-r--r--   0        0        0     1790 2023-08-09 03:09:27.626110 nonebot_plugin_send_anything_anywhere-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6941 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.8/setup.py
+-rw-r--r--   0        0        0     7038 1970-01-01 00:00:00.000000 nonebot_plugin_send_anything_anywhere-0.2.8/PKG-INFO
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/LICENSE` & `nonebot_plugin_send_anything_anywhere-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/README.md` & `nonebot_plugin_send_anything_anywhere-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,21 +96,21 @@
 | 文字 |     ✅     |     ✅     |    ✅    |   ✅   |
 | 图片 |     ✅     |     ✅     |    ✅    |   ✅   |
 |  at  |     ✅     |     ✅     |    ✅    |   ✅   |
 | 回复 |     ✅     |     ✅     |    ✅    |   ✅   |
 
 ### 支持的发送目标
 
-|                   | OneBot v11 | OneBot v12  | QQ Guild | Kaiheila |
-| :---------------: | :--------: | :---------: | :------: | :------: |
-|       QQ 群       |     ✅     |     ✅      |          |          |
-|      QQ 私聊      |     ✅     |     ✅      |          |          |
-| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |          |
-|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |          |
-|  开黑啦私聊/频道  |            |             |          |    ✅    |
+|                   | OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |
+| :---------------: | :--------: | :--------: | :------: | :------: |
+|       QQ 群       |     ✅     |     ✅     |          |          |
+|      QQ 私聊      |     ✅     |     ✅     |          |          |
+| QQ 频道子频道消息 |            |     ✅     |    ✅    |          |
+|    QQ 频道私聊    |            |     ✅     |    ✅    |          |
+|  开黑啦私聊/频道  |            |            |          |    ✅    |
 
 注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用
 
 ## 问题与例子
 
 因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/kaiheila.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/onebot_v11.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/telegram.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,164 @@
+from io import BytesIO
+from typing import cast
+from pathlib import Path
 from functools import partial
-from typing import Any, Dict, List, Optional
 
-from nonebot.adapters import Bot, Event
+import anyio
+from nonebot.adapters import Event
 
 from ..types import Text, Image, Reply, Mention
 from ..utils import (
-    TargetQQGroup,
     MessageFactory,
-    PlatformTarget,
-    TargetQQPrivate,
     SupportedAdapters,
-    SupportedPlatform,
+    TargetTelegramForum,
+    TargetTelegramCommon,
     MessageSegmentFactory,
-    AggregatedMessageFactory,
     register_sender,
     register_ms_adapter,
-    register_list_targets,
-    register_convert_to_arg,
     assamble_message_factory,
     register_target_extractor,
 )
 
 try:
-    from nonebot.adapters.onebot.v11 import Bot as BotOB11
-    from nonebot.adapters.onebot.v11.message import Message, MessageSegment
-    from nonebot.adapters.onebot.v11 import (
+    from nonebot.adapters.telegram import Bot as BotTG
+    from nonebot.adapters.telegram.message import File, Entity
+    from nonebot.adapters.telegram import Message, MessageSegment
+    from nonebot.adapters.telegram.event import (
         MessageEvent,
+        ChannelPostEvent,
         GroupMessageEvent,
         PrivateMessageEvent,
+        ForumTopicMessageEvent,
     )
 
-    adapter = SupportedAdapters.onebot_v11
-    register_onebot_v11 = partial(register_ms_adapter, adapter)
+    adapter = SupportedAdapters.telegram
+    register_telegram = partial(register_ms_adapter, adapter)
 
-    MessageFactory.register_adapter_message(SupportedAdapters.onebot_v11, Message)
+    MessageFactory.register_adapter_message(SupportedAdapters.telegram, Message)
 
-    @register_onebot_v11(Text)
+    @register_telegram(Text)
     def _text(t: Text) -> MessageSegment:
-        return MessageSegment.text(t.data["text"])
+        return Entity.text(t.data["text"])
 
-    @register_onebot_v11(Image)
+    @register_telegram(Image)
     async def _image(i: Image) -> MessageSegment:
-        return MessageSegment.image(i.data["image"])
+        image = i.data["image"]
+        if isinstance(image, Path):
+            image = await anyio.Path(image).read_bytes()
+        if isinstance(image, BytesIO):
+            image = image.getvalue()
+        return File.photo(image)
 
-    @register_onebot_v11(Mention)
+    @register_telegram(Mention)
     async def _mention(m: Mention) -> MessageSegment:
-        return MessageSegment.at(m.data["user_id"])
+        user_id = m.data["user_id"]
+        return (
+            Entity.mention(f"{user_id} ")
+            if user_id.startswith("@")
+            else Entity.text_link("用户 ", f"tg://user?id={user_id}")
+        )
 
-    @register_onebot_v11(Reply)
+    @register_telegram(Reply)
     async def _reply(r: Reply) -> MessageSegment:
-        return MessageSegment.reply(int(r.data["message_id"]))
+        return MessageSegment("reply", cast(dict, r.data))
 
     @register_target_extractor(PrivateMessageEvent)
-    def _extract_private_msg_event(event: Event) -> TargetQQPrivate:
-        assert isinstance(event, PrivateMessageEvent)
-        return TargetQQPrivate(user_id=event.user_id)
-
     @register_target_extractor(GroupMessageEvent)
-    def _extract_group_msg_event(event: Event) -> TargetQQGroup:
-        assert isinstance(event, GroupMessageEvent)
-        return TargetQQGroup(group_id=event.group_id)
-
-    @register_convert_to_arg(adapter, SupportedPlatform.qq_private)
-    def _gen_private(target: PlatformTarget) -> Dict[str, Any]:
-        assert isinstance(target, TargetQQPrivate)
-        return {
-            "message_type": "private",
-            "user_id": target.user_id,
-        }
-
-    @register_convert_to_arg(adapter, SupportedPlatform.qq_group)
-    def _gen_group(target: PlatformTarget) -> Dict[str, Any]:
-        assert isinstance(target, TargetQQGroup)
-        return {
-            "message_type": "group",
-            "group_id": target.group_id,
-        }
+    @register_target_extractor(ChannelPostEvent)
+    def _extract_private_msg_event(event: Event) -> TargetTelegramCommon:
+        assert isinstance(event, MessageEvent)
+        return TargetTelegramCommon(chat_id=event.chat.id)
+
+    @register_target_extractor(ForumTopicMessageEvent)
+    def _extract_forum_msg_event(event: Event) -> TargetTelegramForum:
+        assert isinstance(event, ForumTopicMessageEvent)
+        return TargetTelegramForum(
+            chat_id=event.chat.id,
+            message_thread_id=event.message_thread_id,
+        )
+
+    def build_mention_from_event(event: MessageEvent) -> MessageSegment:
+        # has user
+        if isinstance(
+            event,
+            (PrivateMessageEvent, GroupMessageEvent, ForumTopicMessageEvent),
+        ):
+            user = event.from_
+
+            # has username
+            if username := user.username:
+                return Entity.mention(f"@{username} ")
+
+            # no username
+            last_name = f" {user.last_name}" if user.last_name else ""
+            return Entity.text_link(
+                f"{user.first_name}{last_name} ",
+                f"tg://user?id={user.id}",
+            )
 
-    @register_sender(SupportedAdapters.onebot_v11)
+        # no user
+        return Entity.text("")
+
+    @register_sender(SupportedAdapters.telegram)
     async def send(
         bot,
         msg: MessageFactory[MessageSegmentFactory],
         target,
         event,
         at_sender: bool,
         reply: bool,
     ):
-        assert isinstance(bot, BotOB11)
-        assert isinstance(target, (TargetQQGroup, TargetQQPrivate))
+        assert isinstance(bot, BotTG)
+        assert isinstance(target, (TargetTelegramCommon, TargetTelegramForum))
+
         if event:
             assert isinstance(event, MessageEvent)
             full_msg = assamble_message_factory(
                 msg,
-                Mention(event.get_user_id()),
+                (
+                    None
+                    if isinstance(event, ChannelPostEvent)
+                    else Mention(event.get_user_id())
+                ),
                 Reply(event.message_id),
                 at_sender,
                 reply,
             )
         else:
             full_msg = msg
+
+        reply_to_message_id = None
         message_to_send = Message()
         for message_segment_factory in full_msg:
-            message_segment = await message_segment_factory.build(bot)
-            message_to_send += message_segment
-        await bot.send_msg(message=message_to_send, **target.arg_dict(bot))
+            if isinstance(message_segment_factory, Reply):
+                reply_to_message_id = int(message_segment_factory.data["message_id"])
+                continue
+
+            if (
+                event
+                and isinstance(message_segment_factory, Mention)
+                and message_segment_factory.data["user_id"] == event.get_user_id()
+            ):
+                message_segment = build_mention_from_event(event)
+            else:
+                message_segment = await message_segment_factory.build(bot)
 
-    @AggregatedMessageFactory.register_aggregated_sender(adapter)
-    async def aggregate_send(
-        bot: Bot,
-        message_factories: List[MessageFactory],
-        target: PlatformTarget,
-        event: Optional[Event],
-    ):
-        assert isinstance(bot, BotOB11)
-        login_info = await bot.get_login_info()
+            message_to_send += message_segment
 
-        msg_list: List[Message] = []
-        for msg_fac in message_factories:
-            msg = await msg_fac.build(bot)
-            assert isinstance(msg, Message)
-            msg_list.append(msg)
-        aggregated_message_segment = Message(
-            [
-                MessageSegment.node_custom(
-                    user_id=login_info["user_id"],
-                    nickname=login_info["nickname"],
-                    content=msg,
-                )
-                for msg in msg_list
-            ]
+        chat_id = target.chat_id
+        message_thread_id = (
+            target.message_thread_id
+            if isinstance(target, TargetTelegramForum)
+            else None
+        )
+        await bot.send_to(
+            chat_id,
+            message_to_send,
+            message_thread_id=message_thread_id,
+            reply_to_message_id=reply_to_message_id,
         )
-
-        if isinstance(target, TargetQQGroup):
-            await bot.send_group_forward_msg(
-                group_id=target.group_id, messages=aggregated_message_segment
-            )
-        elif isinstance(target, TargetQQPrivate):
-            await bot.send_private_forward_msg(
-                user_id=target.user_id, messages=aggregated_message_segment
-            )
-        else:  # pragma: no cover
-            raise RuntimeError(f"{target.__class__.__name__} not supported")
-
-    @register_list_targets(SupportedAdapters.onebot_v11)
-    async def list_targets(bot: Bot) -> List[PlatformTarget]:
-        assert isinstance(bot, BotOB11)
-
-        targets = []
-        groups = await bot.get_group_list()
-        for group in groups:
-            group_id = group["group_id"]
-            target = TargetQQGroup(group_id=group_id)
-            targets.append(target)
-
-        # 获取好友列表
-        users = await bot.get_friend_list()
-        for user in users:
-            user_id = user["user_id"]
-            target = TargetQQPrivate(user_id=user_id)
-            targets.append(target)
-
-        return targets
 
 except ImportError:
     pass
-except Exception as e:
-    raise e
+except Exception:
+    raise
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/onebot_v12.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/onebot_v12.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,35 +9,50 @@
 from ..types import Text, Image, Reply, Mention
 from ..utils import (
     TargetQQGroup,
     MessageFactory,
     PlatformTarget,
     TargetQQPrivate,
     TargetOB12Unknow,
+    QQGuildDMSManager,
     SupportedAdapters,
     SupportedPlatform,
+    TargetQQGuildDirect,
     TargetQQGuildChannel,
     MessageSegmentFactory,
     register_sender,
     register_ms_adapter,
+    register_qqguild_dms,
     register_list_targets,
     register_convert_to_arg,
     assamble_message_factory,
     register_target_extractor,
 )
 
 try:
     from nonebot.adapters.onebot.v12.exception import UnsupportedAction
-    from nonebot.adapters.onebot.v12 import (  # ChannelMessageEvent,
+    from nonebot.adapters.onebot.v12 import (
         Bot,
         Message,
         MessageEvent,
         MessageSegment,
         GroupMessageEvent,
+        ChannelCreateEvent,
+        ChannelDeleteEvent,
+        ChannelMessageEvent,
+        FriendDecreaseEvent,
+        FriendIncreaseEvent,
         PrivateMessageEvent,
+        GroupMessageDeleteEvent,
+        GroupMemberDecreaseEvent,
+        GroupMemberIncreaseEvent,
+        ChannelMessageDeleteEvent,
+        PrivateMessageDeleteEvent,
+        ChannelMemberDecreaseEvent,
+        ChannelMemberIncreaseEvent,
     )
 
     adapter = SupportedAdapters.onebot_v12
     register_onebot_v12 = partial(register_ms_adapter, adapter)
 
     MessageFactory.register_adapter_message(adapter, Message)
 
@@ -77,32 +92,100 @@
         return MessageSegment.reply(r.data["message_id"])
 
     @register_target_extractor(PrivateMessageEvent)
     def _extract_private_msg_event(event: Event) -> PlatformTarget:
         assert isinstance(event, PrivateMessageEvent)
         if event.self.platform == "qq":
             return TargetQQPrivate(user_id=int(event.user_id))
-        return TargetOB12Unknow(detail_type="private", user_id=event.user_id)
+        if event.self.platform == "qqguild":
+            event_dict = event.dict()
+            return TargetQQGuildDirect(
+                recipient_id=int(event.user_id),
+                source_guild_id=event_dict["qqguild"]["src_guild_id"],
+            )
+        return TargetOB12Unknow(
+            platform=event.self.platform, detail_type="private", user_id=event.user_id
+        )
 
     @register_target_extractor(GroupMessageEvent)
     def _extract_group_msg_event(event: Event) -> PlatformTarget:
         assert isinstance(event, GroupMessageEvent)
         if event.self.platform == "qq":
             return TargetQQGroup(group_id=int(event.group_id))
-        return TargetOB12Unknow(detail_type="group", group_id=event.group_id)
+        return TargetOB12Unknow(
+            platform=event.self.platform, detail_type="group", group_id=event.group_id
+        )
+
+    @register_target_extractor(ChannelMessageEvent)
+    def _extarct_channel_msg_event(event: Event) -> PlatformTarget:
+        assert isinstance(event, ChannelMessageEvent)
+        if event.self.platform == "qqguild":  # all4one
+            return TargetQQGuildChannel(channel_id=int(event.channel_id))
+        return TargetOB12Unknow(
+            platform=event.self.platform,
+            detail_type="channel",
+            channel_id=event.channel_id,
+            guild_id=event.guild_id,
+        )
+
+    @register_target_extractor(FriendIncreaseEvent)
+    @register_target_extractor(FriendDecreaseEvent)
+    @register_target_extractor(PrivateMessageDeleteEvent)
+    def _extract_private_notice_event(event: Event) -> PlatformTarget:
+        assert isinstance(
+            event, (FriendIncreaseEvent, FriendDecreaseEvent, PrivateMessageDeleteEvent)
+        )
+        if event.self.platform == "qq":
+            return TargetQQPrivate(user_id=int(event.user_id))
+        return TargetOB12Unknow(
+            platform=event.self.platform, detail_type="private", user_id=event.user_id
+        )
+
+    @register_target_extractor(GroupMemberIncreaseEvent)
+    @register_target_extractor(GroupMemberDecreaseEvent)
+    @register_target_extractor(GroupMessageDeleteEvent)
+    def _extract_group_notice_event(event: Event) -> PlatformTarget:
+        assert isinstance(
+            event,
+            (
+                GroupMemberIncreaseEvent,
+                GroupMemberDecreaseEvent,
+                GroupMessageDeleteEvent,
+            ),
+        )
+        if event.self.platform == "qq":
+            return TargetQQGroup(group_id=int(event.group_id))
+        return TargetOB12Unknow(
+            platform=event.self.platform, detail_type="group", group_id=event.group_id
+        )
 
-    # @register_target_extractor(ChannelMessageEvent)
-    # def _extarct_channel_msg_event(event: Event) -> PlatformTarget:
-    #     assert isinstance(event, ChannelMessageEvent)
-    #     if event.self.platform == 'qqguild': # all4one
-    #         return TargetQQGuildChannel(channel_id=int(event.channel_id))
-    #     return TargetOB12Unknow(
-    #         detail_type="channel", channel_id=event.channel_id,
-    #       guild_id=event.guild_id
-    #     )
+    @register_target_extractor(ChannelMemberIncreaseEvent)
+    @register_target_extractor(ChannelMemberDecreaseEvent)
+    @register_target_extractor(ChannelMessageDeleteEvent)
+    @register_target_extractor(ChannelCreateEvent)
+    @register_target_extractor(ChannelDeleteEvent)
+    def _extarct_channel_notice_event(event: Event) -> PlatformTarget:
+        assert isinstance(
+            event,
+            (
+                ChannelMemberIncreaseEvent,
+                ChannelMemberDecreaseEvent,
+                ChannelMessageDeleteEvent,
+                ChannelCreateEvent,
+                ChannelDeleteEvent,
+            ),
+        )
+        if event.self.platform == "qqguild":  # all4one
+            return TargetQQGuildChannel(channel_id=int(event.channel_id))
+        return TargetOB12Unknow(
+            platform=event.self.platform,
+            detail_type="channel",
+            channel_id=event.channel_id,
+            guild_id=event.guild_id,
+        )
 
     @register_convert_to_arg(adapter, SupportedPlatform.qq_group)
     def _to_qq_group(target: PlatformTarget):
         assert isinstance(target, TargetQQGroup)
         return {
             "detail_type": "group",
             "group_id": str(target.group_id),
@@ -112,60 +195,89 @@
     def _to_qq_private(target: PlatformTarget):
         assert isinstance(target, TargetQQPrivate)
         return {
             "detail_type": "private",
             "user_id": str(target.user_id),
         }
 
-    # @register_convert_to_arg(adapter, SupportedPlatform.qq_guild_channel)
-    # def _to_qq_guild_channel(target: PlatformTarget):
-    #     assert isinstance(target, TargetQQGuildChannel)
-    #     return {
-    #             "detail_type": "channel",
-    #             "channel_id": target.channel_id,
-    #             }
-
-    # @register_convert_to_arg(adapter, SupportedPlatform.qq_guild_direct)
-    # def _to_qq_guild_direct(target: PlatformTarget):
-    #     assert isinstance(target, TargetQQGuildDirect)
-    #     return {
-    #             "detail_type": "private",
-    #             "guild_id": target.source_guild_id,
-    #             }
+    @register_convert_to_arg(adapter, SupportedPlatform.qq_guild_channel)
+    def _to_qq_guild_channel(target: PlatformTarget):
+        assert isinstance(target, TargetQQGuildChannel)
+        return {
+            "detail_type": "channel",
+            "channel_id": str(target.channel_id),
+        }
+
+    @register_convert_to_arg(adapter, SupportedPlatform.qq_guild_direct)
+    def _to_qq_guild_direct(target: PlatformTarget):
+        assert isinstance(target, TargetQQGuildDirect)
+        return {
+            "detail_type": "private",
+            "guild_id": str(QQGuildDMSManager.get_guild_id(target)),
+        }
+
+    @register_qqguild_dms(adapter)
+    async def _qqguild_dms(target: TargetQQGuildDirect, bot: BaseBot) -> int:
+        assert isinstance(bot, Bot)
+
+        resp = await bot.create_dms(
+            user_id=str(target.recipient_id), src_guild_id=str(target.source_guild_id)
+        )
+        return resp["guild_id"]
 
     @register_convert_to_arg(adapter, SupportedPlatform.unknown_ob12)
     def _to_unknow(target: PlatformTarget):
         assert isinstance(target, TargetOB12Unknow)
-        return target.dict(exclude={"platform_type"})
+        return target.dict(exclude={"platform", "platform_type"})
 
     @register_sender(SupportedAdapters.onebot_v12)
     async def send(
         bot,
         msg: MessageFactory[MessageSegmentFactory],
         target,
         event,
         at_sender: bool,
         reply: bool,
     ):
         assert isinstance(bot, Bot)
         assert isinstance(
             target,
-            (TargetQQGroup, TargetQQPrivate, TargetQQGuildChannel, TargetOB12Unknow),
+            (
+                TargetQQGroup,
+                TargetQQPrivate,
+                TargetQQGuildChannel,
+                TargetQQGuildDirect,
+                TargetOB12Unknow,
+            ),
         )
 
         if event:
             assert isinstance(event, MessageEvent)
             full_msg = assamble_message_factory(
                 msg, Mention(event.user_id), Reply(event.message_id), at_sender, reply
             )
         else:
             full_msg = msg
         msg_to_send = await full_msg.build(bot)
         assert isinstance(msg_to_send, Message)
-        await bot.send_message(message=msg_to_send, **target.arg_dict(bot))
+        if bot.platform == "qqguild":
+            assert isinstance(target, (TargetQQGuildChannel, TargetQQGuildDirect))
+            if isinstance(target, TargetQQGuildDirect):
+                await QQGuildDMSManager.aget_guild_id(target, bot)
+            params = {}
+            if event:
+                # 传递 event_id，用来支持频道的被动消息
+                params["event_id"] = event.id
+            await bot.send_message(
+                message=msg_to_send,
+                **target.arg_dict(bot),
+                **params,
+            )
+        else:
+            await bot.send_message(message=msg_to_send, **target.arg_dict(bot))
 
     @register_list_targets(SupportedAdapters.onebot_v12)
     async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
         assert isinstance(bot, Bot)
 
         targets = []
         try:
@@ -176,15 +288,17 @@
                     targets.append(TargetQQPrivate(user_id=int(friend["user_id"])))
                 elif platform == "qqguild":
                     # FIXME: 怎么获取 src_guild_id 捏？
                     pass
                 else:
                     targets.append(
                         TargetOB12Unknow(
-                            detail_type="private", user_id=friend["user_id"]
+                            platform=platform,
+                            detail_type="private",
+                            user_id=friend["user_id"],
                         )
                     )
 
         except UnsupportedAction:  # pragma: no cover
             pass
 
         try:
@@ -192,15 +306,17 @@
             for group in groups:
                 platform = bot.platform
                 if platform == "qq":
                     targets.append(TargetQQGroup(group_id=int(group["group_id"])))
                 else:
                     targets.append(
                         TargetOB12Unknow(
-                            detail_type="group", group_id=group["group_id"]
+                            platform=platform,
+                            detail_type="group",
+                            group_id=group["group_id"],
                         )
                     )
 
         except UnsupportedAction:  # pragma: no cover
             pass
 
         try:
@@ -212,14 +328,15 @@
                     if platform == "qqguild":
                         targets.append(
                             TargetQQGuildChannel(channel_id=int(channel["channel_id"]))
                         )
                     else:
                         targets.append(
                             TargetOB12Unknow(
+                                platform=platform,
                                 detail_type="channel",
                                 channel_id=channel["channel_id"],
                                 guild_id=guild["guild_id"],
                             )
                         )
 
         except UnsupportedAction:  # pragma: no cover
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/adapters/qqguild.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/adapters/qqguild.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,31 +4,35 @@
 from nonebot.adapters import Event
 from nonebot.adapters import Bot as BaseBot
 
 from ..types import Text, Image, Reply, Mention
 from ..utils import (
     MessageFactory,
     PlatformTarget,
+    QQGuildDMSManager,
     SupportedAdapters,
     TargetQQGuildDirect,
     TargetQQGuildChannel,
     MessageSegmentFactory,
     register_sender,
     register_ms_adapter,
+    register_qqguild_dms,
     register_list_targets,
     assamble_message_factory,
     register_target_extractor,
 )
 
 try:
     from nonebot.adapters.qqguild import (
         Bot,
         Message,
         MessageEvent,
         MessageSegment,
+        MessageCreateEvent,
+        AtMessageCreateEvent,
         DirectMessageCreateEvent,
     )
 
     adapter = SupportedAdapters.qqguild
     register_qqguild = partial(register_ms_adapter, adapter)
 
     MessageFactory.register_adapter_message(adapter, Message)
@@ -50,25 +54,36 @@
 
     @register_qqguild(Reply)
     def _reply(r: Reply) -> MessageSegment:
         return MessageSegment.reference(r.data["message_id"])
 
     @register_target_extractor(MessageEvent)
     def extract_message_event(event: Event) -> PlatformTarget:
-        assert isinstance(event, MessageEvent)
-        if not event.to_me:
-            assert event.channel_id
-            return TargetQQGuildChannel(channel_id=int(event.channel_id))
-        else:
-            # TODO send dms not support yet
+        if isinstance(event, DirectMessageCreateEvent):
             assert event.guild_id
             assert event.author and event.author.id
             return TargetQQGuildDirect(
                 source_guild_id=event.guild_id, recipient_id=event.author.id
             )
+        elif isinstance(event, (MessageCreateEvent, AtMessageCreateEvent)):
+            assert event.channel_id
+            return TargetQQGuildChannel(channel_id=int(event.channel_id))
+        else:
+            raise ValueError(f"{type(event)} not supported")
+
+    @register_qqguild_dms(adapter)
+    async def get_dms(target: TargetQQGuildDirect, bot: BaseBot) -> int:
+        assert isinstance(bot, Bot)
+
+        dms = await bot.post_dms(
+            recipient_id=str(target.recipient_id),
+            source_guild_id=str(target.source_guild_id),
+        )
+        assert dms.guild_id
+        return dms.guild_id
 
     @register_sender(SupportedAdapters.qqguild)
     async def send(
         bot,
         msg: MessageFactory[MessageSegmentFactory],
         target,
         event,
@@ -140,15 +155,25 @@
                     ark=ark,  # type: ignore
                     image=image,  # type: ignore
                     file_image=file_image,  # type: ignore
                     markdown=markdown,  # type: ignore
                     message_reference=reference,  # type: ignore
                 )
             else:
-                raise NotImplementedError("QQ频道主动发送私信暂未实现")
+                guild_id = await QQGuildDMSManager.aget_guild_id(target, bot)
+                await bot.post_dms_messages(
+                    guild_id=guild_id,  # type: ignore
+                    content=content,
+                    embed=embed,  # type: ignore
+                    ark=ark,  # type: ignore
+                    image=image,  # type: ignore
+                    file_image=file_image,  # type: ignore
+                    markdown=markdown,  # type: ignore
+                    message_reference=reference,  # type: ignore
+                )
 
     @register_list_targets(SupportedAdapters.qqguild)
     async def list_targets(bot: BaseBot) -> List[PlatformTarget]:
         assert isinstance(bot, Bot)
 
         targets = []
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/types/common_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/types/common_message_segment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/types/custom_message_segment.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/types/custom_message_segment.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/auto_select_bot.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/auto_select_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     return wrapper
 
 
 async def refresh_bots():
     """刷新缓存的 Bot 数据"""
     BOT_CACHE.clear()
-    for bot in get_bots().values():
+    for bot in list(get_bots().values()):
         adapter_name = extract_adapter_type(bot)
         if list_targets := list_targets_map.get(adapter_name):
             targets = await list_targets(bot)
             for target in targets:
                 BOT_CACHE[target].append(bot)
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/const.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 
 class SupportedAdapters(StrEnum):
     onebot_v11 = "OneBot V11"
     onebot_v12 = "OneBot V12"
     qqguild = "QQ Guild"
     kaiheila = "Kaiheila"
     telegram = "Telegram"
+    feishu = "Feishu"
 
     fake = "fake"  # for nonebug
 
 
 class SupportedPlatform(StrEnum):
     qq_group = "QQ Group"
     qq_private = "QQ Private"
     qq_guild_channel = "QQ Guild Channel"
     qq_guild_direct = "QQ Guild Direct"
     kaiheila_channel = "Kaiheila Channel"
     kaiheila_private = "Kaiheila Private"
     unknown_ob12 = "Unknow Onebot 12 Platform"
     telegram_common = "Telegram Common"
     telegram_forum = "Telegram Forum"
+    feishu_private = "Feishu Private"
+    feishu_group = "Feishu Group"
 
 
 supported_adapter_names = set(SupportedAdapters._member_map_.values())  # noqa: SLF001
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/platform_send_target.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/platform_send_target.py`

 * *Files 17% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         detail_type: "private" or "group" or "channel"
         user_id, group_id, channel_id, guild_id: 同 ob12 定义
     """
 
     platform_type: Literal[
         SupportedPlatform.unknown_ob12
     ] = SupportedPlatform.unknown_ob12
+    platform: str
     detail_type: Literal["private", "group", "channel"]
     user_id: Optional[str] = None
     group_id: Optional[str] = None
     guild_id: Optional[str] = None
     channel_id: Optional[str] = None
 
 
@@ -178,25 +179,53 @@
     platform_type: Literal[
         SupportedPlatform.telegram_forum
     ] = SupportedPlatform.telegram_forum
     chat_id: int
     message_thread_id: int
 
 
+class TargetFeishuPrivate(PlatformTarget):
+    """飞书私聊
+
+    参数
+        open_id: 用户 Open ID
+    """
+
+    platform_type: Literal[
+        SupportedPlatform.feishu_private
+    ] = SupportedPlatform.feishu_private
+    open_id: str
+
+
+class TargetFeishuGroup(PlatformTarget):
+    """飞书群聊
+
+    参数
+        chat_id: 群 ID
+    """
+
+    platform_type: Literal[
+        SupportedPlatform.feishu_group
+    ] = SupportedPlatform.feishu_group
+    chat_id: str
+
+
 # this union type is for deserialize pydantic model with nested PlatformTarget
 AllSupportedPlatformTarget = Union[
     TargetQQGroup,
     TargetQQPrivate,
     TargetQQGuildChannel,
     TargetQQGuildDirect,
     TargetKaiheilaPrivate,
     TargetKaiheilaChannel,
     TargetOB12Unknow,
     TargetTelegramCommon,
     TargetTelegramForum,
+    TargetFeishuPrivate,
+    TargetFeishuGroup,
 ]
 
 
 ConvertToArg = Callable[[PlatformTarget], Dict[str, Any]]
 convert_to_arg_map: Dict[Tuple[SupportedPlatform, SupportedAdapters], ConvertToArg] = {}
 
 
@@ -248,7 +277,43 @@
 
 def register_sender(adapter: SupportedAdapters):
     def wrapper(sender: Sender):
         sender_map[adapter] = sender
         return sender
 
     return wrapper
+
+
+QQGuild_DMS = Callable[[TargetQQGuildDirect, Bot], Awaitable[int]]
+qqguild_dms_map: Dict[SupportedAdapters, QQGuild_DMS] = {}
+
+
+def register_qqguild_dms(adapter: SupportedAdapters):
+    def wrapper(func: QQGuild_DMS):
+        qqguild_dms_map[adapter] = func
+        return func
+
+    return wrapper
+
+
+class QQGuildDMSManager:
+    _cache: ClassVar[Dict[TargetQQGuildDirect, int]] = {}
+
+    @classmethod
+    def get_guild_id(cls, target: TargetQQGuildDirect) -> int:
+        """从缓存中获取私聊所需 guild_id"""
+        return cls._cache[target]
+
+    @classmethod
+    async def aget_guild_id(cls, target: TargetQQGuildDirect, bot: Bot) -> int:
+        """获取私聊所需 guild_id"""
+        if target in cls._cache:
+            return cls._cache[target]
+
+        adapter = extract_adapter_type(bot)
+        if not (qqguild_dms := qqguild_dms_map.get(adapter)):
+            raise RuntimeError(
+                f"qqguild dms method for {adapter} not registered",
+            )  # pragma: no cover
+        guild_id = await qqguild_dms(target, bot)
+        cls._cache[target] = guild_id
+        return guild_id
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/nonebot_plugin_saa/utils/types.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/nonebot_plugin_saa/utils/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
         bot: Bot,
         target: PlatformTarget,
         event: Optional[Event],
         at_sender: bool,
         reply: bool,
     ):
         adapter = extract_adapter_type(bot)
-        if not (sender := sender_map[adapter]):
+        if not (sender := sender_map.get(adapter)):
             raise RuntimeError(
                 f"send method for {adapter} not registered",
             )  # pragma: no cover
         await sender(bot, self, target, event, at_sender, reply)
 
 
 AggregatedSender = Callable[
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/pyproject.toml` & `nonebot_plugin_send_anything_anywhere-0.2.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-send-anything-anywhere"
-version = "0.2.7"
+version = "0.2.8"
 description = "An adaptor for nonebot2 adaptors"
 authors = ["felinae98 <731499577@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_saa" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -39,14 +39,15 @@
 optional = true
 
 [tool.poetry.group.adapters.dependencies]
 nonebot-adapter-onebot = "^2.2.2"
 nonebot-adapter-qqguild = ">=0.2.1"
 nonebot-adapter-kaiheila = { version = "^0.2.4", python = ">=3.9" }
 nonebot-adapter-telegram = "^0.1.0b12"
+nonebot-adapter-feishu = "^2.0.1"
 
 [tool.black]
 line-length = 88
 target-version = ["py38", "py39", "py310"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/setup.py` & `nonebot_plugin_send_anything_anywhere-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['anyio>=3.6.2,<4.0.0',
  'nonebot2>=2.0.0,<3.0.0',
  'pydantic>=1.10.5,<2.0.0',
  'strenum>=0.4.8,<0.5.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-send-anything-anywhere',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': 'An adaptor for nonebot2 adaptors',
-    'long_description': '<div align="center">\n\n~logo征集中，假装有图片~\n\n# Nonebot Plugin<br>Send Anything Anywhere\n\n你只管业务实现，把发送交给我们\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/felinae98/nonebot-plugin-send-anything-anywhere/test.yml)\n![Codecov](https://img.shields.io/codecov/c/github/felinae98/nonebot-plugin-send-anything-anywhere)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nonebot-plugin-send-anything-anywhere)\n![PyPI](https://img.shields.io/pypi/v/nonebot-plugin-send-anything-anywhere)\n![GitHub](https://img.shields.io/github/license/felinae98/nonebot-plugin-send-anything-anywhere)\n\n</div>\n\n这个插件可以做什么\n\n- 为常见的消息类型提供抽象类，自适应转换成对应 adapter 的消息\n- 提供一套统一的，符合直觉的发送接口\n- 为复杂的消息提供易用的生成接口（规划中）\n\n本插件通过传入 bot 的类型来自适应生成对应 bot adapter 所使用的 Message\n\n## 安装\n\n- 使用 nb-cli 安装  \n  `nb plugin install nonebot-plugin-send-anything-anywhere`\n- 使用 poetry 安装  \n  `poetry add nonebot-plugin-send-anything-anywhere`\n- 使用 pip 安装  \n  `pip install nonebot-plugin-send-anything-anywhere`\n\n## 使用\n\n在 handler 中回复消息的情况：\n\n```python\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    # 直接调用 MessageFactory.send() 在 handler 中回复消息\n    await MessageFactory("你好").send(reply=True, at_sender=True)\n    await MessageFactory("需要回复的内容").send()\n    await matcher.finish()\n```\n\n主动发送的情况：\n\n```python\nfrom nonebot_plugin_saa import TargetQQGroup\n\n# 发送目标为 QQ 号 10000, 以私聊形式发送\ntarget = TargetQQGroup(group_id=2233)\nawait MessageFactory("早上好").send_to(target)\n```\n\n从消息事件中提取发送目标:\n\n```python\nfrom nonebot_plugin_saa import extract_target, get_target\n\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    target = extract_target(event)\n\n@matcher.handle()\nasync def handle(target: PlatformTarget = Depends(get_target)):\n    ...\n```\n\n发送目标的序列化与反序列化:\n\n```python\nfrom nonebot_plugin_saa import PlatformTarget, TargetQQPrivate\n\ntarget = TargetQQPrivate(user_id=112233)\nserialized_target = target.json()\ndeserialized_target = PlatformTarget.deserialize(serialized_target)\nassert deserialized_target == target\n```\n\n## 支持情况\n\n✅:支持 ✖️:支持不了 🚧:等待适配\n\n### 支持的 adapter\n\n| OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |\n| :--------: | :--------: | :------: | :------: |\n|     ✅     |     ✅     |    ✅    |    ✅    |\n\n### 支持的消息类型\n\n|      | OneBot v11 | OneBot v12 | QQ Guild | 开黑啦 |\n| :--: | :--------: | :--------: | :------: | :----: |\n| 文字 |     ✅     |     ✅     |    ✅    |   ✅   |\n| 图片 |     ✅     |     ✅     |    ✅    |   ✅   |\n|  at  |     ✅     |     ✅     |    ✅    |   ✅   |\n| 回复 |     ✅     |     ✅     |    ✅    |   ✅   |\n\n### 支持的发送目标\n\n|                   | OneBot v11 | OneBot v12  | QQ Guild | Kaiheila |\n| :---------------: | :--------: | :---------: | :------: | :------: |\n|       QQ 群       |     ✅     |     ✅      |          |          |\n|      QQ 私聊      |     ✅     |     ✅      |          |          |\n| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |          |\n|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |          |\n|  开黑啦私聊/频道  |            |             |          |    ✅    |\n\n注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用\n\n## 问题与例子\n\n因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的\n\nbefore:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v11.message import MessageSegment as V11MessageSegment\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.adapters.onebot.v12.message import MessageSegment as V12MessageSegment\nfrom nonebot.adapters.onebot.v12.bot import Bot as V12Bot\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v11(event: V11MessageEvent):\n    pic_content = ...\n    msg = V11MessageSegment.image(pic_content) + V11MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n\npic_matcher.handle()\nasync def _handle_v12(bot: V12Bot, event: V12MessageEvent):\n    pic_content = ...\n    pic_file = await bot.upload_file(type=\'data\', name=\'image\', data=pic_content)\n    msg = V12MessageSegment.image(pic_file[\'file_id\']) + V12MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n```\n\n现在只需要:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.internal.adapter.bot import Bot\nfrom nonebot_plugin_saa import Image, Text, MessageFactory\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v12(bot: Bot, event: Union[V12MessageEvent, V11MessageEvent]):\n    pic_content = ...\n    msg_builder = MessageFactory([\n        Image(pic_content), Text("这是你要的图片")\n    ])\n    # or msg_builder = Image(pic_content) + Text("这是你要的图片")\n    await msg_builder.send()\n    await pic_matcher.finish()\n```\n\n## 类似项目\n\n- [nonebot-plugin-all4one](https://github.com/nonepkg/nonebot-plugin-all4one) 解决了类似的问题，但是用了不同路径\n- [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 通过 Rule 定制订阅的平台，与本插件联合使用也许会有奇效\n\n## License\n\nMIT\n',
+    'long_description': '<div align="center">\n\n~logo征集中，假装有图片~\n\n# Nonebot Plugin<br>Send Anything Anywhere\n\n你只管业务实现，把发送交给我们\n\n![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/felinae98/nonebot-plugin-send-anything-anywhere/test.yml)\n![Codecov](https://img.shields.io/codecov/c/github/felinae98/nonebot-plugin-send-anything-anywhere)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nonebot-plugin-send-anything-anywhere)\n![PyPI](https://img.shields.io/pypi/v/nonebot-plugin-send-anything-anywhere)\n![GitHub](https://img.shields.io/github/license/felinae98/nonebot-plugin-send-anything-anywhere)\n\n</div>\n\n这个插件可以做什么\n\n- 为常见的消息类型提供抽象类，自适应转换成对应 adapter 的消息\n- 提供一套统一的，符合直觉的发送接口\n- 为复杂的消息提供易用的生成接口（规划中）\n\n本插件通过传入 bot 的类型来自适应生成对应 bot adapter 所使用的 Message\n\n## 安装\n\n- 使用 nb-cli 安装  \n  `nb plugin install nonebot-plugin-send-anything-anywhere`\n- 使用 poetry 安装  \n  `poetry add nonebot-plugin-send-anything-anywhere`\n- 使用 pip 安装  \n  `pip install nonebot-plugin-send-anything-anywhere`\n\n## 使用\n\n在 handler 中回复消息的情况：\n\n```python\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    # 直接调用 MessageFactory.send() 在 handler 中回复消息\n    await MessageFactory("你好").send(reply=True, at_sender=True)\n    await MessageFactory("需要回复的内容").send()\n    await matcher.finish()\n```\n\n主动发送的情况：\n\n```python\nfrom nonebot_plugin_saa import TargetQQGroup\n\n# 发送目标为 QQ 号 10000, 以私聊形式发送\ntarget = TargetQQGroup(group_id=2233)\nawait MessageFactory("早上好").send_to(target)\n```\n\n从消息事件中提取发送目标:\n\n```python\nfrom nonebot_plugin_saa import extract_target, get_target\n\n@matcher.handle()\nasync def handle(event: MessageEvent):\n    target = extract_target(event)\n\n@matcher.handle()\nasync def handle(target: PlatformTarget = Depends(get_target)):\n    ...\n```\n\n发送目标的序列化与反序列化:\n\n```python\nfrom nonebot_plugin_saa import PlatformTarget, TargetQQPrivate\n\ntarget = TargetQQPrivate(user_id=112233)\nserialized_target = target.json()\ndeserialized_target = PlatformTarget.deserialize(serialized_target)\nassert deserialized_target == target\n```\n\n## 支持情况\n\n✅:支持 ✖️:支持不了 🚧:等待适配\n\n### 支持的 adapter\n\n| OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |\n| :--------: | :--------: | :------: | :------: |\n|     ✅     |     ✅     |    ✅    |    ✅    |\n\n### 支持的消息类型\n\n|      | OneBot v11 | OneBot v12 | QQ Guild | 开黑啦 |\n| :--: | :--------: | :--------: | :------: | :----: |\n| 文字 |     ✅     |     ✅     |    ✅    |   ✅   |\n| 图片 |     ✅     |     ✅     |    ✅    |   ✅   |\n|  at  |     ✅     |     ✅     |    ✅    |   ✅   |\n| 回复 |     ✅     |     ✅     |    ✅    |   ✅   |\n\n### 支持的发送目标\n\n|                   | OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |\n| :---------------: | :--------: | :--------: | :------: | :------: |\n|       QQ 群       |     ✅     |     ✅     |          |          |\n|      QQ 私聊      |     ✅     |     ✅     |          |          |\n| QQ 频道子频道消息 |            |     ✅     |    ✅    |          |\n|    QQ 频道私聊    |            |     ✅     |    ✅    |          |\n|  开黑啦私聊/频道  |            |            |          |    ✅    |\n\n注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用\n\n## 问题与例子\n\n因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的\n\nbefore:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v11.message import MessageSegment as V11MessageSegment\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.adapters.onebot.v12.message import MessageSegment as V12MessageSegment\nfrom nonebot.adapters.onebot.v12.bot import Bot as V12Bot\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v11(event: V11MessageEvent):\n    pic_content = ...\n    msg = V11MessageSegment.image(pic_content) + V11MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n\npic_matcher.handle()\nasync def _handle_v12(bot: V12Bot, event: V12MessageEvent):\n    pic_content = ...\n    pic_file = await bot.upload_file(type=\'data\', name=\'image\', data=pic_content)\n    msg = V12MessageSegment.image(pic_file[\'file_id\']) + V12MessageSegment.text("这是你要的图片")\n    await pic_matcher.finish(msg)\n```\n\n现在只需要:\n\n```python\nfrom nonebot.adapters.onebot.v11.event import MessageEvent as V11MessageEvent\nfrom nonebot.adapters.onebot.v12.event import MessageEvent as V12MessageEvent\nfrom nonebot.internal.adapter.bot import Bot\nfrom nonebot_plugin_saa import Image, Text, MessageFactory\n\npic_matcher = nonebot.on_command(\'发送图片\')\n\npic_matcher.handle()\nasync def _handle_v12(bot: Bot, event: Union[V12MessageEvent, V11MessageEvent]):\n    pic_content = ...\n    msg_builder = MessageFactory([\n        Image(pic_content), Text("这是你要的图片")\n    ])\n    # or msg_builder = Image(pic_content) + Text("这是你要的图片")\n    await msg_builder.send()\n    await pic_matcher.finish()\n```\n\n## 类似项目\n\n- [nonebot-plugin-all4one](https://github.com/nonepkg/nonebot-plugin-all4one) 解决了类似的问题，但是用了不同路径\n- [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 通过 Rule 定制订阅的平台，与本插件联合使用也许会有奇效\n\n## License\n\nMIT\n',
     'author': 'felinae98',
     'author_email': '731499577@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `nonebot_plugin_send_anything_anywhere-0.2.7/PKG-INFO` & `nonebot_plugin_send_anything_anywhere-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-send-anything-anywhere
-Version: 0.2.7
+Version: 0.2.8
 Summary: An adaptor for nonebot2 adaptors
 License: MIT
 Author: felinae98
 Author-email: 731499577@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -124,21 +124,21 @@
 | 文字 |     ✅     |     ✅     |    ✅    |   ✅   |
 | 图片 |     ✅     |     ✅     |    ✅    |   ✅   |
 |  at  |     ✅     |     ✅     |    ✅    |   ✅   |
 | 回复 |     ✅     |     ✅     |    ✅    |   ✅   |
 
 ### 支持的发送目标
 
-|                   | OneBot v11 | OneBot v12  | QQ Guild | Kaiheila |
-| :---------------: | :--------: | :---------: | :------: | :------: |
-|       QQ 群       |     ✅     |     ✅      |          |          |
-|      QQ 私聊      |     ✅     |     ✅      |          |          |
-| QQ 频道子频道消息 |            | 🚧(all4one) |    ✅    |          |
-|    QQ 频道私聊    |            | 🚧(all4one) |    ✅    |          |
-|  开黑啦私聊/频道  |            |             |          |    ✅    |
+|                   | OneBot v11 | OneBot v12 | QQ Guild | Kaiheila |
+| :---------------: | :--------: | :--------: | :------: | :------: |
+|       QQ 群       |     ✅     |     ✅     |          |          |
+|      QQ 私聊      |     ✅     |     ✅     |          |          |
+| QQ 频道子频道消息 |            |     ✅     |    ✅    |          |
+|    QQ 频道私聊    |            |     ✅     |    ✅    |          |
+|  开黑啦私聊/频道  |            |            |          |    ✅    |
 
 注：对于使用 Onebot v12，但是没有专门适配的发送目标，使用了 TargetOB12Unknow 来保证其可以正常使用
 
 ## 问题与例子
 
 因为在现在的 Nonebot 插件开发中，消息的构建和发送是和 adapter 高度耦合的，这导致一个插件要适配不同的 adapter 是困难的
```

