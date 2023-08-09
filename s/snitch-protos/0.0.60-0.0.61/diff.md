# Comparing `tmp/snitch-protos-0.0.60.tar.gz` & `tmp/snitch-protos-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.60.tar", last modified: Tue Aug  8 23:48:55 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.61.tar", last modified: Wed Aug  9 00:26:48 2023, max compression
```

## Comparing `snitch-protos-0.0.60.tar` & `snitch-protos-0.0.61.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:55.400436 snitch-protos-0.0.60/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 23:48:55.400436 snitch-protos-0.0.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 23:48:31.000000 snitch-protos-0.0.60/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:48:55.400436 snitch-protos-0.0.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-08 23:48:55.000000 snitch-protos-0.0.60/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:55.396436 snitch-protos-0.0.60/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:31.000000 snitch-protos-0.0.60/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:55.400436 snitch-protos-0.0.60/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    35747 2023-08-08 23:48:31.000000 snitch-protos-0.0.60/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:55.400436 snitch-protos-0.0.60/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-08 23:48:31.000000 snitch-protos-0.0.60/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:55.396436 snitch-protos-0.0.60/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 23:48:55.000000 snitch-protos-0.0.60/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 23:48:55.000000 snitch-protos-0.0.60/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:48:55.000000 snitch-protos-0.0.60/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 23:48:55.000000 snitch-protos-0.0.60/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:26:48.372481 snitch-protos-0.0.61/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-09 00:26:48.372481 snitch-protos-0.0.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-09 00:26:01.000000 snitch-protos-0.0.61/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 00:26:48.376481 snitch-protos-0.0.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-09 00:26:47.000000 snitch-protos-0.0.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:26:48.372481 snitch-protos-0.0.61/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 00:26:01.000000 snitch-protos-0.0.61/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:26:48.372481 snitch-protos-0.0.61/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36063 2023-08-09 00:26:01.000000 snitch-protos-0.0.61/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:26:48.372481 snitch-protos-0.0.61/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-09 00:26:01.000000 snitch-protos-0.0.61/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:26:48.372481 snitch-protos-0.0.61/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-09 00:26:48.000000 snitch-protos-0.0.61/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-09 00:26:48.000000 snitch-protos-0.0.61/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:26:48.000000 snitch-protos-0.0.61/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-09 00:26:48.000000 snitch-protos-0.0.61/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.60/PKG-INFO` & `snitch-protos-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.60
+Version: 0.0.61
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.60/setup.py` & `snitch-protos-0.0.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.60',
+    version='0.0.61',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.60/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.61/snitch_protos/protos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,18 @@
     """
     Pipeline is a structure that holds one or more pipeline steps. This
     structure is intended to be immutable; clients are expected to generate
     WASMRequest's that contain a pipeline step.
     """
 
     id: str = betterproto.string_field(1)
-    """Set by snitch-server on Create; must be present on Update calls"""
+    """
+    ID should NOT be set by external gRPC client on CreatePipelineRequest - it
+    will be ignored; it _does_ need to be set on UpdatePipelineRequest.
+    """
 
     name: str = betterproto.string_field(2)
     """Friendly name for the pipeline"""
 
     steps: List["PipelineStep"] = betterproto.message_field(3)
     """One or more steps to execute"""
 
@@ -253,14 +256,20 @@
 
 @dataclass(eq=False, repr=False)
 class CreatePipelineRequest(betterproto.Message):
     pipeline: "Pipeline" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
+class CreatePipelineResponse(betterproto.Message):
+    message: str = betterproto.string_field(1)
+    pipeline_id: str = betterproto.string_field(2)
+
+
+@dataclass(eq=False, repr=False)
 class UpdatePipelineRequest(betterproto.Message):
     pipeline: "Pipeline" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class DeletePipelineRequest(betterproto.Message):
     pipeline_id: str = betterproto.string_field(1)
@@ -547,19 +556,19 @@
     async def create_pipeline(
         self,
         create_pipeline_request: "CreatePipelineRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "StandardResponse":
+    ) -> "CreatePipelineResponse":
         return await self._unary_unary(
             "/protos.External/CreatePipeline",
             create_pipeline_request,
-            StandardResponse,
+            CreatePipelineResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
     async def update_pipeline(
         self,
@@ -781,15 +790,15 @@
     async def get_pipeline(
         self, get_pipeline_request: "GetPipelineRequest"
     ) -> "GetPipelineResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def create_pipeline(
         self, create_pipeline_request: "CreatePipelineRequest"
-    ) -> "StandardResponse":
+    ) -> "CreatePipelineResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def update_pipeline(
         self, update_pipeline_request: "UpdatePipelineRequest"
     ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
@@ -839,15 +848,16 @@
         self, stream: "grpclib.server.Stream[GetPipelineRequest, GetPipelineResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.get_pipeline(request)
         await stream.send_message(response)
 
     async def __rpc_create_pipeline(
-        self, stream: "grpclib.server.Stream[CreatePipelineRequest, StandardResponse]"
+        self,
+        stream: "grpclib.server.Stream[CreatePipelineRequest, CreatePipelineResponse]",
     ) -> None:
         request = await stream.recv_message()
         response = await self.create_pipeline(request)
         await stream.send_message(response)
 
     async def __rpc_update_pipeline(
         self, stream: "grpclib.server.Stream[UpdatePipelineRequest, StandardResponse]"
@@ -918,15 +928,15 @@
                 GetPipelineRequest,
                 GetPipelineResponse,
             ),
             "/protos.External/CreatePipeline": grpclib.const.Handler(
                 self.__rpc_create_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 CreatePipelineRequest,
-                StandardResponse,
+                CreatePipelineResponse,
             ),
             "/protos.External/UpdatePipeline": grpclib.const.Handler(
                 self.__rpc_update_pipeline,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 UpdatePipelineRequest,
                 StandardResponse,
             ),
```

### Comparing `snitch-protos-0.0.60/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.61/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.60/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.61/snitch_protos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.60
+Version: 0.0.61
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

