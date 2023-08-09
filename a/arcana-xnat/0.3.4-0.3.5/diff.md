# Comparing `tmp/arcana_xnat-0.3.4.tar.gz` & `tmp/arcana_xnat-0.3.5.tar.gz`

## Comparing `arcana_xnat-0.3.4.tar` & `arcana_xnat-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/_version.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/base.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/entrypoint.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/update_release.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_add_columns.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_dataset_export.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_store.py
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_xnat_images.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/data/__init__.py
--rw-r--r--   0        0        0    24191 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/data/api.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/data/cs.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/data/tests/test_store.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/deploy/__init__.py
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/deploy/command.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/deploy/image.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/deploy/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/utils/__init__.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/utils/testing.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/.gitignore
--rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/LICENSE
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/README.rst
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    21749 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/cli/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/cli/base.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/cli/entrypoint.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/cli/update_release.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/cli/tests/test_cli_add_columns.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/cli/tests/test_cli_dataset_export.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/cli/tests/test_cli_store.py
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/cli/tests/test_cli_xnat_images.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/data/__init__.py
+-rw-r--r--   0        0        0    24191 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/data/api.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/data/cs.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/data/tests/test_store.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/deploy/__init__.py
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/deploy/command.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/deploy/image.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/deploy/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/utils/__init__.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/arcana/xnat/utils/testing.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/.gitignore
+-rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/README.rst
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    21749 2020-02-02 00:00:00.000000 arcana_xnat-0.3.5/PKG-INFO
```

### Comparing `arcana_xnat-0.3.4/arcana/xnat/cli/entrypoint.py` & `arcana_xnat-0.3.5/arcana/xnat/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/cli/update_release.py` & `arcana_xnat-0.3.5/arcana/xnat/cli/update_release.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_add_columns.py` & `arcana_xnat-0.3.5/arcana/xnat/cli/tests/test_cli_add_columns.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_dataset_export.py` & `arcana_xnat-0.3.5/arcana/xnat/cli/tests/test_cli_dataset_export.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_store.py` & `arcana_xnat-0.3.5/arcana/xnat/cli/tests/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_xnat_images.py` & `arcana_xnat-0.3.5/arcana/xnat/cli/tests/test_cli_xnat_images.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/data/api.py` & `arcana_xnat-0.3.5/arcana/xnat/data/api.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/data/cs.py` & `arcana_xnat-0.3.5/arcana/xnat/data/cs.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/data/tests/test_store.py` & `arcana_xnat-0.3.5/arcana/xnat/data/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/deploy/command.py` & `arcana_xnat-0.3.5/arcana/xnat/deploy/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 import typing as ty
 import re
 import attrs
-from fileformats.core import FileSet
+from fileformats.core import FileSet, to_mime
 from arcana.core.deploy.command.base import ContainerCommand
 from arcana.xnat.data import XnatViaCS
 from arcana.common import Clinical
-from arcana.core.utils.serialize import ClassResolver
 
 if ty.TYPE_CHECKING:
     from .image import XnatApp
 
 
 @attrs.define(kw_only=True)
 class XnatCommand(ContainerCommand):
@@ -117,18 +116,22 @@
             list of arguments to be appended to the command line
         """
         # Add task inputs to inputs JSON specification
         cmd_args = []
         for inpt in self.inputs:
             replacement_key = f"[{inpt.field.upper()}_INPUT]"
             if issubclass(inpt.datatype, FileSet):
-                desc = f"Match resource [SCAN_TYPE]: {inpt.help} "
+                if inpt.column_defaults.datatype:
+                    datatype = inpt.column_defaults.datatype
+                else:
+                    datatype = inpt.datatype
+                desc = f"Match resource ({to_mime(datatype)}) [SCAN-TYPE]: {inpt.help} "
                 input_type = "string"
             else:
-                desc = f"Match field ({inpt.datatype}) [FIELD_NAME]: {inpt.help} "
+                desc = f"Match field ({inpt.datatype}) [FIELD-NAME]: {inpt.help} "
                 input_type = self.COMMAND_INPUT_TYPES.get(inpt.datatype, "string")
             cmd_json["inputs"].append(
                 {
                     "name": self.path2xnatname(inpt.name),
                     "description": desc,
                     "type": input_type,
                     "default-value": inpt.config_dict.get("path", ""),
@@ -173,15 +176,15 @@
             out_fname = output.name + (
                 output.datatype.ext if output.datatype.ext else ""
             )
             # Set the path to the
             cmd_json["outputs"].append(
                 {
                     "name": output.name,
-                    "description": f"{output.field} ({ClassResolver.tostr(output.datatype)})",
+                    "description": f"{output.field} ({to_mime(output.datatype)})",
                     "required": True,
                     "mount": "out",
                     "path": out_fname,
                     "glob": None,
                 }
             )
             cmd_json["xnat"][0]["output-handlers"].append(
```

### Comparing `arcana_xnat-0.3.4/arcana/xnat/deploy/image.py` & `arcana_xnat-0.3.5/arcana/xnat/deploy/image.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/deploy/tests/test_app.py` & `arcana_xnat-0.3.5/arcana/xnat/deploy/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/arcana/xnat/utils/testing.py` & `arcana_xnat-0.3.5/arcana/xnat/utils/testing.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/LICENSE` & `arcana_xnat-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/README.rst` & `arcana_xnat-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/pyproject.toml` & `arcana_xnat-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.4/PKG-INFO` & `arcana_xnat-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-xnat
-Version: 0.3.4
+Version: 0.3.5
 Summary: An extension of the Arcana framework to apply workflows and analyses on data stored within XNAT data repositories
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-xnat.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
```

