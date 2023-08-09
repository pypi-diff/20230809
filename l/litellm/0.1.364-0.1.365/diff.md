# Comparing `tmp/litellm-0.1.364.tar.gz` & `tmp/litellm-0.1.365.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.364.tar", max compression
+gzip compressed data, was "litellm-0.1.365.tar", max compression
```

## Comparing `litellm-0.1.364.tar` & `litellm-0.1.365.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2023-08-09 00:05:03.734609 litellm-0.1.364/LICENSE
--rw-r--r--   0        0        0     2787 2023-08-09 00:05:03.734609 litellm-0.1.364/README.md
--rw-r--r--   0        0        0     6148 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/.DS_Store
--rw-r--r--   0        0        0     2131 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3556 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    16894 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0     1372 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2592 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_client.py
--rw-r--r--   0        0        0     6242 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_completion.py
--rw-r--r--   0        0        0      658 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_embedding.py
--rw-r--r--   0        0        0     5938 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/timeout.py
--rw-r--r--   0        0        0    25269 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/utils.py
--rw-r--r--   0        0        0      378 2023-08-09 00:05:03.738609 litellm-0.1.364/pyproject.toml
--rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 litellm-0.1.364/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-09 00:57:16.297403 litellm-0.1.365/LICENSE
+-rw-r--r--   0        0        0     2787 2023-08-09 00:57:16.297403 litellm-0.1.365/README.md
+-rw-r--r--   0        0        0     6148 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/.DS_Store
+-rw-r--r--   0        0        0     2131 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3556 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    16493 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0     1372 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2592 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     7033 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0      658 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_embedding.py
+-rw-r--r--   0        0        0     5938 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/timeout.py
+-rw-r--r--   0        0        0    26566 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/utils.py
+-rw-r--r--   0        0        0      378 2023-08-09 00:57:16.301404 litellm-0.1.365/pyproject.toml
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 litellm-0.1.365/PKG-INFO
```

### Comparing `litellm-0.1.364/LICENSE` & `litellm-0.1.365/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/README.md` & `litellm-0.1.365/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/.DS_Store` & `litellm-0.1.365/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/__init__.py` & `litellm-0.1.365/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.365/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.365/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.365/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.365/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/integrations/aispend.py` & `litellm-0.1.365/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/integrations/berrispend.py` & `litellm-0.1.365/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/integrations/helicone.py` & `litellm-0.1.365/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/integrations/supabase.py` & `litellm-0.1.365/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/main.py` & `litellm-0.1.365/litellm/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,40 +3,17 @@
 from functools import partial
 import dotenv, traceback, random, asyncio, time
 from copy import deepcopy
 import litellm
 from litellm import client, logging, exception_type, timeout, get_optional_params
 import tiktoken
 encoding = tiktoken.get_encoding("cl100k_base")
-from litellm.utils import get_secret, install_and_import
+from litellm.utils import get_secret, install_and_import, CustomStreamWrapper
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
-
-# TODO this will evolve to accepting models
-# replicate/anthropic/cohere
-class CustomStreamWrapper:
-    def __init__(self, completion_stream, model):
-        self.model = model
-        if model in litellm.cohere_models:
-           # cohere does not return an iterator, so we need to wrap it in one
-           self.completion_stream = iter(completion_stream)
-        else: 
-          self.completion_stream = completion_stream
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        if self.model in litellm.anthropic_models:
-          chunk = next(self.completion_stream)
-          return {"choices": [{"delta": chunk.completion}]}
-        elif self.model in litellm.cohere_models:
-          chunk = next(self.completion_stream)
-          return {"choices": [{"delta": chunk.text}]}
-
 new_response = {
         "choices": [
           {
             "finish_reason": "stop",
             "index": 0,
             "message": {
                 "role": "assistant"
@@ -63,25 +40,26 @@
     model, messages, # required params
     # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
     functions=[], function_call="", # optional params
     temperature=1, top_p=1, n=1, stream=False, stop=None, max_tokens=float('inf'),
     presence_penalty=0, frequency_penalty=0, logit_bias={}, user="", deployment_id=None,
     # Optional liteLLM function params
     *, return_async=False, api_key=None, force_timeout=60, azure=False, logger_fn=None, verbose=False,
-    hugging_face = False
+    hugging_face = False, replicate=False,
   ):
   try:
     global new_response
     model_response = deepcopy(new_response) # deep copy the default response format so we can mutate it and it's thread-safe. 
     # check if user passed in any of the OpenAI optional params
     optional_params = get_optional_params(
       functions=functions, function_call=function_call, 
       temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
       presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user, deployment_id=deployment_id,
-      model=model
+      # params to identify the model
+      model=model, replicate=replicate, hugging_face=hugging_face
     )
     if azure == True:
       # azure configs
       openai.api_type = "azure"
       openai.api_base = litellm.api_base if litellm.api_base is not None else get_secret("AZURE_API_BASE")
       openai.api_version = litellm.api_version if litellm.api_version is not None else get_secret("AZURE_API_VERSION")
       # set key
@@ -168,15 +146,15 @@
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
       ## RESPONSE OBJECT
       model_response["choices"][0]["message"]["content"] = completion_response
       model_response["created"] = response["created"]
       model_response["model"] = model
       model_response["usage"] = response["usage"]
       response = model_response
-    elif "replicate" in model:
+    elif "replicate" in model or replicate == True:
       # import replicate/if it fails then pip install replicate
       install_and_import("replicate")
       import replicate
       # replicate defaults to os.environ.get("REPLICATE_API_TOKEN")
       # checking in case user set it to REPLICATE_API_KEY instead 
       if not get_secret("REPLICATE_API_TOKEN") and get_secret("REPLICATE_API_KEY"):
         replicate_api_token = get_secret("REPLICATE_API_KEY")
@@ -192,14 +170,19 @@
         input["max_new_tokens"] = max_tokens # for llama2 models 
       ## LOGGING
       logging(model=model, input=input, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
       ## COMPLETION CALL
       output = replicate.run(
         model,
         input=input)
+      if 'stream' in optional_params and optional_params['stream'] == True:
+        # don't try to access stream object,
+        # let the stream handler know this is replicate
+        response = CustomStreamWrapper(output, "replicate")
+        return response
       response = ""
       for item in output: 
         response += item
       completion_response = response
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
       prompt_tokens = len(encoding.encode(prompt))
```

### Comparing `litellm-0.1.364/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.365/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.365/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.365/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.365/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.365/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.365/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.365/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_api_key_param.py` & `litellm-0.1.365/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_async_fn.py` & `litellm-0.1.365/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_bad_params.py` & `litellm-0.1.365/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.365/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_client.py` & `litellm-0.1.365/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_completion.py` & `litellm-0.1.365/litellm/tests/test_completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,24 +135,40 @@
     try:
         response = completion(model="gpt-3.5-turbo", deployment_id="chatgpt-test", messages=messages, azure=True)
         # Add any assertions here to check the response
         print(response)
     except Exception as e:
         pytest.fail(f"Error occurred: {e}")
 
+# Replicate API endpoints are unstable -> throw random CUDA errors -> this means our tests can fail even if our tests weren't incorrect. 
+def test_completion_replicate_llama_stream():
+    model_name = "replicate/llama-2-70b-chat:2c1608e18606fad2812020dc541930f2d0495ce32eee50074220b87300bc16e1"
+    try:
+        response = completion(model=model_name, messages=messages, stream=True)
+        # Add any assertions here to check the response
+        for result in response:
+            print(result)
+        print(response)
+    except Exception as e:
+        pytest.fail(f"Error occurred: {e}")
 
+def test_completion_replicate_stability_stream():
+    model_name = "stability-ai/stablelm-tuned-alpha-7b:c49dae362cbaecd2ceabb5bd34fdb68413c4ff775111fea065d259d577757beb"
+    try:
+        response = completion(model=model_name, messages=messages, stream=True, replicate=True)
+        # Add any assertions here to check the response
+        for result in response:
+            print(result)
+        print(response)
+    except Exception as e:
+        pytest.fail(f"Error occurred: {e}")
 
-# Replicate API endpoints are unstable -> throw random CUDA errors -> this means our tests can fail even if our tests weren't incorrect. 
-# [TODO] improve our try-except block to handle for these
-# def test_completion_replicate_llama():
-#     model_name = "replicate/llama-2-70b-chat:2c1608e18606fad2812020dc541930f2d0495ce32eee50074220b87300bc16e1"
-#     try:
-#         response = completion(model=model_name, messages=messages, max_tokens=500)
-#         # Add any assertions here to check the response
-#         print(response)
-#     except Exception as e:
-#         print(f"in replicate llama, got error {e}")
-#         pass
-#         if e == "FunctionTimedOut":
-#             pass
-#         else:
-#             pytest.fail(f"Error occurred: {e}")
+def test_completion_replicate_stability():
+    model_name = "stability-ai/stablelm-tuned-alpha-7b:c49dae362cbaecd2ceabb5bd34fdb68413c4ff775111fea065d259d577757beb"
+    try:
+        response = completion(model=model_name, messages=messages, replicate=True)
+        # Add any assertions here to check the response
+        for result in response:
+            print(result)
+        print(response)
+    except Exception as e:
+        pytest.fail(f"Error occurred: {e}")
```

### Comparing `litellm-0.1.364/litellm/tests/test_embedding.py` & `litellm-0.1.365/litellm/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_exceptions.py` & `litellm-0.1.365/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_helicone_integration.py` & `litellm-0.1.365/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_logging.py` & `litellm-0.1.365/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_model_fallback.py` & `litellm-0.1.365/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_no_client.py` & `litellm-0.1.365/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_secrets.py` & `litellm-0.1.365/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_supabase_integration.py` & `litellm-0.1.365/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/tests/test_timeout.py` & `litellm-0.1.365/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/timeout.py` & `litellm-0.1.365/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.364/litellm/utils.py` & `litellm-0.1.365/litellm/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,14 +144,16 @@
     max_tokens = float('inf'),
     presence_penalty = 0,
     frequency_penalty = 0,
     logit_bias = {},
     user = "",
     deployment_id = None,
     model = None,
+    replicate = False,
+    hugging_face = False,
 ):
   optional_params = {}
   if model in litellm.anthropic_models:
     # handle anthropic params
     if stream:
       optional_params["stream"] = stream
     if stop != None:
@@ -166,15 +168,20 @@
     if stream:
       optional_params["stream"] = stream
     if temperature != 1:
         optional_params["temperature"] = temperature
     if max_tokens != float('inf'):
         optional_params["max_tokens"] = max_tokens
     return optional_params
-
+  elif replicate == True:
+    # any replicate models
+    # TODO: handle translating remaining replicate params
+    if stream:
+      optional_params["stream"] = stream
+      return optional_params
   else:# assume passing in params for openai/azure openai
     if functions != []:
         optional_params["functions"] = functions
     if function_call != "":
         optional_params["function_call"] = function_call
     if temperature != 1:
         optional_params["temperature"] = temperature
@@ -195,14 +202,15 @@
     if logit_bias != {}:
         optional_params["logit_bias"] = logit_bias
     if user != "":
         optional_params["user"] = user
     if deployment_id != None:
         optional_params["deployment_id"] = deployment_id
     return optional_params
+  return optional_params
 
 def set_callbacks(callback_list):
   global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel, heliconeLogger, aispendLogger, berrispendLogger, supabaseClient
   try:
     for callback in callback_list:
       if callback == "sentry":
         try:
@@ -553,7 +561,34 @@
         # if secret manager fails default to using .env variables
         os.environ[secret_name] = secret # set to env to be safe
         return secret
      else:
       return os.environ.get(secret_name)
   else:
     return os.environ.get(secret_name)
+
+######## Streaming Class ############################
+# wraps the completion stream to return the correct format for the model
+# replicate/anthropic/cohere
+class CustomStreamWrapper:
+    def __init__(self, completion_stream, model):
+        self.model = model
+        if model in litellm.cohere_models:
+           # cohere does not return an iterator, so we need to wrap it in one
+           self.completion_stream = iter(completion_stream)
+        else: 
+          self.completion_stream = completion_stream
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self.model in litellm.anthropic_models:
+          chunk = next(self.completion_stream)
+          return {"choices": [{"delta": chunk.completion}]}
+        elif self.model == "replicate":
+           chunk = next(self.completion_stream)
+           return {"choices": [{"delta": chunk}]}
+        elif self.model in litellm.cohere_models:
+          chunk = next(self.completion_stream)
+          return {"choices": [{"delta": chunk.text}]}
+
```

### Comparing `litellm-0.1.364/PKG-INFO` & `litellm-0.1.365/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.364
+Version: 0.1.365
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

