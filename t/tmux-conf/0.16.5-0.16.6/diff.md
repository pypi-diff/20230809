# Comparing `tmp/tmux_conf-0.16.5.tar.gz` & `tmp/tmux_conf-0.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/usr/local/my_tmux_conf/local_tmux_conf/dist/.tmp-38_n9vn4/tmux_conf-0.16.5.tar", last modified: Sun Aug  6 15:47:11 2023, max compression
+gzip compressed data, was "tmux_conf-0.16.6.tar", last modified: Tue Aug  8 21:57:55 2023, max compression
```

## Comparing `tmux_conf-0.16.5.tar` & `tmux_conf-0.16.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/
--rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-16 01:20:21.000000 tmux_conf-0.16.5/LICENSE
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-16 01:20:21.000000 tmux_conf-0.16.5/README.md
--rw-r--r--   0 jaclu      (501) staff       (20)     1588 2023-08-06 14:30:02.000000 tmux_conf-0.16.5/pyproject.toml
--rw-r--r--   0 jaclu      (501) staff       (20)       38 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/setup.cfg
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/src/
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/src/tmux_conf/
--rw-r--r--   0 jaclu      (501) staff       (20)      202 2023-08-05 13:31:39.000000 tmux_conf-0.16.5/src/tmux_conf/__init__.py
--rw-r--r--   0 jaclu      (501) staff       (20)      269 2023-08-06 14:29:47.000000 tmux_conf-0.16.5/src/tmux_conf/constants.py
--rw-r--r--   0 jaclu      (501) staff       (20)     5939 2023-08-06 01:57:04.000000 tmux_conf-0.16.5/src/tmux_conf/embedded_scripts.py
--rw-r--r--   0 jaclu      (501) staff       (20)      436 2023-08-06 01:51:53.000000 tmux_conf-0.16.5/src/tmux_conf/exceptions.py
--rw-r--r--   0 jaclu      (501) staff       (20)    15864 2023-08-06 14:28:30.000000 tmux_conf-0.16.5/src/tmux_conf/plugins.py
--rw-r--r--   0 jaclu      (501) staff       (20)    23393 2023-08-06 01:56:54.000000 tmux_conf-0.16.5/src/tmux_conf/tmux_conf.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4780 2023-08-06 01:47:51.000000 tmux_conf-0.16.5/src/tmux_conf/utils.py
--rw-r--r--   0 jaclu      (501) staff       (20)     3983 2023-08-06 01:59:30.000000 tmux_conf-0.16.5/src/tmux_conf/vers_check.py
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/src/tmux_conf.egg-info/
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/src/tmux_conf.egg-info/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)      519 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/src/tmux_conf.egg-info/SOURCES.txt
--rw-r--r--   0 jaclu      (501) staff       (20)        1 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/src/tmux_conf.egg-info/dependency_links.txt
--rw-r--r--   0 jaclu      (501) staff       (20)       10 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/src/tmux_conf.egg-info/top_level.txt
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 15:47:11.000000 tmux_conf-0.16.5/tests/
--rw-r--r--   0 jaclu      (501) staff       (20)     3775 2023-07-09 10:30:18.000000 tmux_conf-0.16.5/tests/test_embeded_scripts.py
--rw-r--r--   0 jaclu      (501) staff       (20)     8194 2023-07-11 08:30:17.000000 tmux_conf-0.16.5/tests/test_plugins.py
--rw-r--r--   0 jaclu      (501) staff       (20)    15013 2023-07-09 10:30:02.000000 tmux_conf-0.16.5/tests/test_tmux_conf.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4061 2023-07-09 10:30:07.000000 tmux_conf-0.16.5/tests/test_utils.py
--rw-r--r--   0 jaclu      (501) staff       (20)     2915 2023-07-09 10:30:10.000000 tmux_conf-0.16.5/tests/test_vers_check.py
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-08 21:57:55.575091 tmux_conf-0.16.6/
+-rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-16 01:20:21.000000 tmux_conf-0.16.6/LICENSE
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-08 21:57:55.574602 tmux_conf-0.16.6/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-16 01:20:21.000000 tmux_conf-0.16.6/README.md
+-rw-r--r--   0 jaclu      (501) staff       (20)     1588 2023-08-07 15:13:42.000000 tmux_conf-0.16.6/pyproject.toml
+-rw-r--r--   0 jaclu      (501) staff       (20)       38 2023-08-08 21:57:55.575191 tmux_conf-0.16.6/setup.cfg
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-08 21:57:55.563785 tmux_conf-0.16.6/src/
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-08 21:57:55.569284 tmux_conf-0.16.6/src/tmux_conf/
+-rw-r--r--   0 jaclu      (501) staff       (20)      202 2023-08-05 13:31:39.000000 tmux_conf-0.16.6/src/tmux_conf/__init__.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      269 2023-08-07 15:13:30.000000 tmux_conf-0.16.6/src/tmux_conf/constants.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     6136 2023-08-07 14:58:25.000000 tmux_conf-0.16.6/src/tmux_conf/embedded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      436 2023-08-06 01:51:53.000000 tmux_conf-0.16.6/src/tmux_conf/exceptions.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    15864 2023-08-06 14:28:30.000000 tmux_conf-0.16.6/src/tmux_conf/plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    23389 2023-08-07 15:12:28.000000 tmux_conf-0.16.6/src/tmux_conf/tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4780 2023-08-06 01:47:51.000000 tmux_conf-0.16.6/src/tmux_conf/utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     3983 2023-08-06 01:59:30.000000 tmux_conf-0.16.6/src/tmux_conf/vers_check.py
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-08 21:57:55.571519 tmux_conf-0.16.6/src/tmux_conf.egg-info/
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-08 21:57:55.000000 tmux_conf-0.16.6/src/tmux_conf.egg-info/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)      519 2023-08-08 21:57:55.000000 tmux_conf-0.16.6/src/tmux_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)        1 2023-08-08 21:57:55.000000 tmux_conf-0.16.6/src/tmux_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)       10 2023-08-08 21:57:55.000000 tmux_conf-0.16.6/src/tmux_conf.egg-info/top_level.txt
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-08 21:57:55.573987 tmux_conf-0.16.6/tests/
+-rw-r--r--   0 jaclu      (501) staff       (20)     3775 2023-07-09 10:30:18.000000 tmux_conf-0.16.6/tests/test_embeded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     8194 2023-07-11 08:30:17.000000 tmux_conf-0.16.6/tests/test_plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    15013 2023-07-09 10:30:02.000000 tmux_conf-0.16.6/tests/test_tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4061 2023-07-09 10:30:07.000000 tmux_conf-0.16.6/tests/test_utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     2915 2023-07-09 10:30:10.000000 tmux_conf-0.16.6/tests/test_vers_check.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tmux_conf-0.16.5/LICENSE` & `tmux_conf-0.16.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/PKG-INFO` & `tmux_conf-0.16.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux_conf
-Version: 0.16.5
+Version: 0.16.6
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

### Comparing `tmux_conf-0.16.5/README.md` & `tmux_conf-0.16.6/README.md`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/pyproject.toml` & `tmux_conf-0.16.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tmux_conf"
-version = "0.16.5"
+version = "0.16.6"
 authors = [
   { name="Jacob Lundqvist", email="Jacob.Lundqvist@gmail.com" },
 ]
 description = "Generates version checked tmux conf"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["tmux", "automation"]
```

### Comparing `tmux_conf-0.16.5/src/tmux_conf/embedded_scripts.py` & `tmux_conf-0.16.6/src/tmux_conf/embedded_scripts.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             os.makedirs(script_dir, exist_ok=True)
             if use_bash:
                 shebang = "#!/usr/bin/env bash"
             else:
                 shebang = "#!/bin/sh"
 
             script.insert(0, f"{shebang}\n")
-            script.append(scr_name)  # trigger it to run without a param
+            script.append(f'{scr_name} "$@"')  # trigger it to run without a param
 
             fname = f"{script_dir}/{scr_name}.sh"
             with open(fname, "w", encoding="utf-8") as f:
                 for line in script:
                     f.write(f"{line}\n")
 
             #  Make it run able
@@ -113,14 +113,20 @@
                 cmd += "sh"
             cmd += f" -s {scr_name}"
         else:
             cmd += f"{self.get_dir()}/{scr_name}.sh"
         cmd += '"'
         return cmd
 
+    def call_script(self, scr_name: str) -> str:
+        cmd = scr_name
+        if not self._use_embedded_scripts:
+            cmd = f"{self.get_dir()}/{scr_name}.sh"
+        return cmd
+
     def content(self):
         """Generates the code for embedded scripts to be written to
         the conf file"""
         if not (self._use_embedded_scripts and self._scripts):
             return []
 
         output = [
```

### Comparing `tmux_conf-0.16.5/src/tmux_conf/plugins.py` & `tmux_conf-0.16.6/src/tmux_conf/plugins.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/src/tmux_conf/tmux_conf.py` & `tmux_conf-0.16.6/src/tmux_conf/tmux_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     #  this is essential. It ensures tpm and other processes started
     #  inside tmux use the running tmux bin.
     #
     #  My fork also reports more detailed progress on what plugin is
     #  processed
     #
     #  set this to 'jaclu/tpm' if you want to try that one!
-    #  set it to '' if you do not want to use tpm at all.
+    #  set it to "manual" if you dont want to use tpm.
+    #  set it to '' if you do not want to use plugins at all.
     #
     plugin_handler: str = "tmux-plugins/tpm"
 
     #
     #  If true and tmux is < 3.1 thus not supporting -N bind notes
     #  this extracts the note and inserts it before the line as a comment.
     #  If false, the note is just discarded.
@@ -65,20 +66,20 @@
     #  If false, scripts are saved in scripts/ inside the tmux conf dir
     #
     use_embedded_scripts: bool = True
 
     #
     #  Indicates if this host is low on performance, don't enable
     #  demanding plugins etc, I use this on my iSH nodes.
-    #  This must be set during __init__(). It is assumed to alreadt been
+    #  This must be set during __init__(). It is assumed to already been
     #  set to the intended state when self.run() is done.
     #
     #  The only usage of this in this package is to propagate it to
     #  the plugin handler, indicating as plugins are installed and
-    #  activated, since this might take a noticeable time on slowe nodes.
+    #  activated, since this might take a noticeable time on slower nodes.
     #  It is also avaiable in derived plugin_ methods
     #
     #  Other usages of this is up to implementation classes
     #
     is_limited_host: bool = False
 
     lib_version: str = __version__
@@ -139,15 +140,15 @@
                 #
                 print()
                 print(
                     "Config has been requested for another version of tmux,"
                     + " than the one used to generate this.\n"
                     + "Since the config file will point to the tmux used, "
                     + "this might cause problems\n"
-                    + f"\ttmux vers is:    {self.vers.get_actual()}\n"  # type: ignore
+                    + f"\ttmux vers is:    {self.vers.get_actual()}\n"
                     + f"\trequested vers:  {self.vers.get()}"  # type: ignore
                 )
                 print()
                 print("WARNING: Running this config with the current tmux")
                 print("         might give some errors!")
                 print()
         self.replace_config = replace_config
@@ -349,15 +350,15 @@
         what tmux and config file is used, so that external commands
         know what to call if needed.
         """
         self.remove_conf_file()
         self._write_stdout = False
         self.write_enable(True)
 
-        print(f"Writing tmux {self.vers.get()} config to {self.conf_file}")  # type: ignore
+        print(f"Writing tmux {self.vers.get()} config to {self.conf_file}")
 
         w = self.write
         if self.use_embedded_scripts:
             w(
                 """# : << EMBEDDED-SCRIPTS-STARTING-POINT
             #
             # The above line tells embedded scripts where they start
@@ -370,15 +371,15 @@
         #      https://github.com/jaclu/tmux-conf
         #
         #      Creation time: {datetime.datetime.now().strftime("%y-%m-%d %H:%M:%S")}
         #          tmux-conf: {self.lib_version}
         #         Created on: {run_shell('hostname').strip()}"""
         )
         if self.vers.get() != self.vers.get_actual():  # type: ignore
-            w(f"#     actual version: ({self.vers.get_actual()})")  # type: ignore
+            w(f"#     actual version: ({self.vers.get_actual()})")
         w(f"#   For tmux version: {self.vers.get()}")  # type: ignore
         w(
             f"""#
         #
         #  Three env variables defining this instance of tmux:
         #
 
@@ -622,15 +623,15 @@
                 print(f"ERROR: asdf tmux does not seem to be valid: {cmd}")
                 sys.exit(1)
             #
             #  Convert asdf shim into absolute path
             #
             cmd_asdf = (
                 f'{cmd.split("shims/")[0]}installs/tmux/'
-                f'{self.vers.get().split("-",maxsplit=1)[0]}/bin/tmux'  # type: ignore
+                f'{self.vers.get().split("-",maxsplit=1)[0]}/bin/tmux'
             )
             self.use_tmux_bin(cmd_asdf)
 
     def full_path_cmd(self, cmd: str = "tmux") -> str:
         c = run_shell(f"command -v {cmd}")
         if c and c.lower().find("not found") < 0:
             cmd = c
```

### Comparing `tmux_conf-0.16.5/src/tmux_conf/utils.py` & `tmux_conf-0.16.6/src/tmux_conf/utils.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/src/tmux_conf/vers_check.py` & `tmux_conf-0.16.6/src/tmux_conf/vers_check.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/src/tmux_conf.egg-info/PKG-INFO` & `tmux_conf-0.16.6/src/tmux_conf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux-conf
-Version: 0.16.5
+Version: 0.16.6
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

### Comparing `tmux_conf-0.16.5/src/tmux_conf.egg-info/SOURCES.txt` & `tmux_conf-0.16.6/src/tmux_conf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/tests/test_embeded_scripts.py` & `tmux_conf-0.16.6/tests/test_embeded_scripts.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/tests/test_plugins.py` & `tmux_conf-0.16.6/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/tests/test_tmux_conf.py` & `tmux_conf-0.16.6/tests/test_tmux_conf.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/tests/test_utils.py` & `tmux_conf-0.16.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.5/tests/test_vers_check.py` & `tmux_conf-0.16.6/tests/test_vers_check.py`

 * *Files identical despite different names*

