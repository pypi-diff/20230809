# Comparing `tmp/llmx-0.0.6a0.tar.gz` & `tmp/llmx-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmx-0.0.6a0.tar", last modified: Sat Aug  5 01:08:49 2023, max compression
+gzip compressed data, was "llmx-0.0.7a0.tar", last modified: Tue Aug  8 22:13:02 2023, max compression
```

## Comparing `llmx-0.0.6a0.tar` & `llmx-0.0.7a0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3170 2023-08-03 03:11:18.000000 llmx-0.0.6a0/.gitignore
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1083 2023-08-04 04:13:34.000000 llmx-0.0.6a0/LICENSE
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       27 2023-08-02 21:17:22.000000 llmx-0.0.6a0/MANIFEST.in
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6762 2023-08-05 01:08:49.743155 llmx-0.0.6a0/PKG-INFO
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4948 2023-08-04 16:57:35.000000 llmx-0.0.6a0/README.md
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/llmx/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      185 2023-08-02 22:29:16.000000 llmx-0.0.6a0/llmx/__init__.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1322 2023-08-04 03:49:25.000000 llmx-0.0.6a0/llmx/datamodel.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/llmx/generators/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      128 2023-08-02 22:29:06.000000 llmx-0.0.6a0/llmx/generators/__init__.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/llmx/generators/text/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-02 20:54:42.000000 llmx-0.0.6a0/llmx/generators/text/__init__.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1063 2023-08-02 23:44:59.000000 llmx-0.0.6a0/llmx/generators/text/base_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2865 2023-08-02 23:47:07.000000 llmx-0.0.6a0/llmx/generators/text/cohere_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     8497 2023-08-02 23:46:52.000000 llmx-0.0.6a0/llmx/generators/text/hf_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2728 2023-08-02 23:46:09.000000 llmx-0.0.6a0/llmx/generators/text/openai_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4110 2023-08-04 21:13:28.000000 llmx-0.0.6a0/llmx/generators/text/palm_textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1561 2023-08-04 18:29:17.000000 llmx-0.0.6a0/llmx/generators/text/textgen.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4369 2023-08-04 20:18:07.000000 llmx-0.0.6a0/llmx/utils.py
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       37 2023-08-05 01:08:42.000000 llmx-0.0.6a0/llmx/version.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/llmx.egg-info/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6762 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/PKG-INFO
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      670 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/SOURCES.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/dependency_links.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/entry_points.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      119 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/requires.txt
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        5 2023-08-05 01:08:49.000000 llmx-0.0.6a0/llmx.egg-info/top_level.txt
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/notebooks/
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/notebooks/research/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      775 2023-08-01 22:45:11.000000 llmx-0.0.6a0/notebooks/research/travelbenchmark.ipynb
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3669 2023-08-04 14:18:45.000000 llmx-0.0.6a0/notebooks/tutorial.ipynb
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1384 2023-08-04 14:14:13.000000 llmx-0.0.6a0/pyproject.toml
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-05 01:08:49.743155 llmx-0.0.6a0/setup.cfg
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-01 22:45:11.000000 llmx-0.0.6a0/setup.py
-drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-05 01:08:49.743155 llmx-0.0.6a0/tests/
--rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1936 2023-08-05 01:07:46.000000 llmx-0.0.6a0/tests/test_generators.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-08 22:13:02.841908 llmx-0.0.7a0/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3170 2023-08-03 03:11:18.000000 llmx-0.0.7a0/.gitignore
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1083 2023-08-04 04:13:34.000000 llmx-0.0.7a0/LICENSE
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       27 2023-08-02 21:17:22.000000 llmx-0.0.7a0/MANIFEST.in
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     7099 2023-08-08 22:13:02.841908 llmx-0.0.7a0/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     5285 2023-08-08 22:08:45.000000 llmx-0.0.7a0/README.md
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-08 22:13:02.837908 llmx-0.0.7a0/llmx/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      271 2023-08-08 20:50:55.000000 llmx-0.0.7a0/llmx/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1322 2023-08-04 03:49:25.000000 llmx-0.0.7a0/llmx/datamodel.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-08 22:13:02.837908 llmx-0.0.7a0/llmx/generators/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      117 2023-08-08 20:51:06.000000 llmx-0.0.7a0/llmx/generators/__init__.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-08 22:13:02.837908 llmx-0.0.7a0/llmx/generators/text/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       25 2023-08-08 20:49:12.000000 llmx-0.0.7a0/llmx/generators/text/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1063 2023-08-02 23:44:59.000000 llmx-0.0.7a0/llmx/generators/text/base_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2865 2023-08-02 23:47:07.000000 llmx-0.0.7a0/llmx/generators/text/cohere_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     8509 2023-08-05 22:58:16.000000 llmx-0.0.7a0/llmx/generators/text/hf_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2728 2023-08-02 23:46:09.000000 llmx-0.0.7a0/llmx/generators/text/openai_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4112 2023-08-05 23:18:07.000000 llmx-0.0.7a0/llmx/generators/text/palm_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1550 2023-08-08 20:49:04.000000 llmx-0.0.7a0/llmx/generators/text/textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4380 2023-08-05 23:23:51.000000 llmx-0.0.7a0/llmx/utils.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       37 2023-08-08 22:12:49.000000 llmx-0.0.7a0/llmx/version.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-08 22:13:02.837908 llmx-0.0.7a0/llmx.egg-info/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     7099 2023-08-08 22:13:02.000000 llmx-0.0.7a0/llmx.egg-info/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      670 2023-08-08 22:13:02.000000 llmx-0.0.7a0/llmx.egg-info/SOURCES.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-08-08 22:13:02.000000 llmx-0.0.7a0/llmx.egg-info/dependency_links.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-08 22:13:02.000000 llmx-0.0.7a0/llmx.egg-info/entry_points.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      119 2023-08-08 22:13:02.000000 llmx-0.0.7a0/llmx.egg-info/requires.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        5 2023-08-08 22:13:02.000000 llmx-0.0.7a0/llmx.egg-info/top_level.txt
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-08 22:13:02.837908 llmx-0.0.7a0/notebooks/
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-08 22:13:02.837908 llmx-0.0.7a0/notebooks/research/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      775 2023-08-01 22:45:11.000000 llmx-0.0.7a0/notebooks/research/travelbenchmark.ipynb
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     5296 2023-08-08 20:53:25.000000 llmx-0.0.7a0/notebooks/tutorial.ipynb
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1384 2023-08-04 14:14:13.000000 llmx-0.0.7a0/pyproject.toml
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-08 22:13:02.841908 llmx-0.0.7a0/setup.cfg
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-01 22:45:11.000000 llmx-0.0.7a0/setup.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-08 22:13:02.841908 llmx-0.0.7a0/tests/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1955 2023-08-08 20:59:34.000000 llmx-0.0.7a0/tests/test_generators.py
```

### Comparing `llmx-0.0.6a0/.gitignore` & `llmx-0.0.7a0/.gitignore`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/LICENSE` & `llmx-0.0.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/PKG-INFO` & `llmx-0.0.7a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmx
-Version: 0.0.6a0
+Version: 0.0.7a0
 Summary: LLMX: A library for LLM Text Generation
 Author-email: Victor Dibia <victor.dibia@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) <year> Adam Veldhousen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,34 +31,37 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: web
 Provides-Extra: transformers
 License-File: LICENSE
 
-# LLMX - An API for Language Models
+# LLMX - An API for Chat Fine-Tuned Language Models
 
 [![PyPI version](https://badge.fury.io/py/llmx.svg)](https://badge.fury.io/py/llmx)
 
-A simple python package that provides a unified interface to several LLM providers [ OpenAI (default), PaLM, Cohere and local HuggingFace Models ].
+A simple python package that provides a unified interface to several LLM providers of chat fine-tuned models [OpenAI (default), PaLM, Cohere and local HuggingFace Models].
 
-There is nothing special about this library, but some of the requirements I needed when I startec building this (that other libraries did not have):
+> **Note**
+> LLMx wraps multiple api providers and its interface _may_ change as the providers as well as the general field of LLMs evolve.
+
+There is nothing particularly special about this library, but some of the requirements I needed when I started building this (that other libraries did not have):
 
 - **Unified Model Interface**: Single interface to create LLM text generators with support for **multiple LLM providers**.
 
 ```python
-from llmx import  text_generator as generator
+from llmx import  llm
 
-openai_generator = generator(provider="openai")
-palm_generator = generator(provider="google") # or palm
-cohere_generator = generator(provider="cohere") # or palm
-hf_generator = generator(provider="huggingface") # run locally
+gen = llm(provider="openai") # openai is default
+gen = llm(provider="google") # or palm
+gen = llm(provider="cohere") # or palm
+gen = llm(provider="hf", model="TheBloke/Llama-2-7b-chat-fp16", device_map="auto") # run huggingface model locally
 ```
 
-- **Unified Messaging Interface**. Standardizes on the OpenAI ChatML format. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content of the form. A single request is list one only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. For all models.
+- **Unified Messaging Interface**. Standardizes on the OpenAI ChatML message format and is designed for _chat finetuned_ models. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content (see below). A single request is list of only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. Same format for all models.
 
 ```python
 messages = [
     {"role": "user", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
     {"role": "user", "content": "What is  gravity?"}
 ]
 ```
@@ -77,15 +80,15 @@
 
 ```
 
 Are there other libraries that do things like this really well? Yes! I'd recommend looking at [guidance](https://github.com/microsoft/guidance) which does a lot more. Interested in optimized inference? Try somthing like [vllm](https://github.com/vllm-project/vllm).
 
 ## Installation
 
-Install from pypi. Please use python3.9 or higher.
+Install from pypi. Please use **python3.10** or higher.
 
 ```bash
 pip install llmx
 ```
 
 Install in development mode
 
@@ -99,34 +102,34 @@
 `python3 -m pip install --upgrade pip`
 
 ## Usage
 
 Set your api keys first for each service.
 
 ```bash
+# for openai and cohere
 export OPENAI_API_KEY=<your key>
-export PALM_API_KEY=<your key>
 export COHERE_API_KEY=<your key>
 
-# for palm ..
+# for PaLM (Vertex AI), setup a gcp project, and get a service account key file
 export PALM_SERVICE_ACCOUNT_KEY_FILE= <path to your service account key file>
 export PALM_PROJECT_ID=<your gcp project id>
 export PALM_PROJECT_LOCATION=<your project location>
 ```
 
 ```python
-from llmx import  text_generator as generator
+from llmx import llm
 from llmx.datamodel import TextGenerationConfig
 
-messages =  messages = [
+messages = [
     {"role": "system", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
     {"role": "user", "content": "What is  gravity?"}
 ]
 
-openai_gen = generator(provider="openai")
+openai_gen = llm(provider="openai")
 openai_config = TextGenerationConfig(model="gpt-4", max_tokens=50)
 openai_response = openai_gen.generate(messages, config=openai_config, use_cache=True)
 print(openai_response.text[0].content)
 
 ```
 
 See the [tutorial](/notebooks/tutorial.ipynb) for more examples.
@@ -138,23 +141,23 @@
   - [x] PaLM
   - [x] Cohere
   - [x] HuggingFace (local)
 
 ## Caveats
 
 - **Prompting**. llmx makes some assumptions around how prompts are constructed e.g., how the chat message interface is assembled into a prompt for each model type. If your application or use case requires more control over the prompt, you may want to use a different library (ideally query the LLM models directly).
-- **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference, I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
+- **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference (tensor parrelization, distributed inference etc), I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
 
 ## Citation
 
 If you use this library in your work, please cite:
 
 ```bibtex
 @software{victordibiallmx,
 author = {Victor Dibia},
 license = {MIT},
 month =  {10},
-title = {LLMX - An API for Language Models},
+title = {LLMX - An API for Chat Fine-Tuned Language Models},
 url = {https://github.com/victordibia/llmx},
 year = {2023}
 }
 ```
```

### Comparing `llmx-0.0.6a0/README.md` & `llmx-0.0.7a0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-# LLMX - An API for Language Models
+# LLMX - An API for Chat Fine-Tuned Language Models
 
 [![PyPI version](https://badge.fury.io/py/llmx.svg)](https://badge.fury.io/py/llmx)
 
-A simple python package that provides a unified interface to several LLM providers [ OpenAI (default), PaLM, Cohere and local HuggingFace Models ].
+A simple python package that provides a unified interface to several LLM providers of chat fine-tuned models [OpenAI (default), PaLM, Cohere and local HuggingFace Models].
 
-There is nothing special about this library, but some of the requirements I needed when I startec building this (that other libraries did not have):
+> **Note**
+> LLMx wraps multiple api providers and its interface _may_ change as the providers as well as the general field of LLMs evolve.
+
+There is nothing particularly special about this library, but some of the requirements I needed when I started building this (that other libraries did not have):
 
 - **Unified Model Interface**: Single interface to create LLM text generators with support for **multiple LLM providers**.
 
 ```python
-from llmx import  text_generator as generator
+from llmx import  llm
 
-openai_generator = generator(provider="openai")
-palm_generator = generator(provider="google") # or palm
-cohere_generator = generator(provider="cohere") # or palm
-hf_generator = generator(provider="huggingface") # run locally
+gen = llm(provider="openai") # openai is default
+gen = llm(provider="google") # or palm
+gen = llm(provider="cohere") # or palm
+gen = llm(provider="hf", model="TheBloke/Llama-2-7b-chat-fp16", device_map="auto") # run huggingface model locally
 ```
 
-- **Unified Messaging Interface**. Standardizes on the OpenAI ChatML format. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content of the form. A single request is list one only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. For all models.
+- **Unified Messaging Interface**. Standardizes on the OpenAI ChatML message format and is designed for _chat finetuned_ models. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content (see below). A single request is list of only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. Same format for all models.
 
 ```python
 messages = [
     {"role": "user", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
     {"role": "user", "content": "What is  gravity?"}
 ]
 ```
@@ -40,15 +43,15 @@
 
 ```
 
 Are there other libraries that do things like this really well? Yes! I'd recommend looking at [guidance](https://github.com/microsoft/guidance) which does a lot more. Interested in optimized inference? Try somthing like [vllm](https://github.com/vllm-project/vllm).
 
 ## Installation
 
-Install from pypi. Please use python3.9 or higher.
+Install from pypi. Please use **python3.10** or higher.
 
 ```bash
 pip install llmx
 ```
 
 Install in development mode
 
@@ -62,34 +65,34 @@
 `python3 -m pip install --upgrade pip`
 
 ## Usage
 
 Set your api keys first for each service.
 
 ```bash
+# for openai and cohere
 export OPENAI_API_KEY=<your key>
-export PALM_API_KEY=<your key>
 export COHERE_API_KEY=<your key>
 
-# for palm ..
+# for PaLM (Vertex AI), setup a gcp project, and get a service account key file
 export PALM_SERVICE_ACCOUNT_KEY_FILE= <path to your service account key file>
 export PALM_PROJECT_ID=<your gcp project id>
 export PALM_PROJECT_LOCATION=<your project location>
 ```
 
 ```python
-from llmx import  text_generator as generator
+from llmx import llm
 from llmx.datamodel import TextGenerationConfig
 
-messages =  messages = [
+messages = [
     {"role": "system", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
     {"role": "user", "content": "What is  gravity?"}
 ]
 
-openai_gen = generator(provider="openai")
+openai_gen = llm(provider="openai")
 openai_config = TextGenerationConfig(model="gpt-4", max_tokens=50)
 openai_response = openai_gen.generate(messages, config=openai_config, use_cache=True)
 print(openai_response.text[0].content)
 
 ```
 
 See the [tutorial](/notebooks/tutorial.ipynb) for more examples.
@@ -101,23 +104,23 @@
   - [x] PaLM
   - [x] Cohere
   - [x] HuggingFace (local)
 
 ## Caveats
 
 - **Prompting**. llmx makes some assumptions around how prompts are constructed e.g., how the chat message interface is assembled into a prompt for each model type. If your application or use case requires more control over the prompt, you may want to use a different library (ideally query the LLM models directly).
-- **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference, I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
+- **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference (tensor parrelization, distributed inference etc), I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
 
 ## Citation
 
 If you use this library in your work, please cite:
 
 ```bibtex
 @software{victordibiallmx,
 author = {Victor Dibia},
 license = {MIT},
 month =  {10},
-title = {LLMX - An API for Language Models},
+title = {LLMX - An API for Chat Fine-Tuned Language Models},
 url = {https://github.com/victordibia/llmx},
 year = {2023}
 }
 ```
```

### Comparing `llmx-0.0.6a0/llmx/datamodel.py` & `llmx-0.0.7a0/llmx/datamodel.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/llmx/generators/text/base_textgen.py` & `llmx-0.0.7a0/llmx/generators/text/base_textgen.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/llmx/generators/text/cohere_textgen.py` & `llmx-0.0.7a0/llmx/generators/text/cohere_textgen.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/llmx/generators/text/hf_textgen.py` & `llmx-0.0.7a0/llmx/generators/text/hf_textgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,20 +173,20 @@
             prompt, return_tensors="pt", return_token_type_ids=False
         ).to(self.model.device)
         input_ids = batch["input_ids"]
 
         max_new_tokens = kwargs.get(
             "max_new_tokens", self.max_context_tokens - input_ids.shape[-1]
         )
-        print(
-            "Prompt tokens: ",
-            input_ids.shape[-1],
-            " | Max new tokens: ",
-            max_new_tokens,
-        )
+        # print(
+        #     "Prompt tokens: ",
+        #     input_ids.shape[-1],
+        #     " | Max new tokens: ",
+        #     max_new_tokens,
+        # )
 
         top_k = kwargs.get("top_k", config.top_k)
         min_new_tokens = kwargs.get("min_new_tokens", 32)
         repetition_penalty = kwargs.get("repetition_penalty", 1.0)
 
         gen_config = GenerationConfig(
             max_new_tokens=max_new_tokens,
```

### Comparing `llmx-0.0.6a0/llmx/generators/text/openai_textgen.py` & `llmx-0.0.7a0/llmx/generators/text/openai_textgen.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/llmx/generators/text/palm_textgen.py` & `llmx-0.0.7a0/llmx/generators/text/palm_textgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             **kwargs) -> TextGenerationResponse:
 
         use_cache = config.use_cache
         model = config.model or "codechat-bison"
         system_messages, messages = self.format_messages(messages)
         self.model_name = model
 
-        print("*********", messages)
+        # print("*********", messages)
 
         api_url = f"https://us-central1-aiplatform.googleapis.com/v1/projects/{self.project_id}/locations/{self.project_location}/publishers/google/models/{model}:predict"
 
 #  'candidateCount': max(1, min(8, config.n)),  # 1 <= n <= 8,
 # 'topP': config.top_p,
 #                 'topK': config.top_k,
```

### Comparing `llmx-0.0.6a0/llmx/generators/text/textgen.py` & `llmx-0.0.7a0/llmx/generators/text/textgen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .openai_textgen import OpenAITextGenerator
 from .palm_textgen import PalmTextGenerator
 from .cohere_textgen import CohereTextGenerator
 
 
-def text_generator(provider: str = "openai", **kwargs):
+def llm(provider: str = "openai", **kwargs):
     if provider.lower() == "openai" or provider.lower() == "default":
         return OpenAITextGenerator(**kwargs)
     elif provider.lower() == "palm" or provider.lower() == "google":
         return PalmTextGenerator(provider=provider, **kwargs)
     elif provider.lower() == "cohere":
         return CohereTextGenerator(provider=provider, **kwargs)
     elif provider.lower() == "hf" or provider.lower() == "huggingface":
```

### Comparing `llmx-0.0.6a0/llmx/utils.py` & `llmx-0.0.7a0/llmx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import asdict
+import sys
 import logging
 import json
 from typing import Any
 import tiktoken
 from diskcache import Cache
 import hashlib
 import os
```

### Comparing `llmx-0.0.6a0/llmx.egg-info/PKG-INFO` & `llmx-0.0.7a0/llmx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmx
-Version: 0.0.6a0
+Version: 0.0.7a0
 Summary: LLMX: A library for LLM Text Generation
 Author-email: Victor Dibia <victor.dibia@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) <year> Adam Veldhousen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,34 +31,37 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: web
 Provides-Extra: transformers
 License-File: LICENSE
 
-# LLMX - An API for Language Models
+# LLMX - An API for Chat Fine-Tuned Language Models
 
 [![PyPI version](https://badge.fury.io/py/llmx.svg)](https://badge.fury.io/py/llmx)
 
-A simple python package that provides a unified interface to several LLM providers [ OpenAI (default), PaLM, Cohere and local HuggingFace Models ].
+A simple python package that provides a unified interface to several LLM providers of chat fine-tuned models [OpenAI (default), PaLM, Cohere and local HuggingFace Models].
 
-There is nothing special about this library, but some of the requirements I needed when I startec building this (that other libraries did not have):
+> **Note**
+> LLMx wraps multiple api providers and its interface _may_ change as the providers as well as the general field of LLMs evolve.
+
+There is nothing particularly special about this library, but some of the requirements I needed when I started building this (that other libraries did not have):
 
 - **Unified Model Interface**: Single interface to create LLM text generators with support for **multiple LLM providers**.
 
 ```python
-from llmx import  text_generator as generator
+from llmx import  llm
 
-openai_generator = generator(provider="openai")
-palm_generator = generator(provider="google") # or palm
-cohere_generator = generator(provider="cohere") # or palm
-hf_generator = generator(provider="huggingface") # run locally
+gen = llm(provider="openai") # openai is default
+gen = llm(provider="google") # or palm
+gen = llm(provider="cohere") # or palm
+gen = llm(provider="hf", model="TheBloke/Llama-2-7b-chat-fp16", device_map="auto") # run huggingface model locally
 ```
 
-- **Unified Messaging Interface**. Standardizes on the OpenAI ChatML format. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content of the form. A single request is list one only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. For all models.
+- **Unified Messaging Interface**. Standardizes on the OpenAI ChatML message format and is designed for _chat finetuned_ models. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content (see below). A single request is list of only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. Same format for all models.
 
 ```python
 messages = [
     {"role": "user", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
     {"role": "user", "content": "What is  gravity?"}
 ]
 ```
@@ -77,15 +80,15 @@
 
 ```
 
 Are there other libraries that do things like this really well? Yes! I'd recommend looking at [guidance](https://github.com/microsoft/guidance) which does a lot more. Interested in optimized inference? Try somthing like [vllm](https://github.com/vllm-project/vllm).
 
 ## Installation
 
-Install from pypi. Please use python3.9 or higher.
+Install from pypi. Please use **python3.10** or higher.
 
 ```bash
 pip install llmx
 ```
 
 Install in development mode
 
@@ -99,34 +102,34 @@
 `python3 -m pip install --upgrade pip`
 
 ## Usage
 
 Set your api keys first for each service.
 
 ```bash
+# for openai and cohere
 export OPENAI_API_KEY=<your key>
-export PALM_API_KEY=<your key>
 export COHERE_API_KEY=<your key>
 
-# for palm ..
+# for PaLM (Vertex AI), setup a gcp project, and get a service account key file
 export PALM_SERVICE_ACCOUNT_KEY_FILE= <path to your service account key file>
 export PALM_PROJECT_ID=<your gcp project id>
 export PALM_PROJECT_LOCATION=<your project location>
 ```
 
 ```python
-from llmx import  text_generator as generator
+from llmx import llm
 from llmx.datamodel import TextGenerationConfig
 
-messages =  messages = [
+messages = [
     {"role": "system", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
     {"role": "user", "content": "What is  gravity?"}
 ]
 
-openai_gen = generator(provider="openai")
+openai_gen = llm(provider="openai")
 openai_config = TextGenerationConfig(model="gpt-4", max_tokens=50)
 openai_response = openai_gen.generate(messages, config=openai_config, use_cache=True)
 print(openai_response.text[0].content)
 
 ```
 
 See the [tutorial](/notebooks/tutorial.ipynb) for more examples.
@@ -138,23 +141,23 @@
   - [x] PaLM
   - [x] Cohere
   - [x] HuggingFace (local)
 
 ## Caveats
 
 - **Prompting**. llmx makes some assumptions around how prompts are constructed e.g., how the chat message interface is assembled into a prompt for each model type. If your application or use case requires more control over the prompt, you may want to use a different library (ideally query the LLM models directly).
-- **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference, I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
+- **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference (tensor parrelization, distributed inference etc), I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
 
 ## Citation
 
 If you use this library in your work, please cite:
 
 ```bibtex
 @software{victordibiallmx,
 author = {Victor Dibia},
 license = {MIT},
 month =  {10},
-title = {LLMX - An API for Language Models},
+title = {LLMX - An API for Chat Fine-Tuned Language Models},
 url = {https://github.com/victordibia/llmx},
 year = {2023}
 }
 ```
```

### Comparing `llmx-0.0.6a0/llmx.egg-info/SOURCES.txt` & `llmx-0.0.7a0/llmx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/notebooks/research/travelbenchmark.ipynb` & `llmx-0.0.7a0/notebooks/research/travelbenchmark.ipynb`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/notebooks/tutorial.ipynb` & `llmx-0.0.7a0/notebooks/tutorial.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9701318027210885%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'source': {insert: [(0, 'from llmx import  llm\\n')], "*

 * *            "delete: [0]}}, 1: {'execution_count': 2, 'source': {insert: [(9, 'messages = [\\n')], "*

 * *            'delete: [9]}}, 4: {\'outputs\': {0: {\'text\': ["Gravity is a force that pulls things '*

 * *            "down to Earth. It's what makes things fall down when you drop them, and it's what "*

 * *            "keeps the moon in orbit around the Earth. Gravity is a very strong force, but it's "*

 * *            'also\\ […]*

```diff
@@ -1,35 +1,35 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from llmx import  text_generator as generator\n",
+                "from llmx import  llm\n",
                 "from llmx.datamodel import TextGenerationConfig"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "config = TextGenerationConfig( \n",
                 "    n=1,\n",
                 "    temperature=0.8,\n",
                 "    max_tokens=100,\n",
                 "    top_p=1.0,\n",
                 "    top_k=50,\n",
                 "    frequency_penalty=0.0,\n",
                 "    presence_penalty=0.0,\n",
                 ")\n",
-                "messages =  messages = [\n",
+                "messages = [\n",
                 "    {\"role\": \"system\", \"content\": \"You are a helpful assistant that can explain concepts clearly to a 6 year old child.\"},\n",
                 "    {\"role\": \"user\", \"content\": \"What is  gravity?\"}\n",
                 "]"
             ]
         },
         {
             "attachments": {},
@@ -37,71 +37,100 @@
             "metadata": {},
             "source": [
                 "## Multiple Providers - OpenAI, PaLM etc"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Gravity is like a special invisible force that pulls things towards each other. It's what keeps us on the ground instead of floating off into space! It's also what makes things fall when you drop them. Imagine if you're holding a toy and you let it go, it falls down, right? That's gravity pulling it towards the ground.\n"
                     ]
                 }
             ],
             "source": [
-                "openai_gen = generator(provider=\"openai\")\n",
+                "openai_gen = llm(provider=\"openai\")\n",
                 "openai_config = TextGenerationConfig(model=\"gpt-4\", use_cache=True)\n",
                 "openai_response = openai_gen.generate(messages, config=openai_config)\n",
                 "print(openai_response.text[0].content)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Gravity is a force that pulls things down to Earth. It's what makes things fall down when you drop them, and it's what keeps the moon in orbit around the Earth. Gravity is a very strong force, but it's also\n"
                     ]
                 }
             ],
             "source": [
-                "palm_gen = generator(provider=\"palm\")\n",
+                "palm_gen = llm(provider=\"palm\")\n",
                 "palm_config = TextGenerationConfig(model=\"codechat-bison\", temperature=0, max_tokens=50, use_cache=False)\n",
                 "palm_response = palm_gen.generate(messages, config=palm_config)\n",
                 "print(palm_response.text[0].content)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Gravity is a force that pulls things together. It's what makes things fall to the ground and what holds us on the earth. It's also what makes the moon orbit the earth and the planets orbit the sun. Gravity is a fundamental force of nature\n"
+                        "Gravity is a force that pulls things together. It is what makes things fall to the ground and what holds us on the earth. Gravity is a fundamental force of nature that affects everything around us. It is a property of all matter, and it is what makes things heavy. Gravity is also what causes the moon to orbit the earth and the planets to orbit the sun. It is a very important force that plays a big role in our lives.\n"
                     ]
                 }
             ],
             "source": [
-                "cohere_gen = generator(provider=\"cohere\")\n",
-                "cohere_config = TextGenerationConfig(model=\"command\", max_tokens=50, use_cache=True)\n",
+                "cohere_gen = llm(provider=\"cohere\")\n",
+                "cohere_config = TextGenerationConfig(model=\"command\", max_tokens=4050, use_cache=True)\n",
                 "cohere_response = cohere_gen.generate(messages, config=cohere_config)\n",
                 "print(cohere_response.text[0].content)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/victordibia/miniconda3/envs/coral/lib/python3.11/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html\n",
+                        "  from .autonotebook import tqdm as notebook_tqdm\n",
+                        "Loading checkpoint shards: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 2/2 [00:05<00:00,  2.67s/it]\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Hey there, little buddy! *smiling* Gravity is a magic that pulls everything towards each other! *excitedly* Just like how you like to hug your favorite toy or play with your friends, everything in the world has gravity too! *nodding* It's like a big hug that keeps everything close together. *giggles* Even you and me right now, we're being pulled towards each other by gravity! *winks* Isn't that cool? *grinning* So, let's have some fun and see how gravity works, okay? *excitedly*\n"
+                    ]
+                }
+            ],
+            "source": [
+                "hf_generator = llm(provider=\"hf\", model=\"TheBloke/Llama-2-7b-chat-fp16\", device_map=\"auto\")\n",
+                "hf_config = TextGenerationConfig(temperature=0, max_tokens=650, use_cache=False)\n",
+                "hf_response = hf_generator.generate(messages, config=hf_config)\n",
+                "print(hf_response.text[0].content)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "base",
             "language": "python",
             "name": "python3"
```

### Comparing `llmx-0.0.6a0/pyproject.toml` & `llmx-0.0.7a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llmx-0.0.6a0/tests/test_generators.py` & `llmx-0.0.7a0/tests/test_generators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import os
-from llmx import text_generator as generator
+from llmx import llm
 from llmx.datamodel import TextGenerationConfig
 
 
 config = TextGenerationConfig(
     n=2,
     temperature=0.4,
     max_tokens=100,
@@ -17,48 +17,49 @@
 
 messages = [
     {"role": "user",
      "content": "What is the capital of France? Only respond with the exact answer"}]
 
 
 def test_openai():
-    openai_gen = generator(provider="openai")
+    openai_gen = llm(provider="openai")
     openai_response = openai_gen.generate(messages, config=config)
     answer = openai_response.text[0].content
     print(openai_response.text[0].content)
 
     assert ("paris" in answer.lower())
     assert len(openai_response.text) == 2
 
 
 def test_google():
-    google_gen = generator(provider="google")
+    google_gen = llm(provider="google")
     config.model = "chat-bison@001"
     google_response = google_gen.generate(messages, config=config)
     answer = google_response.text[0].content
     print(google_response.text[0].content)
 
     assert ("paris" in answer.lower())
     # assert len(google_response.text) == 2 palm may chose to return 1 or 2 responses
 
 
 def test_cohere():
-    cohere_gen = generator(provider="cohere")
+    cohere_gen = llm(provider="cohere")
     config.model = "command"
     cohere_response = cohere_gen.generate(messages, config=config)
     answer = cohere_response.text[0].content
     print(cohere_response.text[0].content)
 
     assert ("paris" in answer.lower())
     assert len(cohere_response.text) == 2
 
 
-@pytest.mark.skipif(os.environ.get("LLMX_RUNALL", None) == "False", reason="takes too long")
+@pytest.mark.skipif(os.environ.get("LLMX_RUNALL", None) is None
+                    or os.environ.get("LLMX_RUNALL", None) == "False", reason="takes too long")
 def test_hf_local():
-    hf_local_gen = generator(
+    hf_local_gen = llm(
         provider="hf",
         model="TheBloke/Llama-2-7b-chat-fp16",
         device_map="auto")
     hf_local_response = hf_local_gen.generate(messages, config=config)
     answer = hf_local_response.text[0].content
     print(hf_local_response.text[0].content)
```

