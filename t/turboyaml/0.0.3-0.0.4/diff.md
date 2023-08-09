# Comparing `tmp/turboyaml-0.0.3.tar.gz` & `tmp/turboyaml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turboyaml-0.0.3.tar", last modified: Fri Jul 28 03:03:40 2023, max compression
+gzip compressed data, was "turboyaml-0.0.4.tar", last modified: Wed Aug  9 02:02:00 2023, max compression
```

## Comparing `turboyaml-0.0.3.tar` & `turboyaml-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 03:03:40.374927 turboyaml-0.0.3/
--rw-r--r--   0 fredbrowne   (501) staff       (20)     1067 2023-07-26 03:34:01.000000 turboyaml-0.0.3/LICENSE
--rw-r--r--   0 fredbrowne   (501) staff       (20)     5970 2023-07-28 03:03:40.374802 turboyaml-0.0.3/PKG-INFO
--rw-r--r--   0 fredbrowne   (501) staff       (20)     5397 2023-07-28 02:57:28.000000 turboyaml-0.0.3/README.md
--rw-r--r--   0 fredbrowne   (501) staff       (20)       38 2023-07-28 03:03:40.374967 turboyaml-0.0.3/setup.cfg
--rw-r--r--   0 fredbrowne   (501) staff       (20)      939 2023-07-28 03:02:30.000000 turboyaml-0.0.3/setup.py
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 03:03:40.373439 turboyaml-0.0.3/turboyaml/
--rw-r--r--   0 fredbrowne   (501) staff       (20)       22 2023-07-28 02:21:13.000000 turboyaml-0.0.3/turboyaml/__init__.py
--rw-r--r--   0 fredbrowne   (501) staff       (20)     9193 2023-07-28 02:27:09.000000 turboyaml-0.0.3/turboyaml/cli.py
-drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-07-28 03:03:40.374611 turboyaml-0.0.3/turboyaml.egg-info/
--rw-r--r--   0 fredbrowne   (501) staff       (20)     5970 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/PKG-INFO
--rw-r--r--   0 fredbrowne   (501) staff       (20)      265 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)        1 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)       50 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/entry_points.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)       29 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/requires.txt
--rw-r--r--   0 fredbrowne   (501) staff       (20)       10 2023-07-28 03:03:40.000000 turboyaml-0.0.3/turboyaml.egg-info/top_level.txt
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-08-09 02:02:00.969116 turboyaml-0.0.4/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     1067 2023-07-26 03:34:01.000000 turboyaml-0.0.4/LICENSE
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     6198 2023-08-09 02:02:00.968993 turboyaml-0.0.4/PKG-INFO
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     5625 2023-08-09 01:57:13.000000 turboyaml-0.0.4/README.md
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       38 2023-08-09 02:02:00.969159 turboyaml-0.0.4/setup.cfg
+-rw-r--r--   0 fredbrowne   (501) staff       (20)      914 2023-08-09 01:57:13.000000 turboyaml-0.0.4/setup.py
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-08-09 02:02:00.967545 turboyaml-0.0.4/turboyaml/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       67 2023-08-09 01:57:13.000000 turboyaml-0.0.4/turboyaml/__init__.py
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     3855 2023-08-09 01:57:13.000000 turboyaml-0.0.4/turboyaml/cli.py
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-08-09 02:02:00.968823 turboyaml-0.0.4/turboyaml/utils/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)        0 2023-08-09 01:57:13.000000 turboyaml-0.0.4/turboyaml/utils/__init__.py
+-rw-r--r--   0 fredbrowne   (501) staff       (20)      363 2023-08-09 01:57:13.000000 turboyaml-0.0.4/turboyaml/utils/dbt_utils.py
+-rw-r--r--   0 fredbrowne   (501) staff       (20)      720 2023-08-09 01:57:13.000000 turboyaml-0.0.4/turboyaml/utils/openai_utils.py
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     4372 2023-08-09 01:57:13.000000 turboyaml-0.0.4/turboyaml/utils/turboyaml_utils.py
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       18 2023-08-09 01:57:13.000000 turboyaml-0.0.4/turboyaml/utils/version.py
+drwxr-xr-x   0 fredbrowne   (501) staff       (20)        0 2023-08-09 02:02:00.968255 turboyaml-0.0.4/turboyaml.egg-info/
+-rw-r--r--   0 fredbrowne   (501) staff       (20)     6198 2023-08-09 02:02:00.000000 turboyaml-0.0.4/turboyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fredbrowne   (501) staff       (20)      416 2023-08-09 02:02:00.000000 turboyaml-0.0.4/turboyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)        1 2023-08-09 02:02:00.000000 turboyaml-0.0.4/turboyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       50 2023-08-09 02:02:00.000000 turboyaml-0.0.4/turboyaml.egg-info/entry_points.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       15 2023-08-09 02:02:00.000000 turboyaml-0.0.4/turboyaml.egg-info/requires.txt
+-rw-r--r--   0 fredbrowne   (501) staff       (20)       10 2023-08-09 02:02:00.000000 turboyaml-0.0.4/turboyaml.egg-info/top_level.txt
```

### Comparing `turboyaml-0.0.3/LICENSE` & `turboyaml-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `turboyaml-0.0.3/PKG-INFO` & `turboyaml-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turboyaml
-Version: 0.0.3
+Version: 0.0.4
 Summary: An AI-powered CLI tool for converting DBT SQL files to YAML using OpenAI.
 Home-page: https://github.com/fredbrowne/turboyaml
 Author: Fred Setra
 Author-email: fred.setra@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 
 To install turboyaml, use the following command:
 
 ```bash
 pip install turboyaml
 ```
 
+Check if the installation was successful:
+
+```bash
+turboyaml --version
+```
+
 ## Usage
 
 To harness the full potential of turboyaml in converting dbt SQL files to YAML, simply follow these steps:
 
 1. **Single File Processing**
 
    - Run turboyaml from the command line, providing your OpenAI API key and the path to the dbt SQL file:
@@ -106,14 +112,17 @@
 
 ## Version History
 
 - 0.0.1 (2023-07-25): Initial release.
 
 - 0.0.2 (2023-07-26): Added support for processing multiple files and unifying the output in a single YAML file. Implemented the `--yaml` parameter to specify the YAML output file. Updated the README with new functionalities and disclaimers. Improved error handling and logging.
 
+- 0.0.3 (2023-07-26): Bug fix and corrected typo
+
+- 0.0.4 (2023-08-08): Refactor of code and implemented async processing for performance optimization.
 
 ## Feedback
 
 We value your feedback! If you have any questions, suggestions, or encounter any issues while using turboyaml, please feel free to open an issue or reach out to us.
 
 Experience the power of AI-driven YAML generation with turboyaml. Say hello to a new era of effortless data modeling and configuration management!
```

### Comparing `turboyaml-0.0.3/README.md` & `turboyaml-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 
 To install turboyaml, use the following command:
 
 ```bash
 pip install turboyaml
 ```
 
+Check if the installation was successful:
+
+```bash
+turboyaml --version
+```
+
 ## Usage
 
 To harness the full potential of turboyaml in converting dbt SQL files to YAML, simply follow these steps:
 
 1. **Single File Processing**
 
    - Run turboyaml from the command line, providing your OpenAI API key and the path to the dbt SQL file:
@@ -89,14 +95,17 @@
 
 ## Version History
 
 - 0.0.1 (2023-07-25): Initial release.
 
 - 0.0.2 (2023-07-26): Added support for processing multiple files and unifying the output in a single YAML file. Implemented the `--yaml` parameter to specify the YAML output file. Updated the README with new functionalities and disclaimers. Improved error handling and logging.
 
+- 0.0.3 (2023-07-26): Bug fix and corrected typo
+
+- 0.0.4 (2023-08-08): Refactor of code and implemented async processing for performance optimization.
 
 ## Feedback
 
 We value your feedback! If you have any questions, suggestions, or encounter any issues while using turboyaml, please feel free to open an issue or reach out to us.
 
 Experience the power of AI-driven YAML generation with turboyaml. Say hello to a new era of effortless data modeling and configuration management!
```

### Comparing `turboyaml-0.0.3/setup.py` & `turboyaml-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="turboyaml",
-    version="0.0.3",
+    version="0.0.4",
     author="Fred Setra",
     author_email="fred.setra@gmail.com",
     description="An AI-powered CLI tool for converting DBT SQL files to YAML using OpenAI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredbrowne/turboyaml",
     packages=find_packages(),
     install_requires=[
         "openai==0.27.8",
-        "pyyaml==6.0.1",
     ],
     entry_points={
         "console_scripts": [
             "turboyaml=turboyaml.cli:main",
         ],
     },
     classifiers=[
```

### Comparing `turboyaml-0.0.3/turboyaml.egg-info/PKG-INFO` & `turboyaml-0.0.4/turboyaml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turboyaml
-Version: 0.0.3
+Version: 0.0.4
 Summary: An AI-powered CLI tool for converting DBT SQL files to YAML using OpenAI.
 Home-page: https://github.com/fredbrowne/turboyaml
 Author: Fred Setra
 Author-email: fred.setra@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 
 To install turboyaml, use the following command:
 
 ```bash
 pip install turboyaml
 ```
 
+Check if the installation was successful:
+
+```bash
+turboyaml --version
+```
+
 ## Usage
 
 To harness the full potential of turboyaml in converting dbt SQL files to YAML, simply follow these steps:
 
 1. **Single File Processing**
 
    - Run turboyaml from the command line, providing your OpenAI API key and the path to the dbt SQL file:
@@ -106,14 +112,17 @@
 
 ## Version History
 
 - 0.0.1 (2023-07-25): Initial release.
 
 - 0.0.2 (2023-07-26): Added support for processing multiple files and unifying the output in a single YAML file. Implemented the `--yaml` parameter to specify the YAML output file. Updated the README with new functionalities and disclaimers. Improved error handling and logging.
 
+- 0.0.3 (2023-07-26): Bug fix and corrected typo
+
+- 0.0.4 (2023-08-08): Refactor of code and implemented async processing for performance optimization.
 
 ## Feedback
 
 We value your feedback! If you have any questions, suggestions, or encounter any issues while using turboyaml, please feel free to open an issue or reach out to us.
 
 Experience the power of AI-driven YAML generation with turboyaml. Say hello to a new era of effortless data modeling and configuration management!
```

