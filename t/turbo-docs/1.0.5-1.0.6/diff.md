# Comparing `tmp/turbo_docs-1.0.5.tar.gz` & `tmp/turbo_docs-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-1.0.5.tar", last modified: Tue Aug  8 22:57:21 2023, max compression
+gzip compressed data, was "turbo_docs-1.0.6.tar", last modified: Tue Aug  8 23:00:49 2023, max compression
```

## Comparing `turbo_docs-1.0.5.tar` & `turbo_docs-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 22:57:21.207882 turbo_docs-1.0.5/
--rw-rw-rw-   0        0        0     2600 2023-08-08 22:57:21.206871 turbo_docs-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2103 2023-08-08 22:57:20.000000 turbo_docs-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-08-08 22:57:21.207882 turbo_docs-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      901 2023-08-08 22:57:10.000000 turbo_docs-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-08 22:57:21.169124 turbo_docs-1.0.5/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.5/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 22:57:21.191159 turbo_docs-1.0.5/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.5/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2144 2023-07-03 17:25:01.000000 turbo_docs-1.0.5/turbo_docs/commands/docs.py
--rw-rw-rw-   0        0        0     1038 2023-07-03 17:25:01.000000 turbo_docs-1.0.5/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     2399 2023-07-15 12:47:32.000000 turbo_docs-1.0.5/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-08-08 22:57:21.204357 turbo_docs-1.0.5/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.5/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      826 2023-07-03 17:25:01.000000 turbo_docs-1.0.5/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2369 2023-08-08 21:30:55.000000 turbo_docs-1.0.5/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      799 2023-07-03 17:25:01.000000 turbo_docs-1.0.5/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-08-08 22:57:21.185099 turbo_docs-1.0.5/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2600 2023-08-08 22:57:21.000000 turbo_docs-1.0.5/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-08-08 22:57:21.000000 turbo_docs-1.0.5/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 22:57:21.000000 turbo_docs-1.0.5/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-08 22:57:21.000000 turbo_docs-1.0.5/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-08-08 22:57:21.000000 turbo_docs-1.0.5/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-08 22:57:21.000000 turbo_docs-1.0.5/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 23:00:49.357099 turbo_docs-1.0.6/
+-rw-rw-rw-   0        0        0     2833 2023-08-08 23:00:49.355593 turbo_docs-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-08-08 22:58:15.000000 turbo_docs-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 23:00:49.357099 turbo_docs-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-08-08 23:00:43.000000 turbo_docs-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:00:49.293017 turbo_docs-1.0.6/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.6/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:00:49.341053 turbo_docs-1.0.6/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.6/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-07-03 17:25:01.000000 turbo_docs-1.0.6/turbo_docs/commands/docs.py
+-rw-rw-rw-   0        0        0     1038 2023-07-03 17:25:01.000000 turbo_docs-1.0.6/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     2399 2023-07-15 12:47:32.000000 turbo_docs-1.0.6/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:00:49.352594 turbo_docs-1.0.6/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.6/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-07-03 17:25:01.000000 turbo_docs-1.0.6/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2369 2023-08-08 21:30:55.000000 turbo_docs-1.0.6/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      799 2023-07-03 17:25:01.000000 turbo_docs-1.0.6/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:00:49.333995 turbo_docs-1.0.6/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2833 2023-08-08 23:00:49.000000 turbo_docs-1.0.6/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-08-08 23:00:49.000000 turbo_docs-1.0.6/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 23:00:49.000000 turbo_docs-1.0.6/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-08 23:00:49.000000 turbo_docs-1.0.6/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-08-08 23:00:49.000000 turbo_docs-1.0.6/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 23:00:49.000000 turbo_docs-1.0.6/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-1.0.5/PKG-INFO` & `turbo_docs-1.0.6/turbo_docs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 Metadata-Version: 2.1
-Name: turbo_docs
-Version: 1.0.5
+Name: turbo-docs
+Version: 1.0.6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Turbo Docs 🚀
 
-![GitHub stars](https://img.shields.io/github/stars/turbo_docs/turbo_docs?style=social)
+![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs?style=social)
 ![PyPI](https://img.shields.io/pypi/v/turbo_docs)
 
-Turbo Docs is a Python package that automates the process of generating documentation for your Python projects. It uses OpenAI's GPT-3.5 Turbo and GPT-4 models to generate concise and informative documentation for your functions, and even creates a README.md for your repository.
+Turbo Docs is a powerful Python package that automates the generation of documentation for your Python projects. It utilizes OpenAI's GPT models to create concise and informative documentation, making it easier for you and your users to understand your code.
 
-## Why Use Turbo Docs? 🎯
+## 📚 Table of Contents
 
-Writing documentation can be a tedious task, especially for large projects. Turbo Docs takes this burden off your shoulders by automating the process. It generates concise and informative documentation for your functions, and even creates a README.md for your repository. This allows you to focus on what you do best: writing code.
+- [Why Use Turbo Docs?](#why-use-turbo-docs)
+- [Repo Structure](#repo-structure)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Examples](#examples)
+- [Contributing](#contributing)
+- [License](#license)
+
+## 🎯 Why Use Turbo Docs?
+
+- **Save time**: Turbo Docs automatically generates documentation for your Python functions, so you can focus on writing code.
+- **Stay up-to-date**: Turbo Docs can be easily integrated into your development workflow, ensuring your documentation is always current.
+- **High-quality documentation**: Turbo Docs leverages the power of OpenAI's GPT models to generate concise and informative documentation.
+- **Customizable**: You can choose between GPT-3.5 Turbo and GPT-4 models, and even provide your own templates for generating documentation.
 
-## Repo Structure 🌳
+## 🌳 Repo Structure
 
 ```
 turbo_docs/
 ├── commands/
 │   ├── docs.py
 │   ├── readme.py
 │   └── __init__.py
@@ -34,44 +47,46 @@
 │   ├── cli_options.py
 │   ├── directory.py
 │   ├── openai_api.py
 │   └── __init__.py
 ├── generate.py
 ├── __init__.py
 ├── setup.py
-└── requirements.txt
+├── requirements.txt
+└── turbo_docs.toml
 ```
 
-## Example Usage 📖
+## 📦 Installation
 
-```python
-from turbo_docs.commands import readme as readme_module
-from turbo_docs.commands import docs as docs_module
-from turbo_docs.utils import directory
+To install Turbo Docs, simply run:
 
-# Get a dictionary of all text in the current repo
-dir_text_dict = directory.get_repo_text_dict()
+```bash
+pip install turbo_docs
+```
 
-# Generate README.md
-readme_module.readme(dir_text_dict, model="gpt-4")
+## 🛠 Usage
 
-# Generate documentation for all code files
-docs_module.docs(dir_text_dict, model="gpt-4")
-```
+To generate documentation for your Python project, navigate to your project's root directory and run:
 
-## Installation 📦
+```bash
+turbo_docs --docs
+```
 
-You can install Turbo Docs via pip:
+To generate a README.md file for your project, run:
 
 ```bash
-pip install turbo_docs
+turbo_docs --readme
 ```
 
-Please note that you need to have an OpenAI API key to use Turbo Docs. If you don't have one, you can create an account at [OpenAI](https://platform.openai.com/overview).
+For more options, run:
+
+```bash
+turbo_docs --help
+```
 
-## Contributing 🤝
+## 🤝 Contributing
 
-Contributions are welcome! Please feel free to submit a Pull Request.
+Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss any improvements or suggestions.
 
-## License 📄
+## 📄 License
 
-Turbo Docs is licensed under the MIT License.
+Turbo Docs is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `turbo_docs-1.0.5/README.md` & `turbo_docs-1.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # Turbo Docs 🚀
 
-![GitHub stars](https://img.shields.io/github/stars/turbo_docs/turbo_docs?style=social)
+![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs?style=social)
 ![PyPI](https://img.shields.io/pypi/v/turbo_docs)
 
-Turbo Docs is a Python package that automates the process of generating documentation for your Python projects. It uses OpenAI's GPT-3.5 Turbo and GPT-4 models to generate concise and informative documentation for your functions, and even creates a README.md for your repository.
+Turbo Docs is a powerful Python package that automates the generation of documentation for your Python projects. It utilizes OpenAI's GPT models to create concise and informative documentation, making it easier for you and your users to understand your code.
 
-## Why Use Turbo Docs? 🎯
+## 📚 Table of Contents
 
-Writing documentation can be a tedious task, especially for large projects. Turbo Docs takes this burden off your shoulders by automating the process. It generates concise and informative documentation for your functions, and even creates a README.md for your repository. This allows you to focus on what you do best: writing code.
+- [Why Use Turbo Docs?](#why-use-turbo-docs)
+- [Repo Structure](#repo-structure)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Examples](#examples)
+- [Contributing](#contributing)
+- [License](#license)
+
+## 🎯 Why Use Turbo Docs?
+
+- **Save time**: Turbo Docs automatically generates documentation for your Python functions, so you can focus on writing code.
+- **Stay up-to-date**: Turbo Docs can be easily integrated into your development workflow, ensuring your documentation is always current.
+- **High-quality documentation**: Turbo Docs leverages the power of OpenAI's GPT models to generate concise and informative documentation.
+- **Customizable**: You can choose between GPT-3.5 Turbo and GPT-4 models, and even provide your own templates for generating documentation.
 
-## Repo Structure 🌳
+## 🌳 Repo Structure
 
 ```
 turbo_docs/
 ├── commands/
 │   ├── docs.py
 │   ├── readme.py
 │   └── __init__.py
@@ -21,44 +34,46 @@
 │   ├── cli_options.py
 │   ├── directory.py
 │   ├── openai_api.py
 │   └── __init__.py
 ├── generate.py
 ├── __init__.py
 ├── setup.py
-└── requirements.txt
+├── requirements.txt
+└── turbo_docs.toml
 ```
 
-## Example Usage 📖
+## 📦 Installation
 
-```python
-from turbo_docs.commands import readme as readme_module
-from turbo_docs.commands import docs as docs_module
-from turbo_docs.utils import directory
+To install Turbo Docs, simply run:
 
-# Get a dictionary of all text in the current repo
-dir_text_dict = directory.get_repo_text_dict()
+```bash
+pip install turbo_docs
+```
 
-# Generate README.md
-readme_module.readme(dir_text_dict, model="gpt-4")
+## 🛠 Usage
 
-# Generate documentation for all code files
-docs_module.docs(dir_text_dict, model="gpt-4")
-```
+To generate documentation for your Python project, navigate to your project's root directory and run:
 
-## Installation 📦
+```bash
+turbo_docs --docs
+```
 
-You can install Turbo Docs via pip:
+To generate a README.md file for your project, run:
 
 ```bash
-pip install turbo_docs
+turbo_docs --readme
 ```
 
-Please note that you need to have an OpenAI API key to use Turbo Docs. If you don't have one, you can create an account at [OpenAI](https://platform.openai.com/overview).
+For more options, run:
+
+```bash
+turbo_docs --help
+```
 
-## Contributing 🤝
+## 🤝 Contributing
 
-Contributions are welcome! Please feel free to submit a Pull Request.
+Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss any improvements or suggestions.
 
-## License 📄
+## 📄 License
 
-Turbo Docs is licensed under the MIT License.
+Turbo Docs is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `turbo_docs-1.0.5/setup.py` & `turbo_docs-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="1.0.5",
+	version="1.0.6",
 	packages=find_packages(),
 	install_requires=[
 		"openai",
 		"click",
 		"pyperclip",
     	"toml",
         "pathspec",
```

### Comparing `turbo_docs-1.0.5/turbo_docs/commands/docs.py` & `turbo_docs-1.0.6/turbo_docs/commands/docs.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.5/turbo_docs/commands/readme.py` & `turbo_docs-1.0.6/turbo_docs/commands/readme.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.5/turbo_docs/generate.py` & `turbo_docs-1.0.6/turbo_docs/generate.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.5/turbo_docs/utils/cli_options.py` & `turbo_docs-1.0.6/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.5/turbo_docs/utils/directory.py` & `turbo_docs-1.0.6/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.5/turbo_docs/utils/openai_api.py` & `turbo_docs-1.0.6/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.5/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 Metadata-Version: 2.1
-Name: turbo-docs
-Version: 1.0.5
+Name: turbo_docs
+Version: 1.0.6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Turbo Docs 🚀
 
-![GitHub stars](https://img.shields.io/github/stars/turbo_docs/turbo_docs?style=social)
+![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs?style=social)
 ![PyPI](https://img.shields.io/pypi/v/turbo_docs)
 
-Turbo Docs is a Python package that automates the process of generating documentation for your Python projects. It uses OpenAI's GPT-3.5 Turbo and GPT-4 models to generate concise and informative documentation for your functions, and even creates a README.md for your repository.
+Turbo Docs is a powerful Python package that automates the generation of documentation for your Python projects. It utilizes OpenAI's GPT models to create concise and informative documentation, making it easier for you and your users to understand your code.
 
-## Why Use Turbo Docs? 🎯
+## 📚 Table of Contents
 
-Writing documentation can be a tedious task, especially for large projects. Turbo Docs takes this burden off your shoulders by automating the process. It generates concise and informative documentation for your functions, and even creates a README.md for your repository. This allows you to focus on what you do best: writing code.
+- [Why Use Turbo Docs?](#why-use-turbo-docs)
+- [Repo Structure](#repo-structure)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Examples](#examples)
+- [Contributing](#contributing)
+- [License](#license)
+
+## 🎯 Why Use Turbo Docs?
+
+- **Save time**: Turbo Docs automatically generates documentation for your Python functions, so you can focus on writing code.
+- **Stay up-to-date**: Turbo Docs can be easily integrated into your development workflow, ensuring your documentation is always current.
+- **High-quality documentation**: Turbo Docs leverages the power of OpenAI's GPT models to generate concise and informative documentation.
+- **Customizable**: You can choose between GPT-3.5 Turbo and GPT-4 models, and even provide your own templates for generating documentation.
 
-## Repo Structure 🌳
+## 🌳 Repo Structure
 
 ```
 turbo_docs/
 ├── commands/
 │   ├── docs.py
 │   ├── readme.py
 │   └── __init__.py
@@ -34,44 +47,46 @@
 │   ├── cli_options.py
 │   ├── directory.py
 │   ├── openai_api.py
 │   └── __init__.py
 ├── generate.py
 ├── __init__.py
 ├── setup.py
-└── requirements.txt
+├── requirements.txt
+└── turbo_docs.toml
 ```
 
-## Example Usage 📖
+## 📦 Installation
 
-```python
-from turbo_docs.commands import readme as readme_module
-from turbo_docs.commands import docs as docs_module
-from turbo_docs.utils import directory
+To install Turbo Docs, simply run:
 
-# Get a dictionary of all text in the current repo
-dir_text_dict = directory.get_repo_text_dict()
+```bash
+pip install turbo_docs
+```
 
-# Generate README.md
-readme_module.readme(dir_text_dict, model="gpt-4")
+## 🛠 Usage
 
-# Generate documentation for all code files
-docs_module.docs(dir_text_dict, model="gpt-4")
-```
+To generate documentation for your Python project, navigate to your project's root directory and run:
 
-## Installation 📦
+```bash
+turbo_docs --docs
+```
 
-You can install Turbo Docs via pip:
+To generate a README.md file for your project, run:
 
 ```bash
-pip install turbo_docs
+turbo_docs --readme
 ```
 
-Please note that you need to have an OpenAI API key to use Turbo Docs. If you don't have one, you can create an account at [OpenAI](https://platform.openai.com/overview).
+For more options, run:
+
+```bash
+turbo_docs --help
+```
 
-## Contributing 🤝
+## 🤝 Contributing
 
-Contributions are welcome! Please feel free to submit a Pull Request.
+Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss any improvements or suggestions.
 
-## License 📄
+## 📄 License
 
-Turbo Docs is licensed under the MIT License.
+Turbo Docs is released under the [MIT License](https://opensource.org/licenses/MIT).
```

