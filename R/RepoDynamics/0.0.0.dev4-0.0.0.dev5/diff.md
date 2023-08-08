# Comparing `tmp/RepoDynamics-0.0.0.dev4.tar.gz` & `tmp/RepoDynamics-0.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepoDynamics-0.0.0.dev4.tar", last modified: Tue Aug  8 21:47:45 2023, max compression
+gzip compressed data, was "RepoDynamics-0.0.0.dev5.tar", last modified: Tue Aug  8 22:53:29 2023, max compression
```

## Comparing `RepoDynamics-0.0.0.dev4.tar` & `RepoDynamics-0.0.0.dev5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.652122 RepoDynamics-0.0.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 21:47:45.652122 RepoDynamics-0.0.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:47:45.652122 RepoDynamics-0.0.0.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 21:47:45.000000 RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/repodynamics/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/actions/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/cd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:47:45.648122 RepoDynamics-0.0.0.dev4/src/repodynamics/files/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/files/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/format_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 21:47:37.000000 RepoDynamics-0.0.0.dev4/src/repodynamics/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.860682 RepoDynamics-0.0.0.dev5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 22:53:29.000000 RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/src/repodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/actions/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/cd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 22:53:29.864682 RepoDynamics-0.0.0.dev5/src/repodynamics/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/files/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/format_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 22:53:19.000000 RepoDynamics-0.0.0.dev5/src/repodynamics/workflow.py
```

### Comparing `RepoDynamics-0.0.0.dev4/pyproject.toml` & `RepoDynamics-0.0.0.dev5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 where = ["src"]
 namespaces = true
 
 
 # ----------------------------------------- Project Metadata -------------------------------------
 #
 [project]
-version = "0.0.0.dev4"
+version = "0.0.0.dev5"
 name = "RepoDynamics"
 #dependencies = [
 #    # https://yaml.readthedocs.io/en/stable/
 #    "ruamel.yaml >= 0.17.32, < 0.18",
 #    # https://tomlkit.readthedocs.io/en/stable/
 #    "tomlkit >= 0.11.8, < 0.12",
 #    "trove-classifiers",
```

### Comparing `RepoDynamics-0.0.0.dev4/src/RepoDynamics.egg-info/SOURCES.txt` & `RepoDynamics-0.0.0.dev5/src/RepoDynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/__main__.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 ┃╭╮╭┫┃━┫╭╮┃╭╮┃┃┃┃┃┃ ┃┃╭╮┫╭╮┃╰╯┣┫╭━┫━━┫ 
 ┃┃┃╰┫┃━┫╰╯┃╰╯┣╯╰╯┃╰━╯┃┃┃┃╭╮┃┃┃┃┃╰━╋━━┃ 
 ╰╯╰━┻━━┫╭━┻━━┻━━━┻━╮╭┻╯╰┻╯╰┻┻┻┻┻━━┻━━╯ 
        ┃┃        ╭━╯┃
        ╰╯        ╰━━╯
 """
 
-print(SGR.format(logo, styles=SGR.style("bold", "blue")))
+print(SGR.format(logo, style=SGR.style("bold", "blue")))
```

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/actions/__main__.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/actions/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,31 +6,26 @@
 from repodynamics.ansi import SGR
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("action", type=str, help="Name of the action to run.")
     action = parser.parse_args().action
-    print()
     action_name = action.replace('-', '_')
     try:
         action_module = importlib.import_module(f"repodynamics.actions.{action_name}")
         action = getattr(action_module, action_name)
         inputs = io.input(action=action)
         outputs, summary = action(**inputs)
         if outputs:
             io.output(**outputs)
         if summary:
             io.summary(content=summary)
     except Exception as e:
-        print(f"ERROR: {e}")
+        print(SGR.format("An unexpected error occurred:", "error"))
+        print(e)
         sys.exit(1)
     return
 
 
 if __name__ == "__main__":
     main()
-
-
-
-
-
```

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/actions/context.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/actions/context.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/actions/io.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/actions/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,92 @@
-from typing import Callable, Optional, get_type_hints
+from typing import Callable, get_type_hints
 import os
 import sys
 import json
 
 from repodynamics.ansi import SGR
 
+
 def input(action: Callable) -> dict:
     """
     Parse inputs from environment variables.
     """
     print(
         SGR.format(
             f"Reading inputs for action '{action.__name__}':",
-            styles=SGR.style("bold", "cyan"),
+            style=SGR.style("bold", "b_blue"),
         )
     )
     params = get_type_hints(action)
     args = {}
     if not params:
-        print(
-            SGR.format(
-                f"\tAction requires no inputs.",
-                styles=SGR.style(text_color="green"),
-            )
-        )
+        print(SGR.format(f"Action requires no inputs.", "success"))
         return args
     params.pop("return", None)
     for param, typ in params.items():
         action_name = action.__name__.upper().replace('_', '-')
-        param_name = param.upper().replace('_', '-')
+        param_name = param.upper()
         param_env_name = f"RD__{action_name}__{param_name}"
         val = os.environ.get(param_env_name)
         if val is None:
-            print(f"ERROR: Missing input: {param_env_name}")
+            print(SGR.format(f"Missing input: {param_env_name}", "error"))
             sys.exit(1)
         if typ is str:
             args[param] = val
         elif typ is bool:
             if isinstance(val, bool):
                 args[param] = val
             elif isinstance(val, str):
                 if val.lower() not in ("true", "false", ""):
                     print(
-                        "ERROR! Invalid boolean input: "
-                        f"'{param_env_name}' has value '{val}' with type {type(val)}."
+                        SGR.format(
+                            (
+                                "Invalid boolean input: "
+                                f"'{param_env_name}' has value '{val}' with type '{type(val)}'."
+                            ),
+                            "error",
+                        )
                     )
                     sys.exit(1)
                 args[param] = val.lower() == "true"
             else:
                 print(
-                    "ERROR! Invalid boolean input: "
-                    f"'{param_env_name}' has value '{val}' with type {type(val)}."
+                    SGR.format(
+                        (
+                            "Invalid boolean input: "
+                            f"'{param_env_name}' has value '{val}' with type '{type(val)}'."
+                        ),
+                        "error",
+                    )
                 )
                 sys.exit(1)
         elif typ is dict:
             args[param] = json.loads(val, strict=False)
         else:
-            print(f"ERROR: Unknown input type: {typ}")
+            print(
+                SGR.format(
+                    (
+                        "Unknown input type: "
+                        f"'{param_env_name}' has value '{val}' with type '{type(val)}'."
+                    ),
+                    "error",
+                )
+            )
             sys.exit(1)
     return args
 
 
 def output(**kwargs) -> None:
+    print(SGR.format("Writing outputs:", style="info"))
     with open(os.environ["GITHUB_OUTPUT"], "a") as fh:
         for name, value in kwargs.items():
-            print(f"{name.replace('_', '-')}={value}", file=fh)
+            output_name = name.replace('_', '-')
+            print(f"{output_name}={value}", file=fh)
+            print(SGR.format(f"  {output_name}", style="success"), f"= {value}")
     return
 
 
 def summary(content: str) -> None:
+    print(SGR.format("Writing summary", style="info"))
     with open(os.environ["GITHUB_STEP_SUMMARY"], "a") as fh:
         print(content, file=fh)
     return
```

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/actions/meta.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/actions/meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import sys
 
 from markitup import html, md
 
 from repodynamics.ansi import SGR
 
+
 def meta(
     cache_hit: bool,
     force_update: str,
     metadata_filepath: str,
     cache_filepath: str,
     github_token: str,
 ) -> tuple[dict, str]:
 
     if force_update not in ["all", "core", "none"]:
-        print(
-           SGR.format(
-                f"ERROR! Invalid input for 'force_update': '{force_update}'.",
-                styles=SGR.style(background_color="red"),
-           )
-        )
+        print(SGR.format(f"Invalid input for 'force_update': '{force_update}'.","error"))
         sys.exit(1)
 
     if force_update != "none" or not cache_hit:
         from repodynamics.metadata import Metadata
         metadata = Metadata(
             path_cache=cache_filepath,
             update_cache=force_update == "all",
@@ -42,18 +38,16 @@
 
     force_update_emoji = "✅" if force_update == "all" else ("❌" if force_update == "none" else "☑️")
     cache_hit_emoji = "✅" if cache_hit else "❌"
     if not cache_hit or force_update == "all":
         result = "Updated all metadata"
     elif force_update == "core":
         result = "Updated core metadata but loaded API metadata from cache"
-    elif force_update == "none":
-        result = "Loaded all metadata from cache"
     else:
-        raise ValueError(f"Unknown force_update value: {force_update}")
+        result = "Loaded all metadata from cache"
 
     metadata_details = html.details(
         content=md.code_block(metadata_str_pretty, "json"),
         summary="🖥 Metadata",
         content_indent=""
     )
     results_list = html.ul(
```

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/ansi.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/ansi.py`

 * *Files 17% similar despite different names*

```diff
@@ -79,9 +79,21 @@
                 raise TypeError(f"Invalid color type: {type(background_color)}")
             style_str += f"{SGR.color[background_color] + 10};"
         if not style_str:
             return SGR.reset
         return SGR.temp.format(style_str.removesuffix(";"))
 
     @staticmethod
-    def format(text, styles: str):
-        return f"{styles}{text}{SGR.reset}"
+    def format(text, style: str):
+        if style == "error":
+            s1 = SGR.style(text_styles="bold", text_color="b_white", background_color="red")
+            s2 = SGR.style(text_styles="bold", background_color="red")
+            return f"{s1}ERROR! {s2}{text}{SGR.reset}"
+        if style == "warning":
+            s1 = SGR.style(text_styles="bold", text_color="b_white", background_color="yellow")
+            s2 = SGR.style(text_styles="bold", background_color="yellow")
+            return f"{s1}WARNING! {s2}{text}{SGR.reset}"
+        if style == "info":
+            style = SGR.style(text_styles="bold", text_color="b_blue")
+        elif style == "success":
+            style = SGR.style(text_styles="bold", text_color="green")
+        return f"{style}{text}{SGR.reset}"
```

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/cd.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/cd.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/files/__main__.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/files/__main__.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/files/pyproject.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/files/pyproject.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/files/readme.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/files/readme.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/files/templates.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/files/templates.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/format_issue.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/format_issue.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/metadata.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/metadata.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev4/src/repodynamics/workflow.py` & `RepoDynamics-0.0.0.dev5/src/repodynamics/workflow.py`

 * *Files identical despite different names*

