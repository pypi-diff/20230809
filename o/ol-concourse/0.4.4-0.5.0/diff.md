# Comparing `tmp/ol-concourse-0.4.4.tar.gz` & `tmp/ol-concourse-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ol-concourse-0.4.4.tar", last modified: Thu Jul 13 19:54:01 2023, max compression
+gzip compressed data, was "ol-concourse-0.5.0.tar", last modified: Tue Aug  8 22:53:12 2023, max compression
```

## Comparing `ol-concourse-0.4.4.tar` & `ol-concourse-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.723010 ol-concourse-0.4.4/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/MANIFEST.in
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       79 2023-07-13 19:54:01.723010 ol-concourse-0.4.4/PKG-INFO
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      762 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/backend_shim.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.716344 ol-concourse-0.4.4/ol_concourse/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/__init__.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.719677 ol-concourse-0.4.4/ol_concourse/lib/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/__init__.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       34 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/constants.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1038 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/containers.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.719677 ol-concourse-0.4.4/ol_concourse/lib/jobs/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)    11721 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/jobs/infrastructure.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.719677 ol-concourse-0.4.4/ol_concourse/lib/models/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/models/__init__.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3678 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/models/fragment.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)   107808 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/models/pipeline.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      303 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/models/resource.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1191 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/notifications.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2088 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/resource_types.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     4073 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/resources.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3199 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse/lib/tasks.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-13 19:54:01.719677 ol-concourse-0.4.4/ol_concourse.egg-info/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       79 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse.egg-info/PKG-INFO
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      684 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse.egg-info/SOURCES.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse.egg-info/dependency_links.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse.egg-info/namespace_packages.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       19 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse.egg-info/requires.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       13 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/ol_concourse.egg-info/top_level.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-07-13 19:54:01.723010 ol-concourse-0.4.4/setup.cfg
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      491 2023-07-13 19:54:01.000000 ol-concourse-0.4.4/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.839303 ol-concourse-0.5.0/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       79 2023-08-08 22:53:12.839303 ol-concourse-0.5.0/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      762 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/backend_shim.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.835970 ol-concourse-0.5.0/ol_concourse/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.839303 ol-concourse-0.5.0/ol_concourse/lib/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       34 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/constants.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1091 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/containers.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.839303 ol-concourse-0.5.0/ol_concourse/lib/jobs/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    11689 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/jobs/infrastructure.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.839303 ol-concourse-0.5.0/ol_concourse/lib/models/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/models/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)   428503 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/models/concourse_pipeline_models.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3688 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/models/fragment.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)   108829 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/models/pipeline.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      327 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/models/resource.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1191 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/notifications.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2088 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/resource_types.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     4321 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/resources.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3199 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse/lib/tasks.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-08-08 22:53:12.835970 ol-concourse-0.5.0/ol_concourse.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       79 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      737 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       19 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       13 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/ol_concourse.egg-info/top_level.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-08-08 22:53:12.839303 ol-concourse-0.5.0/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      491 2023-08-08 22:53:12.000000 ol-concourse-0.5.0/setup.py
```

### Comparing `ol-concourse-0.4.4/backend_shim.py` & `ol-concourse-0.5.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.4/ol_concourse/lib/containers.py` & `ol-concourse-0.5.0/ol_concourse/lib/containers.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ol_concourse.lib.jobs.infrastructure import Output
 from ol_concourse.lib.models.pipeline import (
     Command,
     Identifier,
     Input,
     TaskConfig,
     TaskStep,
+    Cache,
 )
 
 
 def container_build_task(
     inputs: list[Input],
     build_parameters: Optional[dict[str, str]],
     build_args: Optional[list[str]] = None,
@@ -21,14 +22,15 @@
         config=TaskConfig(
             platform="linux",
             image_resource={
                 "type": "registry-image",
                 "source": {"repository": "concourse/oci-build-task"},
             },
             params=build_parameters,
+            caches=[Cache(path="cache")],
             run=Command(
                 path="build",
                 args=build_args or [],
             ),
             inputs=inputs,
             # This output needs to be named exactly "image" or it won't actually export
             # the built image.
```

### Comparing `ol-concourse-0.4.4/ol_concourse/lib/jobs/infrastructure.py` & `ol-concourse-0.5.0/ol_concourse/lib/jobs/infrastructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#  noqa: WPS232
 from collections.abc import Iterable
 from copy import deepcopy
 from pathlib import Path
 from typing import Optional
 
 from ol_concourse.lib.constants import REGISTRY_IMAGE
 from ol_concourse.lib.models.fragment import PipelineFragment
@@ -169,15 +168,15 @@
         passed_param = None
         if index != 0:
             previous_job = chain_fragment.jobs[-1]
             passed_param = [previous_job.name]
         for dependency in dependencies or []:
             # These mutations apply globally if the dependencies aren't copied below
             dependency.trigger = not bool(previous_job or production_stack)
-            dependency.passed = passed_param or dependency.passed  # type: ignore
+            dependency.passed = passed_param or dependency.passed
 
         # Need to copy the dependencies because otherwise they are globally mutated
         local_dependencies = [
             dependency_step.copy() for dependency_step in (dependencies or [])
         ]
         if custom_dependency := (custom_dependencies or {}).get(index):
             local_custom_dependencies = [
```

### Comparing `ol-concourse-0.4.4/ol_concourse/lib/models/fragment.py` & `ol-concourse-0.5.0/ol_concourse/lib/models/fragment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from pydantic import BaseModel, Field, validator
+from pydantic import field_validator, BaseModel, Field
 
 from ol_concourse.lib.models.pipeline import Job, Resource, ResourceType
 
 
 class PipelineFragment(BaseModel):
     resource_types: list[ResourceType] = Field(default_factory=list)
     resources: list[Resource] = Field(default_factory=list)
     jobs: list[Job] = Field(default_factory=list)
 
-    @validator("resource_types")
+    @field_validator("resource_types")
+    @classmethod
     def deduplicate_resource_types(
-        cls, resource_types: list[ResourceType]  # noqa: N805
+        cls, resource_types: list[ResourceType]
     ) -> list[ResourceType]:
         """Ensure that there are no duplicate resource type definitions.
 
         Concourse pipelines don't support duplicate definitions of resource types, where
         the `name` identifier is used to determine uniqueness.  This ensurs that
         `PipelineFragment` objects can be composed together without violating that
         requirement.
@@ -34,18 +35,17 @@
         resource_type_identifiers: set[str] = set()
         for resource_type in resource_types or []:
             if resource_type.name not in resource_type_identifiers:
                 resource_type_identifiers.add(resource_type.name)
                 unique_resource_types.append(resource_type)
         return unique_resource_types
 
-    @validator("resources")
-    def deduplicate_resources(
-        cls, resources: list[Resource]  # noqa: N805
-    ) -> list[Resource]:
+    @field_validator("resources")
+    @classmethod
+    def deduplicate_resources(cls, resources: list[Resource]) -> list[Resource]:
         """Ensure that there are no duplicate resource definitions.
 
         Concourse pipelines don't support duplicate definitions of resources, where the
         `name` identifier is used to determine uniqueness.  This ensurs that
         `PipelineFragment` objects can be composed together without violating that
         requirement.
```

### Comparing `ol-concourse-0.4.4/ol_concourse/lib/models/pipeline.py` & `ol-concourse-0.5.0/ol_concourse/lib/models/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 # generated by datamodel-codegen:
 #   filename:  concourse_pipeline_schema.json
 #   timestamp: 2022-07-13T17:57:35+00:00
 
 from __future__ import annotations
 
-import re
 from enum import Enum
-from typing import Any, Literal, Optional, Union
+from typing import Annotated, Any, Literal, Optional, Union
 
-from pydantic import BaseModel, ConstrainedStr, Extra, Field, PositiveInt
-
-
-class Identifier(ConstrainedStr):
-    regex = re.compile(r"^[a-z][\w\d\-_.]*$")
+from pydantic import (
+    ConfigDict,
+    BaseModel,
+    Field,
+    PositiveInt,
+    RootModel,
+    SerializeAsAny,
+    StringConstraints,
+    model_serializer,
+    model_validator,
+)
+
+
+class Identifier(RootModel[str]):
+    root: Annotated[
+        str,
+        StringConstraints(
+            strip_whitespace=True, strict=False, pattern=r"^[a-z][\w\d\-_.]*$"
+        ),
+    ]
+
+    def __hash__(self):
+        return str.__hash__(self.root)
+
+    @model_serializer
+    def serialize(self):
+        if hasattr(self, "root"):
+            return self.root
+        return self
+        # return self.root
+
+    @model_validator(mode="after")  # type: ignore[arg-type]
+    def coerce_to_string(self):
+        if hasattr(self, "root"):
+            return self.root
+        return self
 
 
 class Step(BaseModel):
     pass
 
 
-class Version(BaseModel):
-    __root__: dict[str, str]
+class Version(RootModel[dict[str, str]]):
+    root: dict[str, str]
 
 
-class Value(str):
-    pass
+class Value(RootModel[str]):
+    root: str
 
 
-class Duration(BaseModel):
-    __root__: str
+class Duration(RootModel[str]):
+    root: str
 
 
 class RegistryImage(BaseModel):
     repository: str
     tag: str = "latest"
 
 
 class DisplayConfig(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     background_image: Optional[str] = Field(
         None,
         description=(
             "Allow users to specify a custom background image which is put at 30% "
             " opacity, grayscaled and blended into existing background. Must be an "
             " http, https, or relative URL."
         ),
     )
 
 
 class Cache(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     path: Optional[str] = Field(
         None,
         description=(
             "The path to a directory to be cached.    Paths are relative to the working"
             " directory of the task. Absolute paths  are not respected."
         ),
@@ -128,16 +156,15 @@
 
     linux = "linux"
     darwin = "darwin"
     windows = "windows"
 
 
 class VarSource(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     name: Optional[str] = Field(
         None,
         description=(
             "The name of the `((var))` source. This should be short and  simple. This"
             " name will be referenced  var-syntax  throughout  the config."
         ),
@@ -145,16 +172,15 @@
 
 
 class Vars(BaseModel):
     pass
 
 
 class Command(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     args: Optional[list[str]] = Field(
         None,
         description=(
             "Arguments to pass to the command. Note that when executed with    fly-cli "
             " Fly  , any arguments passed to  fly-execute    are appended to this"
             " array."
@@ -176,39 +202,37 @@
             " directory, then `path` is relative to  it.    This is commonly a path to"
             " a script provided by one of the task's inputs,  e.g."
             " `my-resource/scripts/test` . It could also be a command like   `bash`"
             " (respecting standard `$PATH` lookup rules), or an absolute  path to a"
             " file to execute, e.g. `/bin/bash` ."
         ),
     )
-    dir: Optional[str] = Field(
+    dir: Optional[str | Identifier] = Field(
         None,
         description=(
             "A directory, relative to the initial working directory, to set as the "
             " working directory when running the script."
         ),
     )
 
 
-class Number(BaseModel):
-    __root__: float
+class Number(RootModel[float]):
+    root: float
 
 
 class DummyConfig(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     vars: Optional[Vars] = Field(
         None, description="A mapping of var name to var value."
     )
 
 
 class GroupConfig(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     name: Optional[Identifier] = Field(
         None,
         description=(
             "A unique name for the group. This should be short and simple as it will "
             " be used as the tab name for navigation."
         ),
@@ -253,54 +277,53 @@
         "30 minutes.",
     )
     tags: Optional[list[str]] = Field(
         None,
         description="The tags by which to match workers. The step will be placed within"
         " the a pool of workers that match all of the given set of tags.",
     )
-    ensure: Optional[Step] = Field(
+    ensure: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute regardless of whether the job succeeds, fails, errors, or "
             " aborts. Equivalent to the  schema.ensure  hook."
         ),
     )
-    on_abort: Optional[Step] = Field(
+    on_abort: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute when the task aborts. Equivalent to the schema.on_abort"
             " hook."
         ),
     )
-    on_error: Optional[Step] = Field(
+    on_error: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute when the task errors. Equivalent to the schema.on_error"
             " hook."
         ),
     )
-    on_failure: Optional[Step] = Field(
+    on_failure: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute when the task fails. Equivalent to the schema.on_failure"
             " hook."
         ),
     )
-    on_success: Optional[Step] = Field(
+    on_success: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute when the task succeeds. Equivalent to the"
             " schema.on_success  hook."
         ),
     )
 
 
 class PutStep(Step, StepModifierMixin):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     resource: Optional[str] = Field(
         None,
         description=(
             "Defaults to the value of `put` .  The resource to update,  as configured"
             " in  schema.pipeline.resources  .     \n@example  Re-label Put Resource \n"
             '    ```yaml\njobs:\n- name: fetch-repo\n  plan:\n    # puts to "repo" and'
@@ -381,18 +404,17 @@
             " app-image\n  type: mock\n- name: ci\n  type: mock\n  source:\n   "
             ' create_files:\n      version.txt: "42"\n```'
         ),
     )
 
 
 class AnonymousResource(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    source: Optional[dict[str, Any]] = Field(
+    source: Optional[dict[str, Any] | RegistryImage] = Field(
         None,
         description=(
             "The configuration for the resource; see    schema.resource.source  ."
         ),
     )
     params: Optional[dict[str, Any]] = Field(
         None,
@@ -417,16 +439,15 @@
             " `/rootfs` directory containing a full filesystem, and a   `metadata.json`"
             " file containing."
         ),
     )
 
 
 class Output(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     path: Optional[str] = Field(
         None,
         description=(
             "The path to a directory where the output will be taken from. If not "
             " specified, the output's `name` is used.    Paths are relative to the"
             " working directory of the task. Absolute paths are not respected."
@@ -438,16 +459,15 @@
             "The name of the output. The contents under `path` will be made  available"
             " to the rest of the plan under this name."
         ),
     )
 
 
 class BuildLogRetentionPolicy(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     days: Optional[Number] = Field(
         None,
         description=(
             "Keep logs for builds which have finished within the specified number of "
             " days."
         ),
@@ -467,16 +487,15 @@
     )
     builds: Optional[Number] = Field(
         None, description="Keep logs for the last specified number of builds."
     )
 
 
 class Input(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     path: Optional[str] = Field(
         None,
         description=(
             "The path where the input will be placed. If not specified, the input's  "
             " `name` is used.    Paths are relative to the working directory of the"
             " task. Absolute paths  are not respected."
@@ -491,16 +510,15 @@
             " running task."
         ),
     )
     name: Optional[Identifier] = Field(None, description="The name of the input.")
 
 
 class AcrossVar(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     var: Optional[Identifier] = Field(
         None,
         description=(
             'The name of the variable that will be added to the    local-vars  " `.` "'
             " var source  . This variable will only be  accessible in the scope of the"
             " step - each iteration of the step gets  its own scope.    If a variable"
@@ -557,16 +575,15 @@
             " will run in parallel, since all 3 of   `var1` 's values can run in"
             " parallel, and 2 of `var3` 's  values can run in parallel."
         ),
     )
 
 
 class DummyVarSource(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     config: Optional[DummyConfig] = Field(
         None,
         description=(
             "dummy_config      vars  vars    A mapping of var name to var value."
         ),
     )
@@ -578,16 +595,15 @@
             " credential  management but still have sensitive values that you would"
             " like to    creds-redacting  redact  them from build output."
         ),
     )
 
 
 class VaultConfig(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     path_prefix: Optional[str] = Field(
         None,
         description=(
             "Default `/concourse` .  A prefix under which to  look for all credential"
             " values.    See  vault-path-prefix  for more information."
         ),
@@ -684,16 +700,15 @@
             "When retrying during authentication, start with this retry  interval. The"
             " interval will increase exponentially until   `auth_retry_max` is reached."
         ),
     )
 
 
 class SetPipelineStep(Step, StepModifierMixin):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     set_pipeline: Optional[Union[Identifier, Literal["self"]]] = Field(
         None,
         description=(
             "The identifier specifies the name of the pipeline to configure. Unless   "
             " schema.set-pipeline.team  is set, it will be configured  within the"
             " current team and be created  unpaused  . If set to `self` ,  the current"
@@ -825,16 +840,15 @@
             " github\n  source:\n    uri:"
             " https://github.com/concourse/examples.git\n```"
         ),
     )
 
 
 class LoadVarStep(Step, StepModifierMixin):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     format: Optional[Format] = Field(
         None,
         description=(
             "The format of the file's content.    If unset, Concourse will try to"
             " detect the format from the file  extension. If the file format cannot be"
             " determined, Concourse will  fallback to `trim` .    If set to `json` ,"
@@ -889,16 +903,15 @@
             "The path to a file whose content shall be read and used as the var's "
             " value."
         ),
     )
 
 
 class Resource(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="allow")
 
     name: Optional[Identifier] = Field(
         None,
         description=(
             "The name of the resource. This should be short and simple. This name will "
             " be referenced by  build-plans  build plans  of jobs in the  pipeline."
         ),
@@ -1029,16 +1042,15 @@
     type: Optional[str] = Field(
         None,
         description="The  resource-types  resource type  implementing the resource.",
     )
 
 
 class ContainerLimits(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     cpu: Optional[Number] = Field(
         None,
         description=(
             "The maximum amount of CPU available to the task container, measured in "
             " shares. 0 means unlimited.    CPU shares are relative to the CPU shares"
             " of other containers on a  worker. For example, if you have two containers"
@@ -1057,16 +1069,15 @@
             "The maximum amount of memory available to the task container, measured in "
             " bytes. 0 means unlimited."
         ),
     )
 
 
 class ResourceType(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     privileged: Optional[bool] = Field(
         None,
         description=(
             "Default `false` .  If set to `true` , the resource's  containers will be"
             " run with full capabilities, as determined by the worker  backend the task"
             " runs on.    For Linux-based backends it typically determines whether or"
@@ -1082,15 +1093,15 @@
     params: Optional[dict[str, Any]] = Field(
         None,
         description=(
             "Arbitrary config to pass when running the `get` to fetch the resource "
             " type's image."
         ),
     )
-    source: Optional[dict[str, Any]] = Field(
+    source: Optional[dict[str, Any] | RegistryImage] = Field(
         None,
         description=(
             "The configuration for the resource type's resource. This varies  by"
             " resource type, and is a black box to Concourse; it is blindly passed to "
             " the resource at runtime.    To use `registry-image` as an example, the"
             " source would contain something  like `repository: username/reponame` ."
             " See the  Registry Image  resource "
@@ -1159,16 +1170,15 @@
             " busybox\n```     Alternatively, the web node can be configured to use   "
             " resource-defaults  defaults for base resource types"
         ),
     )
 
 
 class GetStep(Step, StepModifierMixin):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     version: Optional[Union[Literal["latest"], Literal["every"], Version]] = Field(
         None,
         description=(
             "Default `latest` .  The version of the resource to fetch.    If set to"
             " `latest` , scheduling will just find the latest available  version of a"
             " resource and use it, allowing versions to be skipped.  This is  usually"
@@ -1276,16 +1286,15 @@
             "     file: cyberdeck/version_to_put.txt\n\n\nresources:\n- name:"
             " cyberdeck\n  type: mock\n```"
         ),
     )
 
 
 class VaultVarSource(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     type: Optional[Literal["vault"]] = Field(
         None,
         description=(
             "The `vault` type supports configuring a    Vault "
             " https://www.vaultproject.io  server as a   `((var))` source."
         ),
@@ -1327,16 +1336,15 @@
             " When retrying during authentication, start with this retry  interval. The"
             " interval will increase exponentially until   `auth_retry_max` is reached."
         ),
     )
 
 
 class TaskConfig(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     image_resource: Optional[AnonymousResource] = Field(
         None,
         description=(
             "The container image to run with, as provided by an anonymous    resources "
             " resource  definition.    Whenever the task runs, the anonymous resource"
             " will be `check` ed to  discover the latest version available. The image"
@@ -1489,16 +1497,15 @@
             " the preferred way to specify base image.  You should only use this if you"
             " have no other option and you really know  what you're doing."
         ),
     )
 
 
 class TaskStep(Step, StepModifierMixin):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     config: Optional[TaskConfig] = Field(
         None,
         description=(
             "The  tasks  task config  to execute.   \n@example  Task config \n   "
             " ```yaml\njobs:\n- name: job\n  public: true\n  plan:\n  - task:"
             " simple-task\n    config: # contains all field in a task config\n     "
@@ -1713,18 +1720,17 @@
             " source: { repository: busybox }\n      run:\n        path: echo\n       "
             ' args: ["Hello world!"]\n```'
         ),
     )
 
 
 class InParallelStep(Step, StepModifierMixin):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    in_parallel: Optional[Union[list[Step], InParallelConfig]] = Field(
+    in_parallel: Optional[Union[list[SerializeAsAny[Step]], InParallelConfig]] = Field(
         None,
         description=(
             "Steps are either configured as a array or within an   "
             " schema.in_parallel_config  .     \n@example  Fetching artifacts in"
             " parallel \n   Using the `in_parallel` step where possible is the easiest"
             " way  to speeding up a builds.    It is often used to fetch all dependent"
             " resources together at the  start of a build plan:     ```yaml\njobs:\n-"
@@ -1738,16 +1744,15 @@
             "   file: some-repo/ci/linux.yml\n  - task: unit-darwin\n    file:"
             " some-repo/ci/darwin.yml\n```"
         ),
     )
 
 
 class Job(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     build_log_retention: Optional[BuildLogRetentionPolicy] = Field(
         None,
         description=(
             "Configures the retention policy for build logs. This is useful if you have"
             "  a job that runs often but after some amount of time the logs aren't"
             " worth  keeping around.    Builds which are not retained by the configured"
@@ -1792,15 +1797,15 @@
     disable_manual_trigger: Optional[bool] = Field(
         None,
         description=(
             "Default `false` .  If set to `true` , manual triggering of  the job (via"
             " the web UI or  fly-trigger-job  ) will be disabled."
         ),
     )
-    ensure: Optional[Step] = Field(
+    ensure: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute regardless of whether the job succeeds, fails, errors, or "
             " aborts. Equivalent to the  schema.ensure  hook."
         ),
     )
     interruptible: Optional[bool] = Field(
@@ -1842,44 +1847,44 @@
             " job \n   This can be used to rename a job without losing its history,"
             " like so:     ```yaml\njobs:\n- name: new-name\n  old_name: current-name\n"
             "  plan: [{get: 10m}]\n```     After the pipeline is set, because the"
             " builds have been inherited, the job can  have the field removed:    "
             " ```yaml\njobs:\n- name: new-name\n  plan: [{get: 10m}]\n```"
         ),
     )
-    on_abort: Optional[Step] = Field(
+    on_abort: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute when the job aborts. Equivalent to the    schema.on_abort "
             " hook."
         ),
     )
-    on_error: Optional[Step] = Field(
+    on_error: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute when the job errors. Equivalent to the    schema.on_error "
             " hook."
         ),
     )
-    on_failure: Optional[Step] = Field(
+    on_failure: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
             "Step to execute when the job fails. Equivalent to the    schema.on_failure"
             "  hook."
         ),
     )
-    on_success: Optional[Step] = Field(
+    on_success: Optional[SerializeAsAny[Step]] = Field(
         None,
         description=(
-            "Step to execute when the job succeeds. Equivalent to the   "
+            "Step to execute when the job succeeds. Equivalent to the"
             " schema.on_success  hook."
         ),
     )
-    plan: Optional[list[Step]] = Field(
-        None, description="The sequence of  steps  steps  to execute."
+    plan: Optional[list[SerializeAsAny[Step]]] = Field(
+        None, description="The sequence of steps to execute."
     )
     public: Optional[bool] = Field(
         None,
         description=(
             "Default `false` .  If set to `true` , the build log of this  job will be"
             " viewable by unauthenticated users. Unauthenticated users will  always be"
             " able to see the inputs, outputs, and build status history of a  job. This"
@@ -1911,20 +1916,23 @@
             " time as `job-b` .    The builds are executed in their order of creation,"
             " across all jobs with  common tags."
         ),
     )
 
 
 class Pipeline(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    def json(self, *args, **kwargs):
+    def model_dump_json(self, *args, **kwargs):
         kwargs["exclude_none"] = True
-        return super().json(*args, **kwargs)
+        kwargs["by_alias"] = True
+        return super().model_dump_json(*args, **kwargs)
+
+    def json(self, *args, **kwargs):
+        return self.model_dump_json(*args, **kwargs)
 
     jobs: Optional[list[Job]] = Field(
         None,
         description=(
             "A set of  jobs  jobs  for the pipeline to continuously schedule. At least"
             " one job is required for a pipeline to be valid."
         ),
@@ -1993,19 +2001,17 @@
         description=(
             "A set of  resources  resources  for the pipeline to continuously  check."
         ),
     )
 
 
 class TryStep(Step, StepModifierMixin):
-    class Config:
-        extra = Extra.forbid
-        allow_population_by_field_name = True
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
 
-    try_: Optional[Step] = Field(
+    try_: Optional[SerializeAsAny[Step]] = Field(
         None,
         alias="try",
         description=(
             "Performs the given step, ignoring any failure and masking it with "
             " success.    This can be used when you want to perform some side-effect,"
             " but you  don't really want the whole build to fail if it doesn't work.   "
             "  \n@example  Allowing non-critical behavior to fail \n   When emitting"
@@ -2015,16 +2021,15 @@
             " try:\n      put: test-logs\n      params:\n        from:"
             " run-tests/*.log\n- task: do-something-else\n  config: # ...\n```"
         ),
     )
 
 
 class InParallelConfig(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     limit: Optional[Number] = Field(
         None,
         description=(
             "Default unlimited.  A sempahore which limits the  parallelism when"
             " executing the steps in a `in_parallel` step.  When set, the number of"
             " running steps will not exceed the limit.    When not specified,"
@@ -2046,15 +2051,15 @@
         None,
         description=(
             "Default `false` .  When enabled the parallel step will  fail fast by"
             " returning as soon as any sub-step fails. This means that running steps "
             " will be interrupted and pending steps will no longer be scheduled."
         ),
     )
-    steps: Optional[list[Step]] = Field(
+    steps: Optional[list[SerializeAsAny[Step]]] = Field(
         None,
         description=(
             "The steps to perform in parallel.   \n@example  Fetching artifacts in"
             " parallel \n   Using the `in_parallel` step where possible is the easiest"
             " way  to speeding up a builds.    It is often used to fetch all dependent"
             " resources together at the  start of a build plan:     ```yaml\njobs:\n-"
             " name: get-in-parallel\n  plan:\n  - in_parallel:\n      limit: 2\n     "
@@ -2062,18 +2067,17 @@
             " - get: code\n\n\nresources:\n- name: repo\n  type: mock\n- name: code\n "
             " type: mock\n- name: ci\n  type: mock\n```"
         ),
     )
 
 
 class DoStep(Step, StepModifierMixin):
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    do: Optional[list[Step]] = Field(
+    do: Optional[list[SerializeAsAny[Step]]] = Field(
         None,
         description=(
             "@example  Running multiple steps in a try \n   This can be used to perform"
             " multiple steps serially in a    try-step  :     ```yaml\njobs:\n- name:"
             " with-do\n  plan:\n  - try:\n      do:\n      - get: black-ice\n      -"
             " get: control-node\n      - get: cyberdeck\n\nresources:\n- name:"
             " black-ice\n  type: mock\n- name: control-node\n  type: mock\n- name:"
```

### Comparing `ol-concourse-0.4.4/ol_concourse/lib/notifications.py` & `ol-concourse-0.5.0/ol_concourse/lib/notifications.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.4/ol_concourse/lib/resource_types.py` & `ol-concourse-0.5.0/ol_concourse/lib/resource_types.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.4/ol_concourse/lib/resources.py` & `ol-concourse-0.5.0/ol_concourse/lib/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Optional, Union
 
 from ol_concourse.lib.models.pipeline import Identifier, RegistryImage, Resource
 from ol_concourse.lib.models.resource import Git
 
 
-def git_repo(
+def git_repo(  # noqa: PLR0913
     name: Identifier,
     uri: str,
     branch: str = "main",
     check_every: str = "60s",
     paths: Optional[list[str]] = None,
+    depth: Optional[int] = None,
     **kwargs,
 ) -> Resource:
     return Resource(
         name=name,
         type="git",
         icon="git",
         check_every=check_every,
-        source=Git(uri=uri, branch=branch, paths=paths),
+        source=Git(uri=uri, branch=branch, paths=paths).model_dump(exclude_none=True),
         **kwargs,
     )
 
 
 def ssh_git_repo(
     name: Identifier,
     uri: str,
@@ -29,15 +30,17 @@
     branch: str = "main",
     paths: Optional[list[str]] = None,
 ) -> Resource:
     return Resource(
         name=name,
         type="git",
         icon="git",
-        source=Git(uri=uri, branch=branch, paths=paths, private_key=private_key),
+        source=Git(
+            uri=uri, branch=branch, paths=paths, private_key=private_key
+        ).model_dump(exclude_none=True),
     )
 
 
 def github_release(name: Identifier, owner: str, repository: str) -> Resource:
     """Generate a github-release resource for the given owner/repository.
 
     :param name: The name of the resource. This will get used across subsequent
@@ -115,27 +118,30 @@
         name=name,
         type="time",
         icon="clock",
         source={"interval": interval},
     )
 
 
-def registry_image(
+def registry_image(  # noqa: PLR0913
     name: Identifier,
     image_repository: str,
     image_tag: Optional[str] = None,
+    variant: Optional[str] = None,
     username=None,
     password=None,
 ) -> Resource:
     image_source = RegistryImage(
         repository=image_repository, tag=image_tag or "latest"
-    ).dict()
+    ).model_dump()
     if username and password:
         image_source["username"] = username
         image_source["password"] = password
+    if variant:
+        image_source["variant"] = variant
     return Resource(
         name=name,
         type="registry-image",
         source=image_source,
     )
```

### Comparing `ol-concourse-0.4.4/ol_concourse/lib/tasks.py` & `ol-concourse-0.5.0/ol_concourse/lib/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             },
             params={},
             run=Command(
                 path="bash",
                 args=[
                     "-ec",
                     f"""ASG_NAME=$(aws autoscaling describe-auto-scaling-groups --color on --no-cli-auto-prompt --no-cli-pager --filters {filters} --query "{queries}" --output text);
-                    aws autoscaling start-instance-refresh --color on --no-cli-auto-prompt --no-cli-pager --auto-scaling-group-name $ASG_NAME --preferences MinHealthyPercentage=50,InstanceWarmup=120""",  # noqa: #501
+                    aws autoscaling start-instance-refresh --color on --no-cli-auto-prompt --no-cli-pager --auto-scaling-group-name $ASG_NAME --preferences MinHealthyPercentage=50,InstanceWarmup=120""",  # noqa: E501
                 ],
             ),
         ),
     )
 
 
 # Generates a TaskStep that can be used to block a job from completing until
@@ -57,12 +57,12 @@
                     f""" ASG_NAME=$(aws autoscaling describe-auto-scaling-groups --color on --no-cli-auto-prompt --no-cli-pager --filters {filters} --query "{queries}" --output text);
                     status="InProgress"
                     while [ "$status" = "InProgress" ] || [ "$status" == "Pending" ] || [ "$status" == "Canceling" ]
                     do
                         sleep {check_freq}
                         status=$(aws autoscaling describe-instance-refreshes --color on --no-cli-auto-prompt --no-cli-pager --auto-scaling-group-name $ASG_NAME --query "sort_by(InstanceRefreshes, &StartTime)[].{{Status: Status}}" --output text | tail -n 1)
                         aws autoscaling describe-instance-refreshes --color on --no-cli-auto-prompt --no-cli-pager --auto-scaling-group-name $ASG_NAME --query "sort_by(InstanceRefreshes, &StartTime)[].{{InstanceRefreshId: InstanceRefreshId, StartTime: StartTime, Status: Status}}" --output text | tail -n 1
-                    done""",  # noqa: #501
+                    done""",  # noqa: E501
                 ],
             ),
         ),
     )
```

### Comparing `ol-concourse-0.4.4/ol_concourse.egg-info/SOURCES.txt` & `ol-concourse-0.5.0/ol_concourse.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 ol_concourse/lib/containers.py
 ol_concourse/lib/notifications.py
 ol_concourse/lib/resource_types.py
 ol_concourse/lib/resources.py
 ol_concourse/lib/tasks.py
 ol_concourse/lib/jobs/infrastructure.py
 ol_concourse/lib/models/__init__.py
+ol_concourse/lib/models/concourse_pipeline_models.py
 ol_concourse/lib/models/fragment.py
 ol_concourse/lib/models/pipeline.py
 ol_concourse/lib/models/resource.py
```

