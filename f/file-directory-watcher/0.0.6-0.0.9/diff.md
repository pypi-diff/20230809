# Comparing `tmp/file-directory-watcher-0.0.6.tar.gz` & `tmp/file-directory-watcher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-directory-watcher-0.0.6.tar", last modified: Thu Aug  3 22:26:31 2023, max compression
+gzip compressed data, was "file-directory-watcher-0.0.9.tar", last modified: Wed Aug  9 01:01:43 2023, max compression
```

## Comparing `file-directory-watcher-0.0.6.tar` & `file-directory-watcher-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.913291 file-directory-watcher-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.905290 file-directory-watcher-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.909290 file-directory-watcher-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.909290 file-directory-watcher-0.0.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 22:26:31.913291 file-directory-watcher-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-03 22:26:20.000000 file-directory-watcher-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 22:26:31.913291 file-directory-watcher-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.909290 file-directory-watcher-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.909290 file-directory-watcher-0.0.6/src/fdw/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/src/fdw/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.909290 file-directory-watcher-0.0.6/src/file_directory_watcher/
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/src/file_directory_watcher/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/src/file_directory_watcher/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/src/file_directory_watcher/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/src/file_directory_watcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.913291 file-directory-watcher-0.0.6/src/file_directory_watcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 22:26:31.000000 file-directory-watcher-0.0.6/src/file_directory_watcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-03 22:26:31.000000 file-directory-watcher-0.0.6/src/file_directory_watcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 22:26:31.000000 file-directory-watcher-0.0.6/src/file_directory_watcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 22:26:31.000000 file-directory-watcher-0.0.6/src/file_directory_watcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 22:26:31.000000 file-directory-watcher-0.0.6/src/file_directory_watcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:26:31.913291 file-directory-watcher-0.0.6/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/tools/reinstall.bash
--rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-08-03 22:26:09.000000 file-directory-watcher-0.0.6/tools/update-version.bash
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.047843 file-directory-watcher-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.043843 file-directory-watcher-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.043843 file-directory-watcher-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.043843 file-directory-watcher-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-09 01:01:43.047843 file-directory-watcher-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.043843 file-directory-watcher-0.0.9/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   105889 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/images/fdw-running-normal.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-09 01:01:34.000000 file-directory-watcher-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:01:43.047843 file-directory-watcher-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.043843 file-directory-watcher-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.043843 file-directory-watcher-0.0.9/src/fdw/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/src/fdw/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.043843 file-directory-watcher-0.0.9/src/file_directory_watcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/src/file_directory_watcher/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/src/file_directory_watcher/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/src/file_directory_watcher/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/src/file_directory_watcher/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/src/file_directory_watcher/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/src/file_directory_watcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.047843 file-directory-watcher-0.0.9/src/file_directory_watcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-09 01:01:43.000000 file-directory-watcher-0.0.9/src/file_directory_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-09 01:01:43.000000 file-directory-watcher-0.0.9/src/file_directory_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:01:43.000000 file-directory-watcher-0.0.9/src/file_directory_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-09 01:01:43.000000 file-directory-watcher-0.0.9/src/file_directory_watcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-09 01:01:43.000000 file-directory-watcher-0.0.9/src/file_directory_watcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:01:43.047843 file-directory-watcher-0.0.9/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/tools/reinstall.bash
+-rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-08-09 01:01:26.000000 file-directory-watcher-0.0.9/tools/update-version.bash
```

### Comparing `file-directory-watcher-0.0.6/.github/workflows/publish-to-pypi.yaml` & `file-directory-watcher-0.0.9/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.0.6/LICENSE` & `file-directory-watcher-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `file-directory-watcher-0.0.6/pyproject.toml` & `file-directory-watcher-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "file-directory-watcher"
-version = "0.0.6"
+version = "0.0.9"
 description = "CLI tool for monitoring changes, additions, removals in files and directories and optionally running commands on specified operations."
 readme = "README.md"
 keywords = ["file", "directory", "watcher", "fdw", "changes", "monitoring", "monitor", "watch"]
 
 [project.urls]
 Repository = "https://github.com/michalpokusa/file-directory-watcher"
```

### Comparing `file-directory-watcher-0.0.6/src/file_directory_watcher/app.py` & `file-directory-watcher-0.0.9/src/file_directory_watcher/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,120 @@
 from time import sleep
 
 from .argument_parser import FDWArgs
 from .cli import CLI
+from .const import (
+    FILE_ADDED,
+    FILE_MODIFIED,
+    FILE_REMOVED,
+    DIRECTORY_ADDED,
+    DIRECTORY_MODIFIED,
+    DIRECTORY_REMOVED,
+)
 from .utils import (
     File,
     Directory,
-    OperationType,
     fs_entries_from_patterns,
     changes_in_entries,
     compute_state,
     expand_command_variables,
-    run_commands,
+    run_command,
 )
 
 
 class FDW:
 
     args: FDWArgs
 
     def __init__(self, args: FDWArgs):
         self.args = args
 
-        self.cli = CLI(self.args.color)
+        self.cli = CLI(self.args.verbosity, self.args.no_color)
         self.states: "dict[File | Directory]" = {}
 
     def _compute_state_for_entry(self, entry: "File | Directory"):
-        compare_method = type(entry) == File and self.args.file_compare_method or self.args.directory_compare_method
-        return compute_state(entry, compare_method)
+        compare_methods = type(entry) == File and self.args.file_compare_methods or self.args.directory_compare_methods
+        return compute_state(entry, compare_methods)
 
     def compute_starting_states(self):
-        for entry in fs_entries_from_patterns(self.args.patterns):
+        for entry in fs_entries_from_patterns(self.args.patterns, self.args.exclude_patterns):
             self.states.setdefault(entry, self._compute_state_for_entry(entry))
 
     def _should_handle_added(self, entry: "File | Directory") -> bool:
         if type(entry) == File:
-            return OperationType.FILE_ADDED.value in self.args.operations
+            return FILE_ADDED in self.args.watched_operations
         if type(entry) == Directory:
-            return OperationType.DIRECTORY_ADDED.value in self.args.operations
+            return DIRECTORY_ADDED in self.args.watched_operations
 
     def _handle_added(self, entry: "File | Directory"):
         self.states.setdefault(entry, self._compute_state_for_entry(entry))
 
         if not self._should_handle_added(entry):
             return
 
         commands = type(entry) == File and self.args.commands_on_file_add or self.args.commands_on_directory_add
         expanded_commands = [expand_command_variables(command, entry) for command in commands]
 
         self.cli.added_entry(entry)
-        self.cli.running_commands(expanded_commands)
-        run_commands(*expanded_commands, background=self.args.background)
+        for command in expanded_commands:
+            self.cli.running_command(command, self.args.background)
+            run_command(command, self.args.background)
 
     def _compare_file_states(self, entry: "File | Directory") -> bool:
         self._cached_entry_state = self._compute_state_for_entry(entry)
 
         return self.states.get(entry) == self._cached_entry_state
 
     def _should_handle_modified(self, entry: "File | Directory") -> bool:
         if type(entry) == File:
-            return OperationType.FILE_MODIFIED.value in self.args.operations
+            return FILE_MODIFIED in self.args.watched_operations
         if type(entry) == Directory:
-            return OperationType.DIRECTORY_MODIFIED.value in self.args.operations
+            return DIRECTORY_MODIFIED in self.args.watched_operations
 
     def _handle_modified(self, entry: "File | Directory"):
         self.states[entry] = self._cached_entry_state
         self._cached_entry_state = None
 
         if not self._should_handle_modified(entry):
             return
 
         commands = type(entry) == File and self.args.commands_on_file_modify or self.args.commands_on_directory_modify
         expanded_commands = [expand_command_variables(command, entry) for command in commands]
 
         self.cli.modified_entry(entry)
-        self.cli.running_commands(expanded_commands)
-        run_commands(*expanded_commands, background=self.args.background)
+        for command in expanded_commands:
+            self.cli.running_command(command, self.args.background)
+            run_command(command, self.args.background)
 
     def _should_handle_removed(self, entry: "File | Directory") -> bool:
         if type(entry) == File:
-            return OperationType.FILE_REMOVED.value in self.args.operations
+            return FILE_REMOVED in self.args.watched_operations
         if type(entry) == Directory:
-            return OperationType.DIRECTORY_REMOVED.value in self.args.operations
+            return DIRECTORY_REMOVED in self.args.watched_operations
 
     def _handle_removed(self, entry: "File | Directory"):
         self.states.pop(entry)
 
         if not self._should_handle_removed(entry):
             return
 
         commands = type(entry) == File and self.args.commands_on_file_remove or self.args.commands_on_directory_remove
         expanded_commands = [expand_command_variables(command, entry) for command in commands]
 
         self.cli.removed_entry(entry)
-        self.cli.running_commands(expanded_commands)
-        run_commands(*expanded_commands, background=self.args.background)
+        for command in expanded_commands:
+            self.cli.running_command(command, self.args.background)
+            run_command(command, self.args.background)
 
     def watch_for_changes(self):
-        self.cli.watching_files([fse.path for fse in self.states])
+        self.cli.watching_entries(self.states)
 
         while True:
             previous_entries = set(self.states.keys())
-            current_entries = set(fs_entries_from_patterns(self.args.patterns))
+            current_entries = set(fs_entries_from_patterns(self.args.patterns, self.args.exclude_patterns))
 
             for (entry, added, present_in_both, removed) in changes_in_entries(previous_entries, current_entries):
                 self.args.delay and sleep(self.args.delay)
 
                 if added:
                     self._handle_added(entry)
                     continue
```

### Comparing `file-directory-watcher-0.0.6/src/file_directory_watcher.egg-info/SOURCES.txt` & `file-directory-watcher-0.0.9/src/file_directory_watcher.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/publish-to-pypi.yaml
 .vscode/launch.json
+images/fdw-running-normal.jpg
 src/fdw/__main__.py
 src/file_directory_watcher/app.py
 src/file_directory_watcher/argument_parser.py
 src/file_directory_watcher/cli.py
+src/file_directory_watcher/const.py
+src/file_directory_watcher/helpers.py
 src/file_directory_watcher/utils.py
 src/file_directory_watcher.egg-info/PKG-INFO
 src/file_directory_watcher.egg-info/SOURCES.txt
 src/file_directory_watcher.egg-info/dependency_links.txt
 src/file_directory_watcher.egg-info/entry_points.txt
 src/file_directory_watcher.egg-info/top_level.txt
 tools/reinstall.bash
```

