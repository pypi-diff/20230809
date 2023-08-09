# Comparing `tmp/litellm-0.1.365.tar.gz` & `tmp/litellm-0.1.366.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.365.tar", max compression
+gzip compressed data, was "litellm-0.1.366.tar", max compression
```

## Comparing `litellm-0.1.365.tar` & `litellm-0.1.366.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0     1065 2023-08-09 00:57:16.297403 litellm-0.1.365/LICENSE
--rw-r--r--   0        0        0     2787 2023-08-09 00:57:16.297403 litellm-0.1.365/README.md
--rw-r--r--   0        0        0     6148 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/.DS_Store
--rw-r--r--   0        0        0     2131 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3556 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    16493 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0     1372 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2592 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_client.py
--rw-r--r--   0        0        0     7033 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_completion.py
--rw-r--r--   0        0        0      658 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_embedding.py
--rw-r--r--   0        0        0     5938 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-09 00:57:16.297403 litellm-0.1.365/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/timeout.py
--rw-r--r--   0        0        0    26566 2023-08-09 00:57:16.301404 litellm-0.1.365/litellm/utils.py
--rw-r--r--   0        0        0      378 2023-08-09 00:57:16.301404 litellm-0.1.365/pyproject.toml
--rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 litellm-0.1.365/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-09 03:50:10.437374 litellm-0.1.366/LICENSE
+-rw-r--r--   0        0        0     2787 2023-08-09 03:50:10.437374 litellm-0.1.366/README.md
+-rw-r--r--   0        0        0     6148 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/.DS_Store
+-rw-r--r--   0        0        0     3893 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3556 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    16493 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0     1372 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2592 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     7033 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0      658 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_embedding.py
+-rw-r--r--   0        0        0     5938 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0     2893 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/timeout.py
+-rw-r--r--   0        0        0    27788 2023-08-09 03:50:10.441374 litellm-0.1.366/litellm/utils.py
+-rw-r--r--   0        0        0      378 2023-08-09 03:50:10.445374 litellm-0.1.366/pyproject.toml
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 litellm-0.1.366/PKG-INFO
```

### Comparing `litellm-0.1.365/LICENSE` & `litellm-0.1.366/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/README.md` & `litellm-0.1.366/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/.DS_Store` & `litellm-0.1.366/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.366/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.366/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.366/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.366/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/integrations/aispend.py` & `litellm-0.1.366/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/integrations/berrispend.py` & `litellm-0.1.366/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/integrations/helicone.py` & `litellm-0.1.366/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/integrations/supabase.py` & `litellm-0.1.366/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/main.py` & `litellm-0.1.366/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.366/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.366/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.366/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.366/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.366/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.366/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.366/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_api_key_param.py` & `litellm-0.1.366/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_async_fn.py` & `litellm-0.1.366/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_bad_params.py` & `litellm-0.1.366/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.366/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_client.py` & `litellm-0.1.366/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_completion.py` & `litellm-0.1.366/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_embedding.py` & `litellm-0.1.366/litellm/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_exceptions.py` & `litellm-0.1.366/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_helicone_integration.py` & `litellm-0.1.366/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_logging.py` & `litellm-0.1.366/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_model_fallback.py` & `litellm-0.1.366/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_no_client.py` & `litellm-0.1.366/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_secrets.py` & `litellm-0.1.366/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_supabase_integration.py` & `litellm-0.1.366/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/tests/test_timeout.py` & `litellm-0.1.366/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/timeout.py` & `litellm-0.1.366/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.365/litellm/utils.py` & `litellm-0.1.366/litellm/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,14 +127,54 @@
           traceback_exception = traceback.format_exc()
           end_time = datetime.datetime.now()
           my_thread = threading.Thread(target=handle_failure, args=(e, traceback_exception, start_time, end_time, args, kwargs)) # don't interrupt execution of main thread
           my_thread.start()
           raise e
     return wrapper
 
+####### USAGE CALCULATOR ################
+
+def prompt_token_calculator(model, messages):
+  # use tiktoken or anthropic's tokenizer depending on the model
+  text = " ".join(message["content"] for message in messages)
+  num_tokens = 0
+  if "claude" in model:
+    install_and_import('anthropic')
+    from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
+    anthropic = Anthropic()
+    num_tokens = anthropic.count_tokens(text)
+  else:
+    num_tokens = len(encoding.encode(text))
+  return num_tokens
+
+
+def cost_per_token(model="gpt-3.5-turbo", prompt_tokens = 0, completion_tokens = 0):
+   ## given 
+  prompt_tokens_cost_usd_dollar = 0
+  completion_tokens_cost_usd_dollar = 0
+  model_cost_ref = litellm.model_cost
+  if model in model_cost_ref:
+    prompt_tokens_cost_usd_dollar = model_cost_ref[model]["input_cost_per_token"] * prompt_tokens
+    completion_tokens_cost_usd_dollar = model_cost_ref[model]["output_cost_per_token"] * completion_tokens
+    return prompt_tokens_cost_usd_dollar, completion_tokens_cost_usd_dollar
+  else:
+    # calculate average input cost 
+    input_cost_sum = 0
+    output_cost_sum = 0
+    model_cost_ref = litellm.model_cost
+    for model in model_cost_ref:
+        input_cost_sum += model_cost_ref[model]["input_cost_per_token"]
+        output_cost_sum += model_cost_ref[model]["output_cost_per_token"]
+    avg_input_cost = input_cost_sum / len(model_cost_ref.keys())
+    avg_output_cost = output_cost_sum / len(model_cost_ref.keys())
+    prompt_tokens_cost_usd_dollar = avg_input_cost * prompt_tokens
+    completion_tokens_cost_usd_dollar = avg_output_cost * completion_tokens
+  return prompt_tokens_cost_usd_dollar, completion_tokens_cost_usd_dollar
+    
+
 ####### HELPER FUNCTIONS ################
 def get_optional_params(
     # 12 optional params
     functions = [],
     function_call = "",
     temperature = 1,
     top_p = 1,
@@ -363,29 +403,14 @@
         failure_handler(call_details)
       pass
     except Exception as e:
       ## LOGGING
       logging(logger_fn=user_logger_fn, exception=e)
       pass
 
-def prompt_token_calculator(model, messages):
-  # use tiktoken or anthropic's tokenizer depending on the model
-  text = " ".join(message["content"] for message in messages)
-  num_tokens = 0
-  if "claude" in model:
-    install_and_import('anthropic')
-    from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
-    anthropic = Anthropic()
-    num_tokens = anthropic.count_tokens(text)
-  else:
-    num_tokens = len(encoding.encode(text))
-  return num_tokens
-  
-      
-
 def handle_success(args, kwargs, result, start_time, end_time):
   global heliconeLogger, aispendLogger
   try:
     success_handler = additional_details.pop("success_handler", None)
     failure_handler = additional_details.pop("failure_handler", None)
     additional_details["Event_Name"] = additional_details.pop("successful_event_name", "litellm.succes_query")
     for callback in litellm.success_callback:
```

### Comparing `litellm-0.1.365/PKG-INFO` & `litellm-0.1.366/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.365
+Version: 0.1.366
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

