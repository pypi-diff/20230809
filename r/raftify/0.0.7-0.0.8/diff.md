# Comparing `tmp/raftify-0.0.7-py3-none-any.whl.zip` & `tmp/raftify-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,29 @@
-Zip file size: 28729 bytes, number of entries: 26
--rw-r--r--  2.0 unx        6 b- defN 23-Aug-07 09:22 raftify/VERSION
--rw-r--r--  2.0 unx      881 b- defN 23-Aug-07 09:22 raftify/__init__.py
--rw-r--r--  2.0 unx       86 b- defN 23-Aug-07 06:52 raftify/error.py
--rw-r--r--  2.0 unx      368 b- defN 23-Aug-07 07:20 raftify/fsm.py
--rw-r--r--  2.0 unx    11153 b- defN 23-Aug-07 09:17 raftify/lmdb.py
--rw-r--r--  2.0 unx      571 b- defN 23-Aug-07 09:22 raftify/logger.py
--rw-r--r--  2.0 unx     2834 b- defN 23-Aug-07 06:28 raftify/mailbox.py
--rw-r--r--  2.0 unx     1498 b- defN 23-Aug-07 09:12 raftify/message_sender.py
--rw-r--r--  2.0 unx     7907 b- defN 23-Aug-07 06:16 raftify/pb_adapter.py
--rw-r--r--  2.0 unx     2573 b- defN 23-Aug-07 07:19 raftify/raft_client.py
--rw-r--r--  2.0 unx     5365 b- defN 23-Aug-07 09:12 raftify/raft_facade.py
--rw-r--r--  2.0 unx    14661 b- defN 23-Aug-07 09:15 raftify/raft_node.py
--rw-r--r--  2.0 unx     1192 b- defN 23-Aug-07 09:10 raftify/raft_server.py
--rw-r--r--  2.0 unx     4187 b- defN 23-Aug-07 09:10 raftify/raft_service.py
--rw-r--r--  2.0 unx      985 b- defN 23-Aug-07 04:23 raftify/request_message.py
--rw-r--r--  2.0 unx      753 b- defN 23-Aug-07 06:17 raftify/response_message.py
+Zip file size: 29243 bytes, number of entries: 27
+-rw-r--r--  2.0 unx        6 b- defN 23-Aug-09 03:01 raftify/VERSION
+-rw-r--r--  2.0 unx     1148 b- defN 23-Aug-08 10:13 raftify/__init__.py
+-rw-r--r--  2.0 unx      880 b- defN 23-Aug-08 10:15 raftify/deserializer.py
+-rw-r--r--  2.0 unx       86 b- defN 23-Aug-08 07:42 raftify/error.py
+-rw-r--r--  2.0 unx      368 b- defN 23-Aug-08 07:42 raftify/fsm.py
+-rw-r--r--  2.0 unx    11153 b- defN 23-Aug-07 09:34 raftify/lmdb.py
+-rw-r--r--  2.0 unx      571 b- defN 23-Aug-08 07:42 raftify/logger.py
+-rw-r--r--  2.0 unx     2976 b- defN 23-Aug-08 10:19 raftify/mailbox.py
+-rw-r--r--  2.0 unx     1498 b- defN 23-Aug-08 07:43 raftify/message_sender.py
+-rw-r--r--  2.0 unx     7907 b- defN 23-Aug-08 10:11 raftify/pb_adapter.py
+-rw-r--r--  2.0 unx     2573 b- defN 23-Aug-08 07:43 raftify/raft_client.py
+-rw-r--r--  2.0 unx     5376 b- defN 23-Aug-08 10:15 raftify/raft_facade.py
+-rw-r--r--  2.0 unx    14661 b- defN 23-Aug-08 10:16 raftify/raft_node.py
+-rw-r--r--  2.0 unx     1192 b- defN 23-Aug-08 07:43 raftify/raft_server.py
+-rw-r--r--  2.0 unx     4187 b- defN 23-Aug-08 07:43 raftify/raft_service.py
+-rw-r--r--  2.0 unx      985 b- defN 23-Aug-08 10:10 raftify/request_message.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Aug-08 08:03 raftify/response_message.py
 -rw-r--r--  2.0 unx     1480 b- defN 23-Aug-07 08:39 raftify/utils.py
 -rw-r--r--  2.0 unx     5208 b- defN 23-Aug-07 06:51 raftify/protos/eraftpb_pb2.py
 -rw-r--r--  2.0 unx      173 b- defN 23-Aug-07 06:51 raftify/protos/eraftpb_pb2_grpc.py
 -rw-r--r--  2.0 unx     3468 b- defN 23-Aug-07 06:51 raftify/protos/raft_service_pb2.py
 -rw-r--r--  2.0 unx     7397 b- defN 23-Aug-07 06:51 raftify/protos/raft_service_pb2_grpc.py
--rw-r--r--  2.0 unx    10349 b- defN 23-Aug-07 09:23 raftify-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     6098 b- defN 23-Aug-07 09:23 raftify-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 09:23 raftify-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Aug-07 09:23 raftify-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2048 b- defN 23-Aug-07 09:23 raftify-0.0.7.dist-info/RECORD
-26 files, 91341 bytes uncompressed, 25465 bytes compressed:  72.1%
+-rw-r--r--  2.0 unx    10349 b- defN 23-Aug-09 03:02 raftify-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6144 b- defN 23-Aug-09 03:02 raftify-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-09 03:02 raftify-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-09 03:02 raftify-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2128 b- defN 23-Aug-09 03:02 raftify-0.0.8.dist-info/RECORD
+27 files, 92767 bytes uncompressed, 25857 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: raftify/VERSION
 Comment: 
 
 Filename: raftify/__init__.py
 Comment: 
 
+Filename: raftify/deserializer.py
+Comment: 
+
 Filename: raftify/error.py
 Comment: 
 
 Filename: raftify/fsm.py
 Comment: 
 
 Filename: raftify/lmdb.py
@@ -57,23 +60,23 @@
 
 Filename: raftify/protos/raft_service_pb2.py
 Comment: 
 
 Filename: raftify/protos/raft_service_pb2_grpc.py
 Comment: 
 
-Filename: raftify-0.0.7.dist-info/LICENSE
+Filename: raftify-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: raftify-0.0.7.dist-info/METADATA
+Filename: raftify-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: raftify-0.0.7.dist-info/WHEEL
+Filename: raftify-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: raftify-0.0.7.dist-info/top_level.txt
+Filename: raftify-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: raftify-0.0.7.dist-info/RECORD
+Filename: raftify-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## raftify/VERSION

```diff
@@ -1 +1 @@
-0.0.7
+0.0.8
```

## raftify/__init__.py

```diff
@@ -1,9 +1,17 @@
 from pathlib import Path
 
+from .deserializer import (  # noqa: F401
+    confchange_context_deserializer,
+    confchangev2_context_deserializer,
+    entry_context_deserializer,
+    entry_data_deserializer,
+    message_context_deserializer,
+    snapshot_data_deserializer,
+)
 from .error import ClusterJoinError, UnknownError  # noqa: F401
 from .fsm import FSM  # noqa: F401
 from .lmdb import LMDBStorage, LMDBStorageCore  # noqa: F401
 from .logger import RaftifyLogger  # noqa: F401
 from .mailbox import Mailbox  # noqa: F401
 from .message_sender import MessageSender  # noqa: F401
 from .raft_client import RaftClient  # noqa: F401
@@ -21,10 +29,11 @@
     "raft_client",
     "raft_node",
     "raft_server",
     "raft_facade",
     "fsm",
     "utils",
     "logger",
+    "deserializer",
 ]
 
 __version__ = (Path(__file__).parent / "VERSION").read_text().strip()
```

## raftify/mailbox.py

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import pickle
 from asyncio import Queue
 from typing import Optional
 
 from rraft import ConfChange, ConfChangeType
 
 from raftify.error import UnknownError
 from raftify.pb_adapter import ConfChangeAdapter
@@ -11,24 +12,26 @@
 from raftify.request_message import MessageConfigChange, MessagePropose
 from raftify.response_message import (
     RaftRespOk,
     RaftResponse,
     RaftRespResponse,
     RaftRespWrongLeader,
 )
+from raftify.utils import SocketAddr
 
 
 class Mailbox:
     """
     A mailbox to send messages to a running raft node.
     """
 
-    def __init__(self, raft_node: RaftNode, sender: Queue):
+    def __init__(self, addr: SocketAddr, raft_node: RaftNode, sender: Queue):
         self.sender = sender
         self.raft_node = raft_node
+        self.addr = addr
 
     async def __handle_response(
         self,
         response: RaftResponse,
         *,
         reroute_msg_type: raft_service_pb2.RerouteMsgType,
         proposed_data: Optional[bytes] = None,
@@ -69,14 +72,15 @@
         )
         assert resp is not None
         return resp
 
     async def leave(self, node_id: int) -> None:
         cc = ConfChange.default()
         cc.set_node_id(node_id)
+        cc.set_context(pickle.dumps(self.addr))
         cc.set_change_type(ConfChangeType.RemoveNode)
 
         receiver = Queue()
         confchange = ConfChangeAdapter.to_pb(cc)
 
         await self.sender.put(MessageConfigChange(confchange, receiver))
```

## raftify/raft_facade.py

```diff
@@ -50,15 +50,15 @@
         self.raft_node = None
 
     @property
     def mailbox(self) -> Mailbox:
         """
         Get the node's `Mailbox`.
         """
-        return Mailbox(self.raft_node, self.chan)
+        return Mailbox(self.addr, self.raft_node, self.chan)
 
     def get_peers(self) -> dict[int, RaftClient]:
         return self.raft_node.peers
 
     async def bootstrap_cluster(self) -> None:
         """
         Create a new leader for the cluster with node id 1.
```

## Comparing `raftify-0.0.7.dist-info/LICENSE` & `raftify-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `raftify-0.0.7.dist-info/METADATA` & `raftify-0.0.8.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: raftify
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/lablup/raftify
 Author: Lablup Inc.
 Maintainer: jopemachine
 Maintainer-email: gbl@lablup.com
 License: Apache License 2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: grpcio >=1.50.0
-Requires-Dist: lmdb ==1.4.0
-Requires-Dist: protobuf ~=4.21.6
-Requires-Dist: rraft-py ==0.1.0
-Requires-Dist: tomli ~=2.0.1
+Requires-Dist: grpcio (==1.50.0)
+Requires-Dist: lmdb (==1.4.0)
+Requires-Dist: protobuf (~=4.21.6)
+Requires-Dist: rraft-py (==0.1.1)
+Requires-Dist: tomli (~=2.0.1)
 Provides-Extra: build
-Requires-Dist: aiohttp ==3.8.4 ; extra == 'build'
-Requires-Dist: argparse ==1.4.0 ; extra == 'build'
-Requires-Dist: grpcio-tools ==1.54.2 ; extra == 'build'
-Requires-Dist: grpcio ==1.54.2 ; extra == 'build'
-Requires-Dist: lmdb ==1.4.0 ; extra == 'build'
-Requires-Dist: msgpack ==1.0.4 ; extra == 'build'
-Requires-Dist: protobuf ==4.23.2 ; extra == 'build'
-Requires-Dist: rraft-py ==0.1.0 ; extra == 'build'
-Requires-Dist: tomli ~=2.0.1 ; extra == 'build'
-Requires-Dist: twine ~=4.0.1 ; extra == 'build'
+Requires-Dist: aiohttp (==3.8.4) ; extra == 'build'
+Requires-Dist: argparse (==1.4.0) ; extra == 'build'
+Requires-Dist: grpcio-tools (==1.54.2) ; extra == 'build'
+Requires-Dist: grpcio (==1.54.2) ; extra == 'build'
+Requires-Dist: lmdb (==1.4.0) ; extra == 'build'
+Requires-Dist: msgpack (==1.0.4) ; extra == 'build'
+Requires-Dist: protobuf (==4.23.2) ; extra == 'build'
+Requires-Dist: rraft-py (==0.1.0) ; extra == 'build'
+Requires-Dist: tomli (~=2.0.1) ; extra == 'build'
+Requires-Dist: twine (~=4.0.1) ; extra == 'build'
 Requires-Dist: types-protobuf ; extra == 'build'
-Requires-Dist: wheel >=0.41.1 ; extra == 'build'
+Requires-Dist: wheel (>=0.41.1) ; extra == 'build'
 Provides-Extra: dev
-Requires-Dist: aiohttp ==3.8.4 ; extra == 'dev'
-Requires-Dist: argparse ==1.4.0 ; extra == 'dev'
+Requires-Dist: aiohttp (==3.8.4) ; extra == 'dev'
+Requires-Dist: argparse (==1.4.0) ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
-Requires-Dist: grpcio-tools ==1.54.2 ; extra == 'dev'
+Requires-Dist: grpcio-tools (==1.54.2) ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
-Requires-Dist: msgpack ==1.0.4 ; extra == 'dev'
+Requires-Dist: msgpack (==1.0.4) ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
-Requires-Dist: pytest-asyncio ~=0.19.0 ; extra == 'dev'
-Requires-Dist: pytest ~=7.1.2 ; extra == 'dev'
-Requires-Dist: twine ~=4.0.1 ; extra == 'dev'
+Requires-Dist: pytest-asyncio (~=0.19.0) ; extra == 'dev'
+Requires-Dist: pytest (~=7.1.2) ; extra == 'dev'
+Requires-Dist: twine (~=4.0.1) ; extra == 'dev'
 Requires-Dist: types-protobuf ; extra == 'dev'
 
 # raftify
 
 `raftify` is a high-level implementation of the Raft algorithm, developed with the aim to easily and simply integrate the Raft algorithm into any Python application.
 
 It uses [rraft-py](https://github.com/lablup/rraft-py) under the hood, a binding of [tikv/raft-rs](https://github.com/tikv/raft-rs), a well-tested implementation of Raft.
```

## Comparing `raftify-0.0.7.dist-info/RECORD` & `raftify-0.0.8.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-raftify/VERSION,sha256=_F7mY-yQhcTU_cEUAaOyHdkxo_oz4zXfT8D_YYcL-qA,6
-raftify/__init__.py,sha256=Rg4QxQkYP2364Dkc0sPFXZkrCGOZ0T0mYJCKwxpsL_c,881
+raftify/VERSION,sha256=cQVYnU2_-MS_s1pStBXJFXaD_wAXJawALOskWlNZD9k,6
+raftify/__init__.py,sha256=oY_hqe9n8hV3bl6Eup0aK1LTfr-KBSYfL2Y1ysqXJZQ,1148
+raftify/deserializer.py,sha256=8LLVkwmVlT3xfEYXe1MlE5zl25Lx5Kj8RrzjhCnLVtw,880
 raftify/error.py,sha256=phpDb13pDFlOGcbafx5lIPlRoSeHhXYYL9a2ozaNw7k,86
 raftify/fsm.py,sha256=Frq-qi5sYcmXEx-WS37XO-so7dbktD6gU_xMeQdFPo4,368
 raftify/lmdb.py,sha256=ql-19FcwTNBnNLGE6lGL3JDqsqBxgCx5_7Kxbsf_bbI,11153
 raftify/logger.py,sha256=lpqzp7B7Ol47ufGysjybVaW2UmkCAPlgy_Fch4xEYPg,571
-raftify/mailbox.py,sha256=BXcTd_65_AYW7LqhpLxNK8H3TTE1JgpyPXbdzadJJtI,2834
+raftify/mailbox.py,sha256=wXrucg3skLVEVrA2QK4rDoxkoLI9pRvSqHmGh8ueWxI,2976
 raftify/message_sender.py,sha256=1jDDPsy5Uji84TEpGxs63ra8U67UIpjtx_db5qMZVYM,1498
 raftify/pb_adapter.py,sha256=XrhEFIu_Wal0RpIFnQpuA4iWTLXbduSXVpTlg0lCWsM,7907
 raftify/raft_client.py,sha256=5pG1uiK0BWAIvOfYP3dxjH6XShnm9ri6_0lAqBXvsdE,2573
-raftify/raft_facade.py,sha256=9u63daW5FJyfy28v-LXsjT5T7SjUQ07NPo_d-d8SM1k,5365
+raftify/raft_facade.py,sha256=VnwDvTOzySoscr1L5o84JXl3SWDQAwA5SF3AMc8UrDs,5376
 raftify/raft_node.py,sha256=6oGP6-cXAwAtcMdjnryX9fTBClZI8aXPxJxqjg0Sdxc,14661
 raftify/raft_server.py,sha256=3yCnTm01KhwswMnJt-DJE39vFocCYSkCVi4DXdWPmfQ,1192
 raftify/raft_service.py,sha256=tRUxIv_YcjH2kKXnXxC8INGGn-vPq1Gnkb1FoUOXNwg,4187
 raftify/request_message.py,sha256=N0BvOhoUY42NNXkbPL756GxdV-0couVibTBKB6u7Uk0,985
 raftify/response_message.py,sha256=yXhYIlsEdX7ctu3b-ULjjgDpPSb9zORPaP8P_pGLSMU,753
 raftify/utils.py,sha256=OpI9rhcznLvHLPltxzMDN8mnkFEuxG8Zc-GLVyAJfgU,1480
 raftify/protos/eraftpb_pb2.py,sha256=hMZpRF6ZdPRgCtiDeQjM13nFkeQH33oFuk_lQ7pYtQY,5208
 raftify/protos/eraftpb_pb2_grpc.py,sha256=D9D_GNbjWDVKDVCox27Wikgacjp7CYgT8pdeAjuug9Y,173
 raftify/protos/raft_service_pb2.py,sha256=ubgWvJP8tOlEcMU1RhJZgfdpaKWeBrDszzEHeUVcODA,3468
 raftify/protos/raft_service_pb2_grpc.py,sha256=JyJpCltIKmk3UXUvvno732TK14rvV1HkZopHQAOfEaI,7397
-raftify-0.0.7.dist-info/LICENSE,sha256=PUjIIdfw8YHSoqpovKE5A2TDoWV3l593vG_vCBlEED0,10349
-raftify-0.0.7.dist-info/METADATA,sha256=Jpl1sqECipTDqA5iTXJuT_Yhz5FcDGhzSyB2QAMM6-I,6098
-raftify-0.0.7.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
-raftify-0.0.7.dist-info/top_level.txt,sha256=LQc7dejSGExc0jttlvaa0RJl9XQ7Ye3_-Ik_oWPcqCE,8
-raftify-0.0.7.dist-info/RECORD,,
+raftify-0.0.8.dist-info/LICENSE,sha256=PUjIIdfw8YHSoqpovKE5A2TDoWV3l593vG_vCBlEED0,10349
+raftify-0.0.8.dist-info/METADATA,sha256=kleRobs__zaAlOLoTdXHaSk1NMwg2jd4MXEfSI5JDso,6144
+raftify-0.0.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+raftify-0.0.8.dist-info/top_level.txt,sha256=LQc7dejSGExc0jttlvaa0RJl9XQ7Ye3_-Ik_oWPcqCE,8
+raftify-0.0.8.dist-info/RECORD,,
```

