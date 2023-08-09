# Comparing `tmp/promptquality-0.2.3.tar.gz` & `tmp/promptquality-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptquality-0.2.3.tar", max compression
+gzip compressed data, was "promptquality-0.3.0.tar", max compression
```

## Comparing `promptquality-0.2.3.tar` & `promptquality-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    10946 2023-07-24 19:45:14.732241 promptquality-0.2.3/LICENSE
--rw-r--r--   0        0        0      157 2023-07-24 19:45:14.732241 promptquality-0.2.3/README.md
--rw-r--r--   0        0        0     1543 2023-07-24 19:45:14.732241 promptquality-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      398 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/__init__.py
--rw-r--r--   0        0        0      353 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/config.py
--rw-r--r--   0        0        0       80 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/integrations.py
--rw-r--r--   0        0        0      172 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/job.py
--rw-r--r--   0        0        0      651 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/routes.py
--rw-r--r--   0        0        0      150 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/constants/run.py
--rw-r--r--   0        0        0     1840 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/get_metrics.py
--rw-r--r--   0        0        0     5276 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/helpers.py
--rw-r--r--   0        0        0      543 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/integrations.py
--rw-r--r--   0        0        0     1060 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/job_progress.py
--rw-r--r--   0        0        0      466 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/login.py
--rw-r--r--   0        0        0     1910 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/run.py
--rw-r--r--   0        0        0     1019 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/set_config.py
--rw-r--r--   0        0        0        0 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/types/__init__.py
--rw-r--r--   0        0        0     7781 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/types/config.py
--rw-r--r--   0        0        0     3619 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/types/run.py
--rw-r--r--   0        0        0      632 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/types/settings.py
--rw-r--r--   0        0        0        0 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/__init__.py
--rw-r--r--   0        0        0     4576 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/api_client.py
--rw-r--r--   0        0        0      838 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/config.py
--rw-r--r--   0        0        0       60 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/logger.py
--rw-r--r--   0        0        0    24559 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/name.py
--rw-r--r--   0        0        0     1625 2023-07-24 19:45:14.732241 promptquality-0.2.3/src/promptquality/utils/request.py
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10946 2023-08-09 01:51:21.496399 promptquality-0.3.0/LICENSE
+-rw-r--r--   0        0        0      157 2023-08-09 01:51:21.496399 promptquality-0.3.0/README.md
+-rw-r--r--   0        0        0     1569 2023-08-09 01:51:21.496399 promptquality-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      398 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/constants/__init__.py
+-rw-r--r--   0        0        0      188 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/constants/config.py
+-rw-r--r--   0        0        0       80 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/constants/integrations.py
+-rw-r--r--   0        0        0      172 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/constants/job.py
+-rw-r--r--   0        0        0      802 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/constants/routes.py
+-rw-r--r--   0        0        0      150 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/constants/run.py
+-rw-r--r--   0        0        0     1840 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/get_metrics.py
+-rw-r--r--   0        0        0    12442 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/helpers.py
+-rw-r--r--   0        0        0      543 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/integrations.py
+-rw-r--r--   0        0        0     1060 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/job_progress.py
+-rw-r--r--   0        0        0      466 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/login.py
+-rw-r--r--   0        0        0     1944 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/run.py
+-rw-r--r--   0        0        0     1327 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/set_config.py
+-rw-r--r--   0        0        0        0 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/types/__init__.py
+-rw-r--r--   0        0        0     7493 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/types/config.py
+-rw-r--r--   0        0        0     4110 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/types/run.py
+-rw-r--r--   0        0        0      632 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/types/settings.py
+-rw-r--r--   0        0        0        0 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/utils/__init__.py
+-rw-r--r--   0        0        0     5734 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/utils/api_client.py
+-rw-r--r--   0        0        0      124 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/utils/config.py
+-rw-r--r--   0        0        0     1455 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/utils/dataset.py
+-rw-r--r--   0        0        0       60 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/utils/logger.py
+-rw-r--r--   0        0        0    24559 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/utils/name.py
+-rw-r--r--   0        0        0     1625 2023-08-09 01:51:21.496399 promptquality-0.3.0/src/promptquality/utils/request.py
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.3.0/PKG-INFO
```

### Comparing `promptquality-0.2.3/LICENSE` & `promptquality-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.3/pyproject.toml` & `promptquality-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "promptquality"
-version = "0.2.3"
+version = "0.3.0"
 description = "🦸 Supercharge your prompts with Galileo's Prompt Inspector!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 requests = "^2.31.0"
-pydantic = "^2.0.3"
+pydantic = "^2.1.1"
 pydantic-settings = "^2.0.2"
 tqdm = "^4.65.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 coverage = "^7.2.3"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.3.1"
+requests-mock = "^1.11.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.1"
 pre-commit = "^3.3.3"
 types-requests = "^2.31.0.1"
 pydantic = {extras = ["mypy"], version = "^2.0.2"}
```

### Comparing `promptquality-0.2.3/src/promptquality/constants/routes.py` & `promptquality-0.3.0/src/promptquality/constants/routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,13 +6,15 @@
     healthcheck="healthcheck",
     login="login",
     get_token="get-token",
     current_user="current_user",
     projects="projects",
     all_projects="projects/all",
     templates="projects/{project_id}/templates",
+    versions="projects/{project_id}/templates/{template_id}/versions",
+    version="projects/{project_id}/templates/{template_id}/versions/{version}",
     dataset="projects/{project_id}/upload_prompt_dataset",
     runs="projects/{project_id}/runs",
     jobs="jobs",
     metrics="projects/{project_id}/runs/{run_id}/metrics",
     integrations="integrations/{integration_name}",
 )
```

### Comparing `promptquality-0.2.3/src/promptquality/get_metrics.py` & `promptquality-0.3.0/src/promptquality/get_metrics.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.3/src/promptquality/integrations.py` & `promptquality-0.3.0/src/promptquality/integrations.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.3/src/promptquality/job_progress.py` & `promptquality-0.3.0/src/promptquality/job_progress.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.3/src/promptquality/run.py` & `promptquality-0.3.0/src/promptquality/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from pathlib import Path
 from typing import Optional
 
 from promptquality.get_metrics import get_metrics
 from promptquality.helpers import (
     create_job,
     create_project,
     create_run,
     create_template,
     upload_dataset,
 )
 from promptquality.job_progress import job_progress
 from promptquality.set_config import set_config
 from promptquality.types.run import PromptMetrics
 from promptquality.types.settings import Settings
+from promptquality.utils.dataset import DatasetType
 from promptquality.utils.name import ts_run_name
 
 
 def run(
     template: str,
-    dataset: Path,
+    dataset: DatasetType,
     project_name: Optional[str] = None,
     run_name: Optional[str] = None,
     template_name: Optional[str] = None,
     settings: Optional[Settings] = None,
     wait: bool = True,
 ) -> Optional[PromptMetrics]:
     config = set_config()
```

### Comparing `promptquality-0.2.3/src/promptquality/types/config.py` & `promptquality-0.3.0/src/promptquality/types/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,26 @@
     computed_field,
     field_serializer,
     field_validator,
     model_validator,
 )
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
-from promptquality.constants.config import ConfigDefaults
 from promptquality.constants.routes import Routes
 from promptquality.constants.run import RunDefaults
 from promptquality.types.run import (
+    BaseTemplateResponse,
     CreateJobResponse,
     CreateProjectResponse,
-    CreatePromptTemplateVersionResponse,
     CreateRunResponse,
-    CreateTemplateResponse,
+    CreateTemplateVersionResponse,
     UploadDatasetResponse,
 )
 from promptquality.utils.api_client import ApiClient
-from promptquality.utils.config import _config_location
+from promptquality.utils.config import get_config_location
 from promptquality.utils.logger import logger
 
 
 class Config(BaseSettings):
     console_url: HttpUrl
     # User.
     username: Optional[str] = None
@@ -74,38 +73,36 @@
             api_url = "http://localhost:8088"
         else:
             api_url = self.console_url.unicode_string().replace("console", "api")
         return HttpUrl(api_url)
 
     @property
     def config_file(self) -> Path:
-        return _config_location()
+        return get_config_location()
 
     @field_validator("console_url", mode="before")
     def http_url(cls, value: str) -> str:
         if value and not (value.startswith("https") or value.startswith("http")):
             value = f"https://{value}"
         return value
 
-    # Ignore arg-type until a fix for this issue is released:
-    # https://github.com/pydantic/pydantic/issues/6709
-    @model_validator(mode="after")  # type: ignore[arg-type]
-    def validate_api_url(cls, config: "Config") -> "Config":
-        if not ApiClient.healthcheck(str(config.api_url)):
+    @model_validator(mode="after")
+    def validate_api_url(self) -> "Config":
+        if not ApiClient.healthcheck(str(self.api_url)):
             # TODO: Make this a custom error.
-            raise ValidationError(f"Could not connect to {config.api_url}.")
-        return config
+            raise ValidationError(f"Could not connect to {self.api_url}.")
+        return self
 
     @field_serializer("token", when_used="json")
     def serialize_token(self, value: SecretStr) -> str:
         return value.get_secret_value()
 
     @classmethod
-    def read(cls, config_directory: str = ConfigDefaults.config_directory) -> "Config":
-        return cls.model_validate_json(_config_location().read_text())
+    def read(cls) -> "Config":
+        return cls.model_validate_json(get_config_location().read_text())
 
     def write(self) -> None:
         self.config_file.parent.mkdir(exist_ok=True)
         self.config_file.write_text(self.model_dump_json(exclude_none=True))
 
     @property
     def run_url(self) -> str:
@@ -184,23 +181,23 @@
 
     def merge_project(self, project: CreateProjectResponse) -> None:
         self.current_project_id = project.id
         self.current_project_name = project.name
         self.write()
         logger.debug(f"📝 Set current project to {project.name}.")
 
-    def merge_template(self, template: CreateTemplateResponse) -> None:
+    def merge_template(self, template: BaseTemplateResponse) -> None:
         self.current_template_id = template.id
         self.current_template_name = template.name
         self.merge_template_version(template.selected_version)
         self.write()
         logger.debug(f"📝 Set current template to {template.name}.")
 
     def merge_template_version(
-        self, template_version: CreatePromptTemplateVersionResponse
+        self, template_version: CreateTemplateVersionResponse
     ) -> None:
         self.current_template_version_id = template_version.id
         self.current_template_version = template_version.version
         self.current_template = template_version.template
         self.write()
         logger.debug(f"📝 Set current template version to {template_version.version}.")
```

### Comparing `promptquality-0.2.3/src/promptquality/types/run.py` & `promptquality-0.3.0/src/promptquality/types/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Dict, List, Optional
 
 from pydantic import UUID4, BaseModel, Field, SecretStr, field_validator
 
 from promptquality.constants.integrations import IntegrationName
 from promptquality.constants.run import RunDefaults
 from promptquality.types.settings import Settings
+from promptquality.utils.dataset import DatasetType, dataset_to_path
 from promptquality.utils.name import random_name
 
 
 class RandomName(BaseModel):
     name: str = Field(default_factory=random_name)
 
     @field_validator("name", mode="before")
@@ -24,47 +25,57 @@
     type: str = RunDefaults.project_type
 
 
 class CreateProjectResponse(CreateProjectRequest):
     id: UUID4
 
 
-class CreateTemplateRequest(RandomName):
+class BaseTemplateVersionRequest(BaseModel):
     template: str
+    version: Optional[int] = None
+
+
+class CreateTemplateRequest(RandomName, BaseTemplateVersionRequest):
+    project_id: UUID4
+
+
+class CreateTemplateVersionRequest(BaseTemplateVersionRequest):
+    template_id: UUID4
     project_id: UUID4
 
 
-class CreatePromptTemplateVersionResponse(BaseModel):
+class BaseTemplateVersionResponse(BaseTemplateVersionRequest):
     id: UUID4
-    template: str
+
+
+class CreateTemplateVersionResponse(BaseTemplateVersionResponse):
     version: int
 
 
-class CreateTemplateResponse(RandomName):
+class BaseTemplateResponse(RandomName):
     id: UUID4
     template: str
-    selected_version: CreatePromptTemplateVersionResponse
+    selected_version: CreateTemplateVersionResponse
     selected_version_id: UUID4
-    all_versions: List[CreatePromptTemplateVersionResponse] = Field(
-        default_factory=list
-    )
+    all_versions: List[CreateTemplateVersionResponse] = Field(default_factory=list)
 
 
 class UploadDatasetRequest(BaseModel):
     project_id: UUID4
     file_path: Path
     prompt_template_version_id: UUID4
 
     @classmethod
     def from_dataset(
-        cls, dataset: Path, project_id: UUID4, template_version_id: UUID4
+        cls, dataset: DatasetType, project_id: UUID4, template_version_id: UUID4
     ) -> "UploadDatasetRequest":
+        dataset_path = dataset_to_path(dataset)
         return cls(
             project_id=project_id,
-            file_path=dataset,
+            file_path=dataset_path,
             prompt_template_version_id=template_version_id,
         )
 
     @property
     def data(self) -> Dict[str, str]:
         return dict(prompt_template_version_id=str(self.prompt_template_version_id))
 
@@ -135,7 +146,13 @@
     def body(self) -> Dict[str, Any]:
         extra = (
             dict(organization_id=self.organization_id)
             if self.organization_id
             else dict()
         )
         return dict(token=self.api_key.get_secret_value(), extra=extra)
+
+
+class SelectTemplateVersionRequest(BaseModel):
+    project_id: UUID4
+    template_id: UUID4
+    version: int
```

### Comparing `promptquality-0.2.3/src/promptquality/types/settings.py` & `promptquality-0.3.0/src/promptquality/types/settings.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.3/src/promptquality/utils/api_client.py` & `promptquality-0.3.0/src/promptquality/utils/api_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from promptquality.constants.routes import Routes
 from promptquality.types.run import (
     CreateIntegrationRequest,
     CreateJobRequest,
     CreateProjectRequest,
     CreateRunRequest,
     CreateTemplateRequest,
+    CreateTemplateVersionRequest,
     GetMetricsRequest,
+    SelectTemplateVersionRequest,
     UploadDatasetRequest,
 )
 from promptquality.utils.request import HttpHeaders, make_request
 
 
 class ApiClient(BaseModel):
     api_url: HttpUrl
@@ -74,15 +76,15 @@
             headers=headers,
             timeout=timeout,
         )
 
     def get_current_user(self) -> Dict[str, str]:
         return self._make_request(get, endpoint=Routes.current_user)
 
-    def get_projects(self) -> Dict[str, str]:
+    def get_projects(self) -> List[Dict[str, str]]:
         return self._make_request(get, endpoint=Routes.all_projects)
 
     def create_project(self, project_request: CreateProjectRequest) -> Dict[str, str]:
         return self._make_request(
             post,
             endpoint=Routes.projects,
             body=project_request.model_dump(),
@@ -93,14 +95,33 @@
     ) -> Dict[str, str]:
         return self._make_request(
             post,
             endpoint=Routes.templates.format(project_id=template_request.project_id),
             body=template_request.model_dump(mode="json"),
         )
 
+    def get_templates(self, project_id: UUID4) -> List[Dict[str, str]]:
+        return self._make_request(
+            get,
+            endpoint=Routes.templates.format(project_id=project_id),
+        )
+
+    def create_template_version(
+        self,
+        template_version_request: CreateTemplateVersionRequest,
+    ) -> Dict[str, str]:
+        return self._make_request(
+            post,
+            endpoint=Routes.versions.format(
+                project_id=template_version_request.project_id,
+                template_id=template_version_request.template_id,
+            ),
+            body=template_version_request.model_dump(mode="json", exclude_none=True),
+        )
+
     def upload_dataset(self, dataset_request: UploadDatasetRequest) -> Dict[str, str]:
         return self._make_request(
             post,
             json_request_only=True,
             endpoint=Routes.dataset.format(project_id=dataset_request.project_id),
             data=dataset_request.data,
             files=dataset_request.files,
@@ -135,7 +156,19 @@
         return self._make_request(
             put,
             endpoint=Routes.integrations.format(
                 integration_name=integration_request.name
             ),
             body=integration_request.body,
         )
+
+    def put_template_version_selection(
+        self, select_version: SelectTemplateVersionRequest
+    ) -> Dict[str, Any]:
+        return self._make_request(
+            put,
+            endpoint=Routes.version.format(
+                project_id=select_version.project_id,
+                template_id=select_version.template_id,
+                version=select_version.version,
+            ),
+        )
```

### Comparing `promptquality-0.2.3/src/promptquality/utils/name.py` & `promptquality-0.3.0/src/promptquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.3/src/promptquality/utils/request.py` & `promptquality-0.3.0/src/promptquality/utils/request.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.2.3/PKG-INFO` & `promptquality-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: promptquality
-Version: 0.2.3
+Version: 0.3.0
 Summary: 🦸 Supercharge your prompts with Galileo's Prompt Inspector!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # promptquality
```

