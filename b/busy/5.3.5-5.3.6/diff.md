# Comparing `tmp/busy-5.3.5.tar.gz` & `tmp/busy-5.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-5.3.5.tar", last modified: Fri Aug  4 18:14:03 2023, max compression
+gzip compressed data, was "busy-5.3.6.tar", last modified: Wed Aug  9 04:26:35 2023, max compression
```

## Comparing `busy-5.3.5.tar` & `busy-5.3.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.546876 busy-5.3.5/
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 18:13:14.000000 busy-5.3.5/.version
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-08-04 18:13:55.000000 busy-5.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22714 2023-08-04 18:14:03.546876 busy-5.3.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    22464 2023-08-04 18:13:55.000000 busy-5.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.535876 busy-5.3.5/busy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 18:13:55.000000 busy-5.3.5/busy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-08-04 18:13:55.000000 busy-5.3.5/busy/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.541876 busy-5.3.5/busy/command/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/activate_command.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/add_command.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/base_command.py
--rw-rw-rw-   0 root         (0) root         (0)     6834 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/command.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/curses_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/defer_command.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/delete_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/drop_and_pop_command.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/edit_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/finish_command.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/list_command.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/print_command.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/queues_command.py
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/resource_command.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/show_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/switch_command.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-08-04 18:13:55.000000 busy-5.3.5/busy/command/tags_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3555 2023-08-04 18:13:55.000000 busy-5.3.5/busy/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.541876 busy-5.3.5/busy/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 18:13:55.000000 busy-5.3.5/busy/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.542876 busy-5.3.5/busy/model/collection/
--rw-rw-rw-   0 root         (0) root         (0)     5020 2023-08-04 18:13:55.000000 busy-5.3.5/busy/model/collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-04 18:13:55.000000 busy-5.3.5/busy/model/collection/done_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-04 18:13:55.000000 busy-5.3.5/busy/model/collection/plan_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-04 18:13:55.000000 busy-5.3.5/busy/model/collection/skip_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-04 18:13:55.000000 busy-5.3.5/busy/model/collection/todo_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2023-08-04 18:13:55.000000 busy-5.3.5/busy/model/item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.543876 busy-5.3.5/busy/storage/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-04 18:13:55.000000 busy-5.3.5/busy/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-08-04 18:13:55.000000 busy-5.3.5/busy/storage/file_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.544876 busy-5.3.5/busy/ui/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-08-04 18:13:55.000000 busy-5.3.5/busy/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6690 2023-08-04 18:13:55.000000 busy-5.3.5/busy/ui/curses_ui.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-08-04 18:13:55.000000 busy-5.3.5/busy/ui/shell_ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.544876 busy-5.3.5/busy/ui/tcl_ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 18:13:55.000000 busy-5.3.5/busy/ui/tcl_ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-04 18:13:55.000000 busy-5.3.5/busy/ui/tcl_ui/edit_task_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-08-04 18:13:55.000000 busy-5.3.5/busy/ui/tcl_ui/get_item_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     5588 2023-08-04 18:13:55.000000 busy-5.3.5/busy/ui/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.545876 busy-5.3.5/busy/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 18:13:55.000000 busy-5.3.5/busy/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4443 2023-08-04 18:13:55.000000 busy-5.3.5/busy/util/checklist.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-08-04 18:13:55.000000 busy-5.3.5/busy/util/date_util.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-08-04 18:13:55.000000 busy-5.3.5/busy/util/python_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-08-04 18:13:55.000000 busy-5.3.5/busy/util/selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 18:14:03.537876 busy-5.3.5/busy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22714 2023-08-04 18:14:03.000000 busy-5.3.5/busy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1384 2023-08-04 18:14:03.000000 busy-5.3.5/busy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 18:14:03.000000 busy-5.3.5/busy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-08-04 18:14:03.000000 busy-5.3.5/busy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2023-08-04 18:14:03.000000 busy-5.3.5/busy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-04 18:14:03.000000 busy-5.3.5/busy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-08-04 18:13:55.000000 busy-5.3.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 18:14:03.546876 busy-5.3.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.263558 busy-5.3.6/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-09 04:25:47.000000 busy-5.3.6/.version
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-08-09 04:26:27.000000 busy-5.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-08-09 04:26:35.263558 busy-5.3.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22464 2023-08-09 04:26:27.000000 busy-5.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.253558 busy-5.3.6/busy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-09 04:26:27.000000 busy-5.3.6/busy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-08-09 04:26:27.000000 busy-5.3.6/busy/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.258558 busy-5.3.6/busy/command/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/activate_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/add_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/base_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     6879 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/curses_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/defer_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/delete_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/drop_and_pop_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/edit_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/finish_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/list_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/print_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/queues_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/resource_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/show_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/switch_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-08-09 04:26:27.000000 busy-5.3.6/busy/command/tags_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3555 2023-08-09 04:26:27.000000 busy-5.3.6/busy/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.258558 busy-5.3.6/busy/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-09 04:26:27.000000 busy-5.3.6/busy/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.259558 busy-5.3.6/busy/model/collection/
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-08-09 04:26:27.000000 busy-5.3.6/busy/model/collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-09 04:26:27.000000 busy-5.3.6/busy/model/collection/done_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-08-09 04:26:27.000000 busy-5.3.6/busy/model/collection/plan_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-09 04:26:27.000000 busy-5.3.6/busy/model/collection/skip_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-08-09 04:26:27.000000 busy-5.3.6/busy/model/collection/todo_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-08-09 04:26:27.000000 busy-5.3.6/busy/model/item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.260558 busy-5.3.6/busy/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-08-09 04:26:27.000000 busy-5.3.6/busy/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-08-09 04:26:27.000000 busy-5.3.6/busy/storage/file_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.261558 busy-5.3.6/busy/ui/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-08-09 04:26:27.000000 busy-5.3.6/busy/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7823 2023-08-09 04:26:27.000000 busy-5.3.6/busy/ui/curses_ui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-08-09 04:26:27.000000 busy-5.3.6/busy/ui/shell_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.261558 busy-5.3.6/busy/ui/tcl_ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-09 04:26:27.000000 busy-5.3.6/busy/ui/tcl_ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-09 04:26:27.000000 busy-5.3.6/busy/ui/tcl_ui/edit_task_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-08-09 04:26:27.000000 busy-5.3.6/busy/ui/tcl_ui/get_item_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5588 2023-08-09 04:26:27.000000 busy-5.3.6/busy/ui/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.263558 busy-5.3.6/busy/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-09 04:26:27.000000 busy-5.3.6/busy/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4443 2023-08-09 04:26:27.000000 busy-5.3.6/busy/util/checklist.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-08-09 04:26:27.000000 busy-5.3.6/busy/util/date_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-08-09 04:26:27.000000 busy-5.3.6/busy/util/python_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-08-09 04:26:27.000000 busy-5.3.6/busy/util/selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 04:26:35.254557 busy-5.3.6/busy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-08-09 04:26:35.000000 busy-5.3.6/busy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-08-09 04:26:35.000000 busy-5.3.6/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 04:26:35.000000 busy-5.3.6/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-08-09 04:26:35.000000 busy-5.3.6/busy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-08-09 04:26:35.000000 busy-5.3.6/busy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-09 04:26:35.000000 busy-5.3.6/busy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-08-09 04:26:27.000000 busy-5.3.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-09 04:26:35.263558 busy-5.3.6/setup.cfg
```

### Comparing `busy-5.3.5/LICENSE` & `busy-5.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/PKG-INFO` & `busy-5.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.3.5
+Version: 5.3.6
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.3.5/README.md` & `busy-5.3.6/README.md`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/activate_command.py` & `busy-5.3.6/busy/command/activate_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/add_command.py` & `busy-5.3.6/busy/command/add_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/command.py` & `busy-5.3.6/busy/command/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     @classmethod
     def set_parser(self, parser):
         self.parser = parser
 
     @classmethod
     def _add_confirmation_arg(self, parser):
         """Add argparse argument for confirmation"""
-        parser.add_argument('--yes', '-y', action='store_true')
+        parser.add_argument('--yes', '-y', action='store_true', default=None)
 
     def execute(self, method, *args, **kwargs):
         """Actually perform the command, using SuperWrapper"""
         self.clean_args()
         result = method(self, *args, **kwargs)
         return result
 
@@ -95,15 +95,15 @@
         pass
 
     def provided(self, argument):
         """Was an argument provided?"""
         value = None
         if hasattr(self, argument):
             value = getattr(self, argument)
-        return bool(value)
+        return True if (value is False) else  bool(value)
 
     def confirm(self, verb, other_action=None):
         """Ensure that a command is confirmed by the user"""
         if self.provided('yes'):
             return self.yes
         else:
             chooser = self.ui.get_chooser(intro=f"{verb}?", default="ok")
```

### Comparing `busy-5.3.5/busy/command/defer_command.py` & `busy-5.3.6/busy/command/defer_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/delete_command.py` & `busy-5.3.6/busy/command/delete_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/drop_and_pop_command.py` & `busy-5.3.6/busy/command/drop_and_pop_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/edit_command.py` & `busy-5.3.6/busy/command/edit_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/finish_command.py` & `busy-5.3.6/busy/command/finish_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/list_command.py` & `busy-5.3.6/busy/command/list_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/command/print_command.py` & `busy-5.3.6/busy/command/print_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,36 @@
+from dataclasses import dataclass
+
 from busy.command.command import CollectionCommand
 from busy.util.checklist import Checklist
 
-
+@dataclass
 class PrintCommand(CollectionCommand):
     """Generate a Checklist PDF"""
 
+    full:bool = False
     default_criteria = ["1-"]
     name = "print"
 
+    @classmethod
+    def set_parser(self, parser):
+        super().set_parser(parser)
+        parser.add_argument('--full', '-f', action='store_true')
+
     @CollectionCommand.wrap
     def execute(self):
         checklist = Checklist()
         collection = self.storage.get_collection(
             self.queue, self.collection_state)
         indices = collection.select(*self.criteria)
         if indices:
-            items = [collection[i].base for i in indices]
+            if self.full:
+                items = [collection[i].description for i in indices]
+            else:
+                items = [collection[i].base for i in indices]
         else:
             self.status = f"Queue '{self.queue}' has " + \
                 f"no {self.collection_state} items that meet the criteria"
         queue = self.queue.capitalize()
         state = self.collection_state.capitalize()
         criteria = (": "+",".join(self.criteria)) \
             if (self.criteria != self.default_criteria) else ""
```

### Comparing `busy-5.3.5/busy/command/switch_command.py` & `busy-5.3.6/busy/command/switch_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/handler.py` & `busy-5.3.6/busy/handler.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/model/collection/__init__.py` & `busy-5.3.6/busy/model/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/model/item.py` & `busy-5.3.6/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/storage/file_storage.py` & `busy-5.3.6/busy/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/ui/shell_ui.py` & `busy-5.3.6/busy/ui/shell_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/ui/tcl_ui/edit_task_widget.py` & `busy-5.3.6/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/ui/tcl_ui/get_item_widget.py` & `busy-5.3.6/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/ui/ui.py` & `busy-5.3.6/busy/ui/ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/util/checklist.py` & `busy-5.3.6/busy/util/checklist.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/util/date_util.py` & `busy-5.3.6/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy/util/selector.py` & `busy-5.3.6/busy/util/selector.py`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/busy.egg-info/PKG-INFO` & `busy-5.3.6/busy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.3.5
+Version: 5.3.6
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.3.5/busy.egg-info/SOURCES.txt` & `busy-5.3.6/busy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `busy-5.3.5/pyproject.toml` & `busy-5.3.6/pyproject.toml`

 * *Files identical despite different names*

