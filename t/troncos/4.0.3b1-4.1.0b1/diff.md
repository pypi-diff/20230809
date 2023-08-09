# Comparing `tmp/troncos-4.0.3b1.tar.gz` & `tmp/troncos-4.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.3b1.tar", max compression
+gzip compressed data, was "troncos-4.1.0b1.tar", max compression
```

## Comparing `troncos-4.0.3b1.tar` & `troncos-4.1.0b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1077 2023-07-21 12:51:31.625196 troncos-4.0.3b1/LICENSE
--rw-r--r--   0        0        0     8203 2023-07-21 12:51:31.625196 troncos-4.0.3b1/README.md
--rw-r--r--   0        0        0     2520 2023-07-21 12:51:31.625196 troncos-4.0.3b1/pyproject.toml
--rw-r--r--   0        0        0      291 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5297 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      969 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2361 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      259 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/logging/__init__.py
--rw-r--r--   0        0        0     3455 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/logging/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-07-21 12:51:31.625196 troncos-4.0.3b1/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     5176 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      906 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0       82 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/profiler.py
--rw-r--r--   0        0        0     1155 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/profiling/pyroscope.py
--rw-r--r--   0        0        0        0 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4582 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/_span.py
--rw-r--r--   0        0        0     2675 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     7585 2023-07-21 12:51:31.629196 troncos-4.0.3b1/troncos/tracing/decorators.py
--rw-r--r--   0        0        0     9331 1970-01-01 00:00:00.000000 troncos-4.0.3b1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-09 05:05:31.133617 troncos-4.1.0b1/LICENSE
+-rw-r--r--   0        0        0     8203 2023-08-09 05:05:31.133617 troncos-4.1.0b1/README.md
+-rw-r--r--   0        0        0     2554 2023-08-09 05:05:31.133617 troncos-4.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-08-09 05:05:31.133617 troncos-4.1.0b1/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.133617 troncos-4.1.0b1/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.133617 troncos-4.1.0b1/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.133617 troncos-4.1.0b1/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5297 2023-08-09 05:05:31.133617 troncos-4.1.0b1/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      969 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2361 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      259 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/logging/__init__.py
+-rw-r--r--   0        0        0     3455 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/logging/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     5176 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      906 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0       82 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1843 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0     1155 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/profiling/pyroscope.py
+-rw-r--r--   0        0        0        0 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4644 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     2659 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     7702 2023-08-09 05:05:31.137617 troncos-4.1.0b1/troncos/tracing/decorators.py
+-rw-r--r--   0        0        0     9331 1970-01-01 00:00:00.000000 troncos-4.1.0b1/PKG-INFO
```

### Comparing `troncos-4.0.3b1/LICENSE` & `troncos-4.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/README.md` & `troncos-4.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/pyproject.toml` & `troncos-4.1.0b1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.3b1"
+version = "4.1.0b1"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
@@ -12,45 +12,45 @@
 homepage = "https://github.com/kolonialno/troncos"
 repository = "https://github.com/kolonialno/troncos"
 documentation = "https://github.com/kolonialno/troncos"
 keywords = ["logs", "traces", "opentelemetry"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-ddtrace = "1.15.0"
-opentelemetry-sdk = "1.18.0"
-opentelemetry-exporter-otlp-proto-http = "1.18.0"
-opentelemetry-exporter-otlp-proto-grpc = {version = "1.18.0", optional = true}
+ddtrace = "1.17.3"
+opentelemetry-sdk = "1.19.0"
+opentelemetry-exporter-otlp-proto-http = "1.19.0"
+opentelemetry-exporter-otlp-proto-grpc = {version = "1.19.0", optional = true}
 structlog-sentry = {version = "^2.0.3", optional = true}
 python-ipware = "^0.9.0"
-pyroscope-io = "^0.8.3"
+pyroscope-io = "^0.8.5"
 
 [tool.poetry.extras]
 grpc = ["opentelemetry-exporter-otlp-proto-grpc"]
 sentry = ["structlog-sentry"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
-black = "^23.1.0"
-flake8 = "^6.0.0"
-mypy = "^1.0.1"
-pytest = "^7.2.1"
+black = "^23.7.0"
+flake8 = "^6.1.0"
+mypy = "^1.4.1"
+pytest = "^7.4.0"
 pytest_codeblocks = "^0.16.1"
-fastapi = ">=0.92,<0.96"
-requests = "^2.28.2"
-pytest-cov = "^4.0.0"
+fastapi = ">=0.100.1,<0.101"
+requests = "^2.31.0"
+pytest-cov = "^4.1.0"
 types-requests = "^2.28.11.14"
-pytest-asyncio = ">=0.20.3,<0.22.0"
-django-environ = "^0.9.0"
+pytest-asyncio = ">=0.21.1,<0.22.0"
+django-environ = "^0.10.0"
 pytest-benchmark = "^4.0.0"
 snakeviz = "^2.2.0"
-django = "^4.2.1"
-starlette = "^0.27.0"
+django = "^4.2.4"
+starlette = ">=0.27.0,<0.28.0" # FastAPI constrain
 structlog = "^23.1.0"
-celery = "^5.2.7"
+celery = "^5.3.1"
 ipython = "^8.14.0"
 
 
 [tool.black]
 target-version = ['py311']
 line-length = 88
 include = '\.pyi?$'
```

### Comparing `troncos-4.0.3b1/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.1.0b1/troncos/contrib/asgi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/contrib/asgi/profiling/app.py` & `troncos-4.1.0b1/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/contrib/celery/logging/signals.py` & `troncos-4.1.0b1/troncos/contrib/celery/logging/signals.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/contrib/django/logging/middleware.py` & `troncos-4.1.0b1/troncos/contrib/django/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/contrib/logging/tools/__init__.py` & `troncos-4.1.0b1/troncos/contrib/logging/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/contrib/structlog/__init__.py` & `troncos-4.1.0b1/troncos/contrib/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/contrib/structlog/processors.py` & `troncos-4.1.0b1/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/profiling/profiler.py` & `troncos-4.1.0b1/troncos/profiling/profiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
 from ddtrace.profiling import exporter
-from ddtrace.profiling.exporter import pprof
+from ddtrace.profiling.exporter import pprof  # type: ignore[attr-defined]
 from ddtrace.profiling.profiler import (
     Profiler as DDProfiler,
     _ProfilerInstance as DDProfilerInstance,
 )
 
 
 class _PprofExporter(pprof.PprofExporter):  # type: ignore[misc]
@@ -32,23 +32,23 @@
         pprof_profile, _ = super(_PprofExporter, self).export(
             events, start_time_ns, end_time_ns
         )
 
         self.pprof = pprof_profile.SerializeToString()
 
 
-class _ProfilerInstance(DDProfilerInstance):  # type: ignore
+class _ProfilerInstance(DDProfilerInstance):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self.exporter = _PprofExporter()
 
         super().__init__(*args, **kwargs)
 
     def _build_default_exporters(self) -> list[exporter.Exporter]:
         return [self.exporter]
 
 
-class Profiler(DDProfiler):  # type: ignore
+class Profiler(DDProfiler):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self._profiler = _ProfilerInstance(*args, **kwargs)
 
     def get_profile(self) -> str:
-        return self._profiler.exporter.pprof
+        return self._profiler.exporter.pprof  # type: ignore[no-any-return]
```

### Comparing `troncos-4.0.3b1/troncos/profiling/pyroscope.py` & `troncos-4.1.0b1/troncos/profiling/pyroscope.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/tracing/__init__.py` & `troncos-4.1.0b1/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/tracing/_otel.py` & `troncos-4.1.0b1/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.3b1/troncos/tracing/_span.py` & `troncos-4.1.0b1/troncos/tracing/_span.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,26 +66,28 @@
 }
 
 
 def _span_status_and_attributes(
     dd_span: DDSpan, ignore_attrs: set[str]
 ) -> tuple[Status, list[Event], dict[str, Any]]:
     # Collect all "attributes" from the dd span
-    dd_span_attr: dict[str, Any] = {
+    dd_span_attr: dict[str | bytes, Any] = {
         **dd_span._meta,
         **dd_span._metrics,
         "resource": dd_span.resource,
     }
 
     otel_attrs = {}
     events: list[Event] = []
     otel_error_attrs = {}
 
     # Map set OTEL attributes based on DD attributes
     for k, v in dd_span_attr.items():
+        if isinstance(k, bytes):
+            continue
         if k.startswith("_dd"):
             continue
         otel_err_attr = _dd_span_err_attr_mapping.get(k)
         if otel_err_attr:
             otel_error_attrs[otel_err_attr] = v
         elif k not in ignore_attrs:
             otel_attrs[k] = v
```

### Comparing `troncos-4.0.3b1/troncos/tracing/_writer.py` & `troncos-4.1.0b1/troncos/tracing/_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from opentelemetry.sdk.resources import Resource
 
 from ._enums import Exporter
 from ._otel import get_otel_span_processors
 from ._span import default_ignore_attrs, translate_span
 
 
-class OTELWriter(TraceWriter):  # type: ignore
+class OTELWriter(TraceWriter):
     def __init__(
         self,
         service_name: str,
         service_attributes: dict[str, Any] | None,
         endpoint: str,
         exporter: Exporter,
     ) -> None:
```

### Comparing `troncos-4.0.3b1/troncos/tracing/decorators.py` & `troncos-4.1.0b1/troncos/tracing/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,18 @@
     """
 
     def _class_decorator(cls: Type[TClass]) -> Type[TClass]:
         for key, value in cls.__dict__.items():
             if key.startswith("_"):
                 continue
             if not (
-                isinstance(value, FunctionType) or asyncio.iscoroutinefunction(value)
+                isinstance(value, FunctionType)
+                or isinstance(value, classmethod)
+                or isinstance(value, staticmethod)
+                or asyncio.iscoroutinefunction(value)
             ):
                 continue
 
             logging.getLogger(__name__).debug(f"Tracing function {cls.__name__}.{key}")
             setattr(
                 cls,
                 key,
```

### Comparing `troncos-4.0.3b1/PKG-INFO` & `troncos-4.1.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.3b1
+Version: 4.1.0b1
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc
 Provides-Extra: sentry
-Requires-Dist: ddtrace (==1.15.0)
-Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra == "grpc"
-Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0)
-Requires-Dist: opentelemetry-sdk (==1.18.0)
-Requires-Dist: pyroscope-io (>=0.8.3,<0.9.0)
+Requires-Dist: ddtrace (==1.17.3)
+Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.19.0) ; extra == "grpc"
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.19.0)
+Requires-Dist: opentelemetry-sdk (==1.19.0)
+Requires-Dist: pyroscope-io (>=0.8.5,<0.9.0)
 Requires-Dist: python-ipware (>=0.9.0,<0.10.0)
 Requires-Dist: structlog-sentry (>=2.0.3,<3.0.0) ; extra == "sentry"
 Project-URL: Documentation, https://github.com/kolonialno/troncos
 Project-URL: Repository, https://github.com/kolonialno/troncos
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="border-bottom: 0">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.3b1 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.1.0b1 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: grpc Provides-Extra: sentry Requires-Dist: ddtrace (==1.15.0)
-Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra ==
-"grpc" Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0)
-Requires-Dist: opentelemetry-sdk (==1.18.0) Requires-Dist: pyroscope-io
-(>=0.8.3,<0.9.0) Requires-Dist: python-ipware (>=0.9.0,<0.10.0) Requires-Dist:
+Provides-Extra: grpc Provides-Extra: sentry Requires-Dist: ddtrace (==1.17.3)
+Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.19.0) ; extra ==
+"grpc" Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.19.0)
+Requires-Dist: opentelemetry-sdk (==1.19.0) Requires-Dist: pyroscope-io
+(>=0.8.5,<0.9.0) Requires-Dist: python-ipware (>=0.9.0,<0.10.0) Requires-Dist:
 structlog-sentry (>=2.0.3,<3.0.0) ; extra == "sentry" Project-URL:
 Documentation, https://github.com/kolonialno/troncos Project-URL: Repository,
 https://github.com/kolonialno/troncos Description-Content-Type: text/markdown
                                   ****** ðªµ
                                    Troncos
                                      ******
           Collection of Python logging, tracing and profiling tools
```

