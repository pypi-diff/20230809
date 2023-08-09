# Comparing `tmp/pyxxl-0.3.1.tar.gz` & `tmp/pyxxl-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxxl-0.3.1.tar", max compression
+gzip compressed data, was "pyxxl-0.3.2.tar", max compression
```

## Comparing `pyxxl-0.3.1.tar` & `pyxxl-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35149 2023-04-21 09:30:19.865097 pyxxl-0.3.1/LICENSE
--rw-r--r--   0        0        0     3989 2023-04-21 09:30:19.865097 pyxxl-0.3.1/README.md
--rw-r--r--   0        0        0     2083 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      178 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/__init__.py
--rw-r--r--   0        0        0     1041 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/ctx.py
--rw-r--r--   0        0        0      259 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/enum.py
--rw-r--r--   0        0        0      981 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/error.py
--rw-r--r--   0        0        0    12215 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/executor.py
--rw-r--r--   0        0        0       82 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/logger/__init__.py
--rw-r--r--   0        0        0     1420 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/logger/common.py
--rw-r--r--   0        0        0     5026 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/logger/disk.py
--rw-r--r--   0        0        0     4248 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/logger/redis.py
--rw-r--r--   0        0        0     5064 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/main.py
--rw-r--r--   0        0        0     2526 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/prometheus.py
--rw-r--r--   0        0        0      764 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/schema.py
--rw-r--r--   0        0        0     3835 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/server.py
--rw-r--r--   0        0        0     4758 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/setting.py
--rw-r--r--   0        0        0        0 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/api/__init__.py
--rw-r--r--   0        0        0      669 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/api/test_metrics.py
--rw-r--r--   0        0        0     2774 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/api/test_server.py
--rw-r--r--   0        0        0     2190 2023-04-21 09:30:19.865097 pyxxl-0.3.1/pyxxl/tests/conftest.py
--rw-r--r--   0        0        0     1640 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_client.py
--rw-r--r--   0        0        0      889 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_context.py
--rw-r--r--   0        0        0     6572 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_executor.py
--rw-r--r--   0        0        0     1391 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_handler.py
--rw-r--r--   0        0        0     3697 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_logger.py
--rw-r--r--   0        0        0      835 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_register.py
--rw-r--r--   0        0        0     1804 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_setting.py
--rw-r--r--   0        0        0      129 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/test_utils.py
--rw-r--r--   0        0        0      872 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/tests/utils.py
--rw-r--r--   0        0        0      395 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/types.py
--rw-r--r--   0        0        0     2016 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/utils.py
--rw-r--r--   0        0        0     3923 2023-04-21 09:30:19.869098 pyxxl-0.3.1/pyxxl/xxl_client.py
--rw-r--r--   0        0        0     5072 1970-01-01 00:00:00.000000 pyxxl-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-09 01:00:11.978603 pyxxl-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3957 2023-08-09 01:00:11.978603 pyxxl-0.3.2/README.md
+-rw-r--r--   0        0        0     2147 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      178 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/__init__.py
+-rw-r--r--   0        0        0     1041 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/ctx.py
+-rw-r--r--   0        0        0      259 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/enum.py
+-rw-r--r--   0        0        0      981 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/error.py
+-rw-r--r--   0        0        0    12132 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/executor.py
+-rw-r--r--   0        0        0       82 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/logger/__init__.py
+-rw-r--r--   0        0        0     1420 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/logger/common.py
+-rw-r--r--   0        0        0     5026 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/logger/disk.py
+-rw-r--r--   0        0        0     4248 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/logger/redis.py
+-rw-r--r--   0        0        0     5121 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/main.py
+-rw-r--r--   0        0        0     2526 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/prometheus.py
+-rw-r--r--   0        0        0      764 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/schema.py
+-rw-r--r--   0        0        0     3835 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/server.py
+-rw-r--r--   0        0        0     4758 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/setting.py
+-rw-r--r--   0        0        0        0 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/tests/api/__init__.py
+-rw-r--r--   0        0        0      669 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/tests/api/test_metrics.py
+-rw-r--r--   0        0        0     2774 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/tests/api/test_server.py
+-rw-r--r--   0        0        0     2174 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/tests/conftest.py
+-rw-r--r--   0        0        0     1640 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/tests/test_client.py
+-rw-r--r--   0        0        0      905 2023-08-09 01:00:11.978603 pyxxl-0.3.2/pyxxl/tests/test_context.py
+-rw-r--r--   0        0        0     6572 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/tests/test_executor.py
+-rw-r--r--   0        0        0     1391 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/tests/test_handler.py
+-rw-r--r--   0        0        0     3697 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/tests/test_logger.py
+-rw-r--r--   0        0        0      859 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/tests/test_register.py
+-rw-r--r--   0        0        0     1804 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/tests/test_setting.py
+-rw-r--r--   0        0        0      129 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/tests/test_utils.py
+-rw-r--r--   0        0        0      872 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/tests/utils.py
+-rw-r--r--   0        0        0      395 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/types.py
+-rw-r--r--   0        0        0     2119 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/utils.py
+-rw-r--r--   0        0        0     3923 2023-08-09 01:00:11.982603 pyxxl-0.3.2/pyxxl/xxl_client.py
+-rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 pyxxl-0.3.2/PKG-INFO
```

### Comparing `pyxxl-0.3.1/LICENSE` & `pyxxl-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/README.md` & `pyxxl-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,21 +54,21 @@
     xxl_admin_baseurl="http://localhost:8080/xxl-job-admin/api/",
     executor_app_name="xxl-job-executor-sample",
     executor_host="172.17.0.1",
 )
 
 app = PyxxlRunner(config)
 
-@app.handler.register(name="demoJobHandler")
+@app.register(name="demoJobHandler")
 async def test_task():
     await asyncio.sleep(5)
     return "成功..."
 
 # 如果你代码里面没有实现全异步，请使用同步函数，不然会阻塞其他任务
-@app.handler.register(name="xxxxx")
+@app.register(name="xxxxx")
 def test_task3():
     return "成功3"
 
 
 app.run_executor()
 ```
 
@@ -89,25 +89,25 @@
 同步任务会放到线程池中运行，无法正确接受cancel信号和timeout配置
 
 如果需要使用同步任务并且无法控制（预料）里面执行时间，又需要进行超时和cancel功能的，需要接受pyxxl发出的cancel_event，当该cancel_event被设置时需要中断任务，下面是一个案例:
 
 ```python
 ...
 
-@app.handler.register(name="sync_func")
+@app.register(name="sync_func")
 def sync_loop_demo():
     # 如果同步任务里面有循环，为了支持cancel操作，必须每次都判断g.cancel_event.
     task_params_list = []
     while not g.cancel_event.is_set() and task_parasm_list:
         params = task_params_list.pop()
         time.sleep(3)
     return "ok"
 
 # 如下代码会造成线程池里的线程被永远占用，timeout cancel全部不生效
-@app.handler.register(name="sync_func2")
+@app.register(name="sync_func2")
 def sync_loop_demo2():
     while True:
         time.sleep(3) # 模拟你运行的任务
     return "ok"
 
 ```
```

### Comparing `pyxxl-0.3.1/pyproject.toml` & `pyxxl-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 description = "A Python executor for XXL-jobs"
 keywords = ["XXL"]
 license = "GPL-3.0-only"
 name = "pyxxl"
 readme = "README.md"
 repository = "https://github.com/fcfangcc/pyxxl"
-version = "0.3.1"
+version = "0.3.2"
 
 [tool.poetry.dependencies]
 aiofiles = "^22.1.0"
 aiohttp = "^3.8.1"
 prometheus-client = {version = "*", optional = true}
 python = "^3.9"
 python-dotenv = {version = "*", optional = true}
@@ -45,16 +45,21 @@
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 # if your need
 # https://python-poetry.org/docs/repositories/#install-dependencies-from-a-private-repository
 [[tool.poetry.source]]
 name = "aliyun"
-secondary = true
 url = "https://mirrors.aliyun.com/pypi/simple/"
+priority = "primary"
+
+
+[[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = [
   '^pyxxl/tests/test_.*\.py$',
   '^pyxxl/tests/api/test_.*\.py$',
 ]
```

### Comparing `pyxxl-0.3.1/pyxxl/ctx.py` & `pyxxl-0.3.2/pyxxl/ctx.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/error.py` & `pyxxl-0.3.2/pyxxl/error.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/executor.py` & `pyxxl-0.3.2/pyxxl/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,13 +279,9 @@
                 await asyncio.sleep(0.05)
 
         await asyncio.wait_for(_graceful_close(), timeout=timeout)
 
     def reset_handler(self, handler: Optional[JobHandler] = None) -> None:
         self.handler = handler or JobHandler()
 
-    @property
-    def register(self) -> Any:
-        return self.handler.register
-
     def get_queue(self, job_id: int) -> asyncio.Queue[RunData]:
         return self.queue[job_id]
```

### Comparing `pyxxl-0.3.1/pyxxl/logger/common.py` & `pyxxl-0.3.2/pyxxl/logger/common.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/logger/disk.py` & `pyxxl-0.3.2/pyxxl/logger/disk.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/logger/redis.py` & `pyxxl-0.3.2/pyxxl/logger/redis.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/main.py` & `pyxxl-0.3.2/pyxxl/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import functools
 import logging
 from multiprocessing import Process
-from typing import AsyncGenerator, Optional
+from typing import Any, AsyncGenerator, Optional
 
 from aiohttp import web
 
 from pyxxl.executor import Executor, JobHandler
 from pyxxl.logger import DiskLog, LogBase, RedisLog
 from pyxxl.server import create_app
 from pyxxl.setting import ExecutorConfig
@@ -44,15 +44,15 @@
                     executor_host="172.17.0.1"
                     )
                 ,
                 handler=xxl_handler,
             )
             ```
         Args:
-            config (ExecutorConfig): 配置参数 [ExecutorConfig](/apis/config)
+            config (ExecutorConfig): 配置参数
             handler (JobHandler, optional): 执行器支持的job,没有预先定义的job名称也会执行失败
         """
 
         self.handler = handler or JobHandler()
         self.config = config
         log_level = logging.DEBUG if self.config.debug else logging.INFO
         setup_logging(self.config.executor_log_path, level=log_level)
@@ -133,10 +133,14 @@
     def run_with_daemon(self) -> None:
         """新开一个进程以后台方式运行,一般和gunicorn一起使用"""
 
         daemon = Process(target=self._runner, name="pyxxljob", daemon=True)
         daemon.start()
         self.daemon = daemon
 
+    @property
+    def register(self) -> Any:
+        return self.handler.register
+
     # def exit_daemon(self):
     #     logger.info("Exit daemon name=%s", self.daemon.name )
     #     self.daemon.terminate()
```

### Comparing `pyxxl-0.3.1/pyxxl/prometheus.py` & `pyxxl-0.3.2/pyxxl/prometheus.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/schema.py` & `pyxxl-0.3.2/pyxxl/schema.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/server.py` & `pyxxl-0.3.2/pyxxl/server.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/setting.py` & `pyxxl-0.3.2/pyxxl/setting.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/tests/api/test_metrics.py` & `pyxxl-0.3.2/pyxxl/tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/tests/api/test_server.py` & `pyxxl-0.3.2/pyxxl/tests/api/test_server.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/tests/conftest.py` & `pyxxl-0.3.2/pyxxl/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,19 +55,19 @@
     return Executor(MokeXXL("http://localhost:8080/xxl-job-admin/api/"), request.param, handler=None)
 
 
 @pytest.fixture(scope="session")
 def web_app(executor: Executor) -> Application:
     runner = MokePyxxlRunner(executor.config)
 
-    @runner.handler.register(name="demoJobHandler")
+    @runner.register(name="demoJobHandler")
     async def test_task() -> None:
         await asyncio.sleep(10)
 
-    @runner.handler.register(name="demoJobHandlerSync")
+    @runner.register(name="demoJobHandlerSync")
     def test_task_sync() -> None:
         time.sleep(5)
 
     return runner.create_server_app()
 
 
 @pytest_asyncio.fixture
```

### Comparing `pyxxl-0.3.1/pyxxl/tests/test_client.py` & `pyxxl-0.3.2/pyxxl/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/tests/test_context.py` & `pyxxl-0.3.2/pyxxl/tests/test_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from pyxxl.enum import executorBlockStrategy
 from pyxxl.executor import Executor
 from pyxxl.schema import RunData
 
 
 @pytest.mark.asyncio
 async def test_runner_callback(executor: Executor):
-    @executor.register
+    @executor.handler.register
     async def test_ctx():
         logId = g.xxl_run_data.logId
         assert logId == 1
 
-    @executor.register
+    @executor.handler.register
     def test_ctx_sync():
         logId = g.xxl_run_data.logId
         assert logId == 1
 
     for handler in ["test_ctx", "test_ctx_sync"]:
         data = RunData(
             **dict(
```

### Comparing `pyxxl-0.3.1/pyxxl/tests/test_executor.py` & `pyxxl-0.3.2/pyxxl/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/tests/test_handler.py` & `pyxxl-0.3.2/pyxxl/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/tests/test_logger.py` & `pyxxl-0.3.2/pyxxl/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/tests/test_register.py` & `pyxxl-0.3.2/pyxxl/tests/test_register.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 
 # pylint: disable=function-redefined
 @pytest.mark.asyncio
 async def test_hander(executor: Executor):
     executor.reset_handler()
 
-    @executor.register
+    @executor.handler.register
     def test_hander1():
         ...
 
-    @executor.register(replace=True)
+    @executor.handler.register(replace=True)
     async def test_hander1():  # noqa: F811
         ...
 
-    @executor.register(name="test_hander1_dup")
+    @executor.handler.register(name="test_hander1_dup")
     def test_hander1():  # noqa: F811
         ...
```

### Comparing `pyxxl-0.3.1/pyxxl/tests/test_setting.py` & `pyxxl-0.3.2/pyxxl/tests/test_setting.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/tests/utils.py` & `pyxxl-0.3.2/pyxxl/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/pyxxl/utils.py` & `pyxxl-0.3.2/pyxxl/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import importlib
 import logging
+import platform
 import socket
 from logging.handlers import RotatingFileHandler
 from typing import Any, List, Optional
 
 from pyxxl.ctx import g
 
 DEFAULT_FORMAT = (
@@ -14,15 +15,18 @@
 STD_FORMATTER = logging.Formatter(DEFAULT_FORMAT, datefmt=DATE_FORMAT)
 DEFAULT_FILE_SIZE = 50 * 1024 * 1024
 DEFAULT_BACKUP_FILE_COUNT = 5
 
 
 def get_network_ip() -> str:
     """获取本机地址,会获取首个网络地址"""
-    _, _, ipaddrlist = socket.gethostbyname_ex(socket.gethostname())
+    if platform.system() == "Darwin":
+        return "127.0.0.1"  # todo
+    else:
+        _, _, ipaddrlist = socket.gethostbyname_ex(socket.gethostname())
     return ipaddrlist[0]
 
 
 def _init_log_record_factory() -> None:
     old_factory = logging.getLogRecordFactory()
 
     def _record_factory(*args: Any, **kwargs: Any) -> logging.LogRecord:
```

### Comparing `pyxxl-0.3.1/pyxxl/xxl_client.py` & `pyxxl-0.3.2/pyxxl/xxl_client.py`

 * *Files identical despite different names*

### Comparing `pyxxl-0.3.1/PKG-INFO` & `pyxxl-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxxl
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python executor for XXL-jobs
 Home-page: https://github.com/fcfangcc/pyxxl
 License: GPL-3.0-only
 Keywords: XXL
 Author: fcfangcc
 Author-email: swjfc22@live.com
 Requires-Python: >=3.9,<4.0
@@ -82,21 +82,21 @@
     xxl_admin_baseurl="http://localhost:8080/xxl-job-admin/api/",
     executor_app_name="xxl-job-executor-sample",
     executor_host="172.17.0.1",
 )
 
 app = PyxxlRunner(config)
 
-@app.handler.register(name="demoJobHandler")
+@app.register(name="demoJobHandler")
 async def test_task():
     await asyncio.sleep(5)
     return "成功..."
 
 # 如果你代码里面没有实现全异步，请使用同步函数，不然会阻塞其他任务
-@app.handler.register(name="xxxxx")
+@app.register(name="xxxxx")
 def test_task3():
     return "成功3"
 
 
 app.run_executor()
 ```
 
@@ -117,25 +117,25 @@
 同步任务会放到线程池中运行，无法正确接受cancel信号和timeout配置
 
 如果需要使用同步任务并且无法控制（预料）里面执行时间，又需要进行超时和cancel功能的，需要接受pyxxl发出的cancel_event，当该cancel_event被设置时需要中断任务，下面是一个案例:
 
 ```python
 ...
 
-@app.handler.register(name="sync_func")
+@app.register(name="sync_func")
 def sync_loop_demo():
     # 如果同步任务里面有循环，为了支持cancel操作，必须每次都判断g.cancel_event.
     task_params_list = []
     while not g.cancel_event.is_set() and task_parasm_list:
         params = task_params_list.pop()
         time.sleep(3)
     return "ok"
 
 # 如下代码会造成线程池里的线程被永远占用，timeout cancel全部不生效
-@app.handler.register(name="sync_func2")
+@app.register(name="sync_func2")
 def sync_loop_demo2():
     while True:
         time.sleep(3) # 模拟你运行的任务
     return "ok"
 
 ```
```

