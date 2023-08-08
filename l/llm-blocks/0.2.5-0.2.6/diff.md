# Comparing `tmp/llm-blocks-0.2.5.tar.gz` & `tmp/llm-blocks-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-blocks-0.2.5.tar", last modified: Sat Jul 29 00:00:27 2023, max compression
+gzip compressed data, was "llm-blocks-0.2.6.tar", last modified: Tue Aug  8 23:14:16 2023, max compression
```

## Comparing `llm-blocks-0.2.5.tar` & `llm-blocks-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 00:00:27.103679 llm-blocks-0.2.5/
--rw-rw-rw-   0        0        0     2493 2023-07-29 00:00:27.101677 llm-blocks-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2049 2023-07-29 00:00:10.000000 llm-blocks-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 00:00:27.091677 llm-blocks-0.2.5/llm_blocks/
--rw-rw-rw-   0        0        0        0 2023-06-06 22:53:28.000000 llm-blocks-0.2.5/llm_blocks/__init__.py
--rw-rw-rw-   0        0        0     3250 2023-07-28 23:47:36.000000 llm-blocks-0.2.5/llm_blocks/chat_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:00:27.099677 llm-blocks-0.2.5/llm_blocks.egg-info/
--rw-rw-rw-   0        0        0     2493 2023-07-29 00:00:27.000000 llm-blocks-0.2.5/llm_blocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-29 00:00:27.000000 llm-blocks-0.2.5/llm_blocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 00:00:27.000000 llm-blocks-0.2.5/llm_blocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-29 00:00:27.000000 llm-blocks-0.2.5/llm_blocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-29 00:00:27.000000 llm-blocks-0.2.5/llm_blocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 00:00:27.103679 llm-blocks-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-07-29 00:00:25.000000 llm-blocks-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:14:16.197392 llm-blocks-0.2.6/
+-rw-rw-rw-   0        0        0     2493 2023-08-08 23:14:16.196394 llm-blocks-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2049 2023-07-29 00:00:10.000000 llm-blocks-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 23:14:16.183328 llm-blocks-0.2.6/llm_blocks/
+-rw-rw-rw-   0        0        0        0 2023-06-06 22:53:28.000000 llm-blocks-0.2.6/llm_blocks/__init__.py
+-rw-rw-rw-   0        0        0     2787 2023-08-08 23:13:10.000000 llm-blocks-0.2.6/llm_blocks/chat_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:14:16.194394 llm-blocks-0.2.6/llm_blocks.egg-info/
+-rw-rw-rw-   0        0        0     2493 2023-08-08 23:14:16.000000 llm-blocks-0.2.6/llm_blocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-08-08 23:14:16.000000 llm-blocks-0.2.6/llm_blocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 23:14:16.000000 llm-blocks-0.2.6/llm_blocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-08 23:14:16.000000 llm-blocks-0.2.6/llm_blocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 23:14:16.000000 llm-blocks-0.2.6/llm_blocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 23:14:16.198396 llm-blocks-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      826 2023-08-08 23:14:13.000000 llm-blocks-0.2.6/setup.py
```

### Comparing `llm-blocks-0.2.5/PKG-INFO` & `llm-blocks-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-blocks
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple interface for creating and managing LLM chains
 Home-page: https://github.com/voynow/llm-blocks
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm-blocks-0.2.5/README.md` & `llm-blocks-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `llm-blocks-0.2.5/llm_blocks/chat_utils.py` & `llm-blocks-0.2.6/llm_blocks/chat_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import re
 import time
+from typing import Any, Dict, Generator, Union
 
 import dotenv
 import openai
-from IPython.display import Markdown, clear_output, display
 
 dotenv.load_dotenv()
 OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
 if not OPENAI_API_KEY:
     raise ValueError(
         "OPENAI_API_KEY not found. Either create a .env file or set the environment variable."
     )
+openai.api_key = OPENAI_API_KEY
 
 
 class GenericChain:
     def __init__(
         self,
         template: str,
         role: str = "user",
@@ -41,52 +42,40 @@
         self.logs = []
 
 
     def get_input_variables(self) -> list:
         """Get the input variables from the template"""
         return re.findall(r"\{(\w+)\}", self.template)
 
-    def create_completion(self, inputs: dict) -> str:
+    def create_completion(self, inputs: Dict[str, Any]) -> Union[Dict[str, Any], Generator]:
         """Create a GPT completion"""
         self.message['content'] = self.template.format(**inputs)
         response = openai.ChatCompletion.create(
             model=self.model_name,
             messages=[self.message],
             temperature=self.temperature,
             stream=self.stream,
         )
         return response
 
-    def stream_output(self, inputs) -> None:
-        """Get stream GPT completion - fun to watch"""
-        response = self.create_completion(inputs)
-        collected_content = ""
-        for chunk in response:
-            chunk_message = chunk['choices'][0]['delta']  
-            collected_content += chunk_message['content'] if 'content' in chunk_message else ''
-            clear_output(wait=True)
-            display(Markdown(collected_content))
-        return collected_content
-
-    def batch_output(self, inputs) -> None:
-        """Get batch GPT completion - not as fun to watch"""
+    def batch_output(self, inputs: Dict[str, Any]) -> None:
         start_time = time.time()
         response = self.create_completion(inputs).choices[0]["message"]["content"]
         response_time = time.time() - start_time
         self.logs.append({
             "inputs": inputs,
             "response": response,
             "response_time": response_time,
         })
         return response
 
-    def __call__(self, *args, **kwargs) -> str:
+    def __call__(self, *args, **kwargs) -> Union[str, Generator]:
         """Call the model with the given inputs"""
         inputs = {}
         if args:
             inputs = {key: value for key, value in zip(self.input_variables, args)}
         if kwargs:
             inputs.update(kwargs)
 
         if self.stream:
-            return self.stream_output(inputs) 
+            return self.create_completion(inputs)
         return self.batch_output(inputs)
```

### Comparing `llm-blocks-0.2.5/llm_blocks.egg-info/PKG-INFO` & `llm-blocks-0.2.6/llm_blocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-blocks
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple interface for creating and managing LLM chains
 Home-page: https://github.com/voynow/llm-blocks
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llm-blocks-0.2.5/setup.py` & `llm-blocks-0.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="llm-blocks",
-    version="0.2.5",
+    version="0.2.6",
     author="Jamie Voynow",
     author_email="voynow99@gmail.com",
     description="Simple interface for creating and managing LLM chains",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/voynow/llm-blocks",
     packages=find_packages(),
@@ -21,9 +21,8 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
 
-# python setup.py sdist bdist_wheel
-# twine upload dist/*
+# python setup.py sdist bdist_wheel
```

