# Comparing `tmp/DownloadKit-0.5.3.tar.gz` & `tmp/DownloadKit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DownloadKit-0.5.3.tar", last modified: Wed Feb 22 16:01:16 2023, max compression
+gzip compressed data, was "DownloadKit-1.0.0.tar", last modified: Wed Aug  9 03:43:18 2023, max compression
```

## Comparing `DownloadKit-0.5.3.tar` & `DownloadKit-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 16:01:16.115068 DownloadKit-0.5.3/
-drwxrwxrwx   0        0        0        0 2023-02-22 16:01:16.051555 DownloadKit-0.5.3/DownloadKit/
--rw-rw-rw-   0        0        0       62 2022-01-28 13:46:54.000000 DownloadKit-0.5.3/DownloadKit/__init__.py
--rw-rw-rw-   0        0        0     9034 2023-02-22 11:13:08.000000 DownloadKit-0.5.3/DownloadKit/_funcs.py
--rw-rw-rw-   0        0        0     1390 2023-01-23 15:16:53.000000 DownloadKit-0.5.3/DownloadKit/_funcs.pyi
--rw-rw-rw-   0        0        0    23210 2023-02-22 15:49:07.000000 DownloadKit-0.5.3/DownloadKit/downloadKit.py
--rw-rw-rw-   0        0        0     5220 2023-01-26 08:26:48.000000 DownloadKit-0.5.3/DownloadKit/downloadKit.pyi
--rw-rw-rw-   0        0        0     9469 2023-01-26 08:26:49.000000 DownloadKit-0.5.3/DownloadKit/mission.py
--rw-rw-rw-   0        0        0     3399 2023-01-26 14:37:58.000000 DownloadKit-0.5.3/DownloadKit/mission.pyi
-drwxrwxrwx   0        0        0        0 2023-02-22 16:01:16.110645 DownloadKit-0.5.3/DownloadKit.egg-info/
--rw-rw-rw-   0        0        0    10352 2023-02-22 16:01:15.000000 DownloadKit-0.5.3/DownloadKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-02-22 16:01:15.000000 DownloadKit-0.5.3/DownloadKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 16:01:15.000000 DownloadKit-0.5.3/DownloadKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-02-22 16:01:15.000000 DownloadKit-0.5.3/DownloadKit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-22 16:01:15.000000 DownloadKit-0.5.3/DownloadKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1534 2021-08-14 13:50:06.000000 DownloadKit-0.5.3/LICENSE
--rw-rw-rw-   0        0        0       25 2023-01-23 15:02:16.000000 DownloadKit-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0    10352 2023-02-22 16:01:16.114057 DownloadKit-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     9835 2023-01-26 14:24:03.000000 DownloadKit-0.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-02-22 16:01:16.115068 DownloadKit-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-02-22 15:47:27.000000 DownloadKit-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:43:18.195265 DownloadKit-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-08-09 03:43:18.164030 DownloadKit-1.0.0/DownloadKit/
+-rw-rw-rw-   0        0        0       62 2022-01-28 13:46:56.000000 DownloadKit-1.0.0/DownloadKit/__init__.py
+-rw-rw-rw-   0        0        0     9506 2023-07-28 10:16:10.000000 DownloadKit-1.0.0/DownloadKit/_funcs.py
+-rw-rw-rw-   0        0        0     1221 2023-05-16 15:21:36.000000 DownloadKit-1.0.0/DownloadKit/_funcs.pyi
+-rw-rw-rw-   0        0        0    27643 2023-07-26 09:52:05.000000 DownloadKit-1.0.0/DownloadKit/downloadKit.py
+-rw-rw-rw-   0        0        0     7222 2023-07-28 10:00:36.000000 DownloadKit-1.0.0/DownloadKit/downloadKit.pyi
+-rw-rw-rw-   0        0        0    11246 2023-07-21 12:14:12.000000 DownloadKit-1.0.0/DownloadKit/mission.py
+-rw-rw-rw-   0        0        0     3527 2023-07-28 10:00:36.000000 DownloadKit-1.0.0/DownloadKit/mission.pyi
+drwxrwxrwx   0        0        0        0 2023-08-09 03:43:18.179643 DownloadKit-1.0.0/DownloadKit.egg-info/
+-rw-rw-rw-   0        0        0    10352 2023-08-09 03:43:18.000000 DownloadKit-1.0.0/DownloadKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-08-09 03:43:18.000000 DownloadKit-1.0.0/DownloadKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 03:43:18.000000 DownloadKit-1.0.0/DownloadKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-09 03:43:18.000000 DownloadKit-1.0.0/DownloadKit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-09 03:43:18.000000 DownloadKit-1.0.0/DownloadKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1534 2022-01-29 00:43:58.000000 DownloadKit-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-02-16 00:54:03.000000 DownloadKit-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10352 2023-08-09 03:43:18.179643 DownloadKit-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9835 2023-07-26 08:54:55.000000 DownloadKit-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-09 03:43:18.195265 DownloadKit-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      913 2023-08-09 02:33:14.000000 DownloadKit-1.0.0/setup.py
```

### Comparing `DownloadKit-0.5.3/DownloadKit/_funcs.py` & `DownloadKit-1.0.0/DownloadKit/_funcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,43 +64,24 @@
     def __get__(self, goal_path, objtype=None):
         return goal_path._goal_path
 
 
 class FileExistsSetter(object):
     def __set__(self, file_exists, mode):
         mode = mode.lower()
-        if mode not in ('skip', 'overwrite', 'rename'):
-            raise ValueError("file_exists参数只能传入'skip', 'overwrite', 'rename'")
+        if mode not in ('skip', 'overwrite', 'rename', 'add'):
+            raise ValueError("file_exists参数只能传入'skip', 'overwrite', 'rename', 'add'")
         file_exists._file_exists = mode
 
     def __get__(self, file_exists, objtype=None):
         return file_exists._file_exists
 
 
-class LogMode(object):
-    """设置记录或打印哪些任务信息"""
-
-    def __init__(self):
-        self.log_mode = None
-
-    def all(self):
-        """全部"""
-        self.log_mode = 'all'
-
-    def none(self):
-        """不记录或打印"""
-        self.log_mode = None
-
-    def fail(self):
-        """只记录或打印失败任务"""
-        self.log_mode = 'fail'
-
-
 def get_usable_path(path):
-    """检查文件或文件夹是否有重名，并返回可以使用的路径           \n
+    """检查文件或文件夹是否有重名，并返回可以使用的路径
     :param path: 文件或文件夹路径
     :return: 可用的路径，Path对象
     """
     path = Path(path)
     parent = path.parent
     path = parent / make_valid_name(path.name)
     name = path.stem if path.is_file() else path.name
@@ -120,15 +101,15 @@
         path = parent / f'{name}{ext}'
         first_time = None
 
     return path
 
 
 def make_valid_name(full_name):
-    """获取有效的文件名                  \n
+    """获取有效的文件名
     :param full_name: 文件名
     :return: 可用的文件名
     """
     # ----------------去除前后空格----------------
     full_name = full_name.strip()
 
     # ----------------使总长度不大于255个字符（一个汉字是2个字符）----------------
@@ -146,26 +127,28 @@
     full_name = f'{name}{ext}'
 
     # ----------------去除不允许存在的字符----------------
     return sub(r'[<>/\\|:*?\n]', '', full_name)
 
 
 def get_long(txt):
-    """返回字符串中字符个数（一个汉字是2个字符）          \n
+    """返回字符串中字符个数（一个汉字是2个字符）
     :param txt: 字符串
     :return: 字符个数
     """
     txt_len = len(txt)
     return int((len(txt.encode('utf-8')) - txt_len) / 2 + txt_len)
 
 
 def set_charset(response):
     """设置Response对象的编码"""
     # 在headers中获取编码
     content_type = response.headers.get('content-type', '').lower()
+    if not content_type.endswith(';'):
+        content_type += ';'
     charset = search(r'charset[=: ]*(.*)?;?', content_type)
 
     if charset:
         response.encoding = charset.group(1)
 
     # 在headers中获取不到编码，且如果是网页
     elif content_type.replace(' ', '').startswith('text/html'):
@@ -178,15 +161,15 @@
 
         response.encoding = charset
 
     return response
 
 
 def get_file_info(response, goal_path=None, rename=None, file_exists=None, lock=None):
-    """获取文件信息，大小单位为byte                   \n
+    """获取文件信息，大小单位为byte
     包括：size、path、skip
     :param response: Response对象
     :param goal_path: 目标文件夹
     :param rename: 重命名
     :param file_exists: 存在重名文件时的处理方式
     :param lock: 线程锁
     :return: 文件名、文件大小、保存路径、是否跳过
@@ -204,40 +187,45 @@
     goal_path = goal_Path.anchor + sub(r'[*:|<>?"]', '', goal_path.lstrip(goal_Path.anchor)).strip()
     goal_Path = Path(goal_path).absolute()
     goal_Path.mkdir(parents=True, exist_ok=True)
 
     # ------------获取保存文件名------------
     # -------------------重命名，不改变扩展名-------------------
     if rename:
-        ext_name = file_name.split('.')[-1]
-        if '.' in rename or ext_name == file_name:  # 新文件名带后缀或原文件名没有后缀
-            full_name = rename
-        else:
-            full_name = f'{rename}.{ext_name}'
+        tmp = file_name.rsplit('.', 1)
+        ext_name = tmp[-1] if len(tmp) > 1 else ''
+        tmp = rename.rsplit('.', 1)
+        ext_rename = tmp[-1] if len(tmp) > 1 else ''
+        full_name = rename if ext_rename == ext_name else f'{rename}.{ext_name}'
     else:
         full_name = file_name
 
     full_name = make_valid_name(full_name)
 
     # -------------------生成路径-------------------
     skip = False
+    create = True
     full_path = goal_Path / full_name
 
     with lock:
         if full_path.exists():
             if file_exists == 'rename':
                 full_path = get_usable_path(full_path)
 
             elif file_exists == 'skip':
                 skip = True
+                create = False
 
             elif file_exists == 'overwrite':
                 full_path.unlink()
 
-        if not skip:
+            elif file_exists == 'add':
+                create = False
+
+        if create:
             with open(full_path, 'wb'):
                 pass
 
     return {'size': file_size,
             'path': full_path,
             'skip': skip}
 
@@ -278,7 +266,28 @@
     # 找不到则用时间和随机数生成文件名
     if not file_name:
         file_name = f'untitled_{time()}_{randint(0, 100)}'
 
     # 去除非法字符
     charset = charset or 'utf-8'
     return unquote(file_name, charset)
+
+
+def set_session_cookies(session, cookies):
+    """设置Session对象的cookies
+    :param session: Session对象
+    :param cookies: cookies信息
+    :return: None
+    """
+    # cookies = cookies_to_tuple(cookies)
+    for cookie in cookies:
+        if cookie['value'] is None:
+            cookie['value'] = ''
+
+        kwargs = {x: cookie[x] for x in cookie
+                  if x.lower() in ('version', 'port', 'domain', 'path', 'secure',
+                                   'expires', 'discard', 'comment', 'comment_url', 'rest')}
+
+        if 'expiry' in cookie:
+            kwargs['expires'] = cookie['expiry']
+
+        session.cookies.set(cookie['name'], cookie['value'], **kwargs)
```

### Comparing `DownloadKit-0.5.3/DownloadKit/_funcs.pyi` & `DownloadKit-1.0.0/DownloadKit/_funcs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -27,27 +27,14 @@
 
 class FileExistsSetter(object):
     def __set__(self, file_exists, mode: str): ...
 
     def __get__(self, file_exists, objtype=None): ...
 
 
-class LogMode(object):
-    """设置记录或打印哪些任务信息"""
-
-    def __init__(self):
-        self.log_mode: str = ...
-
-    def all(self) -> None: ...
-
-    def none(self) -> None: ...
-
-    def fail(self) -> None: ...
-
-
 def get_usable_path(path: Union[str, Path]) -> Path: ...
 
 
 def make_valid_name(full_name: str) -> str: ...
 
 
 def get_long(txt: str) -> int: ...
@@ -57,7 +44,10 @@
 
 
 def get_file_info(response: Response,
                   goal_path: str = None,
                   rename: str = None,
                   file_exists: str = None,
                   lock: Lock = None) -> dict: ...
+
+
+def set_session_cookies(session: Session, cookies: list) -> None: ...
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `DownloadKit-0.5.3/DownloadKit/downloadKit.pyi` & `DownloadKit-1.0.0/DownloadKit/downloadKit.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -2,166 +2,238 @@
 """
 @Author  :   g1879
 @Contact :   g1879@qq.com
 """
 from pathlib import Path
 from queue import Queue
 from threading import Lock
-from typing import Union, Tuple, Any
+from typing import Union, Tuple, Any, Literal, Optional
 
 from DataRecorder import Recorder
+from DrissionPage import SessionOptions
 from DrissionPage.base import BasePage
 from requests import Session, Response
 
-from ._funcs import FileExistsSetter, PathSetter, BlockSizeSetter, LogMode
+from ._funcs import FileExistsSetter, PathSetter, BlockSizeSetter
 from .mission import Task, Mission, BaseTask
 
+FILE_EXISTS = Literal['add', 'skip', 'rename', 'overwrite']
+
 
 class DownloadKit(object):
     file_exists: FileExistsSetter = ...
     goal_path: PathSetter = ...
     block_size: BlockSizeSetter = ...
 
     def __init__(self,
                  goal_path: Union[str, Path] = None,
                  roads: int = 10,
                  session: Union[Session, BasePage] = None,
-                 file_exists: str = 'rename'):
+                 file_exists: FILE_EXISTS = 'rename'):
         self._roads: int = ...
-        self._print_mode: LogMode = ...
-        self._log_mode: LogMode = ...
+        self._setter: Setter = ...
+        self._print_mode: str = ...
+        self._log_mode: str = ...
         self._logger: Recorder = ...
         self._retry: int = ...
         self._interval: float = ...
-        self._page: Union[BasePage, None] = ...
+        self.page: Optional[BasePage] = ...
         self._waiting_list: Queue = ...
         self._session: Session = ...
         self._running_count: int = ...
         self._missions_num: int = ...
         self._missions: dict = ...
         self._threads: dict = ...
-        self.split: bool = ...
         self._timeout: Union[int, float] = ...
         self._stop_printing: bool = ...
         self._lock: Lock = ...
+        self._copy_cookies: bool = ...
+
+        self.goal_path: str = ...
+        self.file_exists: FILE_EXISTS = ...
+        self.split: bool = ...
+        self.block_size: Union[str, int] = ...
 
     def __call__(self,
                  file_url: str,
-                 goal_path: Union[str, Path] = None,
+                 goal_path: Optional[str, Path] = None,
                  rename: str = None,
-                 file_exists: str = None,
+                 file_exists: FILE_EXISTS = None,
                  show_msg: bool = True,
-                 timeout: Union[float | None] = None,
-                 params: Union[dict | None] = ...,
-                 json: Union[dict, str, None] = ...,
-                 headers: Union[dict | None] = ...,
+                 timeout: Optional[float] = None,
+                 params: Optional[dict] = ...,
+                 data: Any = ...,
+                 json: Any = ...,
+                 headers: Optional[dict] = ...,
                  cookies: Any = ...,
                  files: Any = ...,
                  auth: Any = ...,
                  allow_redirects: bool = ...,
-                 proxies: Union[dict | None] = ...,
+                 proxies: Optional[dict] = ...,
                  hooks: Any = ...,
                  stream: Any = ...,
                  verify: Any = ...,
                  cert: Any = ...) -> tuple: ...
 
-    def set_print(self) -> LogMode: ...
-
-    def set_log(self, log_path: [str, Path] = None) -> LogMode: ...
+    @property
+    def set(self) -> Setter: ...
 
     @property
     def roads(self) -> int: ...
 
-    @roads.setter
-    def roads(self, val: int) -> None: ...
-
     @property
     def retry(self) -> int: ...
 
-    @retry.setter
-    def retry(self, times: int) -> None: ...
-
     @property
     def interval(self) -> float: ...
 
-    @interval.setter
-    def interval(self, seconds: Union[int, float]) -> None: ...
-
     @property
     def timeout(self) -> float: ...
 
-    @timeout.setter
-    def timeout(self, seconds: Union[int, float]) -> None: ...
-
     @property
     def waiting_list(self) -> Queue: ...
 
     @property
     def session(self) -> Session: ...
 
-    @session.setter
-    def session(self, session: Union[Session, BasePage]) -> None: ...
-
     @property
     def is_running(self) -> bool: ...
 
     @property
     def missions(self) -> dict: ...
 
-    def set_proxies(self, http: str = None, https: str = None) -> None: ...
-
     def add(self,
             file_url: str,
-            goal_path: Union[str, Path] = None,
+            goal_path: Optional[str, Path] = None,
             rename: str = None,
-            file_exists: str = None,
-            data: Union[str, dict] = None,
+            file_exists: FILE_EXISTS = None,
             split: bool = None,
-            timeout: Union[float | None] = None,
-            params: Union[dict | None] = ...,
-            json: Union[dict, str, None] = ...,
-            headers: Union[dict | None] = ...,
+            timeout: Optional[float] = None,
+            params: Optional[dict] = ...,
+            data: Any = None,
+            json: Optional[dict, str] = ...,
+            headers: Optional[dict] = ...,
             cookies: Any = ...,
             files: Any = ...,
             auth: Any = ...,
             allow_redirects: bool = ...,
-            proxies: Union[dict | None] = ...,
+            proxies: Optional[dict] = ...,
             hooks: Any = ...,
             stream: Any = ...,
             verify: Any = ...,
             cert: Any = ...) -> Mission: ...
 
-    def _run_or_wait(self, mission: BaseTask): ...
+    def download(self,
+                 file_url: str,
+                 goal_path: Optional[str, Path] = None,
+                 rename: str = None,
+                 file_exists: FILE_EXISTS = None,
+                 show_msg: bool = True,
+                 timeout: Optional[float] = None,
+                 params: Optional[dict] = ...,
+                 data: Any = ...,
+                 json: Any = ...,
+                 headers: Optional[dict] = ...,
+                 cookies: Any = ...,
+                 files: Any = ...,
+                 auth: Any = ...,
+                 allow_redirects: bool = ...,
+                 proxies: Optional[dict] = ...,
+                 hooks: Any = ...,
+                 stream: Any = ...,
+                 verify: Any = ...,
+                 cert: Any = ...) -> tuple: ...
+
+    def _run_or_wait(self, mission: BaseTask) -> None: ...
 
     def _run(self, ID: int, mission: BaseTask) -> None: ...
 
     def get_mission(self, mission_or_id: Union[int, Mission]) -> Mission: ...
 
     def get_failed_missions(self) -> list: ...
 
     def wait(self,
              mission: Union[int, Mission] = None,
              show: bool = False,
-             timeout: float = None) -> Union[tuple, None]: ...
+             timeout: float = None) -> Optional[tuple]: ...
 
-    def cancel(self): ...
+    def cancel(self) -> None: ...
 
     def show(self, asyn: bool = True, keep: bool = False) -> None: ...
 
     def _show(self, wait: float, keep: bool = False) -> None: ...
 
-    def _connect(self,
-                 url: str,
-                 mode: str = 'get',
-                 data: Union[dict, str] = None,
-                 json: Union[dict, str] = None,
-                 **kwargs) -> Tuple[Union[Response, None], str]: ...
+    def _connect(self, url: str, session: Session, method: str, **kwargs) -> Tuple[Union[Response, None], str]: ...
 
-    def _get_usable_thread(self) -> Union[int, None]: ...
+    def _get_usable_thread(self) -> Optional[int]: ...
 
     def _stop_show(self) -> None: ...
 
     def _when_mission_done(self, mission: Mission) -> None: ...
 
     def _download(self,
                   mission_or_task: Union[Mission, Task],
                   thread_id: int) -> None: ...
+
+
+class Setter(object):
+    def __init__(self, downloadKit: DownloadKit):
+        self._downloadKit: DownloadKit = ...
+
+    @property
+    def DownloadKit(self) -> DownloadKit: ...
+
+    @property
+    def if_file_exists(self) -> FileExists: ...
+
+    @property
+    def log_mode(self) -> LogSet: ...
+
+    def driver(self, driver: Union[Session, BasePage, SessionOptions]) -> None: ...
+
+    def roads(self, num: int) -> None: ...
+
+    def retry(self, times: int) -> None: ...
+
+    def interval(self, seconds: float) -> None: ...
+
+    def timeout(self, seconds: float) -> None: ...
+
+    def goal_path(self, path: Union[str, Path]) -> None: ...
+
+    def split(self, on_off: bool) -> None: ...
+
+    def block_size(self, size: Union[str, int]) -> None: ...
+
+    def proxies(self, http: str = None, https: str = None) -> None: ...
+
+
+class LogSet(object):
+    def __init__(self, setter: Setter):
+        self._setter: Setter = ...
+
+    def log_path(self, log_path: Union[str, Path]) -> None: ...
+
+    def print_all(self) -> None: ...
+
+    def print_failed(self) -> None: ...
+
+    def print_nothing(self) -> None: ...
+
+    def log_all(self) -> None: ...
+
+    def log_failed(self) -> None: ...
+
+    def log_nothing(self) -> None: ...
+
+
+class FileExists(object):
+    def __init__(self, setter: Setter):
+        self._setter: Setter = ...
+
+    def __call__(self, mode: FILE_EXISTS): ...
+
+    def skip(self) -> None: ...
+
+    def rename(self) -> None: ...
+
+    def overwrite(self) -> None: ...
```

### Comparing `DownloadKit-0.5.3/DownloadKit/mission.py` & `DownloadKit-1.0.0/DownloadKit/mission.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 # -*- coding:utf-8 -*-
 """
 @Author  :   g1879
 @Contact :   g1879@qq.com
 """
 from pathlib import Path
 from time import sleep, perf_counter
-from typing import Union, List
+from urllib.parse import quote, urlparse
 
 from DataRecorder import ByteRecorder
+from requests.structures import CaseInsensitiveDict
 
+from ._funcs import copy_session, set_session_cookies
 
-class MissionData(object):
-    """保存任务数据的对象"""
 
-    def __init__(self, url, goal_path, rename, file_exists, data, json, split, kwargs):
-        """
+class MissionData(object):
+    def __init__(self, url, goal_path, rename, file_exists, split, kwargs, offset=0):
+        """保存任务数据的对象
         :param url: 下载文件url
         :param goal_path: 保存文件夹
         :param rename: 文件重命名
         :param file_exists: 存在重名文件时处理方式
-        :param data: post方式的data参数
-        :param json: post方式的json参数
         :param split: 是否允许分块下载
         :param kwargs: requests其它参数
+        :param offset: 文件存储偏移量
         """
-        self.url = url
+        self.url = quote(url, safe='/:&?=%;#@+![]')
         self.goal_path = goal_path
         self.rename = rename
         self.file_exists = file_exists
-        self.post_data = data
-        self.post_json = json
         self.split = split
         self.kwargs = kwargs
+        self.offset = offset
 
 
 class BaseTask(object):
-    """任务类基类"""
     _DONE = 'done'
+    RESULT_TEXTS = {'success': '成功', 'skipped': '跳过', 'canceled': '取消', False: '失败', None: '未知'}
 
     def __init__(self, ID):
-        """初始化                   \n
+        """任务类基类
         :param ID: 任务id
         """
         self._id = ID
-        self.state = 'waiting'  # 状态：'waiting'、'running'、'done'
-        self.result = None  # 结果：'success'、'skip'、'cancel'、False、None
+        self.state = 'waiting'  # 'waiting'、'running'、'done'
+        self.result = None  # 'success'、'skipped'、'canceled'、False、None
         self.info = '等待下载'  # 信息
 
     @property
     def id(self):
         """返回任务或子任务id"""
         return self._id
 
@@ -56,72 +55,72 @@
     def data(self):
         """返回任务数据"""
         return
 
     @property
     def is_done(self):
         """返回任务是否结束"""
-        return self.state == self._DONE
+        return self.state in ('done', 'cancel')
 
     def set_states(self, result=None, info=None, state='done'):
-        """设置任务结果值                                                  \n
-        :param result: 结果：'success'、'skip'、'cancel'、False、None
+        """设置任务结果值
+        :param result: 结果：'success'、'skipped'、'canceled'、False、None
         :param info: 任务信息
         :param state: 任务状态：'waiting'、'running'、'done'
         :return: None
         """
         self.result = result
         self.info = info
         self.state = state
 
 
 class Mission(BaseTask):
-    """任务类"""
-
-    def __init__(self, ID, data, download_kit):
-        """初始化                               \n
+    def __init__(self, ID, download_kit, file_url, goal_path, rename,
+                 file_exists, split, kwargs):
+        """任务类
         :param ID: 任务id
-        :param data: 任务数据
+        :param download_kit: 所属DownloadKit对象
+        :param file_url: 文件网址
+        :param goal_path: 保存文件夹路径
+        :param rename: 重命名
+        :param file_exists: 存在同名文件处理方式
+        :param split: 是否分块下载
+        :param kwargs: 连接参数
         """
         super().__init__(ID)
         self.download_kit = download_kit
-        self._data: MissionData = data
         self.size = None
 
-        self.tasks: List[Task] = []  # 多线程下载单个文件时的子任务
+        self.tasks = []
         self.tasks_count = 1
         self.done_tasks_count = 0
 
         self.file_name = None
-        self._path: Union[Path, None] = None  # 文件完整路径，Path对象
+        self._path = None  # 文件完整路径，Path对象
         self._recorder = None
 
+        self.session = self._set_session()
+        kwargs = self._handle_kwargs(file_url, kwargs)
+        self._data = MissionData(file_url, goal_path, rename, file_exists, split, kwargs)
+        self.method = 'post' if (self._data.kwargs.get('data', None) is not None or
+                                 self._data.kwargs.get('json', None) is not None) else 'get'
+
     def __repr__(self):
         return f'<Mission {self.id} {self.info} {self.file_name}>'
 
     @property
     def data(self):
         """返回任务数据"""
         return self._data
 
     @property
     def path(self):
         """返回文件保存路径"""
         return self._path
 
-    @path.setter
-    def path(self, path):
-        """设置文件保存路径"""
-        if isinstance(path, (Path, str)):
-            path = Path(path)
-            self.file_name = path.name
-
-        self._path = path
-        self.recorder.set_path(path)
-
     @property
     def recorder(self):
         """返回记录器对象"""
         if self._recorder is None:
             self._recorder = ByteRecorder(cache_size=100)
             self._recorder.show_msg = False
         return self._recorder
@@ -130,87 +129,28 @@
     def rate(self):
         """返回下载进度百分比"""
         if self.path and self.path.exists():
             return round((self.path.stat().st_size / self.size) * 100, 2) if self.size else None
         else:
             return
 
-    def set_done(self, result, info):
-        """设置一个任务为done状态                                          \n
-        :param result: 结果：'success'、'skip'、'cancel'、False、None
-        :param info: 任务信息
-        :return: None
-        """
-        if result == 'skip':
-            self.set_states(result=result, info=info, state=self._DONE)
-
-        elif result == 'cancel' or result is False:
-            self.recorder.clear()
-            self.set_states(result=result, info=info, state=self._DONE)
-
-        elif result == 'success':
-            self.recorder.record()
-            if self.size and self.path.stat().st_size < self.size:
-                self.del_file()
-                self.set_states(False, '下载失败', self._DONE)
-            else:
-                self.set_states('success', info, self._DONE)
-
-        self.download_kit._when_mission_done(self)
-
-    def a_task_done(self, is_success, info):
-        """当一个task完成时调用                 \n
-        :param is_success: 该task是否成功
-        :param info: 该task传入的信息
-        :return: None
-        """
-        if self.is_done:
-            return
-
-        if is_success is False:
-            self.break_mission(False, info)
-            return
-
-        self.done_tasks_count += 1
-        if self.done_tasks_count == self.tasks_count:
-            self.set_done('success', info)
-
-    def break_mission(self, result, info):
-        """中止该任务，停止未下载完的task                                  \n
-        :param result: 结果：'success'、'skip'、'cancel'、False、None
-        :param info: 任务信息
-        :return: None
-        """
-        if self.is_done:
-            return
-
-        for task in self.tasks:
-            if not task.is_done:
-                task.set_states(result=result, info=info, state='cancel')
-
-        while any((not i.is_done for i in self.tasks)):
-            sleep(.1)
-
-        self.set_done(result, info)
-        self.del_file()
-
     def cancel(self) -> None:
         """取消该任务，停止未下载完的task"""
-        self.break_mission('cancel', '已取消')
+        self._break_mission('canceled', '已取消')
 
     def del_file(self):
         """删除下载的文件"""
         if self.path and self.path.exists():
             try:
                 self.path.unlink()
             except Exception:
                 pass
 
     def wait(self, show=True, timeout=0):
-        """等待当前任务完成                  \n
+        """等待当前任务完成
         :param show: 是否显示下载进度
         :param timeout: 超时时间
         :return: 任务结果和信息组成的tuple
         """
         if show:
             print(f'url：{self.data.url}')
             t2 = perf_counter()
@@ -234,33 +174,130 @@
 
         if show:
             if self.result is False:
                 print(f'下载失败 {self.info}')
             elif self.result == 'success':
                 print('\r100% ', end='')
                 print(f'下载完成 {self.info}')
-            elif self.result == 'skip':
+            elif self.result == 'skipped':
                 print(f'已跳过 {self.info}')
             print()
 
         return self.result, self.info
 
+    def _set_session(self):
+        """复制Session对象，并设置coookies"""
+        session = copy_session(self.download_kit.session)
+        if self.download_kit.page:
+            set_session_cookies(session, self.download_kit.page.get_cookies())
+            session.headers.update({"User-Agent": self.download_kit.page.user_agent})
+        return session
+
+    def _handle_kwargs(self, url, kwargs):
+        """处理接收到的参数
+        :param url: 要访问的url
+        :param kwargs: 传入的参数dict
+        :return: 处理后的参数dict
+        """
+        if 'timeout' not in kwargs:
+            kwargs['timeout'] = self.download_kit.timeout
+
+        headers = CaseInsensitiveDict(kwargs['headers']) if 'headers' in kwargs else CaseInsensitiveDict()
+
+        parsed_url = urlparse(url)
+        hostname = parsed_url.hostname
+        scheme = parsed_url.scheme
+
+        if not ('Referer' in headers or 'Referer' in self.session.headers):
+            headers['Referer'] = self.download_kit.page.url if self.download_kit.page else f'{scheme}://{hostname}'
+        if not ('Host' in headers or 'Host' in self.session.headers):
+            headers['Host'] = hostname
+        kwargs['headers'] = headers
 
-class Task(BaseTask):
-    """子任务类"""
+        return kwargs
+
+    def _set_path(self, path):
+        """设置文件保存路径"""
+        if isinstance(path, (Path, str)):
+            path = Path(path)
+            self.file_name = path.name
+
+        self._path = path
+        self.recorder.set.path(path)
+
+    def _set_done(self, result, info):
+        """设置一个任务为done状态
+        :param result: 结果：'success'、'skipped'、'canceled'、False、None
+        :param info: 任务信息
+        :return: None
+        """
+        if result == 'skipped':
+            self.set_states(result=result, info=info, state=self._DONE)
+
+        elif result == 'canceled' or result is False:
+            self.recorder.clear()
+            self.set_states(result=result, info=info, state=self._DONE)
+
+        elif result == 'success':
+            self.recorder.record()
+            if self.size and self.path.stat().st_size < self.size:
+                self.del_file()
+                self.set_states(False, '下载失败', self._DONE)
+            else:
+                self.set_states('success', info, self._DONE)
+
+        self.download_kit._when_mission_done(self)
+
+    def _a_task_done(self, is_success, info):
+        """当一个task完成时调用
+        :param is_success: 该task是否成功
+        :param info: 该task传入的信息
+        :return: None
+        """
+        if self.is_done:
+            return
+
+        if is_success is False:
+            self._break_mission(False, info)
+            return
+
+        self.done_tasks_count += 1
+        if self.done_tasks_count == self.tasks_count:
+            self._set_done('success', info)
+
+    def _break_mission(self, result, info):
+        """中止该任务，停止未下载完的task
+        :param result: 结果：'success'、'skipped'、'canceled'、False、None
+        :param info: 任务信息
+        :return: None
+        """
+        if self.is_done:
+            return
+
+        for task in self.tasks:
+            if not task.is_done:
+                task.set_states(result=result, info=info, state='cancel')
+
+        while any((not i.is_done for i in self.tasks)):
+            sleep(.3)
 
+        self._set_done(result, info)
+        self.del_file()
+
+
+class Task(BaseTask):
     def __init__(self, mission, range_, ID):
-        """初始化                               \n
+        """子任务类
         :param mission: 父任务对象
         :param range_: 读取文件数据范围
         :param ID: 任务id
         """
         super().__init__(ID)
-        self.mission = mission  # 父任务
-        self.range = range_  # 分块范围
+        self.mission = mission
+        self.range = range_
 
     def __repr__(self):
         return f'<Task M{self.mid} T{self._id}  {self.info} {self.file_name}>'
 
     @property
     def mid(self):
         """返回父任务id"""
@@ -278,22 +315,26 @@
 
     @property
     def file_name(self):
         """返回文件名"""
         return self.mission.file_name
 
     def add_data(self, data, seek=None):
-        """把数据输入到记录器                           \n
+        """把数据输入到记录器
         :param data: 文件字节数据
         :param seek: 在文件中的位置，None表示最后
         :return: None
         """
         self.mission.recorder.add_data(data, seek)
 
-    def set_done(self, result, info):
-        """设置一个子任务为done状态                                          \n
-        :param result: 结果：'success'、'skip'、'cancel'、False、None
+    def clear_cache(self):
+        """清除以接收但未写入硬盘的缓存"""
+        self.mission.recorder.clear()
+
+    def _set_done(self, result, info):
+        """设置一个子任务为done状态
+        :param result: 结果：'success'、'skipped'、'canceled'、False、None
         :param info: 任务信息
         :return: None
         """
         self.set_states(result=result, info=info, state=self._DONE)
-        self.mission.a_task_done(result, info)
+        self.mission._a_task_done(result, info)
```

### Comparing `DownloadKit-0.5.3/DownloadKit/mission.pyi` & `DownloadKit-1.0.0/DownloadKit/mission.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 # -*- coding:utf-8 -*-
 from pathlib import Path
-from typing import Union, List
+from typing import Union, List, Optional
 
 from DataRecorder import ByteRecorder
+from requests import Session
 
 from .downloadKit import DownloadKit
 
 
 class MissionData(object):
     """保存任务数据的对象"""
 
-    def __init__(self, url: str,
-                 goal_path: Union[str, Path],
-                 rename: Union[str, None],
-                 file_exists: str,
-                 data: Union[str, dict, None],
-                 json: Union[str, dict, None],
-                 split: bool,
-                 kwargs: dict):
+    def __init__(self, url: str, goal_path: Union[str, Path], rename: Optional[str],
+                 file_exists: str, split: bool, kwargs: dict, offset: int = 0):
         self.url: str = ...
         self.goal_path: Union[str, Path] = ...
-        self.rename: Union[str, None] = ...
+        self.rename: Optional[str] = ...
         self.file_exists: str = ...
-        self.post_data: Union[str, dict, None] = ...
-        self.post_json: Union[str, dict, None] = ...
         self.split: bool = ...
         self.kwargs: dict = ...
+        self.offset: int = ...
 
 
 class BaseTask(object):
     """任务类基类"""
     _DONE: str = ...
+    RESULT_TEXTS: dict = ...
 
     def __init__(self, ID: Union[int, str]):
         self._id: str = ...
         self.state: str = ...
 
     @property
     def id(self) -> Union[int, str]: ...
@@ -42,73 +37,79 @@
     @property
     def data(self): ...
 
     @property
     def is_done(self) -> bool: ...
 
     def set_states(self,
-                   result: Union[bool, None, str] = None,
+                   result: Optional[bool, str] = None,
                    info: str = None,
                    state: str = 'done') -> None: ...
 
 
 class Mission(BaseTask):
     """任务类"""
 
-    def __init__(self, ID: int, data: MissionData, download_kit: DownloadKit):
+    def __init__(self, ID: int, download_kit: DownloadKit, file_url: str, goal_path: Union[str, Path], rename: str,
+                 file_exists: str, split: bool, kwargs: dict):
         self.info: str = ...
         self.file_name: str = ...
         self._data: MissionData = ...
         self._path: Union[str, Path] = ...
         self._recorder: ByteRecorder = ...
         self.size: float = ...
         self.done_tasks_count: int = ...
         self.tasks_count: int = ...
         self.tasks: List[Task] = ...
         self.download_kit: DownloadKit = ...
-        self.result: Union[str, None, bool] = ...
+        self.session: Session = ...
+        self.result: Optional[str, bool] = ...
+        self.method: str = ...
 
     def __repr__(self) -> str: ...
 
+    def _set_session(self) -> Session: ...
+
+    def _handle_kwargs(self, url: str, kwargs: dict) -> dict: ...
+
     @property
     def data(self) -> MissionData: ...
 
     @property
     def path(self) -> Union[str, Path]: ...
 
-    @path.setter
-    def path(self, path: Union[str, Path, None]) -> None: ...
+    def _set_path(self, path: Optional[str, Path]) -> None: ...
 
     @property
     def recorder(self) -> ByteRecorder: ...
 
     @property
-    def rate(self) -> Union[float, None]: ...
+    def rate(self) -> Optional[float]: ...
 
-    def set_done(self, result: Union[bool, None, str], info: str) -> None: ...
+    def _set_done(self, result: Optional[bool, str], info: str) -> None: ...
 
-    def a_task_done(self, is_success: bool, info: str) -> None: ...
+    def _a_task_done(self, is_success: bool, info: str) -> None: ...
 
-    def break_mission(self, result: Union[bool, None, str], info: str) -> None: ...
+    def _break_mission(self, result: Optional[bool, str], info: str) -> None: ...
 
     def cancel(self) -> None: ...
 
     def del_file(self): ...
 
     def wait(self, show: bool = True, timeout: float = 0) -> tuple: ...
 
 
 class Task(BaseTask):
     """子任务类"""
 
-    def __init__(self, mission: Mission, range_: Union[list, None], ID: str):
+    def __init__(self, mission: Mission, range_: Optional[list], ID: str):
         self._id: str = ...
         self.info: str = ...
         self.mission: Mission = ...
-        self.range: Union[list, None] = ...
+        self.range: Optional[list] = ...
 
     def __repr__(self) -> str: ...
 
     @property
     def mid(self) -> int: ...
 
     @property
@@ -118,8 +119,10 @@
     def path(self) -> str: ...
 
     @property
     def file_name(self) -> str: ...
 
     def add_data(self, data: bytes, seek: int = None) -> None: ...
 
-    def set_done(self, result: Union[bool, None, str], info: str) -> None: ...
+    def clear_cache(self) -> None: ...
+
+    def _set_done(self, result: Optional[bool, str], info: str) -> None: ...
```

### Comparing `DownloadKit-0.5.3/DownloadKit.egg-info/PKG-INFO` & `DownloadKit-1.0.0/DownloadKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DownloadKit
-Version: 0.5.3
+Version: 1.0.0
 Summary: 一个简洁易用的多线程文件下载工具。
 Home-page: https://gitee.com/g1879/DownloadKit
 Author: g1879
 Author-email: g1879@qq.com
 License: BSD
 Keywords: DownloadKit
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DownloadKit-0.5.3/LICENSE` & `DownloadKit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DownloadKit-0.5.3/PKG-INFO` & `DownloadKit-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DownloadKit
-Version: 0.5.3
+Version: 1.0.0
 Summary: 一个简洁易用的多线程文件下载工具。
 Home-page: https://gitee.com/g1879/DownloadKit
 Author: g1879
 Author-email: g1879@qq.com
 License: BSD
 Keywords: DownloadKit
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DownloadKit-0.5.3/README.md` & `DownloadKit-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `DownloadKit-0.5.3/setup.py` & `DownloadKit-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="DownloadKit",
-    version="0.5.3",
+    version="1.0.0",
     author="g1879",
     author_email="g1879@qq.com",
     description="一个简洁易用的多线程文件下载工具。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     keywords="DownloadKit",
     url="https://gitee.com/g1879/DownloadKit",
     include_package_data=True,
     packages=find_packages(),
     install_requires=[
         "requests",
-        "DataRecorder"
+        "DataRecorder>=3.4.2"
     ],
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Development Status :: 4 - Beta",
         "Topic :: Utilities",
         "License :: OSI Approved :: BSD License",
     ],
```

