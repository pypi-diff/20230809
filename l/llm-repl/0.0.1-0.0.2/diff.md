# Comparing `tmp/llm-repl-0.0.1.tar.gz` & `tmp/llm-repl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-repl-0.0.1.tar", last modified: Tue Mar 28 02:12:00 2023, max compression
+gzip compressed data, was "llm-repl-0.0.2.tar", last modified: Tue Aug  8 22:48:25 2023, max compression
```

## Comparing `llm-repl-0.0.1.tar` & `llm-repl-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-03-28 02:12:00.470693 llm-repl-0.0.1/
--rw-rw-r--   0 phate     (1000) phate     (1000)     1075 2023-03-28 02:09:29.000000 llm-repl-0.0.1/LICENSE
--rw-rw-r--   0 phate     (1000) phate     (1000)     3294 2023-03-28 02:12:00.470693 llm-repl-0.0.1/PKG-INFO
--rw-rw-r--   0 phate     (1000) phate     (1000)     2725 2023-03-28 01:48:44.000000 llm-repl-0.0.1/README.md
--rw-rw-r--   0 phate     (1000) phate     (1000)     1104 2023-03-28 02:11:37.000000 llm-repl-0.0.1/pyproject.toml
--rw-rw-r--   0 phate     (1000) phate     (1000)       38 2023-03-28 02:12:00.470693 llm-repl-0.0.1/setup.cfg
-drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-03-28 02:12:00.466693 llm-repl-0.0.1/src/
-drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-03-28 02:12:00.466693 llm-repl-0.0.1/src/llm_repl/
--rw-rw-r--   0 phate     (1000) phate     (1000)        0 2023-03-21 00:56:17.000000 llm-repl-0.0.1/src/llm_repl/__init__.py
--rw-rw-r--   0 phate     (1000) phate     (1000)      788 2023-03-28 01:08:07.000000 llm-repl-0.0.1/src/llm_repl/__main__.py
-drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-03-28 02:12:00.470693 llm-repl-0.0.1/src/llm_repl/llms/
--rw-rw-r--   0 phate     (1000) phate     (1000)     2864 2023-03-27 23:43:46.000000 llm-repl-0.0.1/src/llm_repl/llms/__init__.py
--rw-rw-r--   0 phate     (1000) phate     (1000)     3649 2023-03-27 23:43:46.000000 llm-repl-0.0.1/src/llm_repl/llms/chatgpt.py
--rw-rw-r--   0 phate     (1000) phate     (1000)      714 2023-03-27 23:43:45.000000 llm-repl-0.0.1/src/llm_repl/llms/chatgpt4.py
--rw-rw-r--   0 phate     (1000) phate     (1000)     3887 2023-03-27 21:22:31.000000 llm-repl-0.0.1/src/llm_repl/llms/chatgpt_internet.py
--rw-rw-r--   0 phate     (1000) phate     (1000)     5026 2023-03-28 01:07:49.000000 llm-repl-0.0.1/src/llm_repl/repl.py
-drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-03-28 02:12:00.470693 llm-repl-0.0.1/src/llm_repl.egg-info/
--rw-rw-r--   0 phate     (1000) phate     (1000)     3294 2023-03-28 02:12:00.000000 llm-repl-0.0.1/src/llm_repl.egg-info/PKG-INFO
--rw-rw-r--   0 phate     (1000) phate     (1000)      448 2023-03-28 02:12:00.000000 llm-repl-0.0.1/src/llm_repl.egg-info/SOURCES.txt
--rw-rw-r--   0 phate     (1000) phate     (1000)        1 2023-03-28 02:12:00.000000 llm-repl-0.0.1/src/llm_repl.egg-info/dependency_links.txt
--rw-rw-r--   0 phate     (1000) phate     (1000)       52 2023-03-28 02:12:00.000000 llm-repl-0.0.1/src/llm_repl.egg-info/entry_points.txt
--rw-rw-r--   0 phate     (1000) phate     (1000)       85 2023-03-28 02:12:00.000000 llm-repl-0.0.1/src/llm_repl.egg-info/requires.txt
--rw-rw-r--   0 phate     (1000) phate     (1000)        9 2023-03-28 02:12:00.000000 llm-repl-0.0.1/src/llm_repl.egg-info/top_level.txt
+drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-08-08 22:48:25.062841 llm-repl-0.0.2/
+-rw-rw-r--   0 phate     (1000) phate     (1000)     1075 2023-08-08 22:47:44.000000 llm-repl-0.0.2/LICENSE
+-rw-rw-r--   0 phate     (1000) phate     (1000)     3631 2023-08-08 22:48:25.062841 llm-repl-0.0.2/PKG-INFO
+-rw-rw-r--   0 phate     (1000) phate     (1000)     3070 2023-08-08 22:47:44.000000 llm-repl-0.0.2/README.md
+-rw-rw-r--   0 phate     (1000) phate     (1000)     1272 2023-08-08 22:47:55.000000 llm-repl-0.0.2/pyproject.toml
+-rw-rw-r--   0 phate     (1000) phate     (1000)       38 2023-08-08 22:48:25.062841 llm-repl-0.0.2/setup.cfg
+drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-08-08 22:48:25.062841 llm-repl-0.0.2/src/
+drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-08-08 22:48:25.062841 llm-repl-0.0.2/src/llm_repl/
+-rw-rw-r--   0 phate     (1000) phate     (1000)      775 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/__init__.py
+-rw-rw-r--   0 phate     (1000) phate     (1000)      812 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/__main__.py
+-rw-rw-r--   0 phate     (1000) phate     (1000)      663 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/exceptions.py
+drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-08-08 22:48:25.062841 llm-repl-0.0.2/src/llm_repl/llms/
+-rw-rw-r--   0 phate     (1000) phate     (1000)     1026 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/llms/__init__.py
+-rw-rw-r--   0 phate     (1000) phate     (1000)     5274 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/llms/chatgpt.py
+-rw-rw-r--   0 phate     (1000) phate     (1000)      790 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/llms/chatgpt4.py
+drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-08-08 22:48:25.062841 llm-repl-0.0.2/src/llm_repl/repls/
+-rw-rw-r--   0 phate     (1000) phate     (1000)     2945 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/repls/__init__.py
+-rw-rw-r--   0 phate     (1000) phate     (1000)     4370 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/repls/http.py
+-rw-rw-r--   0 phate     (1000) phate     (1000)    11436 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/repls/prompt_toolkit.py
+-rw-rw-r--   0 phate     (1000) phate     (1000)     3424 2023-08-08 22:47:44.000000 llm-repl-0.0.2/src/llm_repl/repls/websocket.py
+drwxrwxr-x   0 phate     (1000) phate     (1000)        0 2023-08-08 22:48:25.062841 llm-repl-0.0.2/src/llm_repl.egg-info/
+-rw-rw-r--   0 phate     (1000) phate     (1000)     3631 2023-08-08 22:48:25.000000 llm-repl-0.0.2/src/llm_repl.egg-info/PKG-INFO
+-rw-rw-r--   0 phate     (1000) phate     (1000)      543 2023-08-08 22:48:25.000000 llm-repl-0.0.2/src/llm_repl.egg-info/SOURCES.txt
+-rw-rw-r--   0 phate     (1000) phate     (1000)        1 2023-08-08 22:48:25.000000 llm-repl-0.0.2/src/llm_repl.egg-info/dependency_links.txt
+-rw-rw-r--   0 phate     (1000) phate     (1000)       52 2023-08-08 22:48:25.000000 llm-repl-0.0.2/src/llm_repl.egg-info/entry_points.txt
+-rw-rw-r--   0 phate     (1000) phate     (1000)      167 2023-08-08 22:48:25.000000 llm-repl-0.0.2/src/llm_repl.egg-info/requires.txt
+-rw-rw-r--   0 phate     (1000) phate     (1000)        9 2023-08-08 22:48:25.000000 llm-repl-0.0.2/src/llm_repl.egg-info/top_level.txt
```

### Comparing `llm-repl-0.0.1/LICENSE` & `llm-repl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-repl-0.0.1/PKG-INFO` & `llm-repl-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: llm-repl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A REPL for ChatGPT
 Author-email: Sebastiano Mariani <mariani.sebastiano@gmail.com>
-Project-URL: homepage, https://github.com/Phat3/ChatGPT-REPL
-Project-URL: repository, https://github.com/Phat3/ChatGPT-REPL.git
+Project-URL: homepage, https://github.com/Phat3/LLM-Repl
+Project-URL: repository, https://github.com/Phat3/LLM-Repl.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
 License-File: LICENSE
 
 # LLM REPL
 
 ## What is this?
 
 The goal of this project is to create a simple, interactive **REPL** (Read-Eval-Print-Loop) that allows users to interact with a variety of Large Language Models (**LLMs**). The project is mainly built on top of two Python libraries: [langchain](https://github.com/hwchase17/langchain), which provides a convenient and flexible interface for working with LLMs, and [rich](https://github.com/Textualize/rich) which provides a user-friendly interface for the REPL.
+The REPL can also be launched in **headledss** mode and it can be interacted with using **websocket**.
 
 Currently, the project is in development and only supports interaction with the ChatGPT but it has been structure to make it easy to extend it use any LLMs, including custom ones (by extending `BaseLLM` in `./src/llm_repl/llms/__init__.py`).
 
 ChatGPT can be interacted by using the models `gpt-3.5-turbo` and `gpt4` (For users who got GPT-4 API beta).
 
 ## Features
 
@@ -44,17 +45,29 @@
 
 The REPL supports Markdown rendering both of the input and the output.
 
 PS: In this initial version of the REPL, the full Markdown syntax is only when running the tool in `non-streaming` mode. In `streaming` mode only code sections will be pretty printed.
 
 ![Pretty Printing](./docs/gifs/pretty_printing.gif)
 
-### Model Switching
+## Headless Mode
 
-The REPL supports the switching between different models. At the moment, the only supported LLMs are `chatgpt` and `chatgpt4`.
+The REPL can be run in headless mode. This means that it can be interacted with using a websocket. This is useful for integrating the REPL with other applications / other UIs.
+
+To launch the REPL in headless mode, run the following command:
+
+```bash
+llm-repl --repl websocket --port <PORT>
+```
+
+### Model Switching on the Fly
+
+**COMING SOON...**
+
+### Conversation History
 
 **COMING SOON...**
 
 ## Installation
 
 ```bash
 pip install llm-repl
```

### Comparing `llm-repl-0.0.1/README.md` & `llm-repl-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # LLM REPL
 
 ## What is this?
 
 The goal of this project is to create a simple, interactive **REPL** (Read-Eval-Print-Loop) that allows users to interact with a variety of Large Language Models (**LLMs**). The project is mainly built on top of two Python libraries: [langchain](https://github.com/hwchase17/langchain), which provides a convenient and flexible interface for working with LLMs, and [rich](https://github.com/Textualize/rich) which provides a user-friendly interface for the REPL.
+The REPL can also be launched in **headledss** mode and it can be interacted with using **websocket**.
 
 Currently, the project is in development and only supports interaction with the ChatGPT but it has been structure to make it easy to extend it use any LLMs, including custom ones (by extending `BaseLLM` in `./src/llm_repl/llms/__init__.py`).
 
 ChatGPT can be interacted by using the models `gpt-3.5-turbo` and `gpt4` (For users who got GPT-4 API beta).
 
 ## Features
 
@@ -28,17 +29,29 @@
 
 The REPL supports Markdown rendering both of the input and the output.
 
 PS: In this initial version of the REPL, the full Markdown syntax is only when running the tool in `non-streaming` mode. In `streaming` mode only code sections will be pretty printed.
 
 ![Pretty Printing](./docs/gifs/pretty_printing.gif)
 
-### Model Switching
+## Headless Mode
 
-The REPL supports the switching between different models. At the moment, the only supported LLMs are `chatgpt` and `chatgpt4`.
+The REPL can be run in headless mode. This means that it can be interacted with using a websocket. This is useful for integrating the REPL with other applications / other UIs.
+
+To launch the REPL in headless mode, run the following command:
+
+```bash
+llm-repl --repl websocket --port <PORT>
+```
+
+### Model Switching on the Fly
+
+**COMING SOON...**
+
+### Conversation History
 
 **COMING SOON...**
 
 ## Installation
 
 ```bash
 pip install llm-repl
```

### Comparing `llm-repl-0.0.1/pyproject.toml` & `llm-repl-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm-repl"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Sebastiano Mariani", email = "mariani.sebastiano@gmail.com"},
 ]
 description = "A REPL for ChatGPT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -21,33 +21,43 @@
 
 ]
 requires-python = ">=3.10"
 
 dependencies = [
   "prompt_toolkit",
   "rich",
-  "langchain",
-  "openai"
+  "langchain == 0.0.133",
+  "openai",
+  "pydantic",
+  "websockets",
+  "fastapi",
+  "uvicorn",
+  "pinecone-client",
+  "jinja2",
+  "sse_starlette"
 ]
 
 [project.optional-dependencies]
 DEV = [
   "pylint",
   "ipdb",
   "black",
   "pytest",
   "mypy",
   "pre-commit",
 ]
 
 [project.urls]
-homepage = "https://github.com/Phat3/ChatGPT-REPL"
-repository = "https://github.com/Phat3/ChatGPT-REPL.git"
+homepage = "https://github.com/Phat3/LLM-Repl"
+repository = "https://github.com/Phat3/LLM-Repl.git"
 
 [tool.pylint.master]
 ignored-modules = ""
 disable = """
 W1514,F0010,useless-super-delegation,E1103,W0108,W0404,R0904,R0922,W0105,
 W0142,C0301,C0321,C0322,C0324,R,W0232,E1001,W0212,W0703,C,I0011,I0012,I0013,E0012,W0511"""
 
 [project.scripts]
 llm-repl = "llm_repl.__main__:main"
+
+[tool.setuptools.package-data]
+"mypkg.data" = ["*.yml"]
```

### Comparing `llm-repl-0.0.1/src/llm_repl.egg-info/PKG-INFO` & `llm-repl-0.0.2/src/llm_repl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: llm-repl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A REPL for ChatGPT
 Author-email: Sebastiano Mariani <mariani.sebastiano@gmail.com>
-Project-URL: homepage, https://github.com/Phat3/ChatGPT-REPL
-Project-URL: repository, https://github.com/Phat3/ChatGPT-REPL.git
+Project-URL: homepage, https://github.com/Phat3/LLM-Repl
+Project-URL: repository, https://github.com/Phat3/LLM-Repl.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
 License-File: LICENSE
 
 # LLM REPL
 
 ## What is this?
 
 The goal of this project is to create a simple, interactive **REPL** (Read-Eval-Print-Loop) that allows users to interact with a variety of Large Language Models (**LLMs**). The project is mainly built on top of two Python libraries: [langchain](https://github.com/hwchase17/langchain), which provides a convenient and flexible interface for working with LLMs, and [rich](https://github.com/Textualize/rich) which provides a user-friendly interface for the REPL.
+The REPL can also be launched in **headledss** mode and it can be interacted with using **websocket**.
 
 Currently, the project is in development and only supports interaction with the ChatGPT but it has been structure to make it easy to extend it use any LLMs, including custom ones (by extending `BaseLLM` in `./src/llm_repl/llms/__init__.py`).
 
 ChatGPT can be interacted by using the models `gpt-3.5-turbo` and `gpt4` (For users who got GPT-4 API beta).
 
 ## Features
 
@@ -44,17 +45,29 @@
 
 The REPL supports Markdown rendering both of the input and the output.
 
 PS: In this initial version of the REPL, the full Markdown syntax is only when running the tool in `non-streaming` mode. In `streaming` mode only code sections will be pretty printed.
 
 ![Pretty Printing](./docs/gifs/pretty_printing.gif)
 
-### Model Switching
+## Headless Mode
 
-The REPL supports the switching between different models. At the moment, the only supported LLMs are `chatgpt` and `chatgpt4`.
+The REPL can be run in headless mode. This means that it can be interacted with using a websocket. This is useful for integrating the REPL with other applications / other UIs.
+
+To launch the REPL in headless mode, run the following command:
+
+```bash
+llm-repl --repl websocket --port <PORT>
+```
+
+### Model Switching on the Fly
+
+**COMING SOON...**
+
+### Conversation History
 
 **COMING SOON...**
 
 ## Installation
 
 ```bash
 pip install llm-repl
```

