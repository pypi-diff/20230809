# Comparing `tmp/jupyter_ai_magics-2.0.0.tar.gz` & `tmp/jupyter_ai_magics-2.0.1.tar.gz`

## Comparing `jupyter_ai_magics-2.0.0.tar` & `jupyter_ai_magics-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/setup.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/aliases.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/embedding_providers.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/parsers.py
--rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/README.md
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/setup.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    21442 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/parsers.py
+-rw-r--r--   0        0        0    16797 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/README.md
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.1/PKG-INFO
```

### Comparing `jupyter_ai_magics-2.0.0/package.json` & `jupyter_ai_magics-2.0.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'2.0.1'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[dev,all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `jupyter_ai_magics-2.0.0/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-2.0.1/jupyter_ai_magics/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.0.0/jupyter_ai_magics/embedding_providers.py` & `jupyter_ai_magics-2.0.1/jupyter_ai_magics/embedding_providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.0.0/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-2.0.1/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.0.0/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-2.0.1/jupyter_ai_magics/magics.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,38 +76,25 @@
     "md": Markdown,
     "json": JSON,
     "text": TextWithMetadata,
 }
 
 NA_MESSAGE = '<abbr title="Not applicable">N/A</abbr>'
 
-MARKDOWN_PROMPT_TEMPLATE = "{prompt}\n\nProduce output in markdown format only."
-
 PROVIDER_NO_MODELS = "This provider does not define a list of models."
 
 CANNOT_DETERMINE_MODEL_TEXT = """Cannot determine model provider from model ID '{0}'.
 
 To see a list of models you can use, run '%ai list'"""
 
 CANNOT_DETERMINE_MODEL_MARKDOWN = """Cannot determine model provider from model ID `{0}`.
 
 To see a list of models you can use, run `%ai list`"""
 
 
-PROMPT_TEMPLATES_BY_FORMAT = {
-    "code": "{prompt}\n\nProduce output as source code only, with no text or explanation before or after it.",
-    "html": "{prompt}\n\nProduce output in HTML format only, with no markup before or afterward.",
-    "image": "{prompt}\n\nProduce output as an image only, with no text before or after it.",
-    "markdown": MARKDOWN_PROMPT_TEMPLATE,
-    "md": MARKDOWN_PROMPT_TEMPLATE,
-    "math": "{prompt}\n\nProduce output in LaTeX format only, with $$ at the beginning and end.",
-    "json": "{prompt}\n\nProduce output in JSON format only, with nothing before or after it.",
-    "text": "{prompt}",  # No customization
-}
-
 AI_COMMANDS = {"delete", "error", "help", "list", "register", "update"}
 
 
 class FormatDict(dict):
     """Subclass of dict to be passed to str#format(). Suppresses KeyError and
     leaves replacement field unchanged if replacement field is not associated
     with a value."""
@@ -461,32 +448,14 @@
     def handle_list(self, args: ListArgs):
         return TextOrMarkdown(
             self._ai_list_command_text(args.provider_id),
             self._ai_list_command_markdown(args.provider_id),
         )
 
     def run_ai_cell(self, args: CellArgs, prompt: str):
-        # Apply a prompt template.
-        prompt = PROMPT_TEMPLATES_BY_FORMAT[args.format].format(prompt=prompt)
-
-        # interpolate user namespace into prompt
-        ip = get_ipython()
-        prompt = prompt.format_map(FormatDict(ip.user_ns))
-
-        # Determine provider and local model IDs
-        # If this is a custom chain, send the message to the custom chain.
-        if args.model_id in self.custom_model_registry and isinstance(
-            self.custom_model_registry[args.model_id], LLMChain
-        ):
-            return self.display_output(
-                self.custom_model_registry[args.model_id].run(prompt),
-                args.format,
-                {"jupyter_ai": {"custom_chain_id": args.model_id}},
-            )
-
         provider_id, local_model_id = self._decompose_model_id(args.model_id)
         Provider = self._get_provider(provider_id)
         if Provider is None:
             return TextOrMarkdown(
                 CANNOT_DETERMINE_MODEL_TEXT.format(args.model_id)
                 + "\n\n"
                 + "If you were trying to run a command, run '%ai help' to see a list of commands.",
@@ -496,14 +465,25 @@
             )
 
         # if `--reset` is specified, reset transcript and return early
         if provider_id == "openai-chat" and args.reset:
             self.transcript_openai = []
             return
 
+        # Determine provider and local model IDs
+        # If this is a custom chain, send the message to the custom chain.
+        if args.model_id in self.custom_model_registry and isinstance(
+            self.custom_model_registry[args.model_id], LLMChain
+        ):
+            return self.display_output(
+                self.custom_model_registry[args.model_id].run(prompt),
+                args.format,
+                {"jupyter_ai": {"custom_chain_id": args.model_id}},
+            )
+
         # validate presence of authn credentials
         auth_strategy = self.providers[provider_id].auth_strategy
         if auth_strategy:
             # TODO: handle auth strategies besides EnvAuthStrategy
             if auth_strategy.type == "env" and auth_strategy.name not in os.environ:
                 raise OSError(
                     f"Authentication environment variable {auth_strategy.name} not provided.\n"
@@ -537,14 +517,21 @@
                 raise ValueError(
                     "request-schema must be valid JSON. "
                     f"Error at line {e.lineno}, column {e.colno}: {e.msg}"
                 ) from None
 
         provider = Provider(**provider_params)
 
+        # Apply a prompt template.
+        prompt = provider.get_prompt_template(args.format).format(prompt=prompt)
+
+        # interpolate user namespace into prompt
+        ip = get_ipython()
+        prompt = prompt.format_map(FormatDict(ip.user_ns))
+
         # generate output from model via provider
         result = provider.generate([prompt])
         output = result.generations[0][0].text
 
         # if openai-chat, append exchange to transcript
         if provider_id == "openai-chat":
             self._append_exchange_openai(prompt, output)
```

### Comparing `jupyter_ai_magics-2.0.0/jupyter_ai_magics/parsers.py` & `jupyter_ai_magics-2.0.1/jupyter_ai_magics/parsers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.0.0/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-2.0.1/jupyter_ai_magics/providers.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import functools
 import io
 import json
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, ClassVar, Coroutine, Dict, List, Literal, Optional, Union
 
 from jsonpath_ng import parse
+from langchain import PromptTemplate
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import (
     AI21,
     Anthropic,
     Bedrock,
     Cohere,
     HuggingFaceHub,
@@ -113,39 +114,90 @@
     """User inputs expected by this provider when initializing it. Each `Field` `f`
     should be passed in the constructor as a keyword argument, keyed by `f.key`."""
 
     #
     # instance attrs
     #
     model_id: str
+    prompt_templates: Dict[str, PromptTemplate]
+    """Prompt templates for each output type. Can be overridden with
+    `update_prompt_template`. The function `prompt_template`, in the base class,
+    refers to this."""
 
     def __init__(self, *args, **kwargs):
         try:
             assert kwargs["model_id"]
         except:
             raise AssertionError(
                 "model_id was not specified. Please specify it as a keyword argument."
             )
 
         model_kwargs = {}
         if self.__class__.model_id_key != "model_id":
             model_kwargs[self.__class__.model_id_key] = kwargs["model_id"]
 
+        model_kwargs["prompt_templates"] = {
+            "code": PromptTemplate.from_template(
+                "{prompt}\n\nProduce output as source code only, "
+                "with no text or explanation before or after it."
+            ),
+            "html": PromptTemplate.from_template(
+                "{prompt}\n\nProduce output in HTML format only, "
+                "with no markup before or afterward."
+            ),
+            "image": PromptTemplate.from_template(
+                "{prompt}\n\nProduce output as an image only, "
+                "with no text before or after it."
+            ),
+            "markdown": PromptTemplate.from_template(
+                "{prompt}\n\nProduce output in markdown format only."
+            ),
+            "md": PromptTemplate.from_template(
+                "{prompt}\n\nProduce output in markdown format only."
+            ),
+            "math": PromptTemplate.from_template(
+                "{prompt}\n\nProduce output in LaTeX format only, "
+                "with $$ at the beginning and end."
+            ),
+            "json": PromptTemplate.from_template(
+                "{prompt}\n\nProduce output in JSON format only, "
+                "with nothing before or after it."
+            ),
+            "text": PromptTemplate.from_template("{prompt}"),  # No customization
+        }
+
         super().__init__(*args, **kwargs, **model_kwargs)
 
     async def _call_in_executor(self, *args, **kwargs) -> Coroutine[Any, Any, str]:
         """
         Calls self._call() asynchronously in a separate thread for providers
         without an async implementation. Requires the event loop to be running.
         """
         executor = ThreadPoolExecutor(max_workers=1)
         loop = asyncio.get_running_loop()
         _call_with_args = functools.partial(self._call, *args, **kwargs)
         return await loop.run_in_executor(executor, _call_with_args)
 
+    def update_prompt_template(self, format: str, template: str):
+        """
+        Changes the class-level prompt template for a given format.
+        """
+        self.prompt_templates[format] = PromptTemplate.from_template(template)
+
+    def get_prompt_template(self, format) -> PromptTemplate:
+        """
+        Produce a prompt template suitable for use with a particular model, to
+        produce output in a desired format.
+        """
+
+        if format in self.prompt_templates:
+            return self.prompt_templates[format]
+        else:
+            return self.prompt_templates["text"]  # Default to plain format
+
 
 class AI21Provider(BaseProvider, AI21):
     id = "ai21"
     name = "AI21"
     models = [
         "j1-large",
         "j1-grande",
@@ -168,14 +220,15 @@
 class AnthropicProvider(BaseProvider, Anthropic):
     id = "anthropic"
     name = "Anthropic"
     models = [
         "claude-v1",
         "claude-v1.0",
         "claude-v1.2",
+        "claude-2",
         "claude-instant-v1",
         "claude-instant-v1.0",
     ]
     model_id_key = "model"
     pypi_package_deps = ["anthropic"]
     auth_strategy = EnvAuthStrategy(name="ANTHROPIC_API_KEY")
 
@@ -431,14 +484,15 @@
 class BedrockProvider(BaseProvider, Bedrock):
     id = "bedrock"
     name = "Amazon Bedrock"
     models = [
         "amazon.titan-tg1-large",
         "anthropic.claude-v1",
         "anthropic.claude-instant-v1",
+        "anthropic.claude-v2",
         "ai21.j2-jumbo-instruct",
         "ai21.j2-grande-instruct",
     ]
     model_id_key = "model_id"
     pypi_package_deps = ["boto3"]
     auth_strategy = AwsAuthStrategy()
```

### Comparing `jupyter_ai_magics-2.0.0/jupyter_ai_magics/utils.py` & `jupyter_ai_magics-2.0.1/jupyter_ai_magics/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.0.0/.gitignore` & `jupyter_ai_magics-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.0.0/LICENSE` & `jupyter_ai_magics-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.0.0/pyproject.toml` & `jupyter_ai_magics-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-2.0.0/PKG-INFO` & `jupyter_ai_magics-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 2.0.0
+Version: 2.0.1
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

