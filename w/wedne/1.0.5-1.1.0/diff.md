# Comparing `tmp/wedne-1.0.5.tar.gz` & `tmp/wedne-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedne-1.0.5.tar", max compression
+gzip compressed data, was "wedne-1.1.0.tar", max compression
```

## Comparing `wedne-1.0.5.tar` & `wedne-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1463 2023-08-08 17:39:59.372075 wedne-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0     4499 2023-08-08 17:45:10.592681 wedne-1.0.5/README.md
--rw-r--r--   0        0        0     1085 2023-08-08 20:23:28.494168 wedne-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.356160 wedne-1.0.5/wedne/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.360160 wedne-1.0.5/wedne/client/__init__.py
--rw-r--r--   0        0        0     1203 2023-08-08 13:10:56.368161 wedne-1.0.5/wedne/client/__main__.py
--rw-r--r--   0        0        0      338 2023-08-08 13:10:56.376161 wedne-1.0.5/wedne/client/consts.py
--rw-r--r--   0        0        0      533 2023-08-08 13:10:56.380161 wedne-1.0.5/wedne/client/shared_commands.py
--rw-r--r--   0        0        0     2802 2023-08-08 13:10:56.384162 wedne-1.0.5/wedne/client/telegram.py
--rw-r--r--   0        0        0     1801 2023-08-08 13:10:56.392162 wedne-1.0.5/wedne/client/watcher.py
--rw-r--r--   0        0        0      399 2023-08-08 13:10:56.396162 wedne-1.0.5/wedne/commands.py
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.404163 wedne-1.0.5/wedne/server/__init__.py
--rw-r--r--   0        0        0     1178 2023-08-08 13:10:56.408163 wedne-1.0.5/wedne/server/__main__.py
--rw-r--r--   0        0        0      186 2023-08-08 13:10:56.416164 wedne-1.0.5/wedne/server/api/__init__.py
--rw-r--r--   0        0        0      759 2023-08-08 13:10:56.420164 wedne-1.0.5/wedne/server/api/stats.py
--rw-r--r--   0        0        0      999 2023-08-08 20:16:32.538473 wedne-1.0.5/wedne/server/api/visits.py
--rw-r--r--   0        0        0     2307 2023-08-08 19:53:55.126368 wedne-1.0.5/wedne/server/db.py
--rw-r--r--   0        0        0      428 2023-08-08 13:10:56.436165 wedne-1.0.5/wedne/server/settings.py
--rw-r--r--   0        0        0     1546 2023-08-08 20:17:18.076597 wedne-1.0.5/wedne/server/tasks.py
--rw-r--r--   0        0        0      288 2023-08-08 13:10:56.448166 wedne-1.0.5/wedne/utils.py
--rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 wedne-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1463 2023-08-08 17:39:59.372075 wedne-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4499 2023-08-08 17:45:10.592681 wedne-1.1.0/README.md
+-rw-r--r--   0        0        0     1173 2023-08-08 23:07:07.726790 wedne-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.356160 wedne-1.1.0/wedne/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.360160 wedne-1.1.0/wedne/client/__init__.py
+-rw-r--r--   0        0        0     1203 2023-08-08 13:10:56.368161 wedne-1.1.0/wedne/client/__main__.py
+-rw-r--r--   0        0        0      338 2023-08-08 13:10:56.376161 wedne-1.1.0/wedne/client/consts.py
+-rw-r--r--   0        0        0      533 2023-08-08 13:10:56.380161 wedne-1.1.0/wedne/client/shared_commands.py
+-rw-r--r--   0        0        0     2802 2023-08-08 13:10:56.384162 wedne-1.1.0/wedne/client/telegram.py
+-rw-r--r--   0        0        0     2172 2023-08-08 22:04:54.562737 wedne-1.1.0/wedne/client/watcher.py
+-rw-r--r--   0        0        0      410 2023-08-08 22:24:44.401889 wedne-1.1.0/wedne/commands.py
+-rw-r--r--   0        0        0      241 2023-08-08 23:01:10.051217 wedne-1.1.0/wedne/commands_test.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.404163 wedne-1.1.0/wedne/server/__init__.py
+-rw-r--r--   0        0        0     1178 2023-08-08 13:10:56.408163 wedne-1.1.0/wedne/server/__main__.py
+-rw-r--r--   0        0        0      186 2023-08-08 13:10:56.416164 wedne-1.1.0/wedne/server/api/__init__.py
+-rw-r--r--   0        0        0      759 2023-08-08 13:10:56.420164 wedne-1.1.0/wedne/server/api/stats.py
+-rw-r--r--   0        0        0      999 2023-08-08 20:16:32.538473 wedne-1.1.0/wedne/server/api/visits.py
+-rw-r--r--   0        0        0     2307 2023-08-08 19:53:55.126368 wedne-1.1.0/wedne/server/db.py
+-rw-r--r--   0        0        0      467 2023-08-08 23:04:31.638177 wedne-1.1.0/wedne/server/settings.py
+-rw-r--r--   0        0        0     1546 2023-08-08 20:17:18.076597 wedne-1.1.0/wedne/server/tasks.py
+-rw-r--r--   0        0        0      657 2023-08-08 22:02:29.915944 wedne-1.1.0/wedne/utils.py
+-rw-r--r--   0        0        0      713 2023-08-08 22:14:10.987567 wedne-1.1.0/wedne/utils_test.py
+-rw-r--r--   0        0        0     5341 1970-01-01 00:00:00.000000 wedne-1.1.0/PKG-INFO
```

### Comparing `wedne-1.0.5/LICENSE.txt` & `wedne-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/README.md` & `wedne-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/pyproject.toml` & `wedne-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 [tool.poetry]
 name = "wedne"
-version = "1.0.5"
+version = "1.1.0"
 description = "Координируем строительство башни"
 authors = ["Oskar Sharipov"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/igoose1/wedne"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = {extras = ["dotenv"], version = "^1.10.9"}
+pydantic = {extras = ["dotenv"], version = "^2.1.0"}
 fire = "^0.5.0"
 httpx = "^0.24.1"
 telethon = "^1.28.5"
 aiorun = "^2023.7.2"
 pytz = "^2023.3"
+pydantic-settings = "^2.0.2"
 
 
 [tool.poetry.group.server.dependencies]
-fastapi = "^0.100.0"
+fastapi = "^0.101.0"
 peewee = "^3.16.2"
 uvicorn = "^0.22.0"
-pydantic = "^1.10.9"
 huey = "^2.4.5"
 
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.3.0"
 pyright = "^1.1.316"
 pre-commit = "^3.3.3"
 autoflake = "^2.2.0"
 ruff = "^0.0.280"
 ptpython = "^3.0.23"
+pytest = "^7.4.0"
 
 [tool.ruff]
 select = [
 	"E",
 	"F",
 	"C90",
 	"I",
@@ -62,11 +63,13 @@
 	"RUF",
 	"UP",
 	"DTZ",
 ]
 ignore = [
 	"TD003",
 ]
+[tool.ruff.per-file-ignores]
+"*_test.py" = ["S101", "PLR2004"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wedne-1.0.5/wedne/client/__main__.py` & `wedne-1.1.0/wedne/client/__main__.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/wedne/client/shared_commands.py` & `wedne-1.1.0/wedne/client/shared_commands.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/wedne/client/telegram.py` & `wedne-1.1.0/wedne/client/telegram.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/wedne/client/watcher.py` & `wedne-1.1.0/wedne/client/watcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,26 +4,33 @@
 from dataclasses import dataclass
 from functools import singledispatchmethod
 from importlib import metadata
 
 import httpx
 
 from wedne.commands import CommandSchema
+from wedne.utils import Backoffer
 
 
 @dataclass
 class Watcher:
     endpoint: str
     delay: datetime.timedelta
     social_media_id: int
     command_processor: Callable[[CommandSchema | None], Awaitable[None]]
 
+    def __post_init__(self) -> None:
+        self.backoffer = Backoffer()
+
     async def __call__(self) -> None:
         version = metadata.version("wedne")
-        client = httpx.AsyncClient(headers={"user-agent": f"wedne.client/{version}"})
+        client = httpx.AsyncClient(
+            headers={"user-agent": f"wedne.client/{version}"},
+            timeout=10,
+        )
         try:
             await self._watch(client)
         finally:
             await client.aclose()
 
     async def _watch(self, client: httpx.AsyncClient) -> None:
         data = {
@@ -32,31 +39,36 @@
         while True:
             try:
                 response = await client.post(
                     self.endpoint,
                     json=data,
                 )
                 await self.process(response)
+                await asyncio.sleep(self.delay.seconds)
             except httpx.ConnectError as exc:
                 await self.process(exc)
-            await asyncio.sleep(self.delay.seconds)
+                await asyncio.sleep(self.backoffer.failed())
 
     @singledispatchmethod
     async def process(self, response: httpx.Response) -> None:
         print(response)
         print(response.content)
 
         if response.is_server_error:
             print("Server error")
+            await asyncio.sleep(self.backoffer.failed())
             return
 
         if response.is_client_error:
             print("Client error, update me")
+            await asyncio.sleep(self.backoffer.failed())
             return
 
+        self.backoffer.succeeded()
+
         raw_command = response.json()
         command = CommandSchema.parse_obj(raw_command) if raw_command else None
         await self.command_processor(command)
 
     @process.register
     async def _(self, exception: httpx.ConnectError) -> None:
         print(str(exception))
```

### Comparing `wedne-1.0.5/wedne/server/__main__.py` & `wedne-1.1.0/wedne/server/__main__.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/wedne/server/api/stats.py` & `wedne-1.1.0/wedne/server/api/stats.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/wedne/server/api/visits.py` & `wedne-1.1.0/wedne/server/api/visits.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/wedne/server/db.py` & `wedne-1.1.0/wedne/server/db.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/wedne/server/tasks.py` & `wedne-1.1.0/wedne/server/tasks.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.5/PKG-INFO` & `wedne-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: wedne
-Version: 1.0.5
+Version: 1.1.0
 Summary: Координируем строительство башни
 Home-page: https://github.com/igoose1/wedne
 License: BSD-3-Clause
 Author: Oskar Sharipov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiorun (>=2023.7.2,<2024.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: pydantic[dotenv] (>=1.10.9,<2.0.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic[dotenv] (>=2.1.0,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: telethon (>=1.28.5,<2.0.0)
 Project-URL: Repository, https://github.com/igoose1/wedne
 Description-Content-Type: text/markdown
 
 # wedne: координируем строительство башни
```

