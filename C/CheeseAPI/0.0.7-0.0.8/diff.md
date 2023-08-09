# Comparing `tmp/CheeseAPI-0.0.7.tar.gz` & `tmp/CheeseAPI-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheeseAPI-0.0.7.tar", last modified: Mon Aug  7 15:01:26 2023, max compression
+gzip compressed data, was "CheeseAPI-0.0.8.tar", last modified: Wed Aug  9 02:47:16 2023, max compression
```

## Comparing `CheeseAPI-0.0.7.tar` & `CheeseAPI-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-07 15:01:26.476612 CheeseAPI-0.0.7/
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-07 15:01:26.475516 CheeseAPI-0.0.7/CheeseAPI/
--rw-r--r--   0 cheese     (501) staff       (20)      263 2023-08-07 02:05:19.000000 CheeseAPI-0.0.7/CheeseAPI/__init__.py
--rw-r--r--   0 cheese     (501) staff       (20)    16962 2023-08-07 03:18:25.000000 CheeseAPI-0.0.7/CheeseAPI/app.py
--rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.7/CheeseAPI/cSignal.py
--rw-r--r--   0 cheese     (501) staff       (20)     8402 2023-08-03 06:20:30.000000 CheeseAPI-0.0.7/CheeseAPI/command.py
--rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.7/CheeseAPI/exception.py
--rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.7/CheeseAPI/file.py
--rw-r--r--   0 cheese     (501) staff       (20)     2287 2023-08-01 09:12:11.000000 CheeseAPI-0.0.7/CheeseAPI/module.py
--rw-r--r--   0 cheese     (501) staff       (20)     3391 2023-08-07 14:49:57.000000 CheeseAPI-0.0.7/CheeseAPI/request.py
--rw-r--r--   0 cheese     (501) staff       (20)    12440 2023-08-01 08:05:03.000000 CheeseAPI-0.0.7/CheeseAPI/response.py
--rw-r--r--   0 cheese     (501) staff       (20)     4314 2023-08-07 08:33:10.000000 CheeseAPI-0.0.7/CheeseAPI/route.py
--rw-r--r--   0 cheese     (501) staff       (20)     3709 2023-08-02 09:26:09.000000 CheeseAPI-0.0.7/CheeseAPI/server.py
--rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.7/CheeseAPI/system.py
--rw-r--r--   0 cheese     (501) staff       (20)     1345 2023-08-01 07:01:25.000000 CheeseAPI-0.0.7/CheeseAPI/websocket.py
--rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.7/CheeseAPI/workspace.py
-drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-07 15:01:26.476286 CheeseAPI-0.0.7/CheeseAPI.egg-info/
--rw-r--r--   0 cheese     (501) staff       (20)     7964 2023-08-07 15:01:26.000000 CheeseAPI-0.0.7/CheeseAPI.egg-info/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-07 15:01:26.000000 CheeseAPI-0.0.7/CheeseAPI.egg-info/SOURCES.txt
--rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-07 15:01:26.000000 CheeseAPI-0.0.7/CheeseAPI.egg-info/dependency_links.txt
--rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-07 15:01:26.000000 CheeseAPI-0.0.7/CheeseAPI.egg-info/entry_points.txt
--rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-07 15:01:26.000000 CheeseAPI-0.0.7/CheeseAPI.egg-info/requires.txt
--rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-07 15:01:26.000000 CheeseAPI-0.0.7/CheeseAPI.egg-info/top_level.txt
--rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.7/LICENSE
--rw-r--r--   0 cheese     (501) staff       (20)     7964 2023-08-07 15:01:26.476488 CheeseAPI-0.0.7/PKG-INFO
--rw-r--r--   0 cheese     (501) staff       (20)     7513 2023-08-03 09:30:51.000000 CheeseAPI-0.0.7/README.md
--rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-07 15:01:26.476669 CheeseAPI-0.0.7/setup.cfg
--rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-07 15:00:55.000000 CheeseAPI-0.0.7/setup.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-09 02:47:16.964375 CheeseAPI-0.0.8/
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-09 02:47:16.963177 CheeseAPI-0.0.8/CheeseAPI/
+-rw-r--r--   0 cheese     (501) staff       (20)      326 2023-08-08 02:39:46.000000 CheeseAPI-0.0.8/CheeseAPI/__init__.py
+-rw-r--r--   0 cheese     (501) staff       (20)    17021 2023-08-09 02:20:48.000000 CheeseAPI-0.0.8/CheeseAPI/app.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1636 2023-08-01 09:45:24.000000 CheeseAPI-0.0.8/CheeseAPI/cSignal.py
+-rw-r--r--   0 cheese     (501) staff       (20)     8448 2023-08-09 01:07:16.000000 CheeseAPI-0.0.8/CheeseAPI/command.py
+-rw-r--r--   0 cheese     (501) staff       (20)      492 2023-07-31 08:17:28.000000 CheeseAPI-0.0.8/CheeseAPI/exception.py
+-rw-r--r--   0 cheese     (501) staff       (20)     2434 2023-08-01 05:36:54.000000 CheeseAPI-0.0.8/CheeseAPI/file.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3538 2023-08-09 02:36:31.000000 CheeseAPI-0.0.8/CheeseAPI/module.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3400 2023-08-08 02:39:46.000000 CheeseAPI-0.0.8/CheeseAPI/request.py
+-rw-r--r--   0 cheese     (501) staff       (20)    12449 2023-08-08 02:39:46.000000 CheeseAPI-0.0.8/CheeseAPI/response.py
+-rw-r--r--   0 cheese     (501) staff       (20)     4314 2023-08-07 08:33:10.000000 CheeseAPI-0.0.8/CheeseAPI/route.py
+-rw-r--r--   0 cheese     (501) staff       (20)     3829 2023-08-09 01:07:43.000000 CheeseAPI-0.0.8/CheeseAPI/server.py
+-rw-r--r--   0 cheese     (501) staff       (20)      676 2023-07-31 08:11:41.000000 CheeseAPI-0.0.8/CheeseAPI/system.py
+-rw-r--r--   0 cheese     (501) staff       (20)     1478 2023-08-09 01:23:16.000000 CheeseAPI-0.0.8/CheeseAPI/websocket.py
+-rw-r--r--   0 cheese     (501) staff       (20)      295 2023-07-31 08:11:30.000000 CheeseAPI-0.0.8/CheeseAPI/workspace.py
+drwxr-xr-x   0 cheese     (501) staff       (20)        0 2023-08-09 02:47:16.963970 CheeseAPI-0.0.8/CheeseAPI.egg-info/
+-rw-r--r--   0 cheese     (501) staff       (20)     7964 2023-08-09 02:47:16.000000 CheeseAPI-0.0.8/CheeseAPI.egg-info/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)      516 2023-08-09 02:47:16.000000 CheeseAPI-0.0.8/CheeseAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 cheese     (501) staff       (20)        1 2023-08-09 02:47:16.000000 CheeseAPI-0.0.8/CheeseAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       56 2023-08-09 02:47:16.000000 CheeseAPI-0.0.8/CheeseAPI.egg-info/entry_points.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       57 2023-08-09 02:47:16.000000 CheeseAPI-0.0.8/CheeseAPI.egg-info/requires.txt
+-rw-r--r--   0 cheese     (501) staff       (20)       10 2023-08-09 02:47:16.000000 CheeseAPI-0.0.8/CheeseAPI.egg-info/top_level.txt
+-rw-r--r--   0 cheese     (501) staff       (20)     1070 2023-07-26 13:50:19.000000 CheeseAPI-0.0.8/LICENSE
+-rw-r--r--   0 cheese     (501) staff       (20)     7964 2023-08-09 02:47:16.964187 CheeseAPI-0.0.8/PKG-INFO
+-rw-r--r--   0 cheese     (501) staff       (20)     7513 2023-08-03 09:30:51.000000 CheeseAPI-0.0.8/README.md
+-rw-r--r--   0 cheese     (501) staff       (20)       38 2023-08-09 02:47:16.964421 CheeseAPI-0.0.8/setup.cfg
+-rw-r--r--   0 cheese     (501) staff       (20)      984 2023-08-09 02:46:02.000000 CheeseAPI-0.0.8/setup.py
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI/app.py` & `CheeseAPI-0.0.8/CheeseAPI/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os, time, inspect, traceback, multiprocessing, json, shutil
 from typing import Callable, AsyncIterator, Dict, List, Any, Set
 from multiprocessing.process import BaseProcess
 
 import CheeseLog, asyncio
 from CheeseLog import logger, Logger
 
-from . import exception
-from .route import Route, matchPath
-from .request import Request
-from .response import Response, BaseResponse, FileResponse
-from .file import File
-from .websocket import websocket
-from .module import LocalModule, Module
-from .cSignal import signal
+from CheeseAPI import exception
+from CheeseAPI.route import Route, matchPath
+from CheeseAPI.request import Request
+from CheeseAPI.response import Response, BaseResponse, FileResponse
+from CheeseAPI.file import File
+from CheeseAPI.websocket import websocket
+from CheeseAPI.module import LocalModule, Module
+from CheeseAPI.cSignal import signal
 
 async def doFunc(func: Callable, kwargs: Dict[str, Any] = {}):
     if hasattr(func, '__wrapped__'):
         _kwargs = kwargs
     else:
         _kwargs = {}
         sig = inspect.signature(func)
@@ -28,17 +28,17 @@
     else:
         return func(**_kwargs)
 
 class App:
     def __init__(self):
         self.startTimer: float = time.time()
 
-        from .system import System
-        from .workspace import Workspace
-        from .server import Server
+        from CheeseAPI.system import System
+        from CheeseAPI.workspace import Workspace
+        from CheeseAPI.server import Server
 
         self.process: BaseProcess = multiprocessing.current_process()
         self.logger: Logger = logger
 
         self.system: System = System()
         self.workspace: Workspace = Workspace()
         self.server: Server = Server(self)
@@ -262,22 +262,15 @@
                 await send({
                     'type': 'websocket.accept'
                 })
 
                 if (await receive())['type'] == 'websocket.connect':
                     CheeseLog.websocket(f'{request.ip} connected {request.path}', f'{request.ip} connected \033[36m{request.path}\033[0m')
 
-                    websocket._CLIENTS[request.sid] = asyncio.Queue()
-                    async def sendHandle():
-                        try:
-                            while True:
-                                await (await websocket._CLIENTS[request.sid].get())(send)
-                        except asyncio.CancelledError:
-                            ...
-                    task = asyncio.create_task(sendHandle())
+                    task = asyncio.create_task(self._websocket_sendHandle(send, request))
 
                     while True:
                         message = await receive()
                         if message['type'] == 'websocket.receive':
                             if 'text' in message:
                                 kwargs['value'] = message['text']
                             elif 'bytes' in message:
@@ -296,14 +289,22 @@
                     await doFunc(websocket_afterDisconnectHandle, kwargs)
             except Exception as e:
                 CheeseLog.danger(f'The error occured while accessing the WEBSOCKET {request.fullPath}\n{traceback.format_exc()}'[:-1], f'The error occured while accessing the \033[36mWEBSOCKET {request.fullPath}\033[0m\n{traceback.format_exc()}'[:-1])
                 for websocket_errorHandle in self.websocket_errorHandles:
                     kwargs['exception'] = e
                     await doFunc(websocket_errorHandle, kwargs)
 
+    async def _websocket_sendHandle(self, send, request: Request):
+        websocket._CLIENTS[request.sid] = asyncio.Queue()
+        try:
+            while True:
+                await (await websocket._CLIENTS[request.sid].get())(send)
+        except asyncio.CancelledError:
+            ...
+
     def server_startingHandle(self, func: Callable):
         self.server_startingHandles.append(func)
 
     def server_endingHandle(self, func: Callable):
         self.server_endingHandles.append(func)
 
     def http_response404Handle(self, func: Callable):
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI/cSignal.py` & `CheeseAPI-0.0.8/CheeseAPI/cSignal.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.7/CheeseAPI/command.py` & `CheeseAPI-0.0.8/CheeseAPI/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import argparse, time, os, traceback, json, shutil, importlib, importlib.util
+import argparse, time, os, traceback, json, shutil, sys
 
 import CheeseLog, uvicorn, CheeseType, CheeseType.network, uvicorn.importer
 
-from .module import Module, LocalModule
-
 def command():
-    from .app import app
-    from .cSignal import signal
+    sys.path.append(os.getcwd())
+
+    from CheeseAPI.module import Module, LocalModule
+    from CheeseAPI.app import app, App
+    from CheeseAPI.cSignal import signal
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--app', nargs = '?', default = 'app:app', help = '服务器本服务【默认值：app:app】')
     parser.add_argument('--host', nargs = '?', default = '127.0.0.1', help = '服务器地址【默认值：127.0.0.1】')
     parser.add_argument('--port', type = int, nargs = '?', default = 5214, help = '端口号【默认值：5214】')
     parser.add_argument('--reload', action='store_true', help = '热更新。与workers冲突【默认值：False】')
     parser.add_argument('--workers', type = int, nargs = '?', default = 1, help = 'workers为0时会自动设置为cpu核数*2。与reload冲突【默认值：1】')
@@ -102,17 +103,15 @@
 is debug: \033[34m{app.server.IS_DEBUG}\033[0m
 is request logged: \033[34m{app.server.IS_REQUEST_LOGGED}\033[0m''' + (f'''
 static path: \033[34m{app.server.STATIC_PATH}\033[0m''' if app.server.STATIC_PATH is not False else '') + (f'''
 current log file path: \033[4;36m.{app.logger.filePath[len(app.workspace.BASE_PATH):]}\033[0m''' if app.server.LOG_FILENAME is not False else ''))
 
     CheeseLog.starting(f'The server running on http://{app.server.HOST}:{app.server.PORT}', f'The server running on \033[4;36mhttp://{app.server.HOST}:{app.server.PORT}\033[0m')
 
-    import sys
-    sys.path.append(os.getcwd())
-    app = eval(f'__import__(\'{_app.split(":")[0]}\').{_app.split(":")[1]}')
+    app: App = eval(f'__import__(\'{_app.split(":")[0]}\').{_app.split(":")[1]}')
 
     _modules = set()
     if len(app.modules):
         CheeseLog.starting(f'Modules:\n{" | ".join(app.modules)}')
     for module in app.modules:
         _modules.add(Module(_modules, module))
     app.modules = _modules
@@ -175,7 +174,10 @@
         endingMessage += f'{minutes} minutes '
         endingColorfulMessage += f'\033[34m{minutes}\033[0m minutes '
     endingMessage += '{:.6f} seconds'.format(runningTime % 60)
     endingColorfulMessage += '\033[34m{:.6f}\033[0m seconds'.format(runningTime % 60)
     CheeseLog.ending(endingMessage, endingColorfulMessage)
     if app.logger.is_alive():
         app.logger.stop()
+
+if __name__ == '__main__':
+    command()
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI/file.py` & `CheeseAPI-0.0.8/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.7/CheeseAPI/module.py` & `CheeseAPI-0.0.8/CheeseAPI/module.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,25 +22,47 @@
             ...
         if dependencies:
             for dependency in dependencies:
                 if modules not in modules:
                     modules.add(Module(modules, dependency))
 
         modulePath = os.path.dirname(inspect.getfile(mainModule))
-        for filename in os.listdir(modulePath):
-            filePath = os.path.join(modulePath, filename)
-            if os.path.isfile(filePath) and filename != '__init__.py':
-                filename = filename[:-3]
-                try:
-                    module = __import__(f'{self.name}.{filename}')
-                except:
-                    CheeseLog.error(f'The error occured while the module \'{name}\' loading\n{traceback.format_exc()}'[:-1])
-                    raise SystemExit()
 
-                self.subModules.add(module)
+        if not hasattr(mainModule, 'moduleType'):
+            CheeseLog.error(f'The error occured while the module \'{name}\' loading:\nUnknown module type')
+            raise SystemExit()
+
+        if mainModule.moduleType == 'single':
+            for filename in os.listdir(modulePath):
+                filePath = os.path.join(modulePath, filename)
+                if os.path.isfile(filePath) and filename != '__init__.py':
+                    filename = filename[:-3]
+                    try:
+                        module = __import__(f'{self.name}.{filename}')
+                    except:
+                        CheeseLog.error(f'The error occured while the module \'{name}\' loading:\n{traceback.format_exc()}'[:-1])
+                        raise SystemExit()
+
+                    self.subModules.add(module)
+        elif mainModule.moduleType == 'multiple':
+            for foldername in os.listdir(modulePath):
+                folderPath = os.path.join(modulePath, foldername)
+                if os.path.isdir(folderPath):
+                    for filename in os.listdir(folderPath):
+                        filePath = os.path.join(folderPath, filename)
+                        if os.path.isfile(filePath) and filename != '__init__.py':
+                            filename = filename[:-3]
+                            try:
+                                module = __import__(f'{self.name}.{filename}')
+                            except:
+                                CheeseLog.error(f'The error occured while the module \'{name}\' loading:\n{traceback.format_exc()}'[:-1])
+                                raise SystemExit()
+        else:
+            CheeseLog.error(f'The error occured while the module \'{name}\' loading:\nUnknown module type')
+            raise SystemExit()
 
 class LocalModule:
     def __init__(self, basePath: str, name: str):
         self.name: str = name
         self.subModules: Set[str] = set()
 
         modulePath = os.path.join(basePath, name)
@@ -50,10 +72,10 @@
         for filename in os.listdir(modulePath):
             filePath = os.path.join(modulePath, filename)
             if os.path.isfile(filePath) and filename != '__init__.py':
                 filename = filename[:-3]
                 try:
                     module = __import__(f'{self.name}.{filename}')
                 except:
-                    CheeseLog.error(f'The error occured while the local module \'{name}\' loading\n{traceback.format_exc()}'[:-1])
+                    CheeseLog.error(f'The error occured while the local module \'{name}\' loading:\n{traceback.format_exc()}'[:-1])
                     raise SystemExit()
                 self.subModules.add(module)
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI/request.py` & `CheeseAPI-0.0.8/CheeseAPI/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json, traceback, re
 from typing import TypeVar, Dict
 from urllib.parse import unquote
 
 import CheeseType.network, xmltodict, CheeseLog
 
-from .file import File
+from CheeseAPI.file import File
 
 T = TypeVar('T')
 
 class BaseItem:
     def __init__(self):
         self._values: Dict[str, str] = {}
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI/response.py` & `CheeseAPI-0.0.8/CheeseAPI/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Dict, Any
 
-from .file import File
+from CheeseAPI.file import File
 
 CONTENT_TYPE = {
     'tif': 'image/tiff',
     '001': 'application/x-001',
     '301': 'application/x-301',
     '323': 'text/h323',
     '906': 'application/x-906',
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI/route.py` & `CheeseAPI-0.0.8/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.7/CheeseAPI/server.py` & `CheeseAPI-0.0.8/CheeseAPI/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, datetime
 
 import CheeseType, CheeseType.network
 
 class Server:
     def __init__(self, app):
-        from .app import App
+        from CheeseAPI.app import App
 
         self._app: App = app
         self.HOST: CheeseType.network.IPv4 = '127.0.0.1'
         self.PORT: CheeseType.network.Port = 5214
         self._WORKERS: CheeseType.NonNegativeInt = 1
         self.IS_RELOAD: bool = False
 
@@ -63,34 +63,35 @@
 
     @property
     def LOG_FILENAME(self) -> str | bool:
         return self._LOG_FILENAME
 
     @LOG_FILENAME.setter
     def LOG_FILENAME(self, value):
-        if self._app.process.name == 'MainProcess':
-            if value is not False:
-                if value is True:
-                    self._LOG_FILENAME = datetime.datetime.now().strftime('%Y_%m_%d-%H_%M_%S.log')
-                else:
-                    self._LOG_FILENAME = datetime.datetime.now().strftime(str(value))
-                self._app.logger.filePath = os.path.join(self._app.workspace.BASE_PATH + self._app.workspace.LOG_PATH + self.LOG_FILENAME)
-            elif value is False:
-                self._LOG_FILENAME = False
-                self._app.logger.filePath = None
-        else:
-            logPath = os.path.join(self._app.workspace.BASE_PATH + self._app.workspace.LOG_PATH)
-            logFiles = [ os.path.join(logPath, file) for file in os.listdir(logPath) if os.path.isfile(os.path.join(logPath, file)) ]
-            if not logFiles:
-                self._LOG_FILENAME = False
-                self._app.logger.filePath = None
+        if value is not False:
+            if self._app.process.name == 'MainProcess':
+                if value is not False:
+                    if value is True:
+                        self._LOG_FILENAME = datetime.datetime.now().strftime('%Y_%m_%d-%H_%M_%S.log')
+                    else:
+                        self._LOG_FILENAME = datetime.datetime.now().strftime(str(value))
+                    self._app.logger.filePath = os.path.join(self._app.workspace.BASE_PATH + self._app.workspace.LOG_PATH + self.LOG_FILENAME)
+                elif value is False:
+                    self._LOG_FILENAME = False
+                    self._app.logger.filePath = None
             else:
-                logFile = max(logFiles, key = os.path.getmtime)
-                self._LOG_FILENAME = logFile.split('/')[-1]
-                self._app.logger.filePath = logFile
+                logPath = os.path.join(self._app.workspace.BASE_PATH + self._app.workspace.LOG_PATH)
+                logFiles = [ os.path.join(logPath, file) for file in os.listdir(logPath) if os.path.isfile(os.path.join(logPath, file)) ]
+                if not logFiles:
+                    self._LOG_FILENAME = False
+                    self._app.logger.filePath = None
+                else:
+                    logFile = max(logFiles, key = os.path.getmtime)
+                    self._LOG_FILENAME = logFile.split('/')[-1]
+                    self._app.logger.filePath = logFile
 
     @property
     def STATIC_PATH(self) -> str | bool:
         return self._STATIC_PATH
 
     @STATIC_PATH.setter
     def STATIC_PATH(self, value):
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI/system.py` & `CheeseAPI-0.0.8/CheeseAPI/system.py`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.7/CheeseAPI/websocket.py` & `CheeseAPI-0.0.8/CheeseAPI/websocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Dict
 
 import asyncio
 
+from CheeseAPI.route import matchPath
+
 class Websocket:
     def __init__(self):
         self._CLIENTS: Dict[str, asyncio.Queue] = {}
 
     async def _send(self, message: any, sid: str):
         if sid in self._CLIENTS:
             if isinstance(message, bytes):
@@ -18,23 +20,25 @@
                 async def func(send):
                     await send({
                         'type': 'websocket.send',
                         'text': str(message)
                     })
             await self._CLIENTS[sid].put(func)
 
-    async def send(self, message: any, sid: str | list[str] | None = None):
-        if not sid:
-            for key in self._CLIENTS:
-                await self._send(message, key)
-        elif isinstance(sid, list):
-            for s in sid:
-                await self._send(message, s)
-        else:
-            await self._send(message, sid)
+    async def send(self, message: any, path: str, sid: str | list[str] | None = None):
+        func, _ = matchPath(path)
+        if func:
+            if not sid:
+                for key in self._CLIENTS:
+                    await self._send(message, key)
+            elif isinstance(sid, list):
+                for s in sid:
+                    await self._send(message, s)
+            else:
+                await self._send(message, sid)
 
     async def _close(self, send):
         await send({
             'type': 'websocket.close'
         })
 
     async def close(self, sid: str):
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI.egg-info/PKG-INFO` & `CheeseAPI-0.0.8/CheeseAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.7
+Version: 0.0.8
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseAPI-0.0.7/CheeseAPI.egg-info/SOURCES.txt` & `CheeseAPI-0.0.8/CheeseAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.7/LICENSE` & `CheeseAPI-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.7/PKG-INFO` & `CheeseAPI-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CheeseAPI
-Version: 0.0.7
+Version: 0.0.8
 Summary: 一款基于uvicorn的web协程框架
 Home-page: https://github.com/CheeseUnknown/CheeseAPI
 Author: Cheese Unknown
 Author-email: cheese@cheese.ren
 License: MIT
 Keywords: api framework backend asyncio
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CheeseAPI-0.0.7/README.md` & `CheeseAPI-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `CheeseAPI-0.0.7/setup.py` & `CheeseAPI-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('./README.md', 'r', encoding = 'utf-8') as f:
     longDescription = f.read()
 
 setuptools.setup(
     name = 'CheeseAPI',
-    version = '0.0.7',
+    version = '0.0.8',
     author = 'Cheese Unknown',
     author_email = 'cheese@cheese.ren',
     description = '一款基于uvicorn的web协程框架',
     long_description = longDescription,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/CheeseUnknown/CheeseAPI',
     license = 'MIT',
```

