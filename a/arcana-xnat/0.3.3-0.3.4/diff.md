# Comparing `tmp/arcana_xnat-0.3.3.tar.gz` & `tmp/arcana_xnat-0.3.4.tar.gz`

## Comparing `arcana_xnat-0.3.3.tar` & `arcana_xnat-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/_version.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/base.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/entrypoint.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/update_release.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_add_columns.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_dataset_export.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_store.py
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_xnat_images.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/data/__init__.py
--rw-r--r--   0        0        0    24191 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/data/api.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/data/cs.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/data/tests/test_store.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/deploy/__init__.py
--rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/deploy/command.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/deploy/image.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/deploy/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/utils/__init__.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/utils/testing.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/.gitignore
--rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/LICENSE
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/README.rst
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    21749 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/base.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/entrypoint.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/update_release.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_add_columns.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_dataset_export.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_store.py
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_xnat_images.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/data/__init__.py
+-rw-r--r--   0        0        0    24191 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/data/api.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/data/cs.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/data/tests/test_store.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/deploy/__init__.py
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/deploy/command.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/deploy/image.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/deploy/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/utils/__init__.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/arcana/xnat/utils/testing.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/.gitignore
+-rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/README.rst
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    21749 2020-02-02 00:00:00.000000 arcana_xnat-0.3.4/PKG-INFO
```

### Comparing `arcana_xnat-0.3.3/arcana/xnat/cli/entrypoint.py` & `arcana_xnat-0.3.4/arcana/xnat/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/cli/update_release.py` & `arcana_xnat-0.3.4/arcana/xnat/cli/update_release.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_add_columns.py` & `arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_add_columns.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_dataset_export.py` & `arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_dataset_export.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_store.py` & `arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_xnat_images.py` & `arcana_xnat-0.3.4/arcana/xnat/cli/tests/test_cli_xnat_images.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/data/api.py` & `arcana_xnat-0.3.4/arcana/xnat/data/api.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/data/cs.py` & `arcana_xnat-0.3.4/arcana/xnat/data/cs.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/data/tests/test_store.py` & `arcana_xnat-0.3.4/arcana/xnat/data/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/deploy/command.py` & `arcana_xnat-0.3.4/arcana/xnat/deploy/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
                 "replacement-key": "[PROJECT_ID]",
             }
         )
 
         # Access session via Container service args and derive
         if self.row_frequency == Clinical.session:
             # Set the object the pipeline is to be run against
-            cmd_json["xnat"][0]["context"] = ["xnat:imageSessionData"]
+            cmd_json["xnat"][0]["contexts"] = ["xnat:imageSessionData"]
             # Create Session input that  can be passed to the command line, which
             # will be populated by inputs derived from the XNAT session object
             # passed to the pipeline.
             cmd_json["inputs"].extend(
                 [
                     {
                         "name": "SESSION_LABEL",
```

### Comparing `arcana_xnat-0.3.3/arcana/xnat/deploy/image.py` & `arcana_xnat-0.3.4/arcana/xnat/deploy/image.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/deploy/tests/test_app.py` & `arcana_xnat-0.3.4/arcana/xnat/deploy/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/arcana/xnat/utils/testing.py` & `arcana_xnat-0.3.4/arcana/xnat/utils/testing.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/LICENSE` & `arcana_xnat-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/README.rst` & `arcana_xnat-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/pyproject.toml` & `arcana_xnat-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.3/PKG-INFO` & `arcana_xnat-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-xnat
-Version: 0.3.3
+Version: 0.3.4
 Summary: An extension of the Arcana framework to apply workflows and analyses on data stored within XNAT data repositories
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-xnat.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
```

