# Comparing `tmp/neon-phal-plugin-device-updater-0.0.1a5.tar.gz` & `tmp/neon-phal-plugin-device-updater-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-device-updater-0.0.1a5.tar", last modified: Sat Aug  5 01:32:00 2023, max compression
+gzip compressed data, was "neon-phal-plugin-device-updater-0.0.1a6.tar", last modified: Tue Aug  8 23:48:15 2023, max compression
```

## Comparing `neon-phal-plugin-device-updater-0.0.1a5.tar` & `neon-phal-plugin-device-updater-0.0.1a6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-05 01:31:56.000000 neon-phal-plugin-device-updater-0.0.1a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-05 01:31:56.000000 neon-phal-plugin-device-updater-0.0.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater/
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-08-05 01:31:56.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-05 01:31:56.000000 neon-phal-plugin-device-updater-0.0.1a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:15.712632 neon-phal-plugin-device-updater-0.0.1a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-08 23:48:10.000000 neon-phal-plugin-device-updater-0.0.1a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 23:48:15.712632 neon-phal-plugin-device-updater-0.0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 23:48:10.000000 neon-phal-plugin-device-updater-0.0.1a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:15.712632 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater/
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-08-08 23:48:10.000000 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:48:15.712632 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 23:48:15.000000 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-08 23:48:15.000000 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:48:15.000000 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 23:48:15.000000 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-08 23:48:15.000000 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 23:48:15.000000 neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:48:15.712632 neon-phal-plugin-device-updater-0.0.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-08 23:48:10.000000 neon-phal-plugin-device-updater-0.0.1a6/setup.py
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a5/LICENSE.md` & `neon-phal-plugin-device-updater-0.0.1a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.0.1a5/PKG-INFO` & `neon-phal-plugin-device-updater-0.0.1a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater/__init__.py` & `neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,18 +89,22 @@
         if not self.initramfs_url:
             raise RuntimeError("No initramfs_url configured")
         md5_request = requests.get(f"{self.initramfs_url}.md5")
         if not md5_request.ok:
             LOG.warning("Unable to get md5; downloading latest initramfs")
             return self._get_initramfs_latest()
         new_hash = md5_request.text.split('\n')[0]
-        with open(self.initramfs_real_path, 'rb') as f:
-            old_hash = hashlib.md5(f.read()).hexdigest()
+        try:
+            with open(self.initramfs_real_path, 'rb') as f:
+                old_hash = hashlib.md5(f.read()).hexdigest()
+        except Exception as e:
+            LOG.error(e)
+            old_hash = None
         if new_hash == old_hash:
-            LOG.debug("initramfs not changed")
+            LOG.info("initramfs not changed")
             return False
         LOG.info("initramfs update available")
         return True
 
     def _get_initramfs_latest(self) -> bool:
         """
         Get the latest initramfs image and check if it is different from the
@@ -117,18 +121,23 @@
             initramfs_request = requests.get(self.initramfs_url)
             if not initramfs_request.ok:
                 raise ConnectionError(f"Unable to get updated initramfs from: "
                                       f"{self.initramfs_url}")
             new_hash = hashlib.md5(initramfs_request.content).hexdigest()
             with open(self.initramfs_update_path, 'wb+') as f:
                 f.write(initramfs_request.content)
-        with open(self.initramfs_real_path, 'rb') as f:
-            old_hash = hashlib.md5(f.read()).hexdigest()
+        try:
+            with open(self.initramfs_real_path, 'rb') as f:
+                old_hash = hashlib.md5(f.read()).hexdigest()
+        except Exception as e:
+            LOG.error(e)
+            old_hash = None
         if new_hash == old_hash:
-            LOG.debug("initramfs not changed")
+            LOG.info("initramfs not changed. Removing downloaded file.")
+            remove(self.initramfs_update_path)
             return False
         return True
 
     @staticmethod
     def check_version_is_newer(current: str, latest: str) -> bool:
         """
         Compare two image versions to check if an update is available
@@ -252,17 +261,19 @@
     def update_initramfs(self, message: Message):
         """
         Handle a request to update initramfs
         @param message: `neon.update_initramfs` Message
         """
         try:
             LOG.info("Checking initramfs update")
-            if not isfile(self.initramfs_real_path):
+            if not isfile(self.initramfs_real_path) and \
+                    not message.data.get("force_update"):
                 LOG.debug("No initramfs to update")
-                response = message.response({"updated": None})
+                response = message.response({"updated": None,
+                                             "error": "No initramfs to update"})
             elif not self._get_initramfs_latest():
                 LOG.debug("No initramfs update")
                 response = message.response({"updated": False})
             else:
                 LOG.debug("Updating initramfs")
                 proc = Popen("systemctl start update-initramfs", shell=True)
                 success = proc.wait(30) == 0
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/PKG-INFO` & `neon-phal-plugin-device-updater-0.0.1a6/neon_phal_plugin_device_updater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a5/setup.py` & `neon-phal-plugin-device-updater-0.0.1a6/setup.py`

 * *Files identical despite different names*

