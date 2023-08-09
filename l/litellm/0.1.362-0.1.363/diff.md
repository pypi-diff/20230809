# Comparing `tmp/litellm-0.1.362.tar.gz` & `tmp/litellm-0.1.363.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.362.tar", max compression
+gzip compressed data, was "litellm-0.1.363.tar", max compression
```

## Comparing `litellm-0.1.362.tar` & `litellm-0.1.363.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2023-08-08 21:01:05.704367 litellm-0.1.362/LICENSE
--rw-r--r--   0        0        0     2646 2023-08-08 21:01:05.704367 litellm-0.1.362/README.md
--rw-r--r--   0        0        0     6148 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/.DS_Store
--rw-r--r--   0        0        0     2131 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3556 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    15605 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0     1372 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2592 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_client.py
--rw-r--r--   0        0        0     5111 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_completion.py
--rw-r--r--   0        0        0      658 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_embedding.py
--rw-r--r--   0        0        0     5938 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/timeout.py
--rw-r--r--   0        0        0    24462 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/utils.py
--rw-r--r--   0        0        0      378 2023-08-08 21:01:05.708367 litellm-0.1.362/pyproject.toml
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 litellm-0.1.362/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-08 23:12:54.154482 litellm-0.1.363/LICENSE
+-rw-r--r--   0        0        0     2602 2023-08-08 23:12:54.154482 litellm-0.1.363/README.md
+-rw-r--r--   0        0        0     6148 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/.DS_Store
+-rw-r--r--   0        0        0     2131 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3556 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    16220 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0     1372 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2592 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     5665 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0      658 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_embedding.py
+-rw-r--r--   0        0        0     5938 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/timeout.py
+-rw-r--r--   0        0        0    24954 2023-08-08 23:12:54.162483 litellm-0.1.363/litellm/utils.py
+-rw-r--r--   0        0        0      378 2023-08-08 23:12:54.162483 litellm-0.1.363/pyproject.toml
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 litellm-0.1.363/PKG-INFO
```

### Comparing `litellm-0.1.362/LICENSE` & `litellm-0.1.363/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/README.md` & `litellm-0.1.363/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,30 +21,28 @@
 ```
 pip install litellm
 ```
 
 ```python
 from litellm import completion
 
-## set ENV variables
-# ENV variables can be set in .env file, too. Example in .env.example
-os.environ["OPENAI_API_KEY"] = "openai key"
-os.environ["COHERE_API_KEY"] = "cohere key"
-
 messages = [{ "content": "Hello, how are you?","role": "user"}]
 
 # openai call
 response = completion(model="gpt-3.5-turbo", messages=messages)
 
 # cohere call
 response = completion("command-nightly", messages)
 
 # azure openai call
 response = completion("chatgpt-test", messages, azure=True)
 
+# hugging face call
+response = completion(model="stabilityai/stablecode-completion-alpha-3b-4k", messages=messages, hugging_face=True)
+
 # openrouter call
 response = completion("google/palm-2-codechat-bison", messages)
 ```
 Code Sample: [Getting Started Notebook](https://colab.research.google.com/drive/1gR3pY-JzDZahzpVdbGBtrNGDBmzUNJaJ?usp=sharing)
 
 Stable version
 ```
```

### Comparing `litellm-0.1.362/litellm/.DS_Store` & `litellm-0.1.363/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/__init__.py` & `litellm-0.1.363/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.363/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.363/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.363/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.363/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/integrations/aispend.py` & `litellm-0.1.363/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/integrations/berrispend.py` & `litellm-0.1.363/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/integrations/helicone.py` & `litellm-0.1.363/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/integrations/supabase.py` & `litellm-0.1.363/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/main.py` & `litellm-0.1.363/litellm/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 from litellm import client, logging, exception_type, timeout, get_optional_params
 import tiktoken
 encoding = tiktoken.get_encoding("cl100k_base")
 from litellm.utils import get_secret, install_and_import
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
+# TODO this will evolve to accepting models
+# replicate/anthropic/cohere
+class CustomStreamWrapper:
+    def __init__(self, completion_stream):
+        self.completion_stream = completion_stream
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        chunk = next(self.completion_stream)
+        return {"choices": [{"delta": chunk.completion}]}
+
 new_response = {
         "choices": [
           {
             "finish_reason": "stop",
             "index": 0,
             "message": {
                 "role": "assistant"
@@ -50,15 +63,16 @@
   try:
     global new_response
     model_response = deepcopy(new_response) # deep copy the default response format so we can mutate it and it's thread-safe. 
     # check if user passed in any of the OpenAI optional params
     optional_params = get_optional_params(
       functions=functions, function_call=function_call, 
       temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
-      presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user, deployment_id=deployment_id
+      presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user, deployment_id=deployment_id,
+      model=model
     )
     if azure == True:
       # azure configs
       openai.api_type = "azure"
       openai.api_base = litellm.api_base if litellm.api_base is not None else get_secret("AZURE_API_BASE")
       openai.api_version = litellm.api_version if litellm.api_version is not None else get_secret("AZURE_API_VERSION")
       # set key
@@ -218,16 +232,22 @@
         max_tokens_to_sample = litellm.max_tokens # default in Anthropic docs https://docs.anthropic.com/claude/reference/client-libraries
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
       ## COMPLETION CALL
       completion = anthropic.completions.create(
             model=model,
             prompt=prompt,
-            max_tokens_to_sample=max_tokens_to_sample
+            max_tokens_to_sample=max_tokens_to_sample,
+            **optional_params
         )
+      if 'stream' in optional_params and optional_params['stream'] == True:
+        # don't try to access stream object,
+        response = CustomStreamWrapper(completion)
+        return response
+
       completion_response = completion.completion
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
       prompt_tokens = anthropic.count_tokens(prompt)
       completion_tokens = anthropic.count_tokens(completion_response)
       ## RESPONSE OBJECT
       print_verbose(f"raw model_response: {model_response}")
```

### Comparing `litellm-0.1.362/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.363/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.363/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.363/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.363/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.363/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.363/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.363/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_api_key_param.py` & `litellm-0.1.363/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_async_fn.py` & `litellm-0.1.363/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_bad_params.py` & `litellm-0.1.363/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.363/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_client.py` & `litellm-0.1.363/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_completion.py` & `litellm-0.1.363/litellm/tests/test_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,27 @@
     try:
         response = completion(model="claude-instant-1", messages=messages, logger_fn=logger_fn)
         # Add any assertions here to check the response
         print(response)
     except Exception as e:
         pytest.fail(f"Error occurred: {e}")
 
+def test_completion_claude_stream():
+    try:
+        messages = [
+            {"role": "system", "content": "You are a helpful assistant."},
+            {"role": "user", "content": "how does a court case get to the Supreme Court?"}
+        ]
+        response = completion(model="claude-2", messages=messages, stream=True)
+        # Add any assertions here to check the response
+        for chunk in response:
+            print(chunk['choices'][0]['delta']) # same as openai format
+    except Exception as e:
+        pytest.fail(f"Error occurred: {e}")
+
 def test_completion_hf_api():
     try:
         user_message = "write some code to find the sum of two numbers"
         messages = [{ "content": user_message,"role": "user"}]
         response = completion(model="stabilityai/stablecode-completion-alpha-3b-4k", messages=messages, hugging_face=True)
         # Add any assertions here to check the response
         print(response)
```

### Comparing `litellm-0.1.362/litellm/tests/test_embedding.py` & `litellm-0.1.363/litellm/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_exceptions.py` & `litellm-0.1.363/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_helicone_integration.py` & `litellm-0.1.363/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_logging.py` & `litellm-0.1.363/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_model_fallback.py` & `litellm-0.1.363/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_no_client.py` & `litellm-0.1.363/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_secrets.py` & `litellm-0.1.363/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_supabase_integration.py` & `litellm-0.1.363/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/tests/test_timeout.py` & `litellm-0.1.363/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/timeout.py` & `litellm-0.1.363/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.362/litellm/utils.py` & `litellm-0.1.363/litellm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,44 +142,57 @@
     stream = False,
     stop = None,
     max_tokens = float('inf'),
     presence_penalty = 0,
     frequency_penalty = 0,
     logit_bias = {},
     user = "",
-    deployment_id = None
+    deployment_id = None,
+    model = None,
 ):
   optional_params = {}
-  if functions != []:
-      optional_params["functions"] = functions
-  if function_call != "":
-      optional_params["function_call"] = function_call
-  if temperature != 1:
-      optional_params["temperature"] = temperature
-  if top_p != 1:
-      optional_params["top_p"] = top_p
-  if n != 1:
-      optional_params["n"] = n
-  if stream:
+  if model in litellm.anthropic_models:
+    # handle anthropic params
+    if stream:
       optional_params["stream"] = stream
-  if stop != None:
-      optional_params["stop"] = stop
-  if max_tokens != float('inf'):
-      optional_params["max_tokens"] = max_tokens
-  if presence_penalty != 0:
-      optional_params["presence_penalty"] = presence_penalty
-  if frequency_penalty != 0:
-      optional_params["frequency_penalty"] = frequency_penalty
-  if logit_bias != {}:
-      optional_params["logit_bias"] = logit_bias
-  if user != "":
-      optional_params["user"] = user
-  if deployment_id != None:
-      optional_params["deployment_id"] = deployment_id
-  return optional_params
+    if stop != None:
+        optional_params["stop_sequences"] = stop
+    if temperature != 1:
+        optional_params["temperature"] = temperature
+    if top_p != 1:
+        optional_params["top_p"] = top_p
+    return optional_params
+  else:# assume passing in params for openai/azure openai
+    if functions != []:
+        optional_params["functions"] = functions
+    if function_call != "":
+        optional_params["function_call"] = function_call
+    if temperature != 1:
+        optional_params["temperature"] = temperature
+    if top_p != 1:
+        optional_params["top_p"] = top_p
+    if n != 1:
+        optional_params["n"] = n
+    if stream:
+        optional_params["stream"] = stream
+    if stop != None:
+        optional_params["stop"] = stop
+    if max_tokens != float('inf'):
+        optional_params["max_tokens"] = max_tokens
+    if presence_penalty != 0:
+        optional_params["presence_penalty"] = presence_penalty
+    if frequency_penalty != 0:
+        optional_params["frequency_penalty"] = frequency_penalty
+    if logit_bias != {}:
+        optional_params["logit_bias"] = logit_bias
+    if user != "":
+        optional_params["user"] = user
+    if deployment_id != None:
+        optional_params["deployment_id"] = deployment_id
+    return optional_params
 
 def set_callbacks(callback_list):
   global sentry_sdk_instance, capture_exception, add_breadcrumb, posthog, slack_app, alerts_channel, heliconeLogger, aispendLogger, berrispendLogger, supabaseClient
   try:
     for callback in callback_list:
       if callback == "sentry":
         try:
```

### Comparing `litellm-0.1.362/PKG-INFO` & `litellm-0.1.363/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.362
+Version: 0.1.363
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -39,30 +39,28 @@
 ```
 pip install litellm
 ```
 
 ```python
 from litellm import completion
 
-## set ENV variables
-# ENV variables can be set in .env file, too. Example in .env.example
-os.environ["OPENAI_API_KEY"] = "openai key"
-os.environ["COHERE_API_KEY"] = "cohere key"
-
 messages = [{ "content": "Hello, how are you?","role": "user"}]
 
 # openai call
 response = completion(model="gpt-3.5-turbo", messages=messages)
 
 # cohere call
 response = completion("command-nightly", messages)
 
 # azure openai call
 response = completion("chatgpt-test", messages, azure=True)
 
+# hugging face call
+response = completion(model="stabilityai/stablecode-completion-alpha-3b-4k", messages=messages, hugging_face=True)
+
 # openrouter call
 response = completion("google/palm-2-codechat-bison", messages)
 ```
 Code Sample: [Getting Started Notebook](https://colab.research.google.com/drive/1gR3pY-JzDZahzpVdbGBtrNGDBmzUNJaJ?usp=sharing)
 
 Stable version
 ```
```

