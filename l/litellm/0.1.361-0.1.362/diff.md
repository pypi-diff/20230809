# Comparing `tmp/litellm-0.1.361.tar.gz` & `tmp/litellm-0.1.362.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.361.tar", max compression
+gzip compressed data, was "litellm-0.1.362.tar", max compression
```

## Comparing `litellm-0.1.361.tar` & `litellm-0.1.362.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2023-08-08 20:47:32.092622 litellm-0.1.361/LICENSE
--rw-r--r--   0        0        0     2646 2023-08-08 20:47:32.092622 litellm-0.1.361/README.md
--rw-r--r--   0        0        0     6148 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/.DS_Store
--rw-r--r--   0        0        0     2131 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3556 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    15573 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0     1372 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2592 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_client.py
--rw-r--r--   0        0        0     5111 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_completion.py
--rw-r--r--   0        0        0      658 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_embedding.py
--rw-r--r--   0        0        0     5938 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/timeout.py
--rw-r--r--   0        0        0    24462 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/utils.py
--rw-r--r--   0        0        0      378 2023-08-08 20:47:32.096622 litellm-0.1.361/pyproject.toml
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 litellm-0.1.361/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-08 21:01:05.704367 litellm-0.1.362/LICENSE
+-rw-r--r--   0        0        0     2646 2023-08-08 21:01:05.704367 litellm-0.1.362/README.md
+-rw-r--r--   0        0        0     6148 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/.DS_Store
+-rw-r--r--   0        0        0     2131 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3556 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    15605 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0     1372 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2592 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     5111 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0      658 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_embedding.py
+-rw-r--r--   0        0        0     5938 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-08 21:01:05.704367 litellm-0.1.362/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/timeout.py
+-rw-r--r--   0        0        0    24462 2023-08-08 21:01:05.708367 litellm-0.1.362/litellm/utils.py
+-rw-r--r--   0        0        0      378 2023-08-08 21:01:05.708367 litellm-0.1.362/pyproject.toml
+-rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 litellm-0.1.362/PKG-INFO
```

### Comparing `litellm-0.1.361/LICENSE` & `litellm-0.1.362/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/README.md` & `litellm-0.1.362/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/.DS_Store` & `litellm-0.1.362/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/__init__.py` & `litellm-0.1.362/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.362/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.362/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.362/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.362/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/integrations/aispend.py` & `litellm-0.1.362/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/integrations/berrispend.py` & `litellm-0.1.362/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/integrations/helicone.py` & `litellm-0.1.362/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/integrations/supabase.py` & `litellm-0.1.362/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/main.py` & `litellm-0.1.362/litellm/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,15 @@
       model_response["created"] = time.time()
       model_response["model"] = model
       model_response["usage"] = {
           "prompt_tokens": prompt_tokens,
           "completion_tokens": completion_tokens,
           "total_tokens": prompt_tokens + completion_tokens
         }
+      response = model_response
     else: 
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       args = locals()
       raise ValueError(f"No valid completion model args passed in - {args}")
     return response
   except Exception as e:
```

### Comparing `litellm-0.1.361/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.362/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.362/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.362/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.362/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.362/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.362/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.362/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_api_key_param.py` & `litellm-0.1.362/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_async_fn.py` & `litellm-0.1.362/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_bad_params.py` & `litellm-0.1.362/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.362/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_client.py` & `litellm-0.1.362/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_completion.py` & `litellm-0.1.362/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_embedding.py` & `litellm-0.1.362/litellm/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_exceptions.py` & `litellm-0.1.362/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_helicone_integration.py` & `litellm-0.1.362/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_logging.py` & `litellm-0.1.362/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_model_fallback.py` & `litellm-0.1.362/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_no_client.py` & `litellm-0.1.362/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_secrets.py` & `litellm-0.1.362/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_supabase_integration.py` & `litellm-0.1.362/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/tests/test_timeout.py` & `litellm-0.1.362/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/timeout.py` & `litellm-0.1.362/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/litellm/utils.py` & `litellm-0.1.362/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.361/PKG-INFO` & `litellm-0.1.362/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.361
+Version: 0.1.362
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

