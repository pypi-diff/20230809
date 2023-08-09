# Comparing `tmp/dgg-bot-1.1.0.tar.gz` & `tmp/dgg-bot-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgg-bot-1.1.0.tar", last modified: Sun May 28 00:28:32 2023, max compression
+gzip compressed data, was "dgg-bot-1.2.0.tar", last modified: Wed Aug  9 02:41:50 2023, max compression
```

## Comparing `dgg-bot-1.1.0.tar` & `dgg-bot-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.699719 dgg-bot-1.1.0/
--rw-rw-rw-   0        0        0     1081 2022-09-09 16:56:19.000000 dgg-bot-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3886 2023-05-28 00:28:32.699719 dgg-bot-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2023-05-26 14:19:48.000000 dgg-bot-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.663973 dgg-bot-1.1.0/dgg_bot.egg-info/
--rw-rw-rw-   0        0        0     3886 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 00:28:32.000000 dgg-bot-1.1.0/dgg_bot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.691721 dgg-bot-1.1.0/dggbot/
--rw-rw-rw-   0        0        0      479 2023-05-28 00:19:50.000000 dgg-bot-1.1.0/dggbot/__init__.py
--rw-rw-rw-   0        0        0      504 2022-09-11 20:38:19.000000 dgg-bot-1.1.0/dggbot/_logging.py
--rw-rw-rw-   0        0        0     4141 2023-04-03 11:05:30.000000 dgg-bot-1.1.0/dggbot/bot.py
--rw-rw-rw-   0        0        0     8692 2023-05-28 00:23:03.000000 dgg-bot-1.1.0/dggbot/chat.py
--rw-rw-rw-   0        0        0      497 2023-01-15 02:17:22.000000 dgg-bot-1.1.0/dggbot/errors.py
--rw-rw-rw-   0        0        0      736 2023-05-27 22:47:33.000000 dgg-bot-1.1.0/dggbot/event.py
--rw-rw-rw-   0        0        0      863 2023-05-26 13:12:01.000000 dgg-bot-1.1.0/dggbot/flairs.py
--rw-rw-rw-   0        0        0      339 2023-03-13 02:12:12.000000 dgg-bot-1.1.0/dggbot/funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.695720 dgg-bot-1.1.0/dggbot/live/
--rw-rw-rw-   0        0        0     1770 2023-04-28 01:20:01.000000 dgg-bot-1.1.0/dggbot/live/__init__.py
--rw-rw-rw-   0        0        0     2334 2023-05-22 18:25:49.000000 dgg-bot-1.1.0/dggbot/live/message.py
--rw-rw-rw-   0        0        0     5476 2023-05-28 00:17:58.000000 dgg-bot-1.1.0/dggbot/message.py
--rw-rw-rw-   0        0        0      210 2023-05-27 23:15:52.000000 dgg-bot-1.1.0/dggbot/user.py
--rw-rw-rw-   0        0        0     2578 2023-05-26 10:38:55.000000 dgg-bot-1.1.0/dggbot/wsbase.py
--rw-rw-rw-   0        0        0     1238 2023-05-26 21:35:47.000000 dgg-bot-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       41 2023-05-26 14:11:03.000000 dgg-bot-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 00:28:32.699719 dgg-bot-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 00:28:32.697720 dgg-bot-1.1.0/tests/
--rw-rw-rw-   0        0        0      586 2023-05-28 00:09:42.000000 dgg-bot-1.1.0/tests/test_chat.py
+drwxrwxrwx   0        0        0        0 2023-08-09 02:41:50.240239 dgg-bot-1.2.0/
+-rw-rw-rw-   0        0        0     1083 2023-05-31 15:07:25.000000 dgg-bot-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4018 2023-08-09 02:41:50.239239 dgg-bot-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-05-28 01:17:26.000000 dgg-bot-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-09 02:41:50.208239 dgg-bot-1.2.0/dgg_bot.egg-info/
+-rw-rw-rw-   0        0        0     4018 2023-08-09 02:41:50.000000 dgg-bot-1.2.0/dgg_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-08-09 02:41:50.000000 dgg-bot-1.2.0/dgg_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 02:41:50.000000 dgg-bot-1.2.0/dgg_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-08-09 02:41:50.000000 dgg-bot-1.2.0/dgg_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-09 02:41:50.000000 dgg-bot-1.2.0/dgg_bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 02:41:50.231239 dgg-bot-1.2.0/dggbot/
+-rw-rw-rw-   0        0        0      479 2023-08-09 02:38:42.000000 dgg-bot-1.2.0/dggbot/__init__.py
+-rw-rw-rw-   0        0        0      504 2022-09-11 20:38:19.000000 dgg-bot-1.2.0/dggbot/_logging.py
+-rw-rw-rw-   0        0        0     4143 2023-05-31 15:07:25.000000 dgg-bot-1.2.0/dggbot/bot.py
+-rw-rw-rw-   0        0        0     8747 2023-08-09 02:37:16.000000 dgg-bot-1.2.0/dggbot/chat.py
+-rw-rw-rw-   0        0        0      497 2023-01-15 02:17:22.000000 dgg-bot-1.2.0/dggbot/errors.py
+-rw-rw-rw-   0        0        0      736 2023-05-27 22:47:33.000000 dgg-bot-1.2.0/dggbot/event.py
+-rw-rw-rw-   0        0        0      924 2023-08-09 02:19:57.000000 dgg-bot-1.2.0/dggbot/flairs.py
+-rw-rw-rw-   0        0        0      339 2023-03-13 02:12:12.000000 dgg-bot-1.2.0/dggbot/funcs.py
+drwxrwxrwx   0        0        0        0 2023-08-09 02:41:50.236239 dgg-bot-1.2.0/dggbot/live/
+-rw-rw-rw-   0        0        0     1772 2023-05-31 15:07:25.000000 dgg-bot-1.2.0/dggbot/live/__init__.py
+-rw-rw-rw-   0        0        0     2408 2023-05-31 15:07:25.000000 dgg-bot-1.2.0/dggbot/live/message.py
+-rw-rw-rw-   0        0        0     5549 2023-05-31 16:32:00.000000 dgg-bot-1.2.0/dggbot/message.py
+-rw-rw-rw-   0        0        0      718 2023-05-31 15:07:25.000000 dgg-bot-1.2.0/dggbot/user.py
+-rw-rw-rw-   0        0        0     2580 2023-05-31 15:07:25.000000 dgg-bot-1.2.0/dggbot/wsbase.py
+-rw-rw-rw-   0        0        0     1238 2023-05-26 21:35:47.000000 dgg-bot-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       43 2023-05-31 15:07:25.000000 dgg-bot-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 02:41:50.240239 dgg-bot-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-09 02:41:50.238240 dgg-bot-1.2.0/tests/
+-rw-rw-rw-   0        0        0      684 2023-08-09 02:39:01.000000 dgg-bot-1.2.0/tests/test_chat.py
```

### Comparing `dgg-bot-1.1.0/LICENSE` & `dgg-bot-1.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `dgg-bot-1.1.0/PKG-INFO` & `dgg-bot-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgg-bot
-Version: 1.1.0
+Version: 1.2.0
 Summary: A library for connecting to and making a bot in Destiny.gg chat.
 Author: Fritz-02
 License: MIT
 Project-URL: Homepage, https://github.com/Fritz-02/dgg-bot/
 Project-URL: Bug Tracker, https://github.com/Fritz-02/dgg-bot/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 DGG-bot
 =======
 
+.. image:: https://img.shields.io/pypi/l/dgg-bot.svg
+   :target: https://pypi.python.org/pypi/dgg-bot
+   :alt: PyPI license info
 .. image:: https://img.shields.io/pypi/v/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI supported Python versions
```

### Comparing `dgg-bot-1.1.0/README.rst` & `dgg-bot-1.2.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 DGG-bot
 =======
 
+.. image:: https://img.shields.io/pypi/l/dgg-bot.svg
+   :target: https://pypi.python.org/pypi/dgg-bot
+   :alt: PyPI license info
 .. image:: https://img.shields.io/pypi/v/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI supported Python versions
```

### Comparing `dgg-bot-1.1.0/dgg_bot.egg-info/PKG-INFO` & `dgg-bot-1.2.0/dgg_bot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgg-bot
-Version: 1.1.0
+Version: 1.2.0
 Summary: A library for connecting to and making a bot in Destiny.gg chat.
 Author: Fritz-02
 License: MIT
 Project-URL: Homepage, https://github.com/Fritz-02/dgg-bot/
 Project-URL: Bug Tracker, https://github.com/Fritz-02/dgg-bot/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 DGG-bot
 =======
 
+.. image:: https://img.shields.io/pypi/l/dgg-bot.svg
+   :target: https://pypi.python.org/pypi/dgg-bot
+   :alt: PyPI license info
 .. image:: https://img.shields.io/pypi/v/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI supported Python versions
```

### Comparing `dgg-bot-1.1.0/dggbot/bot.py` & `dgg-bot-1.2.0/dggbot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import itertools
 import time
 from typing import Callable, Union
+
 from .chat import DGGChat, EventType
 from .message import Message, PrivateMessage
 
 
 class DGGBot(DGGChat):
     def __init__(
         self,
```

### Comparing `dgg-bot-1.1.0/dggbot/chat.py` & `dgg-bot-1.2.0/dggbot/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import json
-import requests
 from typing import Union
 
+import requests
+
 from ._logging import _logger
-from .event import EventType
-from .flairs import Flair, flair_converter, convert_flairs
-from .funcs import threaded
-from .message import (
-    Message,
-    MuteMessage,
-    PinnedMessage,
-    PollMessage,
-    PrivateMessage,
-    VoteMessage,
-    SubscriptionMessage,
-    MassGiftMessage,
-    GiftSubMessage,
-    DonationMessage,
-    BroadcastMessage,
-    convert_datetime,
-)
-from .user import User
-from .wsbase import WSBase
 from .errors import (
     AccountTooYoung,
     Banned,
     DuplicateMessage,
     InvalidMessage,
     NeedLogin,
     NoPermission,
     NotFound,
     ProtocolError,
     SubMode,
     Throttled,
     TooManyConnections,
 )
+from .event import EventType
+from .flairs import Flair, convert_flairs, flair_converter
+from .funcs import threaded
+from .message import (
+    BroadcastMessage,
+    DonationMessage,
+    GiftSubMessage,
+    MassGiftMessage,
+    Message,
+    MuteMessage,
+    PinnedMessage,
+    PollMessage,
+    PrivateMessage,
+    SubscriptionMessage,
+    VoteMessage,
+    convert_datetime,
+)
+from .user import User
+from .wsbase import WSBase
 
 
 class DGGChat(WSBase):
     _CONFIG = {
         "wss": "wss://chat.destiny.gg/ws",
         "wss-origin": "https://www.destiny.gg",
         "baseurl": "https://www.destiny.gg",
@@ -164,17 +165,19 @@
             msg = GiftSubMessage(self, event_type, data)
         elif event_type == EventType.DONATION:
             msg = DonationMessage(self, event_type, data)
         elif event_type == EventType.BROADCAST:
             msg = BroadcastMessage(self, event_type, data)
         elif event_type == EventType.ERROR:
             if (desc := data["description"]) in self._err_dict:
+                self.on_event("error", self._err_dict[desc])
                 raise self._err_dict[desc]
             else:
                 _logger.error(event_type, data)
+                self.on_event("error", data)
                 raise Exception(desc)
         elif event_type == EventType.NAMES:
             _logger.debug(f"{event_type} {data}")
             self.on_names(data["connectioncount"], data["users"])
             return
         elif event_type == EventType.PIN:
             msg = PinnedMessage(self, event_type, data)
@@ -194,32 +197,29 @@
             msg
         ):
             self.on_event("mention", msg)
         self._post_message(msg)
 
     def _post_message(self, msg):
         """Do stuff after _on_message"""
-        pass
 
     def _on_open(self, ws):
         _logger.info(
             f"Connecting "
             + (f"as {self.username} " if self.username else "")
             + f"to {self.wss}."
         )
         self._connected = True
 
     def mention(self):
         """Decorator to run function on mentions. Shortcut for event('on_mention')."""
         return self.event("on_mention")
 
     def is_mentioned(self, msg: Union[Message, PrivateMessage]) -> bool:
-        return (
-            False if self.username is None else (self.username in msg.data.casefold())
-        )
+        return False if self.user is None else self.user.is_mentioned(msg)
 
     @threaded
     def on_names(self, connection_count: int, users: list):
         """Do stuff when the NAMES message is received upon connecting to chat."""
         self._users = {
             user["nick"].lower(): User(
                 user.get("id"),
```

### Comparing `dgg-bot-1.1.0/dggbot/event.py` & `dgg-bot-1.2.0/dggbot/event.py`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.1.0/dggbot/flairs.py` & `dgg-bot-1.2.0/dggbot/flairs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import dataclasses
-import requests
 from typing import Union
 
+import requests
+
 
 @dataclasses.dataclass
 class Flair:
     label: str
     name: str
     description: str
     hidden: bool
@@ -13,14 +14,17 @@
     color: str
     rainbowColor: bool
     image: list[dict]
 
     def __repr__(self):
         return f"Flair<{self.label}>"
 
+    def __hash__(self):
+        return hash(self.name)
+
 
 def flair_converter(endpoint: str) -> dict:
     """Returns a dict to convert flair names (e.g. flair17) to a Flair object."""
     r = requests.get(endpoint)
     converter = {item["name"]: Flair(**item) for item in r.json()}
     return converter
```

### Comparing `dgg-bot-1.1.0/dggbot/live/__init__.py` & `dgg-bot-1.2.0/dggbot/live/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from typing import Union
-from .message import StreamInfo, YoutubeVideo, YoutubeVod
+
 from .._logging import _logger
 from ..wsbase import WSBase
+from .message import StreamInfo, YoutubeVideo, YoutubeVod
 
 
 class DGGLive(WSBase):
     _CONFIG = {
         "wss": "wss://live.destiny.gg/",
         "wss-origin": "https://www.destiny.gg",
     }
```

### Comparing `dgg-bot-1.1.0/dggbot/live/message.py` & `dgg-bot-1.2.0/dggbot/live/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import dataclasses
-from typing import Union
 
 
 @dataclasses.dataclass
 class Stream:
     live: bool
     game: str
     preview: str
@@ -35,21 +34,29 @@
             for s in (self.twitch, self.youtube, self.facebook, self.rumble, self.kick)
             if s is not None
         )
         return any(stream.live for stream in streams)
 
     def get_livestreams(self) -> tuple[Stream]:
         """Returns streams that are currently live."""
-        streams = tuple(s for s in (self.twitch, self.youtube, self.facebook, self.rumble, self.kick) if isinstance(s, Stream) and s.live)
+        streams = tuple(
+            s
+            for s in (self.twitch, self.youtube, self.facebook, self.rumble, self.kick)
+            if isinstance(s, Stream) and s.live
+        )
         return streams
 
     @property
     def viewers(self) -> int:
         """Returns the sum of viewers from each livestream."""
-        return sum(s.viewers for s in (self.twitch, self.youtube, self.facebook, self.rumble, self.kick) if isinstance(s, Stream) and s.live)
+        return sum(
+            s.viewers
+            for s in (self.twitch, self.youtube, self.facebook, self.rumble, self.kick)
+            if isinstance(s, Stream) and s.live
+        )
 
     @classmethod
     def from_json(cls, data: dict) -> "StreamInfo":
         streams = {
             k: Stream.from_json(v)
             for k, v in data["data"]["streams"].items()
             if v is not None
```

### Comparing `dgg-bot-1.1.0/dggbot/message.py` & `dgg-bot-1.2.0/dggbot/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from datetime import datetime, timezone
+from typing import TYPE_CHECKING, Union
+
 from ._logging import _logger
 from .flairs import Flair, convert_flairs
 from .user import User
 
-from typing import Union, TYPE_CHECKING
-
 if TYPE_CHECKING:
     from .chat import DGGChat
 
 
 def convert_datetime(dt_string: str) -> datetime:
     if (n := len(dt_string)) == 20:  # seconds given
         dt = datetime.strptime(dt_string, "%Y-%m-%dT%H:%M:%SZ")
@@ -146,12 +146,15 @@
         self.now: datetime = convert_datetime(data.get("now"))
         self.time: int = data.get("time")
         self.question: str = data.get("question")
         self.options: list[str] = data.get("options")
         self.totals: list[int] = data.get("totals")
         self.total_votes: int = data.get("totalvotes")
 
+    def vote(self, option: int):
+        self.chat.cast_vote(option)
+
 
 class VoteMessage(_MessageBase):
     def __init__(self, chat: DGGChat, type_: str, data: dict):
         super().__init__(chat, type_, data)
         self.vote: str = data.get("vote")
```

### Comparing `dgg-bot-1.1.0/dggbot/wsbase.py` & `dgg-bot-1.2.0/dggbot/wsbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from abc import abstractmethod, ABC
 import json
 import time
+from abc import ABC, abstractmethod
 from typing import Callable, Union
+
 import websocket
 
-from .funcs import threaded
 from ._logging import _logger
+from .funcs import threaded
 
 
 class WSBase(ABC):
     _CONFIG = {
         "wss": "wss://chat.destiny.gg/ws",
         "wss-origin": "https://www.destiny.gg",
     }
```

### Comparing `dgg-bot-1.1.0/pyproject.toml` & `dgg-bot-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dgg-bot-1.1.0/tests/test_chat.py` & `dgg-bot-1.2.0/tests/test_chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 """
 
 import threading
 import time
 
 from dggbot import DGGChat
 
+import pytest
 
 checks = {"connection": False}
 
 
 class TestChat(DGGChat):
     def _on_open(self, ws):
         super()._on_open(ws)
         checks["connection"] = True
 
 
 chat = TestChat()
 
 
-# Test connection
-t = threading.Thread(target=chat.run)
-t.start()
+@pytest.mark.order(0)
+def test_connection():
+    t = threading.Thread(target=chat.run)
+    t.start()
+    time.sleep(5)
+    assert all(v for v in checks.values())
 
 
-# Close
-time.sleep(5)
-chat.ws.close()
 
 
-for check, result in checks.items():
-    print(f"{check}:", "SUCCESS" if result else "FAILURE")
+
+@pytest.mark.order(after="test_connection")
+def test_other():
+    chat.ws.close()
+    assert "A" in "abefeasfAfaefm"
```

