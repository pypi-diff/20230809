# Comparing `tmp/litellm-0.1.363.tar.gz` & `tmp/litellm-0.1.364.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.363.tar", max compression
+gzip compressed data, was "litellm-0.1.364.tar", max compression
```

## Comparing `litellm-0.1.363.tar` & `litellm-0.1.364.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2023-08-08 23:12:54.154482 litellm-0.1.363/LICENSE
--rw-r--r--   0        0        0     2602 2023-08-08 23:12:54.154482 litellm-0.1.363/README.md
--rw-r--r--   0        0        0     6148 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/.DS_Store
--rw-r--r--   0        0        0     2131 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3556 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    16220 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0     1372 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2592 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_client.py
--rw-r--r--   0        0        0     5665 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_completion.py
--rw-r--r--   0        0        0      658 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_embedding.py
--rw-r--r--   0        0        0     5938 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-08 23:12:54.158483 litellm-0.1.363/litellm/timeout.py
--rw-r--r--   0        0        0    24954 2023-08-08 23:12:54.162483 litellm-0.1.363/litellm/utils.py
--rw-r--r--   0        0        0      378 2023-08-08 23:12:54.162483 litellm-0.1.363/pyproject.toml
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 litellm-0.1.363/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-09 00:05:03.734609 litellm-0.1.364/LICENSE
+-rw-r--r--   0        0        0     2787 2023-08-09 00:05:03.734609 litellm-0.1.364/README.md
+-rw-r--r--   0        0        0     6148 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/.DS_Store
+-rw-r--r--   0        0        0     2131 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3556 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-09 00:05:03.734609 litellm-0.1.364/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    16894 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0     1372 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2592 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     6242 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0      658 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_embedding.py
+-rw-r--r--   0        0        0     5938 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/timeout.py
+-rw-r--r--   0        0        0    25269 2023-08-09 00:05:03.738609 litellm-0.1.364/litellm/utils.py
+-rw-r--r--   0        0        0      378 2023-08-09 00:05:03.738609 litellm-0.1.364/pyproject.toml
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 litellm-0.1.364/PKG-INFO
```

### Comparing `litellm-0.1.363/LICENSE` & `litellm-0.1.364/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/README.md` & `litellm-0.1.364/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,24 @@
 Stable version
 ```
 pip install litellm==0.1.345
 ```
 
 ## Streaming Queries
 liteLLM supports streaming the model response back, pass `stream=True` to get a streaming iterator in response.
+Streaming is supported for OpenAI, Azure, Anthropic models
 ```python
 response = completion(model="gpt-3.5-turbo", messages=messages, stream=True)
 for chunk in response:
     print(chunk['choices'][0]['delta'])
+
+# claude 2
+result = completion('claude-2', messages, stream=True)
+for chunk in result:
+  print(chunk['choices'][0]['delta'])
 ```
 
 # hosted version
 - [Grab time if you want access 👋](https://calendly.com/d/4mp-gd3-k5k/berriai-1-1-onboarding-litellm-hosted-version)
 
 # why did we build this 
 - **Need for simplicity**: Our code started to get extremely complicated managing & translating calls between Azure, OpenAI, Cohere
```

### Comparing `litellm-0.1.363/litellm/.DS_Store` & `litellm-0.1.364/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/__init__.py` & `litellm-0.1.364/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.364/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.364/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.364/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.364/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/integrations/aispend.py` & `litellm-0.1.364/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/integrations/berrispend.py` & `litellm-0.1.364/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/integrations/helicone.py` & `litellm-0.1.364/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/integrations/supabase.py` & `litellm-0.1.364/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/main.py` & `litellm-0.1.364/litellm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,32 @@
 from litellm.utils import get_secret, install_and_import
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 
 # TODO this will evolve to accepting models
 # replicate/anthropic/cohere
 class CustomStreamWrapper:
-    def __init__(self, completion_stream):
-        self.completion_stream = completion_stream
+    def __init__(self, completion_stream, model):
+        self.model = model
+        if model in litellm.cohere_models:
+           # cohere does not return an iterator, so we need to wrap it in one
+           self.completion_stream = iter(completion_stream)
+        else: 
+          self.completion_stream = completion_stream
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        chunk = next(self.completion_stream)
-        return {"choices": [{"delta": chunk.completion}]}
+        if self.model in litellm.anthropic_models:
+          chunk = next(self.completion_stream)
+          return {"choices": [{"delta": chunk.completion}]}
+        elif self.model in litellm.cohere_models:
+          chunk = next(self.completion_stream)
+          return {"choices": [{"delta": chunk.text}]}
 
 new_response = {
         "choices": [
           {
             "finish_reason": "stop",
             "index": 0,
             "message": {
@@ -237,15 +246,15 @@
             model=model,
             prompt=prompt,
             max_tokens_to_sample=max_tokens_to_sample,
             **optional_params
         )
       if 'stream' in optional_params and optional_params['stream'] == True:
         # don't try to access stream object,
-        response = CustomStreamWrapper(completion)
+        response = CustomStreamWrapper(completion, model)
         return response
 
       completion_response = completion.completion
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
       prompt_tokens = anthropic.count_tokens(prompt)
       completion_tokens = anthropic.count_tokens(completion_response)
@@ -273,16 +282,22 @@
       co = cohere.Client(cohere_key)
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       response = co.generate(  
         model=model,
-        prompt = prompt
+        prompt = prompt,
+        **optional_params
       )
+      if 'stream' in optional_params and optional_params['stream'] == True:
+        # don't try to access stream object,
+        response = CustomStreamWrapper(response, model)
+        return response
+
       completion_response = response[0].text
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
       prompt_tokens = len(encoding.encode(prompt))
       completion_tokens = len(encoding.encode(completion_response))
       ## RESPONSE OBJECT
       model_response["choices"][0]["message"]["content"] = completion_response
```

### Comparing `litellm-0.1.363/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.364/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.364/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.364/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.364/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.364/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.364/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.364/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_api_key_param.py` & `litellm-0.1.364/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_async_fn.py` & `litellm-0.1.364/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_bad_params.py` & `litellm-0.1.364/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.364/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_client.py` & `litellm-0.1.364/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_completion.py` & `litellm-0.1.364/litellm/tests/test_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,28 @@
     try:
         response = completion(model="command-nightly", messages=messages, max_tokens=500)
         # Add any assertions here to check the response
         print(response)
     except Exception as e:
         pytest.fail(f"Error occurred: {e}")
 
+
+def test_completion_cohere_stream():
+    try:
+        messages = [
+            {"role": "system", "content": "You are a helpful assistant."},
+            {"role": "user", "content": "how does a court case get to the Supreme Court?"}
+        ]
+        response = completion(model="command-nightly", messages=messages, stream=True, max_tokens=50)
+        # Add any assertions here to check the response
+        for chunk in response:
+            print(chunk['choices'][0]['delta']) # same as openai format
+    except Exception as e:
+        pytest.fail(f"Error occurred: {e}")
+
 def test_completion_openai():
     try:
         response = completion(model="gpt-3.5-turbo", messages=messages)
         # Add any assertions here to check the response
         print(response)
     except Exception as e:
         pytest.fail(f"Error occurred: {e}")
```

### Comparing `litellm-0.1.363/litellm/tests/test_embedding.py` & `litellm-0.1.364/litellm/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_exceptions.py` & `litellm-0.1.364/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_helicone_integration.py` & `litellm-0.1.364/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_logging.py` & `litellm-0.1.364/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_model_fallback.py` & `litellm-0.1.364/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_no_client.py` & `litellm-0.1.364/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_secrets.py` & `litellm-0.1.364/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_supabase_integration.py` & `litellm-0.1.364/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/tests/test_timeout.py` & `litellm-0.1.364/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/timeout.py` & `litellm-0.1.364/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.363/litellm/utils.py` & `litellm-0.1.364/litellm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,24 @@
     if stop != None:
         optional_params["stop_sequences"] = stop
     if temperature != 1:
         optional_params["temperature"] = temperature
     if top_p != 1:
         optional_params["top_p"] = top_p
     return optional_params
+  elif model in litellm.cohere_models:
+     # handle cohere params
+    if stream:
+      optional_params["stream"] = stream
+    if temperature != 1:
+        optional_params["temperature"] = temperature
+    if max_tokens != float('inf'):
+        optional_params["max_tokens"] = max_tokens
+    return optional_params
+
   else:# assume passing in params for openai/azure openai
     if functions != []:
         optional_params["functions"] = functions
     if function_call != "":
         optional_params["function_call"] = function_call
     if temperature != 1:
         optional_params["temperature"] = temperature
```

### Comparing `litellm-0.1.363/PKG-INFO` & `litellm-0.1.364/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.363
+Version: 0.1.364
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -65,18 +65,24 @@
 Stable version
 ```
 pip install litellm==0.1.345
 ```
 
 ## Streaming Queries
 liteLLM supports streaming the model response back, pass `stream=True` to get a streaming iterator in response.
+Streaming is supported for OpenAI, Azure, Anthropic models
 ```python
 response = completion(model="gpt-3.5-turbo", messages=messages, stream=True)
 for chunk in response:
     print(chunk['choices'][0]['delta'])
+
+# claude 2
+result = completion('claude-2', messages, stream=True)
+for chunk in result:
+  print(chunk['choices'][0]['delta'])
 ```
 
 # hosted version
 - [Grab time if you want access 👋](https://calendly.com/d/4mp-gd3-k5k/berriai-1-1-onboarding-litellm-hosted-version)
 
 # why did we build this 
 - **Need for simplicity**: Our code started to get extremely complicated managing & translating calls between Azure, OpenAI, Cohere
```

