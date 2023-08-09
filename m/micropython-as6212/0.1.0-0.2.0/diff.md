# Comparing `tmp/micropython-as6212-0.1.0.tar.gz` & `tmp/micropython-as6212-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-as6212-0.1.0.tar", last modified: Thu Jun 29 23:19:51 2023, max compression
+gzip compressed data, was "micropython-as6212-0.2.0.tar", last modified: Wed Aug  9 03:06:32 2023, max compression
```

## Comparing `micropython-as6212-0.1.0.tar` & `micropython-as6212-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:51.471953 micropython-as6212-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:51.463953 micropython-as6212-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:51.467953 micropython-as6212-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-29 23:19:51.467953 micropython-as6212-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:51.467953 micropython-as6212-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:51.467953 micropython-as6212-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:51.467953 micropython-as6212-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-29 23:19:43.000000 micropython-as6212-0.1.0/examples/as6212_conversion_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-29 23:19:43.000000 micropython-as6212-0.1.0/examples/as6212_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:51.467953 micropython-as6212-0.1.0/micropython_as6212/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:43.000000 micropython-as6212-0.1.0/micropython_as6212/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-29 23:19:43.000000 micropython-as6212-0.1.0/micropython_as6212/as6212.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-29 23:19:43.000000 micropython-as6212-0.1.0/micropython_as6212/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:19:51.467953 micropython-as6212-0.1.0/micropython_as6212.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-29 23:19:51.000000 micropython-as6212-0.1.0/micropython_as6212.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-29 23:19:51.000000 micropython-as6212-0.1.0/micropython_as6212.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:19:51.000000 micropython-as6212-0.1.0/micropython_as6212.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 23:19:51.000000 micropython-as6212-0.1.0/micropython_as6212.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-29 23:19:43.000000 micropython-as6212-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 23:19:32.000000 micropython-as6212-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:19:51.471953 micropython-as6212-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:32.822589 micropython-as6212-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-09 03:06:24.000000 micropython-as6212-0.2.0/examples/as6212_conversion_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-09 03:06:24.000000 micropython-as6212-0.2.0/examples/as6212_interrupt_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-09 03:06:24.000000 micropython-as6212-0.2.0/examples/as6212_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-09 03:06:24.000000 micropython-as6212-0.2.0/examples/as6212_temp_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/micropython_as6212/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:24.000000 micropython-as6212-0.2.0/micropython_as6212/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-08-09 03:06:24.000000 micropython-as6212-0.2.0/micropython_as6212/as6212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-09 03:06:24.000000 micropython-as6212-0.2.0/micropython_as6212/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/micropython_as6212.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-09 03:06:32.000000 micropython-as6212-0.2.0/micropython_as6212.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-09 03:06:32.000000 micropython-as6212-0.2.0/micropython_as6212.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:06:32.000000 micropython-as6212-0.2.0/micropython_as6212.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-09 03:06:32.000000 micropython-as6212-0.2.0/micropython_as6212.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-09 03:06:24.000000 micropython-as6212-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-09 03:06:16.000000 micropython-as6212-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:06:32.826590 micropython-as6212-0.2.0/setup.cfg
```

### Comparing `micropython-as6212-0.1.0/.pre-commit-config.yaml` & `micropython-as6212-0.2.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
-        exclude: "^(docs/|examples/|tests/|setup.py$)"
+        exclude: "^(docs/|examples/|tests/)"
       - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
           - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-      - id: pylint
-        name: pylint (test code)
-        description: Run pylint rules on "tests/*.py" files
-        types: [python]
-        files: "^tests/"
-        args:
-          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `micropython-as6212-0.1.0/.pylintrc` & `micropython-as6212-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-as6212-0.1.0/LICENSE` & `micropython-as6212-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-as6212-0.1.0/PKG-INFO` & `micropython-as6212-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-as6212
-Version: 0.1.0
+Version: 0.2.0
 Summary: MicroPython Library for the ASM AS6212 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_AS6212
 Keywords: sensor,micropython,as6212,temperature,micropython,asm,as6212,driver,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -38,31 +38,28 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Library for the ASM AS612 Temperature Sensor.
 
-Note to self: Could not make the temp threshold to work. keep changing sensor I2C address and
-getting EIO when the temperature came back to the limit
-
 
 Installing with mip
 ====================
 To install using mpremote
 
 .. code-block:: shell
 
     mpremote mip install github:jposada202020/MicroPython_AS6212
 
 To install directly using a WIFI capable board
 
 .. code-block:: shell
 
-    mip install github:jposada202020/MicroPython_AS6212
+    mip.install("github:jposada202020/MicroPython_AS6212")
 
 
 Installing Library Examples
 ============================
 
 If you want to install library examples:
 
@@ -70,15 +67,15 @@
 
     mpremote mip install github:jposada202020/MicroPython_AS6212/examples.json
 
 To install directly using a WIFI capable board
 
 .. code-block:: shell
 
-    mip install github:jposada202020/MicroPython_AS6212/examples.json
+    mip.install("github:jposada202020/MicroPython_AS6212/examples.json")
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-as6212/>`_.
```

### Comparing `micropython-as6212-0.1.0/README.rst` & `micropython-as6212-0.2.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -21,31 +21,28 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Library for the ASM AS612 Temperature Sensor.
 
-Note to self: Could not make the temp threshold to work. keep changing sensor I2C address and
-getting EIO when the temperature came back to the limit
-
 
 Installing with mip
 ====================
 To install using mpremote
 
 .. code-block:: shell
 
     mpremote mip install github:jposada202020/MicroPython_AS6212
 
 To install directly using a WIFI capable board
 
 .. code-block:: shell
 
-    mip install github:jposada202020/MicroPython_AS6212
+    mip.install("github:jposada202020/MicroPython_AS6212")
 
 
 Installing Library Examples
 ============================
 
 If you want to install library examples:
 
@@ -53,15 +50,15 @@
 
     mpremote mip install github:jposada202020/MicroPython_AS6212/examples.json
 
 To install directly using a WIFI capable board
 
 .. code-block:: shell
 
-    mip install github:jposada202020/MicroPython_AS6212/examples.json
+    mip.install("github:jposada202020/MicroPython_AS6212/examples.json")
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-as6212/>`_.
```

### Comparing `micropython-as6212-0.1.0/docs/_static/Logo.png` & `micropython-as6212-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-as6212-0.1.0/docs/_static/favicon.ico` & `micropython-as6212-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-as6212-0.1.0/docs/conf.py` & `micropython-as6212-0.2.0/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # SPDX-FileCopyrightText: 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
 import datetime
@@ -199,65 +197,7 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # These paths are either relative to html_static_path
 # or fully qualified paths (eg. https://...)
 html_css_files = ["extra_css.css"]
-
-
-# -- Options for LaTeX output ---------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "MicroPython_as6212_Library.tex",
-        "MicroPython as6212 Library Documentation",
-        author,
-        "manual",
-    ),
-]
-
-# -- Options for manual page output ---------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (
-        master_doc,
-        "MicroPython_as6212_Library",
-        "MicroPython as6212 Library Documentation",
-        [author],
-        1,
-    ),
-]
-
-# -- Options for Texinfo output -------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        master_doc,
-        "MicroPython_as6212_Library",
-        "MicroPython as6212 Library Documentation",
-        author,
-        "MicroPython_as6212_Library",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
```

### Comparing `micropython-as6212-0.1.0/examples/as6212_conversion_rate.py` & `micropython-as6212-0.2.0/examples/as6212_conversion_rate.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,12 +11,11 @@
 
 as6.conversion_rate = as6212.RATE_8
 
 while True:
     for conversion_rate in as6212.conversion_rate_values:
         print("Current Conversion rate setting: ", as6.conversion_rate)
         for _ in range(10):
-            temp = as6.temperature
-            print("Temperature: {:.2f}C".format(temp))
+            print(f"Temperature: {as6.temperature:.2f}°C")
             print()
             time.sleep(0.5)
         as6.conversion_rate = conversion_rate
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-as6212-0.1.0/micropython_as6212/i2c_helpers.py` & `micropython-as6212-0.2.0/micropython_as6212/i2c_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 """
 # pylint: disable=too-many-arguments
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
+import struct
 
 
 class CBits:
     """
     Changes bits from a byte register
     """
 
@@ -65,30 +62,28 @@
         self.lsb_first = lsb_first
 
     def __get__(
         self,
         obj,
         objtype=None,
     ) -> int:
-
         mem_value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
 
         reg = 0
         order = range(len(mem_value) - 1, -1, -1)
         if not self.lsb_first:
             order = reversed(order)
         for i in order:
             reg = (reg << 8) | mem_value[i]
 
         reg = (reg & self.bit_mask) >> self.star_bit
 
         return reg
 
     def __set__(self, obj, value: int) -> None:
-
         memory_value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
 
         reg = 0
         order = range(len(memory_value) - 1, -1, -1)
         if not self.lsb_first:
             order = range(0, len(memory_value))
         for i in order:
@@ -114,15 +109,14 @@
         self.lenght = struct.calcsize(form)
 
     def __get__(
         self,
         obj,
         objtype=None,
     ):
-
         if self.lenght <= 2:
             value = struct.unpack(
                 self.format,
                 memoryview(
                     obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
                 ),
             )[0]
```

### Comparing `micropython-as6212-0.1.0/micropython_as6212.egg-info/PKG-INFO` & `micropython-as6212-0.2.0/micropython_as6212.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-as6212
-Version: 0.1.0
+Version: 0.2.0
 Summary: MicroPython Library for the ASM AS6212 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_AS6212
 Keywords: sensor,micropython,as6212,temperature,micropython,asm,as6212,driver,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -38,31 +38,28 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Library for the ASM AS612 Temperature Sensor.
 
-Note to self: Could not make the temp threshold to work. keep changing sensor I2C address and
-getting EIO when the temperature came back to the limit
-
 
 Installing with mip
 ====================
 To install using mpremote
 
 .. code-block:: shell
 
     mpremote mip install github:jposada202020/MicroPython_AS6212
 
 To install directly using a WIFI capable board
 
 .. code-block:: shell
 
-    mip install github:jposada202020/MicroPython_AS6212
+    mip.install("github:jposada202020/MicroPython_AS6212")
 
 
 Installing Library Examples
 ============================
 
 If you want to install library examples:
 
@@ -70,15 +67,15 @@
 
     mpremote mip install github:jposada202020/MicroPython_AS6212/examples.json
 
 To install directly using a WIFI capable board
 
 .. code-block:: shell
 
-    mip install github:jposada202020/MicroPython_AS6212/examples.json
+    mip.install("github:jposada202020/MicroPython_AS6212/examples.json")
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-as6212/>`_.
```

### Comparing `micropython-as6212-0.1.0/micropython_as6212.egg-info/SOURCES.txt` & `micropython-as6212-0.2.0/micropython_as6212.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/as6212_conversion_rate.py
+examples/as6212_interrupt_mode.py
 examples/as6212_simpletest.py
+examples/as6212_temp_limits.py
 micropython_as6212/__init__.py
 micropython_as6212/as6212.py
 micropython_as6212/i2c_helpers.py
 micropython_as6212.egg-info/PKG-INFO
 micropython_as6212.egg-info/SOURCES.txt
 micropython_as6212.egg-info/dependency_links.txt
 micropython_as6212.egg-info/top_level.txt
```

### Comparing `micropython-as6212-0.1.0/pyproject.toml` & `micropython-as6212-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-as6212"
 description = "MicroPython Library for the ASM AS6212 Temperature Sensor"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_AS6212"}
 keywords = [
     "sensor",
```

