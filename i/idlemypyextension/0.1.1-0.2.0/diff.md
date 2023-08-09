# Comparing `tmp/idlemypyextension-0.1.1.tar.gz` & `tmp/idlemypyextension-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idlemypyextension-0.1.1.tar", last modified: Sun Mar 12 05:39:47 2023, max compression
+gzip compressed data, was "idlemypyextension-0.2.0.tar", last modified: Wed Aug  9 05:39:31 2023, max compression
```

## Comparing `idlemypyextension-0.1.1.tar` & `idlemypyextension-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-12 05:39:47.636954 idlemypyextension-0.1.1/
--rw-rw-r--   0 samuel    (1000) samuel    (1000)    11343 2022-11-28 05:34:43.000000 idlemypyextension-0.1.1/LICENSE
--rw-r--r--   0 samuel    (1000) samuel    (1000)    17209 2023-03-12 05:39:47.636954 idlemypyextension-0.1.1/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)     3174 2022-12-22 19:25:18.000000 idlemypyextension-0.1.1/README.md
--rw-r--r--   0 samuel    (1000) samuel    (1000)     1760 2023-03-12 04:57:27.000000 idlemypyextension-0.1.1/pyproject.toml
--rw-r--r--   0 samuel    (1000) samuel    (1000)       38 2023-03-12 05:39:47.636954 idlemypyextension-0.1.1/setup.cfg
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-12 05:39:47.632954 idlemypyextension-0.1.1/src/
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-12 05:39:47.636954 idlemypyextension-0.1.1/src/idlemypyextension/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    30346 2023-03-12 05:38:10.000000 idlemypyextension-0.1.1/src/idlemypyextension/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)    25454 2023-03-12 05:25:38.000000 idlemypyextension-0.1.1/src/idlemypyextension/annotate.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)    13841 2023-03-12 05:26:34.000000 idlemypyextension-0.1.1/src/idlemypyextension/client.py
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-03-12 05:39:47.636954 idlemypyextension-0.1.1/src/idlemypyextension.egg-info/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    17209 2023-03-12 05:39:47.000000 idlemypyextension-0.1.1/src/idlemypyextension.egg-info/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)      360 2023-03-12 05:39:47.000000 idlemypyextension-0.1.1/src/idlemypyextension.egg-info/SOURCES.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-03-12 05:39:47.000000 idlemypyextension-0.1.1/src/idlemypyextension.egg-info/dependency_links.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)       72 2023-03-12 05:39:47.000000 idlemypyextension-0.1.1/src/idlemypyextension.egg-info/entry_points.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)       18 2023-03-12 05:39:47.000000 idlemypyextension-0.1.1/src/idlemypyextension.egg-info/top_level.txt
+drwxrwxr-x   0 samuel    (1000) samuel    (1000)        0 2023-08-09 05:39:31.088277 idlemypyextension-0.2.0/
+-rw-rw-r--   0 samuel    (1000) samuel    (1000)    11340 2023-08-09 04:40:25.000000 idlemypyextension-0.2.0/LICENSE
+-rw-rw-r--   0 samuel    (1000) samuel    (1000)    17145 2023-08-09 05:39:31.084277 idlemypyextension-0.2.0/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     3205 2023-04-27 04:15:40.000000 idlemypyextension-0.2.0/README.md
+-rw-rw-r--   0 samuel    (1000) samuel    (1000)     3656 2023-08-09 05:28:45.000000 idlemypyextension-0.2.0/pyproject.toml
+-rw-rw-r--   0 samuel    (1000) samuel    (1000)       38 2023-08-09 05:39:31.088277 idlemypyextension-0.2.0/setup.cfg
+drwxrwxr-x   0 samuel    (1000) samuel    (1000)        0 2023-08-09 05:39:31.076277 idlemypyextension-0.2.0/src/
+drwxrwxr-x   0 samuel    (1000) samuel    (1000)        0 2023-08-09 05:39:31.084277 idlemypyextension-0.2.0/src/idlemypyextension/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    33781 2023-08-09 05:29:05.000000 idlemypyextension-0.2.0/src/idlemypyextension/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    26640 2023-08-09 05:24:57.000000 idlemypyextension-0.2.0/src/idlemypyextension/annotate.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    18750 2023-08-09 05:26:51.000000 idlemypyextension-0.2.0/src/idlemypyextension/ast_annotate.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    14684 2023-08-09 05:26:02.000000 idlemypyextension-0.2.0/src/idlemypyextension/client.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     3721 2023-08-09 04:57:29.000000 idlemypyextension-0.2.0/src/idlemypyextension/moduleguard.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    14452 2023-08-09 04:56:49.000000 idlemypyextension-0.2.0/src/idlemypyextension/tktrio.py
+drwxrwxr-x   0 samuel    (1000) samuel    (1000)        0 2023-08-09 05:39:31.084277 idlemypyextension-0.2.0/src/idlemypyextension.egg-info/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    17145 2023-08-09 05:39:31.000000 idlemypyextension-0.2.0/src/idlemypyextension.egg-info/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      511 2023-08-09 05:39:31.000000 idlemypyextension-0.2.0/src/idlemypyextension.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-08-09 05:39:31.000000 idlemypyextension-0.2.0/src/idlemypyextension.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       72 2023-08-09 05:39:31.000000 idlemypyextension-0.2.0/src/idlemypyextension.egg-info/entry_points.txt
+-rw-rw-r--   0 samuel    (1000) samuel    (1000)       25 2023-08-09 05:39:31.000000 idlemypyextension-0.2.0/src/idlemypyextension.egg-info/requires.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       18 2023-08-09 05:39:31.000000 idlemypyextension-0.2.0/src/idlemypyextension.egg-info/top_level.txt
```

### Comparing `idlemypyextension-0.1.1/LICENSE` & `idlemypyextension-0.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
    Copyright 2022 CoolCat467
-   
+
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
```

### Comparing `idlemypyextension-0.1.1/PKG-INFO` & `idlemypyextension-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: idlemypyextension
-Version: 0.1.1
-Summary: Mypy extension for Python IDLE
+Version: 0.2.0
+Summary: Mypy daemon extension for Python IDLE
 Author: CoolCat467
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -188,15 +188,15 @@
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
            Copyright 2022 CoolCat467
-           
+        
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
@@ -208,25 +208,23 @@
 Project-URL: Homepage, https://github.com/CoolCat467/idlemypyextension
 Project-URL: Source, https://github.com/CoolCat467/idlemypyextension
 Project-URL: Bug Tracker, https://github.com/CoolCat467/idlemypyextension/issues
 Keywords: mypy,dmypy,idle,extension,development,daemon
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: IDLE
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IdleMypyExtension
 Python IDLE extension to preform mypy analysis on an open file
 
 ## What does this extension do?
@@ -256,24 +254,25 @@
 If everything went well, alongside `ZzDummy` there should be and
 option called `idlemypyextension`. This is where you can configure how
 idlemypyextension works.
 
 
 ## Information on options
 `action_max_sec` controls how long an action is allowed to take at most,
-in seconds.
-Values under 5 will make no effect
+in seconds. Default is "None".
 
 For `daemon_flags`, see `mypy --help` for a list of valid flags.
 This extension sets the following flags to be able to work properly:
 ```
     --hide-error-context
     --no-color-output
     --show-absolute-path
     --no-error-summary
+    --soft-error-limit=-1
+    --show-traceback
     --cache-dir="~/.idlerc/mypy"
 ```
 
 If you add the `--show-column-numbers` flag to `daemon_flags`, when using the
 "Type Check File" command, it will add a helpful little `^` sign
 in a new line below the location of the mypy message that provided a column
 number, as long as that comment wouldn't break your file's indentation too much.
```

### Comparing `idlemypyextension-0.1.1/README.md` & `idlemypyextension-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,25 @@
 If everything went well, alongside `ZzDummy` there should be and
 option called `idlemypyextension`. This is where you can configure how
 idlemypyextension works.
 
 
 ## Information on options
 `action_max_sec` controls how long an action is allowed to take at most,
-in seconds.
-Values under 5 will make no effect
+in seconds. Default is "None".
 
 For `daemon_flags`, see `mypy --help` for a list of valid flags.
 This extension sets the following flags to be able to work properly:
 ```
     --hide-error-context
     --no-color-output
     --show-absolute-path
     --no-error-summary
+    --soft-error-limit=-1
+    --show-traceback
     --cache-dir="~/.idlerc/mypy"
 ```
 
 If you add the `--show-column-numbers` flag to `daemon_flags`, when using the
 "Type Check File" command, it will add a helpful little `^` sign
 in a new line below the location of the mypy message that provided a column
 number, as long as that comment wouldn't break your file's indentation too much.
```

### Comparing `idlemypyextension-0.1.1/src/idlemypyextension/__init__.py` & `idlemypyextension-0.2.0/src/idlemypyextension/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Idle Type Check - Use mypy to type check open file, then add comments to file.
-
-"Type Check IDLE Extension"
+"""Type Check IDLE Extension."""
 
 # Programmed by CoolCat467
 
 from __future__ import annotations
 
 __title__ = "idlemypyextension"
 __author__ = "CoolCat467"
 __license__ = "GPLv3"
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __ver_major__ = 0
-__ver_minor__ = 1
-__ver_patch__ = 1
+__ver_minor__ = 2
+__ver_patch__ = 0
 
 import json
 import math
 import os
 import re
 import sys
 import traceback
 from collections.abc import Callable
-from functools import wraps
+from dataclasses import dataclass
+from functools import partial, wraps
 from idlelib import search, searchengine
 from idlelib.config import idleConf
 from idlelib.format import FormatRegion
 from idlelib.iomenu import IOBinding
-from idlelib.multicall import MultiCallCreator
 from idlelib.pyshell import PyShellEditorWindow, PyShellFileList
-from tkinter import Event, Tk, messagebox
-from typing import Any, Final, TypeVar, cast
+from idlelib.undo import UndoDelegator
+from tkinter import Event, Text, Tk, messagebox
+from typing import Any, ClassVar, Final, TypeVar, cast
 
-from idlemypyextension import annotate
+from idlemypyextension import annotate, tktrio
 
 DAEMON_TIMEOUT_MIN: Final = 5
 ACTION_TIMEOUT_MIN: Final = 5
 
 _HAS_MYPY = True
 try:
     from idlemypyextension import client
+
+    # Client imports lots of things from mypy
 except ImportError:
     print(f"{__file__}: Mypy not installed!")
     _HAS_MYPY = False
 
 
+def debug(message: str) -> None:
+    """Print debug message."""
+    # TODO: Censor username
+    print(f"\n[{__title__}] DEBUG: {message}")
+
+
 def get_required_config(
-    values: dict[str, str], bind_defaults: dict[str, str]
+    values: dict[str, str],
+    bind_defaults: dict[str, str],
 ) -> str:
-    "Get required configuration file data"
+    """Get required configuration file data."""
     config = ""
     # Get configuration defaults
     settings = "\n".join(
         f"{key} = {default}" for key, default in values.items()
     )
     if settings:
         config += f"\n[{__title__}]\n{settings}"
@@ -65,178 +71,186 @@
     )
     if settings:
         config += f"\n[{__title__}_cfgBindings]\n{settings}"
     return config
 
 
 def check_installed() -> bool:
-    "Make sure extension installed."
+    """Make sure extension installed."""
     # Get list of system extensions
     extensions = list(idleConf.defaultCfg["extensions"])
     ex_defaults = idleConf.defaultCfg["extensions"].file
 
     # Import this extension (this file),
     module = __import__(__title__)
 
     # Get extension class
     if not hasattr(module, __title__):
         print(
-            f"ERROR: Somehow, {__title__} was installed improperly, no {__title__} class "
-            "found in module. Please report this on github.",
+            f"ERROR: Somehow, {__title__} was installed improperly, "
+            f"no {__title__} class found in module. Please report "
+            "this on github.",
             file=sys.stderr,
         )
         sys.exit(1)
 
     cls = getattr(module, __title__)
 
     # Get extension class keybinding defaults
     required_config = get_required_config(
-        getattr(cls, "values", {}), getattr(cls, "bind_defaults", {})
+        getattr(cls, "values", {}),
+        getattr(cls, "bind_defaults", {}),
     )
 
     # If this extension not in there,
     if __title__ not in extensions:
         # Tell user how to add it to system list.
         print(f"{__title__} not in system registered extensions!")
         print(
-            f"Please run the following command to add {__title__} to system extensions list.\n"
+            f"Please run the following command to add {__title__} "
+            + "to system extensions list.\n",
         )
         # Make sure line-breaks will go properly in terminal
         add_data = required_config.replace("\n", "\\n")
-        # Tell them command
+        # Tell them the command
         print(f"echo -e '{add_data}' | sudo tee -a {ex_defaults}")
         print()
     else:
         print(f"Configuration should be good! (v{__version__})")
         return True
     return False
 
 
 def get_line_selection(line: int) -> tuple[str, str]:
-    "Get selection strings for given line"
+    """Get selection strings for given line."""
     return f"{line}.0", f"{line+1}.0"
 
 
 # Stolen from idlelib.searchengine
 def get_line_col(index: str) -> tuple[int, int]:
-    "Return (line, col) tuple of integers from 'line.col' string."
+    """Return (line, col) tuple of integers from 'line.col' string."""
     line, col = map(int, index.split(".", 1))  # Fails on invalid index
     return line, col
 
 
 def get_line_indent(text: str, char: str = " ") -> int:
-    "Return line indent."
+    """Return line indent."""
     for idx, cur in enumerate(text.split(char)):
         if cur != "":
             return idx
     return 0
 
 
 def ensure_section_exists(section: str) -> bool:
-    "Ensure section exists in user extensions configuration, return if edited"
-    if not section in idleConf.GetSectionList("user", "extensions"):
+    """Ensure section exists in user extensions configuration/.
+
+    Returns True if edited.
+    """
+    if section not in idleConf.GetSectionList("user", "extensions"):
         idleConf.userCfg["extensions"].AddSection(section)
         return True
     return False
 
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 def undo_block(func: F) -> F:
-    "Mark block of edits as a single undo block."
+    """Mark block of edits as a single undo block."""
 
     @wraps(func)
     def undo_wrapper(
-        self: "idlemypyextension", *args: Any, **kwargs: Any
+        self: idlemypyextension,
+        *args: Any,
+        **kwargs: Any,
     ) -> Any:
-        "Wrap function in start and stop undo events."
-        self.text.undo_block_start()
+        """Wrap function in start and stop undo events."""
+        self.undo.undo_block_start()
         try:
             return func(self, *args, **kwargs)
         finally:
-            self.text.undo_block_stop()
+            self.undo.undo_block_stop()
 
     return cast(F, undo_wrapper)
 
 
 def ensure_values_exist_in_section(
-    section: str, values: dict[str, str]
+    section: str,
+    values: dict[str, str],
 ) -> bool:
-    """For each key in values, make sure key exists. Return if edited
+    """For each key in values, make sure key exists. Return if edited.
 
-    If not, create and set to value."""
+    If not, create and set to value.
+    """
     need_save = False
     for key, default in values.items():
         value = idleConf.GetOption(
-            "extensions", section, key, warn_on_default=False
+            "extensions",
+            section,
+            key,
+            warn_on_default=False,
         )
         if value is None:
             idleConf.SetOption("extensions", section, key, default)
             need_save = True
     return need_save
 
 
 def get_search_engine_params(
     engine: searchengine.SearchEngine,
 ) -> dict[str, str | bool]:
-    "Get current search engine parameters"
+    """Get current search engine parameters."""
     return {
         name: getattr(engine, f"{name}var").get()
         for name in ("pat", "re", "case", "word", "wrap", "back")
     }
 
 
 def set_search_engine_params(
-    engine: searchengine.SearchEngine, data: dict[str, str | bool]
+    engine: searchengine.SearchEngine,
+    data: dict[str, str | bool],
 ) -> None:
-    "Get current search engine parameters"
+    """Get current search engine parameters."""
     for name in ("pat", "re", "case", "word", "wrap", "back"):
         if name in data:
             getattr(engine, f"{name}var").set(data[name])
 
 
-# def get_fake_editwin() -> PyShellEditorWindow:
-#     "Get fake edit window for testing"
-#     from idlelib.pyshell import PyShellEditorWindow
-#
-#     class FakeEditWindow(PyShellEditorWindow):  type: ignore[misc]
-#         "FakeEditWindow for testing"
-#         def __init__(self) -> None:
-#             return
-#
-#         from tkinter import Text
-#
-#         class _FakeText(Text):
-#             Make bind do nothing
-#             bind = lambda x, y: None  type: ignore[assignment]
-#
-#         text = _FakeText
-#         fregion = FormatRegion
-#         flist = PyShellFileList
-#         io = IOBinding
-#     return FakeEditWindow()
+@dataclass(slots=True)
+class Message:
+    """Represents one message from mypy."""
+
+    file: str
+    line: int
+    message: str
+    line_end: int | None = None
+    column: int = 0
+    column_end: int | None = None
+    msg_type: str = "unrecognized"
 
 
 # Important weird: If event handler function returns 'break',
 # then it prevents other bindings of same event type from running.
 # If returns None, normal and others are also run.
 
 
-class idlemypyextension:  # pylint: disable=invalid-name
-    "Add comments from mypy to an open program."
+class idlemypyextension:  # noqa: N801
+    """Add comments from mypy to an open program."""
+
     __slots__ = (
         "editwin",
         "text",
+        "undo",
         "formatter",
         "files",
         "flist",
+        "triorun",
     )
     # Extend the file and format menus.
-    menudefs = [
+    menudefs: ClassVar = [
         (
             "edit",
             [
                 None,
                 ("_Type Check File", "<<type-check>>"),
                 ("Find Next Type Comment", "<<find-next-type-comment>>"),
             ],
@@ -247,172 +261,206 @@
                 ("Suggest Signature", "<<suggest-signature>>"),
                 ("Remove Type Comments", "<<remove-type-comments>>"),
             ],
         ),
         ("run", [("Shutdown dmypy daemon", "<<shutdown-dmypy-daemon>>")]),
     ]
     # Default values for configuration file
-    values = {
+    values: ClassVar = {
         "enable": "True",
         "enable_editor": "True",
         "enable_shell": "False",
         "daemon_flags": "None",
         "search_wrap": "True",
         "suggest_replace": "False",
         "timeout_mins": "30",
-        "action_max_sec": "40",
+        "action_max_sec": "None",
     }
     # Default key binds for configuration file
-    bind_defaults = {
+    bind_defaults: ClassVar = {
         "type-check": "<Alt-Key-t>",
         "suggest-signature": "<Alt-Key-s>",
         "remove-type-comments": "<Alt-Shift-Key-T>",
         "find-next-type-comment": "<Alt-Key-g>",
     }
     comment = "# types: "
 
     # Overwritten in reload
     daemon_flags = "None"
     search_wrap = "True"
     suggest_replace = "False"
     timeout_mins = "30"
-    action_max_sec = "40"
+    action_max_sec = "None"
 
     # Class attributes
     idlerc_folder = os.path.expanduser(idleConf.userdir)
     mypy_folder = os.path.join(idlerc_folder, "mypy")
     status_file = os.path.join(mypy_folder, "dmypy.json")
     log_file = os.path.join(mypy_folder, "log.txt")
 
     def __init__(self, editwin: PyShellEditorWindow) -> None:
-        "Initialize the settings for this extension."
+        """Initialize the settings for this extension."""
         self.editwin: PyShellEditorWindow = editwin
-        self.text: MultiCallCreator = editwin.text
+        self.text: Text = editwin.text
+        self.undo: UndoDelegator = editwin.undo
         self.formatter: FormatRegion = editwin.fregion
         self.flist: PyShellFileList = editwin.flist
         self.files: IOBinding = editwin.io
 
         if not os.path.exists(self.mypy_folder):
             os.mkdir(self.mypy_folder)
 
+        self.triorun = tktrio.TkTrioRunner(
+            self.editwin.top,
+            self.editwin.close,
+        )
+
         for attr_name in dir(self):
             if attr_name.startswith("_"):
                 continue
-            if attr_name.endswith("_event"):
-                bind_name = "-".join(attr_name.split("_")[:-1]).lower()
-                self.text.bind(f"<<{bind_name}>>", getattr(self, attr_name))
+            if attr_name.endswith("_event_async"):
+                bind_name = "-".join(attr_name.split("_")[:-2]).lower()
+                self.text.bind(f"<<{bind_name}>>", self.get_async(attr_name))
                 # print(f'{attr_name} -> {bind_name}')
 
+    def get_async(
+        self,
+        name: str,
+    ) -> Callable[[Event[Any]], str]:
+        """Get sync callable to run async function."""
+        async_function = getattr(self, name)
+
+        @wraps(async_function)
+        def call_trio(event: Event[Any]) -> str:
+            self.triorun(partial(async_function, event))
+            return "break"
+
+        return call_trio
+
     def __repr__(self) -> str:
+        """Return representation of self."""
         return f"{self.__class__.__name__}({self.editwin!r})"
 
     @property
     def daemon_timeout(self) -> int:
-        "Daemon timeout"
+        """Daemon timeout."""
         if self.timeout_mins == "None":
             return DAEMON_TIMEOUT_MIN * 60
         try:
             return max(
                 DAEMON_TIMEOUT_MIN * 60,
                 math.ceil(float(self.timeout_mins) * 60),
             )
         except ValueError:
             return DAEMON_TIMEOUT_MIN * 60
 
     @property
     def action_timeout(self) -> int | None:
-        "Action timeout"
+        """Action timeout."""
         if self.action_max_sec == "None":
             return None
         try:
             return max(ACTION_TIMEOUT_MIN, int(self.action_max_sec))
         except ValueError:
             return max(ACTION_TIMEOUT_MIN, int(self.values["action_max_sec"]))
 
     @property
     def flags(self) -> list[str]:
-        "Daemon server flags"
+        """Mypy Daemon flags."""
         base = {
-            f"--cache-dir={self.mypy_folder}",
-            "--cache-fine-grained",
             "--hide-error-context",
             "--no-color-output",
             "--show-absolute-path",
             "--no-error-summary",
             "--soft-error-limit=-1",
             "--show-traceback",
+            f"--cache-dir={self.mypy_folder}",
+            # f"--log-file={self.log_file}",
+            # "--cache-fine-grained",
         }
         if self.daemon_flags == "None":
             return list(base)
-        return list(base | {s.strip() for s in self.daemon_flags.split(" ")})
+        extra = set()
+        for arg in self.daemon_flags.split(" "):
+            value = arg.strip()
+            if value:
+                extra.add(value)
+        return list(base | extra)
 
     @classmethod
     def ensure_bindings_exist(cls) -> bool:
-        "Ensure key bindings exist in user extensions configuration. Return True if need to save."
+        """Ensure key bindings exist in user extensions configuration.
+
+        Return True if need to save.
+        """
         need_save = False
         section = f"{cls.__name__}_cfgBindings"
         if ensure_section_exists(section):
             need_save = True
         if ensure_values_exist_in_section(section, cls.bind_defaults):
             need_save = True
         return need_save
 
     @classmethod
     def ensure_config_exists(cls) -> bool:
-        "Ensure required configuration exists for this extension. Return True if need to save."
+        """Ensure required configuration exists for this extension.
+
+        Return True if need to save.
+        """
         need_save = False
         if ensure_section_exists(cls.__name__):
             need_save = True
         if ensure_values_exist_in_section(cls.__name__, cls.values):
             need_save = True
         return need_save
 
     @classmethod
     def reload(cls) -> None:
-        "Load class variables from configuration."
+        """Load class variables from configuration."""
         # # Ensure file default values exist so they appear in settings menu
         # save = cls.ensure_configuration_exists()
         # if cls.ensure_bindings_exist() or save:
         #     idleConf.SaveUserCfgFiles()
 
         # Reload configuration file
         idleConf.LoadCfgFiles()
 
         # For all possible configuration values
         for key, default in cls.values.items():
             # Set attribute of key name to key value from configuration file
-            if not key in {"enable", "enable_editor", "enable_shell"}:
+            if key not in {"enable", "enable_editor", "enable_shell"}:
                 value = idleConf.GetOption(
-                    "extensions", cls.__name__, key, default=default
+                    "extensions",
+                    cls.__name__,
+                    key,
+                    default=default,
                 )
                 setattr(cls, key, value)
 
     @classmethod
     def get_msg_line(cls, indent: int, msg: str) -> str:
-        "Return message line given indent and message."
+        """Return message line given indent and message."""
         strindent = " " * indent
         return f"{strindent}{cls.comment}{msg}"
 
     def get_line(self, line: int) -> str:
-        "Get the characters from the given line in the currently open file."
+        """Get the characters from the given line in currently open file."""
         chars: str = self.text.get(*get_line_selection(line))
         return chars
 
     def comment_exists(self, line: int, text: str) -> bool:
-        "Return True if comment for message already exists on line."
+        """Return True if comment for message already exists on line."""
         return self.get_msg_line(0, text) in self.get_line(line - 1)
 
-    def add_comment(
-        self, message: dict[str, str | int], max_exist_up: int = 0
-    ) -> bool:
-        "Return True if added new comment, False if already exists."
+    def add_comment(self, message: Message, max_exist_up: int = 0) -> bool:
+        """Return True if added new comment, False if already exists."""
         # Get line and message from output
-        # file = str(message['file'])
-        line = int(message["line"])
-        msg = str(message["message"])
+        # file = message.file
+        line = message.line
+        msg = message.message
 
         # If there is already a comment from us there, ignore that line.
         # +1-1 is so at least up by 1 is checked, range(0) = []
         for i in range(max_exist_up + 1):
             if self.comment_exists(line - (i - 1), msg):
                 return False
 
@@ -429,32 +477,36 @@
         start, end = get_line_selection(line)
         self.text.delete(start, end)
         self.text.insert(start, chars, ())
         return True
 
     @staticmethod
     def parse_comments(
-        comments: str, default_file: str, default_line: int
-    ) -> dict[str, list[dict[str, str | int]]]:
-        "Get list of message dictionaries from mypy output."
+        comments: str,
+        default_file: str,
+        default_line: int,
+    ) -> dict[str, list[Message]]:
+        """Get list of message dictionaries from mypy output."""
         error_type = re.compile(r"  \[[a-z\-]+\]\s*$")
 
-        files: dict[str, list[dict[str, str | int]]] = {}
+        files: dict[str, list[Message]] = {}
         for comment in comments.splitlines():
+            if not comment.strip():
+                continue
             filename = default_file
             line = default_line
             line_end = default_line
             col = 0
             col_end = 0
-            mtype = "unrecognized"
+            msg_type = "unrecognized"
 
             if comment.count(": ") < 2:
                 text = comment
             else:
-                where, mtype, text = comment.split(": ", 2)
+                where, msg_type, text = comment.split(": ", 2)
 
                 position = where.split(":")
 
                 filename = position[0]
                 if len(position) > 1:
                     line = int(position[1])
                     line_end = line
@@ -466,99 +518,113 @@
                     if line_end == line:
                         col_end = int(position[4])
                     else:
                         line_end = line
             comment_type = error_type.search(text)
             if comment_type is not None:
                 text = text[: comment_type.start()]
-                mtype = f"{comment_type.group(0)[3:-1]} {mtype}"
+                msg_type = f"{comment_type.group(0)[3:-1]} {msg_type}"
 
-            message: dict[str, str | int] = {
-                "file": filename,
-                "line": line,
-                "column": col,
-                "line_end": line_end,
-                "column_end": col_end,
-                "type": mtype,
-                "message": f"{mtype}: {text}",
-            }
+            message = Message(
+                file=filename,
+                line=line,
+                message=f"{msg_type}: {text}",
+                column=col,
+                line_end=line_end,
+                column_end=col_end,
+                msg_type=msg_type,
+            )
 
-            if not filename in files:
+            if filename not in files:
                 files[filename] = []
             files[filename].append(message)
         return files
 
-    def get_pointers(
-        self, messages: list[dict[str, int | str]]
-    ) -> dict[str, int | str] | None:
-        "Return message pointing to message column position"
-        line = int(messages[0]["line"]) + 1
+    def get_pointers(self, messages: list[Message]) -> Message | None:
+        """Return message pointing to multiple messages all on the same line.
+
+        Messages must all be on the same line and be in the same file
+        """
+        line = messages[0].line
+        file = messages[0].file
 
         # Figure out line intent
-        line_text = self.get_line(line)
+        line_text = self.get_line(line + 1)
         indent = get_line_indent(line_text)
         line_len = len(line_text)
 
         columns: set[int] = set()
         lastcol = len(self.comment) + indent + 1
 
         for message in messages:
-            start = int(message["column"])
-            end = int(message.get("column_end", start + lastcol)) - lastcol
-            for col in range(start, end + 1):
+            if message.line != line:
+                raise ValueError(f"Message `{message}` not on line `{line}`")
+            if message.file != file:
+                raise ValueError(f"Message `{message}` not in file `{file}`")
+            if message.column_end is None:
+                end = message.column
+            else:
+                end = message.column_end - lastcol
+            for col in range(message.column, end + 1):
                 columns.add(col)
 
         new_line = ""
         for col in sorted(columns):
             if col > line_len:
                 break
             spaces = col - lastcol - 1
             new_line += " " * spaces + "^"
             lastcol = col
 
         if not new_line.strip():
             return None
 
-        return {"line": line, "message": new_line}
+        return Message(file=file, line=line + 1, message=new_line)
 
+    @undo_block
     def add_comments(
-        self, target_filename: str, start_line: int, normal: str
+        self,
+        target_filename: str,
+        start_line: int,
+        normal: str,
     ) -> list[int]:
-        "Add comments for target filename, return list of comments added"
+        """Add comments for target filename, return list of comments added."""
+        assert self.files.filename is not None
         files = self.parse_comments(
-            normal, os.path.abspath(self.files.filename), start_line
+            normal,
+            os.path.abspath(self.files.filename),
+            start_line,
         )
 
         # Only handling messages for target filename
-        line_data: dict[int, list[dict[str, Any]]] = {}
+        line_data: dict[int, list[Message]] = {}
         if target_filename in files:
             for message in files[target_filename]:
-                line = message["line"]
-                assert isinstance(line, int), "Line must be int"
-                if not line in line_data:
-                    line_data[line] = []
-                line_data[line].append(message)
+                if message.line not in line_data:
+                    line_data[message.line] = []
+                line_data[message.line].append(message)
 
-        line_order: list[int] = list(sorted(line_data, reverse=True))
+        line_order: list[int] = sorted(line_data, reverse=True)
         first: int = line_order[-1] if line_order else start_line
 
-        if not first in line_data:  # if used starting line
+        if first not in line_data:  # if used starting line
             line_data[first] = []
             line_order.append(first)
 
-        for filename in {f for f in files if f != target_filename}:
+        for filename in files:
+            if filename == target_filename:
+                continue
             line_data[first].append(
-                {
-                    "file": target_filename,
-                    "line": first,
-                    "column": 0,
-                    "column_end": 0,
-                    "type": "note",
-                    "message": f"Another file has errors: {filename}",
-                }
+                Message(
+                    file=target_filename,
+                    line=first,
+                    message=f"note: Another file has errors: {filename}",
+                    column_end=0,
+                    msg_type="note",
+                ),
             )
 
         comments = []
         for line in line_order:
             messages = line_data[line]
             if not messages:
                 continue
@@ -568,294 +634,349 @@
 
             total = len(messages)
             for message in reversed(messages):
                 if self.add_comment(message, total):
                     comments.append(line)
         return comments
 
+    @undo_block
+    def add_errors(self, file: str, start_line: int, errors: str) -> None:
+        """Add errors to file."""
+        lines = errors.splitlines()
+        lines[0] = f"Error running mypy: {lines[0]}"
+        for message in reversed(lines):
+            self.add_comment(
+                Message(
+                    file=file,
+                    line=start_line,
+                    message=message,
+                ),
+                len(lines),
+            )
+
     def ask_save_dialog(self) -> bool:
-        "Ask to save dialog stolen from idlelib.runscript.ScriptBinding"
+        """Ask to save dialog stolen from idlelib.runscript.ScriptBinding."""
         msg = "Source Must Be Saved\n" + 5 * " " + "OK to Save?"
         confirm: bool = messagebox.askokcancel(
             title="Save Before Run or Check",
             message=msg,
             default=messagebox.OK,
             parent=self.text,
         )
         return confirm
 
-    def ensure_daemon_running(self) -> bool:
-        "Make sure daemon is running. Return False if cannot continue"
+    async def ensure_daemon_running(self) -> bool:
+        """Make sure daemon is running. Return False if cannot continue."""
         if not client.is_running(self.status_file):
-            started = client.start(
+            return await client.start(
                 self.status_file,
                 flags=self.flags,
                 daemon_timeout=self.daemon_timeout,
                 log_file=self.log_file,
             )
-            return started
         return True
 
-    def shutdown_dmypy_daemon_event(self, event: "Event[Any]") -> str:
-        "Shutdown the dmypy daemon"
+    async def shutdown_dmypy_daemon_event_async(
+        self,
+        event: Event[Any],
+    ) -> str:
+        """Shutdown dmypy daemon event handler."""
         # pylint: disable=unused-argument
         if not client.is_running(self.status_file):
             self.text.bell()
             return "break"
+
         # Only stop if running
-        response = client.stop(self.status_file)
-        if any((v in response and response[v] for v in ("err", "error"))):
+        response = await client.stop(self.status_file)
+        if any(v in response and response[v] for v in ("err", "error")):
             # Kill
             client.kill(self.status_file)
+
         return "break"
 
-    def check(self, file: str) -> dict[str, Any]:
-        "Preform dmypy check"
-        if not self.ensure_daemon_running():
+    async def check(self, file: str) -> dict[str, Any]:
+        """Preform dmypy check."""
+        if not await self.ensure_daemon_running():
             return {"out": "", "err": "Error: Could not start mypy daemon"}
         flags = self.flags
         flags += [file]
-        return client.run(
+        # debug(f"check {flags = }")
+        command = " ".join(
+            [
+                "dmypy",
+                f"--status-file={self.status_file}",
+                f"--log-file={self.log_file}",
+                "run",
+                file,
+                "--",
+                *self.flags,
+            ],
+        )
+        debug(f"{command = }")
+        return await client.run(
             self.status_file,
             flags=flags,
             timeout=self.action_timeout,
             daemon_timeout=self.daemon_timeout,
             log_file=self.log_file,
             export_types=True,
         )
 
-    def get_suggestion_text(self, annotation: dict[str, Any]) -> str | None:
+    def get_suggestion_text(
+        self,
+        annotation: dict[str, Any],
+    ) -> tuple[str | None, int]:
         """Get suggestion text from annotation.
 
-        Return None on error or no difference, text if different"""
-        while annotation["line"] >= 0 and not "def" in self.get_line(
-            annotation["line"]
+        Return None on error or no difference, text if different
+        """
+        while annotation["line"] >= 0 and "def" not in self.get_line(
+            annotation["line"],
         ):
             annotation["line"] -= 1
         line = annotation["line"]
 
         try:
-            text = annotate.get_annotation(annotation, self.get_line)
+            text, line_count = annotate.get_annotation(
+                annotation,
+                self.get_line,
+            )
         except annotate.ParseError as ex:
             ex_text, ex_traceback = sys.exc_info()[1:]
             traceback.print_exception(
                 None,  # Ignored since python 3.5
                 value=ex_text,
                 tb=ex_traceback,
                 limit=None,
                 chain=True,
             )
             indent = get_line_indent(self.get_line(line))
-            return self.get_msg_line(
-                indent, f"Error generating suggestion: {ex}"
+            return (
+                self.get_msg_line(
+                    indent,
+                    f"Error generating suggestion: {ex}",
+                ),
+                1,
             )
 
         select_start = f"{line}.0"
-        line_end = line + len(text.splitlines())
+        line_end = line + line_count
         select_end = f"{line_end}.0"
 
         if text == self.text.get(select_start, select_end)[:-1]:
-            return None
-        return text
+            return None, line_count
+        return text, line_count
 
-    def suggest(self, file: str, line: int) -> None:
-        "Preform dmypy suggest"
-        if not self.ensure_daemon_running():
+    async def suggest(self, file: str, line: int) -> None:
+        """Preform dmypy suggest."""
+        if not await self.ensure_daemon_running():
             response = {"err": "Error: Could not start mypy daemon"}
         else:
             function = f"{file}:{line}"
-            response = client.suggest(
+            response = await client.suggest(
                 self.status_file,
                 function=function,
                 do_json=True,
                 timeout=self.action_timeout,
             )
-        # print(f'{__title__} DEBUG: suggest {response = }')
+        # debug(f'suggest {response = }')
 
+        normal = ""
         errors = ""
         if "error" in response:
             errors += response["error"]
         if "err" in response:
+            if errors:
+                errors += "\n"
             errors += response["err"]
+        if "stderr" in response:
+            if normal:
+                normal += "\n"
+            normal += response["stderr"]
 
         # Display errors
         if errors:
-            lines = errors.splitlines()
-            lines[0] = f"Error running mypy: {lines[0]}"
-            for message in reversed(lines):
-                self.add_comment(
-                    {
-                        "file": file,
-                        "line": line,
-                        "message": message,
-                    },
-                    len(lines),
-                )
+            # Add mypy errors
+            self.add_errors(file, self.editwin.getlineno(), errors)
 
             self.text.bell()
             return
 
         annotations = json.loads(response["out"])
 
         line = annotations[0]["line"]
 
         samples: dict[int, list[str]] = {}
+        line_count = 0
         for annotation in annotations:
             count = annotation["samples"]
-            text = self.get_suggestion_text(annotation)
+            text, suggest_lines = self.get_suggestion_text(annotation)
             if text is None:
                 continue
-            if not count in samples:
+            if count not in samples:
                 samples[count] = []
             samples[count].append(text)
+            line_count += suggest_lines
 
         order = sorted(samples, reverse=True)
         lines = []
         for count in order:
             for sample in samples[count]:
-                if not sample in lines:
+                if sample not in lines:
                     lines.append(sample)
 
         replace = self.suggest_replace == "True"
 
         if len(lines) == 1:
             text = lines[0]
             if "Error generating suggestion: " in text:
                 replace = False
         else:
             text = "\n".join(lines)
             replace = False
 
         select_start = f"{line}.0"
-        line_end = line + len(text.splitlines())
+        line_end = line + line_count
         select_end = f"{line_end}.0"
 
         if not text or text == self.text.get(select_start, select_end)[:-1]:
             # Bell to let user know happened, just nothing to do
             self.editwin.gotoline(line)
             self.text.bell()
             return
 
-        if replace:
-            self.text.delete(select_start, select_end)
-        elif "Error generating suggestion: " not in text:
-            text = "\n".join(f"##{l}" for l in text.splitlines())
+        if not replace and "Error generating suggestion: " not in text:
+            text = "\n".join(f"##{line}" for line in text.splitlines())
         text += "\n"
 
-        self.text.insert(select_start, text, None)
-        self.editwin.gotoline(line)
-        self.text.bell()
-
-    @undo_block
-    def suggest_signature_event(self, event: "Event[Any]") -> str:
-        "Handle suggest signature event"
-        # pylint: disable=unused-argument
-        init_return, file, start_line_no = self.initial()
-        if init_return is not None:
-            return init_return
+        self.undo.undo_block_start()
+        try:
+            if replace:
+                self.text.delete(select_start, select_end)
 
-        self.suggest(file, start_line_no)
+            self.text.insert(select_start, text, ())
+        finally:
+            self.undo.undo_block_stop()
 
-        return "break"
+        self.editwin.gotoline(line)
+        self.text.bell()
 
-    def initial(self) -> tuple[str | None, str, int]:
-        """Do common initial setup. Return error or none, file, and start line
+    def initial(self) -> tuple[str | None, str | None]:
+        """Do common initial setup. Return error or none, file, and start line.
 
         Reload configuration, make sure file is saved,
-        and make sure mypy is installed"""
+        and make sure mypy is installed
+        """
         self.reload()
 
         # Get file we are checking
-        file: str = os.path.abspath(self.files.filename)
+        raw_filename: str | None = self.files.filename
+        if raw_filename is None:
+            return "break", None
+        file: str = os.path.abspath(raw_filename)
 
         # Remember where we started
         start_line_no: int = self.editwin.getlineno()
 
         if not _HAS_MYPY:
             self.add_comment(
-                {
-                    "file": file,
-                    "line": start_line_no,
-                    "message": "Could not import mypy. "
-                    "Please install mypy and restart IDLE to use this extension.",
-                },
+                Message(
+                    file=file,
+                    line=start_line_no,
+                    message="Could not import mypy. "
+                    "Please install mypy and restart IDLE "
+                    + "to use this extension.",
+                ),
                 start_line_no,
             )
 
             # Make bell sound so user knows they need to pay attention
             self.text.bell()
-            return "break", file, start_line_no
+            return "break", file
 
         # Make sure file is saved.
         if not self.files.get_saved():
             if not self.ask_save_dialog():
                 # If not ok to save, do not run. Would break file.
                 self.text.bell()
-                return "break", file, start_line_no
+                return "break", file
             # Otherwise, we are clear to save
             self.files.save(None)
             self.files.set_saved(True)
 
         # Everything worked
-        return None, file, start_line_no
+        return None, file
 
-    @undo_block
-    def type_check_event(self, event: "Event[Any]") -> str:
-        "Preform a mypy check and add comments."
+    async def suggest_signature_event_async(self, event: Event[Any]) -> str:
+        """Handle suggest signature event."""
         # pylint: disable=unused-argument
-        init_return, file, start_line_no = self.initial()
+        init_return, file = self.initial()
 
         if init_return is not None:
             return init_return
+        if file is None:
+            return "break"
+
+        await self.suggest(file, self.editwin.getlineno())
+
+        return "break"
+
+    async def type_check_event_async(self, event: Event[Any]) -> str:
+        """Preform a mypy check and add comments."""
+        init_return, file = self.initial()
+
+        if init_return is not None:
+            return init_return
+        if file is None:
+            return "break"
 
         # Run mypy on open file
-        response = self.check(file)
+        response = await self.check(file)
 
-        print(f"{__title__} DEBUG: type check {response = }")
+        debug(f"type check {response = }")
 
         normal = ""
+        errors = ""
         if "out" in response:
             normal = response["out"]
-        errors = ""
-        if "err" in response:
-            errors = response["err"]
         if "error" in response:
             errors += response["error"]
-
-        if errors:
-            lines = errors.splitlines()
-            lines[0] = f"Error running mypy: {lines[0]}"
-            for message in reversed(lines):
-                self.add_comment(
-                    {
-                        "file": file,
-                        "line": start_line_no,
-                        "message": message,
-                    },
-                    len(lines),
-                )
-
-            self.text.bell()
-            return "break"
+        if "err" in response:
+            if errors:
+                errors += "\n"
+            errors += response["err"]
+        if "stdout" in response:
+            if normal:
+                normal += "\n"
+            normal += response["stdout"]
+        if "stderr" in response:
+            if normal:
+                normal += "\n"
+            normal += response["stderr"]
 
         if normal:
             # Add code comments
-            self.add_comments(file, start_line_no, normal)
+            self.add_comments(file, self.editwin.getlineno(), normal)
+
+        if errors:
+            # Add mypy errors
+            self.add_errors(file, self.editwin.getlineno(), errors)
 
         # Make bell sound so user knows we are done,
         # as it freezes a bit while mypy looks at the file
         self.text.bell()
         return "break"
 
-    def remove_type_comments_event(self, event: "Event[Any]") -> str:
-        "Remove selected mypy comments."
+    @undo_block
+    def remove_type_comments_event(self, event: Event[Any]) -> str:
+        """Remove selected mypy comments."""
         # pylint: disable=unused-argument
         # Get selected region lines
         head, tail, chars, lines = self.formatter.get_region()
-        if not self.comment in chars:
+        if self.comment not in chars:
             # Make bell sound so user knows this ran even though
             # nothing happened.
             self.text.bell()
             return "break"
         # Using dict so we can reverse and enumerate
         ldict = dict(enumerate(lines))
         for idx in sorted(ldict.keys(), reverse=True):
@@ -865,16 +986,16 @@
                 # If so, remove line
                 del lines[idx]
         # Apply changes
         self.formatter.set_region(head, tail, chars, lines)
         return "break"
 
     @undo_block
-    def remove_all_type_comments(self, event: "Event[Any]") -> str:
-        "Remove all mypy comments."
+    def remove_all_type_comments(self, event: Event[Any]) -> str:
+        """Remove all mypy comments."""
         # pylint: disable=unused-argument
         eof_idx = self.text.index("end")
 
         chars = self.text.get("0.0", eof_idx)
 
         lines = chars.splitlines()
         modified = False
@@ -885,25 +1006,24 @@
         if not modified:
             return "break"
 
         chars = "\n".join(lines)
 
         # Apply changes
         self.text.delete("0.0", eof_idx)
-        self.text.insert("0.0", chars, None)
+        self.text.insert("0.0", chars, ())
         return "break"
 
     @undo_block
-    def find_next_type_comment_event(self, event: "Event[Any]") -> str:
-        "Find next comment by hacking the search dialog engine."
+    def find_next_type_comment_event(self, event: Event[Any]) -> str:
+        """Find next comment by hacking the search dialog engine."""
         # pylint: disable=unused-argument
         self.reload()
 
-        root: Tk
-        root = self.text._root()  # pylint: disable=protected-access
+        root: Tk = self.editwin.root
 
         # Get search engine singleton from root
         engine: searchengine.SearchEngine = searchengine.get(root)
 
         # Get current search prams
         global_search_params = get_search_engine_params(engine)
 
@@ -923,14 +1043,49 @@
         # Find current pattern
         search.find_again(self.text)
 
         # Re-apply previous search prams
         set_search_engine_params(engine, global_search_params)
         return "break"
 
+    # def close(self) -> None:
+    #    """Called when any idle editor window closes"""
+
 
 idlemypyextension.reload()
 
+
+def get_fake_editwin(root_tk: Tk) -> PyShellEditorWindow:
+    """Get fake edit window for testing."""
+    from idlelib.pyshell import PyShellEditorWindow
+
+    class FakeEditWindow(PyShellEditorWindow):  # type: ignore[misc]
+        """FakeEditWindow for testing."""
+
+        def __init__(self) -> None:
+            return
+
+        from tkinter import Text
+
+        class _FakeText(Text):
+            """Make bind do nothing."""
+
+            def __init__(self) -> None:
+                """Requries no arguments."""
+                return
+
+            bind = lambda x, y: None  # type: ignore[assignment]  # noqa
+            root = root_tk
+            close = None
+
+        text = _FakeText()
+        fregion = FormatRegion
+        flist = PyShellFileList
+        io = IOBinding
+
+    return FakeEditWindow()
+
+
 if __name__ == "__main__":
     print(f"{__title__} v{__version__}\nProgrammed by {__author__}.\n")
     check_installed()
-##    self = idlemypyextension(get_fake_editwin())
+    # self = idlemypyextension(get_fake_editwin())
```

### Comparing `idlemypyextension-0.1.1/src/idlemypyextension/annotate.py` & `idlemypyextension-0.2.0/src/idlemypyextension/annotate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Annotate - Annotate functions given signature
-
-"Annotate functions given signature"
+"""Annotate - Annotate functions given signature."""
 
 # Extensively modified by CoolCat467
 
 # Extensively modified from https://github.com/dropbox/pyannotate/blob/master/pyannotate_tools/annotations/parse.py
 
-## Pyannotate is licensed under the terms of the Apache License, Version 2.0,
-## reproduced below.
-##   Copyright (c) 2017 Dropbox, Inc.
-##
-##   Licensed under the Apache License, Version 2.0 (the "License");
-##   you may not use this file except in compliance with the License.
-##   You may obtain a copy of the License at
-##
-##       http://www.apache.org/licenses/LICENSE-2.0
-##
-##   Unless required by applicable law or agreed to in writing, software
-##   distributed under the License is distributed on an "AS IS" BASIS,
-##   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-##   See the License for the specific language governing permissions and
-##   limitations under the License.
+# Pyannotate is licensed under the terms of the Apache License, Version 2.0,
+# reproduced below.
+#   Copyright (c) 2017 Dropbox, Inc.
+#
+#   Licensed under the Apache License, Version 2.0 (the "License");
+#   you may not use this file except in compliance with the License.
+#   You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#   Unless required by applicable law or agreed to in writing, software
+#   distributed under the License is distributed on an "AS IS" BASIS,
+#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#   See the License for the specific language governing permissions and
+#   limitations under the License.
 
 from __future__ import annotations
 
 __title__ = "Annotate"
 __author__ = "CoolCat467"
 __license__ = "Apache License, Version 2.0"
 
@@ -37,101 +33,138 @@
 from typing import Any, Final, NoReturn
 
 BUILTINS: Final = {"List", "Set", "Type", "Dict", "Tuple"}
 
 
 class ParseError(Exception):
     """Raised on any type comment parse error.
+
     The 'comment' attribute contains the comment that produced the error.
     """
 
     def __init__(self, comment: str | None = None) -> None:
+        """Initialize with comment."""
         if comment is None:
             comment = ""
         elif hasattr(self, "add_note"):  # New in Python 3.11
             self.add_note(comment)
         super().__init__(comment)
 
 
 class Token:
-    "Base token"
+    """Base token."""
+
     __slots__ = ("text",)
 
     def __init__(self, text: str | None = None) -> None:
+        """Initialize self with text."""
         self.text = text
 
     def __repr__(self) -> str:
+        """Get reprentation for this token."""
         value = "" if self.text is None else f"{self.text!r}"
         return f"{self.__class__.__name__}({value})"
 
 
 class Name(Token):
-    """Name Token"""
+    """Name Token."""
+
+    __slots__ = ()
 
 
 class FunctionName(Token):
-    """Function name"""
+    """Function name."""
+
+    __slots__ = ()
 
 
 class ArgumentName(Name):
-    """Argument name"""
+    """Argument name."""
+
+    __slots__ = ()
 
 
 class Operator(Token):
-    """Operator Token"""
+    """Operator Token."""
+
+    __slots__ = ()
 
 
 class DottedName(Name):
-    """An identifier token, such as 'List', 'int' or 'package.name'"""
+    """An identifier token, such as 'List', 'int' or 'package.name'."""
+
+    __slots__ = ()
 
 
 class ArgumentDefault(DottedName):
-    """Argument value"""
+    """Argument value."""
+
+    __slots__ = ()
 
 
 class Separator(Operator):
-    """A separator or punctuator token such as '(', '[' or '->'"""
+    """A separator or punctuator token such as '(', '[' or '->'."""
+
+    __slots__ = ()
 
 
 class EndSeparator(Separator):
-    """End separator that does not need extra space"""
+
+    """End separator that does not need extra space."""
 
 
 class Colin(Separator):
-    """Colin ':'"""
+    """Colin ':'."""
+
+    __slots__ = ()
 
 
 class TypeDef(Colin):
-    """Type Definition Start ':'"""
+    """Type Definition Start ':'."""
+
+    __slots__ = ()
 
 
 class DefaultDef(Separator):
-    """Argument Default Definition Start '='"""
+    """Argument Default Definition Start '='."""
+
+    __slots__ = ()
 
 
 class Keyword(Name):
-    """Keyword such as 'async', 'def'"""
+    """Keyword such as 'async', 'def'."""
+
+    __slots__ = ()
 
 
 class ReturnTypeDef(Separator):
-    """Return type definition '->'"""
+    """Return type definition '->'."""
+
+    __slots__ = ()
 
 
 class Definition(Keyword):
-    """Definition keyword"""
+    """Definition keyword."""
+
+    __slots__ = ()
 
 
 class EndDefinition(Colin):
-    """End Definition Colin"""
+    """End Definition Colin."""
+
+    __slots__ = ()
 
 
 class End(Token):
-    """A token representing the end of a type comment"""
+    """A token representing the end of a type comment."""
+
+    __slots__ = ()
 
     def __init__(self) -> None:
+        """Initialize superclass with no arguments."""
         super().__init__()
 
 
 def tokenize(txt: str) -> list[Token]:
     """Translate a type comment into a list of tokens."""
     original = txt
     txt = txt.replace("?", "")
@@ -173,32 +206,34 @@
                 # than crashing.
                 fullname = "Any"
             tokens.append(DottedName(fullname))
             txt = txt[size:]
 
 
 def get_line_indent(text: str, char: str = " ") -> int:
-    "Return line indent"
+    """Return line indent."""
     for idx, cur in enumerate(text.split(char)):
         if cur != "":
             return idx
     return 0
 
 
 def tokenize_definition(
-    line: int, get_line: Callable[[int], str]
-) -> list[Token]:
-    "Tokenize function definition"
+    start_line: int,
+    get_line: Callable[[int], str],
+) -> tuple[list[Token], int]:
+    """Return list of Tokens and number of lines after start."""
+    current_line_no = start_line
 
     def read_line() -> str:
-        "Incremental wrapper for get_line"
-        nonlocal line
-        value = get_line(line)
+        """Incremental wrapper for get_line."""
+        nonlocal current_line_no
+        value = get_line(current_line_no)
         # print(f'read_line: {value!r}')
-        line += 1
+        current_line_no += 1
         return value
 
     hasdef = False  # Do we have a definition token?
     defstart = False  # Has definition started?
     brackets = 0  # Current number of brackets in use
     typedef = 0  # Brackets in type definition (truthy if in type definition)
     default_arg = 0  # Brackets in default argument value
@@ -213,15 +248,15 @@
             if string == "async":  # Remember async
                 tokens.append(Keyword(string))
             elif (
                 string == "def"
             ):  # Error if more than one in case invalid start
                 if hasdef:
                     raise ParseError(
-                        "Did not expect second definition keyword"
+                        "Did not expect second definition keyword",
                     )
                 tokens.append(Definition(string))
                 hasdef = True  # Have definition now
             elif not defstart:  # If not started definition, only function name
                 tokens.append(FunctionName(string))
             elif typedef:  # If we are doing type definition, add DottedName
                 # If last was also a DottedName and it ended with a dot,
@@ -260,15 +295,15 @@
                 # Left a bracket level
                 brackets -= 1
                 if typedef:  # Maybe left a type def level too
                     typedef -= 1
                 if default_arg:
                     default_arg -= 1
                 tokens.append(EndSeparator(string))
-            elif string in {"*", "**"}:
+            elif string in {"*", "**", "/"}:
                 tokens.append(EndSeparator(string))
             elif string == "|":
                 tokens.append(Separator(string))
             elif string == ",":
                 # If exactly one level, leaving type definition land
                 if typedef == 1:
                     typedef = 0
@@ -336,15 +371,15 @@
             indent = len(string)
         elif tok_name[token.type] in {"NL", "NEWLINE"}:
             # replace separator ends with end separators
             if tokens and isinstance(tokens[-1], Separator):
                 tokens.append(EndSeparator(tokens.pop().text))
             tokens.append(EndSeparator(string))
             # we have a new indent level
-            indent = get_line_indent(get_line(line))
+            indent = get_line_indent(get_line(current_line_no))
             tokens.append(EndSeparator(" " * indent))
         elif tok_name[token.type] == "COMMENT":
             # Remember comments as separators
             tokens.append(EndSeparator(string))
         elif tok_name[token.type] in {"STRING", "NUMBER"}:
             # Only argument default, so add on to previous if exists
             if tokens and isinstance(tokens[-1], ArgumentDefault):
@@ -355,107 +390,117 @@
                 tokens.append(ArgumentDefault(string))
         else:
             raise ParseError(f"Unrecognized token type {tok_name[token.type]}")
         # print(tokens[-1])
     # print(tokens[-1])
     # print()
     tokens.append(End())
-    return tokens
+    return tokens, current_line_no - start_line
 
 
 def get_type_repr(name: str) -> str:
-    "Get representation of name"
+    """Get representation of name."""
     for seperator in (".", ":"):
         if seperator in name:
             module, text = name.split(seperator, 1)
-            if module in ("typing", "mypy_extensions") and text in BUILTINS:
-                return text.lower()
+            if module in ("typing", "mypy_extensions"):
+                if text in BUILTINS:
+                    return text.lower()
+                return text
     return name
 
 
-def get_typevalue_repr(typevalue: "TypeValue") -> str:
-    "Get representation of ClassType"
+def get_typevalue_repr(typevalue: TypeValue) -> str:
+    """Get representation of ClassType."""
     name = get_type_repr(typevalue.name)
     if name in BUILTINS:
         name = name.lower()
     args = []
     for arg in typevalue.args:
         args.append(get_typevalue_repr(arg))
     if not args:
-        return name
+        if name:
+            return name
+        return "[]"
     if name == "Union":
         return " | ".join(args)
     values = ", ".join(args)
     return f"{name}[{values}]"
 
 
 class TypeValue:
-    """A type value, potentially collection of multiple"""
+    """A type value, potentially collection of multiple."""
 
     __slots__ = ("name", "args")
 
     def __init__(
-        self, name: str, args: Sequence["TypeValue"] | None = None
+        self,
+        name: str,
+        args: Sequence[TypeValue] | None = None,
     ) -> None:
+        """Set up name and arguments."""
         self.name = name
         if args:
             self.args = tuple(args)
         else:
             self.args = ()
 
     def __repr__(self) -> str:
+        """Get representation of self."""
         return f"TypeValue({self.name!r}, {self.args!r})"
 
     def __str__(self) -> str:
+        """Get type value representation of self."""
         return get_typevalue_repr(self)
 
 
 def list_or(values: Collection[str]) -> str:
-    "Return comma separated listing of values joined with ` or `"
+    """Return comma separated listing of values joined with ` or `."""
     if len(values) <= 2:
         return " or ".join(values)
     copy = list(values)
     copy[-1] = f"or {copy[-1]}"
     return ", ".join(copy)
 
 
 class Parser:
-    """Implementation of the type comment parser"""
+    """Implementation of the type comment parser."""
 
     __slots__ = ("tokens", "i")
 
     def __init__(self, tokens: list[Token]) -> None:
+        """Initialize with tokens list."""
         self.tokens = tokens
         self.i = 0
 
     def parse_type_list(self) -> list[TypeValue]:
-        "Parse comma separated type list"
+        """Parse comma separated type list."""
         types = []
         while self.lookup() not in (")", "]"):
             typ = self.parse_type()
             types.append(typ)
             string = self.lookup()
             if string == ",":
                 self.expect(",")
             elif string not in {")", "]"}:
                 self.fail(f"Expected ) or ], got {string!r}")
         return types
 
     def parse_union_list(self) -> list[TypeValue]:
-        "Parse | separated union list"
+        """Parse | separated union list."""
         types = []
         while True:
             typ = self.parse_type()
             types.append(typ)
             if self.lookup() != "|":
                 return types
             self.expect("|")
 
     def parse_single(self) -> TypeValue:
-        "Parse single, does not look for | unions. Do not use directly."
+        """Parse single, does not look for | unions. Do not use directly."""
         if self.lookup() == "[":
             # Callable[[...], ...]
             #          ^^^^^
             self.expect("[")
             args = self.parse_type_list()
             self.expect("]")
             return TypeValue("", args)
@@ -493,131 +538,141 @@
                 token.text = "None"
             return TypeValue(token.text, args)
         if token.text is None:
             token.text = "None"
         return TypeValue(token.text)
 
     def parse_lambda_arguments(self) -> list[str]:
-        "Parse lambda arguments"
+        """Parse lambda arguments."""
         arguments = []
         while self.lookup() != ":":
-            typ = self.expect_type(ArgumentDefault)
+            typ = self.expect_type((ArgumentDefault, DottedName))
             assert typ.text is not None
             arguments.append(typ.text)
             string = self.lookup()
             if string == ",":
                 self.expect(",")
             elif string not in {",", ":"}:
                 self.fail(f"Expected , or :, got {string!r}")
         return arguments
 
     def parse_lambda(self) -> str:
-        "Parse lambda expression"
+        """Parse lambda expression."""
         arguments = ", ".join(self.parse_lambda_arguments())
         self.expect(":")
         value = f"{arguments}: "
 
         brackets = 0
         while not isinstance(self.peek(), End):
             if self.lookup() == "," and not brackets:
                 break
             token = self.next()
 
             assert token.text is not None
             value += token.text
 
-            if not isinstance(token, (Name, EndSeparator, DefaultDef)):
+            if not isinstance(token, Name | EndSeparator | DefaultDef):
                 value += " "
 
             if token.text in {"(", "[", "{"}:
                 brackets += 1
             elif token.text in {")", "]", "}"}:
                 brackets -= 1
                 if not brackets:
                     break
+                if brackets < 0:  # Reached end of expression in odd case
+                    self.back()
+                    value = value[:-1]
+                    break
         return value
 
     def parse_type(self) -> TypeValue:
-        "Parse type including | unions"
+        """Parse type including | unions."""
         type_value = self.parse_single()
         if self.lookup() == "|":
             self.expect("|")
-            args = [type_value] + self.parse_union_list()
+            args = [type_value, *self.parse_union_list()]
             return TypeValue("Union", args)
         return type_value
 
     def fail(self, error: str | None) -> NoReturn:
-        "Raise parse error"
+        """Raise parse error."""
         raise ParseError(error)
 
     def peek(self) -> Token:
-        "Peek at next token"
+        """Peek at next token."""
         if self.i >= len(self.tokens):
             self.fail("Ran out of tokens")
         return self.tokens[self.i]
 
-    def next(self) -> Token:
-        "Get next token"
+    def next(self) -> Token:  # noqa: A003
+        """Get next token."""
         token = self.peek()
         self.i += 1
         return token
 
     def expect(self, text: str) -> None:
-        "Expect next token text to be text"
+        """Expect next token text to be text."""
         got = self.next().text
         if got != text:
             self.fail(f"Expected {text!r}, got {got!r}")
 
     def expect_type(
-        self, token_type: type[Token] | tuple[type[Token], ...]
+        self,
+        token_type: type[Token] | tuple[type[Token], ...],
     ) -> Token:
-        "Expect next token to be instance of token_type. Return token."
+        """Expect next token to be instance of token_type. Return token."""
         token = self.next()
         if not isinstance(token, token_type):
             if hasattr(token_type, "__iter__"):
                 assert isinstance(token_type, tuple)
                 expect_str = list_or(
-                    [f"{cls.__name__!r}" for cls in token_type]
+                    [f"{cls.__name__!r}" for cls in token_type],
                 )
             else:
                 expect_str = f"{token_type.__name__!r}"
             self.fail(f"Expected {expect_str}, got {token}")
         return token
 
     def lookup(self) -> str:
-        "Peek at next token and return it's text"
+        """Peek at next token and return it's text."""
         value = self.peek().text
         if value is None:
             return "None"
         return value
 
     def back(self) -> None:
-        "Go back one token"
+        """Go back one token."""
         self.i -= 1
 
     def rest_tokens(self) -> list[Token]:
-        "Return all tokens not processed"
-        return self.tokens[self.i :]
+        """Return all tokens not processed."""
+        return self.tokens[self.i : len(self.tokens)]
 
 
 def get_annotation(
-    annotation: dict[str, Any], get_line: Callable[[int], str]
-) -> str:
-    "Get annotation"
-    # print(f'{annotation = }\n')
+    annotation: dict[str, Any],
+    get_line: Callable[[int], str],
+) -> tuple[str, int]:
+    """Return annotation and end line."""
+    # print(f"[DEBUG] Annotate: {annotation = }\n")
 
     # Get definition tokens
     try:
-        def_tokens = tokenize_definition(annotation["line"], get_line)
+        def_tokens, line_count = tokenize_definition(
+            annotation["line"],
+            get_line,
+        )
     except ParseError:
         print(f"Could not tokenize definition\n{annotation = }")
         raise
     except EOFError as exc:
+        print(f"[ERROR] Annotate: {annotation = }\n")
         raise ParseError(
-            "Reached End of File, expected end of definition"
+            "Reached End of File, expected end of definition",
         ) from exc
 
     # Get the argument and return tokens from signature
     signature = annotation["signature"]
     arg_tokens = [tokenize(arg) for arg in signature["arg_types"]]
     return_tokens = tokenize(signature["return_type"])
 
@@ -678,15 +733,15 @@
             if isinstance(token, EndSeparator):
                 assert token.text is not None
                 new_lines += token.text
             else:
                 new_lines += f"{token.text} "
             if token.text == ")":
                 break
-            if token.text == "*":
+            if token.text in {"*", "/"}:
                 argument += 1
         elif isinstance(token, ArgumentName):
             name = token.text
             type_text = ""
             if isinstance(parser.peek(), TypeDef):
                 parser.expect(":")
                 type_value = parser.parse_type()
@@ -709,20 +764,15 @@
         elif isinstance(token, End):
             print("Found End token during argument parsing")
             parser.back()
             break
     # print(f'{type_text = }')
 
     # Handle the end
-    if isinstance(parser.peek(), EndDefinition):
-        parser.tokens = (
-            [ReturnTypeDef("->")] + return_tokens[:-1] + parser.rest_tokens()
-        )
-        parser.i = 0
-    elif isinstance(parser.peek(), End):
+    if isinstance(parser.peek(), EndDefinition | End):
         parser.tokens = (
             [ReturnTypeDef("->")] + return_tokens[:-1] + parser.rest_tokens()
         )
         parser.i = 0
     # print(f'{parser.rest_tokens() = }')
     parser.expect("->")
     new_lines += " -> "
@@ -731,24 +781,24 @@
     while True:
         token = parser.next()
         if isinstance(token, End):
             break
         assert token.text is not None
         new_lines += token.text
 
-    return new_lines
+    return new_lines, line_count
 
 
 def run(annotation: dict[str, str]) -> None:
-    "Run test of module"
+    """Run test of module."""
 
     def get_line(line: int) -> str:
         path = annotation["path"]
         assert isinstance(path, str), "Path must be string"
-        with open(path, "r", encoding="utf-8") as files:
+        with open(path, encoding="utf-8") as files:
             for line_no, line_text in enumerate(files):
                 if line_no == line - 1:
                     return line_text
             raise EOFError
 
     print(f"{get_annotation(annotation, get_line)!r}")
```

### Comparing `idlemypyextension-0.1.1/src/idlemypyextension/client.py` & `idlemypyextension-0.2.0/src/idlemypyextension/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# Mypy Daemon Client - Modified version of mypy.dmypy.client
-
-"""Client for mypy daemon mode.
+"""Client for mypy daemon mode - Modified version of mypy.dmypy.client.
 
 This manages a daemon process which keeps useful state in memory
 rather than having to read it back from disk on each run.
-
-Modified version of mypy.dmypy.client
 """
 
 # Modified by CoolCat467
 # Original at https://github.com/python/mypy/blob/master/mypy/dmypy/client.py
 # Original retrieved November 24th 2022
 # Last updated to match original on March 11th 2023
 
@@ -31,42 +25,65 @@
 #    Software is furnished to do so, subject to the following conditions:
 #
 #    The above copyright notice and this permission notice shall be included in
 #    all copies or substantial portions of the Software.
 #
 #    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-#    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-#    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+#    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+#    THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #    FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #    DEALINGS IN THE SOFTWARE.
 
 from __future__ import annotations
 
-__title__ = "Mypy Daemon Client"
+__title__ = "Mypy Daemon Asynchronous Client"
 __license__ = "MIT"
 
+import contextlib
+import io
 import json
 import os
 import time
-from typing import Any, Sequence
+from collections.abc import Sequence
+from typing import Any, cast
 
-from mypy.dmypy_os import alive as _alive
-from mypy.dmypy_os import kill as _kill
-from mypy.dmypy_server import Server as _Server
-from mypy.dmypy_server import daemonize as _daemonize
-from mypy.dmypy_server import process_start_options as _process_start_options
-from mypy.dmypy_util import receive as _receive
-from mypy.ipc import IPCClient as _IPCClient
-from mypy.ipc import IPCException as _IPCException
+import trio
+from mypy.dmypy_os import alive as _alive, kill as _kill
+from mypy.dmypy_server import (
+    Server as _Server,
+    daemonize as _daemonize,
+    process_start_options as _process_start_options,
+)
+from mypy.ipc import IPCClient as _IPCClient, IPCException as _IPCException
 from mypy.version import __version__
 
 
-class BadStatus(Exception):
+async def _receive(connection: _IPCClient) -> Any:
+    """Receive JSON data from a connection until EOF.
+
+    Raise OSError if the data received is not valid JSON or if it is
+    not a dict.
+    """
+    async_connection = trio.wrap_file(cast(io.BytesIO, connection))
+    bdata: bytes = await async_connection.read()
+    if not bdata:
+        raise OSError("No data received")
+    try:
+        data = json.loads(bdata.decode("utf8"))
+    except Exception as e:
+        raise OSError("Data received is not valid JSON") from e
+    if not isinstance(data, dict):
+        raise OSError(f"Data received is not a dict ({type(data)})")
+    return data
+
+
+class BadStatusError(Exception):
+
     """Exception raised when there is something wrong with the status file.
 
     For example:
     - No status file found
     - Status file malformed
     - Process whose process id is in the status file does not exist
     """
@@ -74,132 +91,134 @@
 
 # Client-side infrastructure.
 
 
 def _read_status(status_file: str) -> dict[str, object]:
     """Read status file.
 
-    Raise BadStatus if the status file doesn't exist or contains
+    Raise BadStatusError if the status file doesn't exist or contains
     invalid JSON or the JSON is not a dict.
     """
     if not os.path.isfile(status_file):
-        raise BadStatus("No status file found")
-    with open(status_file, "r", encoding="utf-8") as file:
+        raise BadStatusError("No status file found")
+    with open(status_file, encoding="utf-8") as file:
         try:
             data = json.load(file)
         except Exception as ex:
-            raise BadStatus("Malformed status file (not JSON)") from ex
+            raise BadStatusError("Malformed status file (not JSON)") from ex
     if not isinstance(data, dict):
-        raise BadStatus("Invalid status file (not a dict)")
+        raise BadStatusError("Invalid status file (not a dict)")
     return data
 
 
+def _check_status(data: dict[str, Any]) -> tuple[int, str]:
+    """Check if the process is alive.
+
+    Return (process id, connection_name) on success.
+
+    Raise BadStatusError if something's wrong.
+    """
+    if "pid" not in data:
+        raise BadStatusError("Invalid status file (no pid field)")
+    pid = data["pid"]
+    if not isinstance(pid, int):
+        raise BadStatusError("pid field is not an int")
+    if not _alive(pid):
+        raise BadStatusError("Daemon has died")
+    if "connection_name" not in data:
+        raise BadStatusError("Invalid status file (no connection_name field)")
+    connection_name = data["connection_name"]
+    if not isinstance(connection_name, str):
+        raise BadStatusError("connection_name field is not a string")
+    return pid, connection_name
+
+
 def get_status(status_file: str) -> tuple[int, str]:
     """Read status file and check if the process is alive.
 
     Return (process id, connection_name) on success.
 
-    Raise BadStatus if something's wrong.
+    Raise BadStatusError if something's wrong.
     """
     data = _read_status(status_file)
     return _check_status(data)
 
 
-def request(
+async def request(
     status_file: str,
     command: str,
     *,
     timeout: int | None = None,
     **kwds: object,
 ) -> dict[str, Any]:
     """Send a request to the daemon.
 
     Return the JSON dict with the response.
 
-    Raise BadStatus if there is something wrong with the status file
+    Raise BadStatusError if there is something wrong with the status file
     or if the process whose process id is in the status file has died.
 
     Return {'error': <message>} if an IPC operation or receive()
     raised OSError.  This covers cases such as connection refused or
     closed prematurely as well as invalid JSON received.
     """
     response: dict[str, str] = {}
     args = dict(kwds)
     args["command"] = command
-    # Tell the server whether this request was initiated from a human-facing terminal,
-    # so that it can format the type checking output accordingly.
+    # Tell the server whether this request was initiated from a
+    # human-facing terminal, so that it can format the type checking
+    # output accordingly.
     args["is_tty"] = False
     args["terminal_width"] = 80
     bdata = json.dumps(args).encode("utf8")
     _, name = get_status(status_file)
     try:
         with _IPCClient(name, timeout) as client:
-            client.write(bdata)
-            response = _receive(client)
-    except (OSError, _IPCException, ValueError, UnicodeError) as err:
+            async_client = trio.wrap_file(cast(io.BytesIO, client))
+            await async_client.write(bdata)
+            response = await _receive(client)
+    except (OSError, _IPCException, ValueError) as err:
         return {"error": str(err)}
     return response
 
 
-def _check_status(data: dict[str, Any]) -> tuple[int, str]:
-    """Check if the process is alive.
-
-    Return (process id, connection_name) on success.
-
-    Raise BadStatus if something's wrong.
-    """
-    if "pid" not in data:
-        raise BadStatus("Invalid status file (no pid field)")
-    pid = data["pid"]
-    if not isinstance(pid, int):
-        raise BadStatus("pid field is not an int")
-    if not _alive(pid):
-        raise BadStatus("Daemon has died")
-    if "connection_name" not in data:
-        raise BadStatus("Invalid status file (no connection_name field)")
-    connection_name = data["connection_name"]
-    if not isinstance(connection_name, str):
-        raise BadStatus("connection_name field is not a string")
-    return pid, connection_name
-
-
 def is_running(status_file: str) -> bool:
-    """Check if the server is running cleanly"""
+    """Check if the server is running cleanly."""
     try:
         get_status(status_file)
-    except BadStatus:
+    except BadStatusError:
         return False
     return True
 
 
-def stop(status_file: str) -> dict[str, Any]:
+async def stop(status_file: str) -> dict[str, Any]:
     """Stop daemon via a 'stop' request."""
-    return request(status_file, "stop", timeout=5)
+    return await request(status_file, "stop", timeout=5)
 
 
-def _wait_for_server(status_file: str, timeout: float = 5.0) -> bool:
+async def _wait_for_server(status_file: str, timeout: float = 5.0) -> bool:
     """Wait until the server is up. Return False if timed out."""
     endtime = time.time() + timeout
     while time.time() < endtime:
         try:
             data = _read_status(status_file)
-        except BadStatus:
+        except BadStatusError:
             # If the file isn't there yet, retry later.
-            time.sleep(0.1)
+            await trio.sleep(0.1)
             continue
         # If the file's content is bogus or the process is dead, fail.
         try:
             _check_status(data)
-        except BadStatus:
+        except BadStatusError:
             return False
         return True
     return False
 
 
-def _start_server(
+async def _start_server(
     status_file: str,
     *,
     flags: list[str],
     daemon_timeout: int | None = None,
     allow_sources: bool = False,
     log_file: str | None = None,
 ) -> bool:
@@ -211,123 +230,124 @@
             status_file,
             timeout=daemon_timeout,
             log_file=log_file,
         )
         != 0
     ):
         return False
-    return _wait_for_server(status_file)
+    return await _wait_for_server(status_file)
 
 
-def restart(
+async def restart(
     status_file: str,
     *,
     flags: list[str],
     daemon_timeout: int | None = 0,
     allow_sources: bool = False,
     log_file: str | None = None,
 ) -> bool:
     """Restart daemon (it may or may not be running; but not hanging).
 
-    Returns False if error starting."""
-    try:
-        stop(status_file)
-    except BadStatus:
-        # Bad or missing status file or dead process; good to start.
-        pass
-    return _start_server(
+    Returns False if error starting.
+    """
+    # Bad or missing status file or dead process; good to start.
+    with contextlib.suppress(BadStatusError):
+        await stop(status_file)
+    return await _start_server(
         status_file,
         flags=flags,
         daemon_timeout=daemon_timeout,
         allow_sources=allow_sources,
         log_file=log_file,
     )
 
 
 # Action functions
 
 
-def start(
+async def start(
     status_file: str,
     *,
     flags: list[str],
     daemon_timeout: int = 0,
     allow_sources: bool = False,
     log_file: str | None = None,
 ) -> bool:
     """Start daemon if not already running.
 
-    Returns False if error starting / already running."""
+    Returns False if error starting / already running.
+    """
     if not is_running(status_file):
         # Bad or missing status file or dead process; good to start.
-        return _start_server(
+        return await _start_server(
             status_file,
             flags=flags,
             daemon_timeout=daemon_timeout,
             allow_sources=allow_sources,
             log_file=log_file,
         )
     return False
 
 
-def status(
+async def status(
     status_file: str,
     *,
     timeout: int = 5,
     fswatcher_dump_file: str | None = None,
 ) -> dict[str, object]:
     """Ask daemon to return status."""
-    return request(
+    return await request(
         status_file,
         "status",
         timeout=timeout,
         fswatcher_dump_file=fswatcher_dump_file,
     )
 
 
-def run(
+async def run(
     status_file: str,
     *,
     flags: list[str],
     timeout: int | None = None,
     daemon_timeout: int = 0,
     log_file: str | None = None,
     export_types: bool = False,
 ) -> dict[str, Any]:
-    """Do a check, starting (or restarting) the daemon as necessary
+    """Do a check, starting (or restarting) the daemon as necessary.
 
     Restarts the daemon if the running daemon reports that it is
-    required (due to a configuration change, for example)."""
+    required (due to a configuration change, for example).
+    """
     if not is_running(status_file):
         # Bad or missing status file or dead process; good to start.
-        _start_server(
+        await _start_server(
             status_file,
             flags=flags,
             daemon_timeout=daemon_timeout,
             allow_sources=True,
             log_file=log_file,
         )
-    response = request(
+    response = await request(
         status_file,
         "run",
         timeout=timeout,
         version=__version__,
         args=flags,
         export_types=export_types,
     )
     # If the daemon signals that a restart is necessary, do it
     if "restart" in response:
-        restart(
+        await restart(
             status_file,
             flags=flags,
             daemon_timeout=timeout,
             allow_sources=True,
             log_file=log_file,
         )
-        response = request(
+        response = await request(
             status_file,
             "run",
             timeout=timeout,
             version=__version__,
             args=flags,
             export_types=export_types,
         )
@@ -341,82 +361,85 @@
         _kill(pid)
     except OSError as ex:
         print(ex)
         return False
     return True
 
 
-def check(
+async def check(
     status_file: str,
     files: Sequence[str],
     *,
     timeout: int | None = None,
     export_types: bool = False,
 ) -> dict[str, Any]:
     """Ask the daemon to check a list of files."""
-    return request(
+    return await request(
         status_file,
         "check",
         timeout=timeout,
         files=files,
         export_types=export_types,
     )
 
 
-def recheck(
+async def recheck(
     status_file: str,
     export_types: bool,
     *,
     timeout: int | None = None,
     remove: list[str] | None = None,
     update: list[str] | None = None,
 ) -> dict[str, Any]:
-    """Ask the daemon to recheck the previous list of files, with optional modifications.
+    """Ask the daemon to recheck the previous list of files.
 
     If at least one of --remove or --update is given, the server will
-    update the list of files to check accordingly and assume that any other files
-    are unchanged.  If none of these flags are given, the server will call stat()
-    on each file last checked to determine its status.
+    update the list of files to check accordingly and assume that any other
+    files are unchanged.  If none of these flags are given, the server will
+    call stat() on each file last checked to determine its status.
 
-    Files given in --update ought to exist.  Files given in --remove need not exist;
-    if they don't they will be ignored.
+    Files given in --update ought to exist.  Files given in --remove need not
+    exist; if they don't they will be ignored.
     The lists may be empty but oughtn't contain duplicates or overlap.
 
     NOTE: The list of files is lost when the daemon is restarted.
     """
     if remove is not None or update is not None:
-        return request(
+        return await request(
             status_file,
             "recheck",
             timeout=timeout,
             export_types=export_types,
             remove=remove,
             update=update,
         )
-    return request(
-        status_file, "recheck", timeout=timeout, export_types=export_types
+    return await request(
+        status_file,
+        "recheck",
+        timeout=timeout,
+        export_types=export_types,
     )
 
 
-def inspect(
+async def inspect(
     status_file: str,
     location: str,  # line:col
     show: str = "type",  # type, attrs, definition
     *,
     timeout: int | None = None,
     verbosity: int = 0,
     limit: int = 0,
     include_span: bool = False,
     include_kind: bool = False,
     include_object_attrs: bool = False,
     union_attrs: bool = False,
     force_reload: bool = False,
 ) -> dict[str, Any]:
     """Ask daemon to print the type of an expression."""
-    return request(
+    return await request(
         status_file,
         "inspect",
         timeout=timeout,
         show=show,
         location=location,
         verbosity=verbosity,
         limit=limit,
@@ -424,50 +447,51 @@
         include_kind=include_kind,
         include_object_attrs=include_object_attrs,
         union_attrs=union_attrs,
         force_reload=force_reload,
     )
 
 
-def suggest(
+async def suggest(
     status_file: str,
     function: str,
     do_json: bool,
     *,
     timeout: int | None = None,
     callsites: bool = False,
     no_errors: bool = False,
     no_any: bool = False,
     flex_any: float | None = None,
     use_fixme: str | None = None,
     max_guesses: int | None = 64,
 ) -> dict[str, Any]:
     """Ask the daemon for a suggested signature."""
-    return request(
+    return await request(
         status_file,
         "suggest",
         timeout=timeout,
         function=function,
         json=do_json,
         callsites=callsites,
         no_errors=no_errors,
         no_any=no_any,
         flex_any=flex_any,
         use_fixme=use_fixme,
         max_guesses=max_guesses,
     )
 
 
-def hang(status_file: str, *, timeout: int = 1) -> dict[str, Any]:
+async def hang(status_file: str, *, timeout: int = 1) -> dict[str, Any]:
     """Hang for 100 seconds, as a debug hack."""
     if not isinstance(timeout, int):
         raise ValueError("Timeout must be an integer!")
-    return request(status_file, "hang", timeout=timeout)
+    return await request(status_file, "hang", timeout=timeout)
 
 
 def do_daemon(
-    status_file: str, flags: list[str], daemon_timeout: int | None = None
+    status_file: str,
+    flags: list[str],
+    daemon_timeout: int | None = None,
 ) -> None:
     """Serve requests in the foreground."""
-
     options = _process_start_options(flags, allow_sources=False)
     _Server(options, status_file, timeout=daemon_timeout).serve()
```

### Comparing `idlemypyextension-0.1.1/src/idlemypyextension.egg-info/PKG-INFO` & `idlemypyextension-0.2.0/src/idlemypyextension.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: idlemypyextension
-Version: 0.1.1
-Summary: Mypy extension for Python IDLE
+Version: 0.2.0
+Summary: Mypy daemon extension for Python IDLE
 Author: CoolCat467
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -188,15 +188,15 @@
               the brackets!)  The text should be enclosed in the appropriate
               comment syntax for the file format. We also recommend that a
               file or class name and description of purpose be included on the
               same "printed page" as the copyright notice for easier
               identification within third-party archives.
         
            Copyright 2022 CoolCat467
-           
+        
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
@@ -208,25 +208,23 @@
 Project-URL: Homepage, https://github.com/CoolCat467/idlemypyextension
 Project-URL: Source, https://github.com/CoolCat467/idlemypyextension
 Project-URL: Bug Tracker, https://github.com/CoolCat467/idlemypyextension/issues
 Keywords: mypy,dmypy,idle,extension,development,daemon
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: IDLE
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IdleMypyExtension
 Python IDLE extension to preform mypy analysis on an open file
 
 ## What does this extension do?
@@ -256,24 +254,25 @@
 If everything went well, alongside `ZzDummy` there should be and
 option called `idlemypyextension`. This is where you can configure how
 idlemypyextension works.
 
 
 ## Information on options
 `action_max_sec` controls how long an action is allowed to take at most,
-in seconds.
-Values under 5 will make no effect
+in seconds. Default is "None".
 
 For `daemon_flags`, see `mypy --help` for a list of valid flags.
 This extension sets the following flags to be able to work properly:
 ```
     --hide-error-context
     --no-color-output
     --show-absolute-path
     --no-error-summary
+    --soft-error-limit=-1
+    --show-traceback
     --cache-dir="~/.idlerc/mypy"
 ```
 
 If you add the `--show-column-numbers` flag to `daemon_flags`, when using the
 "Type Check File" command, it will add a helpful little `^` sign
 in a new line below the location of the mypy message that provided a column
 number, as long as that comment wouldn't break your file's indentation too much.
```

