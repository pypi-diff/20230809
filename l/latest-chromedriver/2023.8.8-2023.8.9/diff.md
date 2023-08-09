# Comparing `tmp/latest-chromedriver-2023.8.8.tar.gz` & `tmp/latest-chromedriver-2023.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latest-chromedriver-2023.8.8.tar", last modified: Tue Aug  8 06:01:29 2023, max compression
+gzip compressed data, was "latest-chromedriver-2023.8.9.tar", last modified: Wed Aug  9 05:18:06 2023, max compression
```

## Comparing `latest-chromedriver-2023.8.8.tar` & `latest-chromedriver-2023.8.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 06:01:29.424022 latest-chromedriver-2023.8.8/
--rw-rw-rw-   0        0        0     1096 2022-06-23 08:33:50.000000 latest-chromedriver-2023.8.8/LICENSE
--rw-rw-rw-   0        0        0     3373 2023-08-08 06:01:29.423033 latest-chromedriver-2023.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     2558 2022-06-28 12:28:36.000000 latest-chromedriver-2023.8.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 06:01:29.388295 latest-chromedriver-2023.8.8/latest_chromedriver/
--rw-rw-rw-   0        0        0      394 2023-08-08 06:01:26.000000 latest-chromedriver-2023.8.8/latest_chromedriver/__init__.py
--rw-rw-rw-   0        0        0      321 2023-08-08 05:32:08.000000 latest-chromedriver-2023.8.8/latest_chromedriver/__main__.py
--rw-rw-rw-   0        0        0     4408 2023-08-08 05:38:32.000000 latest-chromedriver-2023.8.8/latest_chromedriver/chrome_info.py
--rw-rw-rw-   0        0        0     8197 2023-08-08 05:53:39.000000 latest-chromedriver-2023.8.8/latest_chromedriver/download_driver.py
--rw-rw-rw-   0        0        0     2567 2023-08-08 05:57:11.000000 latest-chromedriver-2023.8.8/latest_chromedriver/enviroment.py
--rw-rw-rw-   0        0        0      492 2023-08-08 05:59:59.000000 latest-chromedriver-2023.8.8/latest_chromedriver/version.py
-drwxrwxrwx   0        0        0        0 2023-08-08 06:01:29.421027 latest-chromedriver-2023.8.8/latest_chromedriver.egg-info/
--rw-rw-rw-   0        0        0     3373 2023-08-08 06:01:28.000000 latest-chromedriver-2023.8.8/latest_chromedriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-08-08 06:01:29.000000 latest-chromedriver-2023.8.8/latest_chromedriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 06:01:28.000000 latest-chromedriver-2023.8.8/latest_chromedriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-08-08 06:01:28.000000 latest-chromedriver-2023.8.8/latest_chromedriver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-08-08 06:01:29.000000 latest-chromedriver-2023.8.8/latest_chromedriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-08 06:01:29.000000 latest-chromedriver-2023.8.8/latest_chromedriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 06:01:29.425019 latest-chromedriver-2023.8.8/setup.cfg
--rw-rw-rw-   0        0        0     1860 2023-08-08 06:01:26.000000 latest-chromedriver-2023.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 05:18:06.712664 latest-chromedriver-2023.8.9/
+-rw-rw-rw-   0        0        0     1096 2022-06-23 08:33:50.000000 latest-chromedriver-2023.8.9/LICENSE
+-rw-rw-rw-   0        0        0     3373 2023-08-09 05:18:06.711665 latest-chromedriver-2023.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2558 2022-06-28 12:28:36.000000 latest-chromedriver-2023.8.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 05:18:06.666761 latest-chromedriver-2023.8.9/latest_chromedriver/
+-rw-rw-rw-   0        0        0      394 2023-08-09 05:18:03.000000 latest-chromedriver-2023.8.9/latest_chromedriver/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-08-08 05:32:08.000000 latest-chromedriver-2023.8.9/latest_chromedriver/__main__.py
+-rw-rw-rw-   0        0        0     4408 2023-08-08 05:38:32.000000 latest-chromedriver-2023.8.9/latest_chromedriver/chrome_info.py
+-rw-rw-rw-   0        0        0     8946 2023-08-09 05:16:14.000000 latest-chromedriver-2023.8.9/latest_chromedriver/download_driver.py
+-rw-rw-rw-   0        0        0     2567 2023-08-08 05:57:11.000000 latest-chromedriver-2023.8.9/latest_chromedriver/enviroment.py
+-rw-rw-rw-   0        0        0      492 2023-08-08 05:59:59.000000 latest-chromedriver-2023.8.9/latest_chromedriver/version.py
+drwxrwxrwx   0        0        0        0 2023-08-09 05:18:06.706706 latest-chromedriver-2023.8.9/latest_chromedriver.egg-info/
+-rw-rw-rw-   0        0        0     3373 2023-08-09 05:18:05.000000 latest-chromedriver-2023.8.9/latest_chromedriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-08-09 05:18:06.000000 latest-chromedriver-2023.8.9/latest_chromedriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 05:18:05.000000 latest-chromedriver-2023.8.9/latest_chromedriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-08-09 05:18:06.000000 latest-chromedriver-2023.8.9/latest_chromedriver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-08-09 05:18:06.000000 latest-chromedriver-2023.8.9/latest_chromedriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-09 05:18:06.000000 latest-chromedriver-2023.8.9/latest_chromedriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 05:18:06.712664 latest-chromedriver-2023.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     1860 2023-08-09 05:18:03.000000 latest-chromedriver-2023.8.9/setup.py
```

### Comparing `latest-chromedriver-2023.8.8/LICENSE` & `latest-chromedriver-2023.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `latest-chromedriver-2023.8.8/PKG-INFO` & `latest-chromedriver-2023.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latest-chromedriver
-Version: 2023.8.8
+Version: 2023.8.9
 Summary: A small package to find the correct chromedriver version in windows machines
 Home-page: https://github.com/hargikas/auto-chromedriver/
 Author: Charalampos Gkikas
 Author-email: hargikas@gmail.com
 License: MIT
 Project-URL: Say Thanks!, https://saythanks.io/to/hargikas
 Project-URL: Source, https://github.com/hargikas/auto-chromedriver/
```

### Comparing `latest-chromedriver-2023.8.8/README.md` & `latest-chromedriver-2023.8.9/README.md`

 * *Files identical despite different names*

### Comparing `latest-chromedriver-2023.8.8/latest_chromedriver/chrome_info.py` & `latest-chromedriver-2023.8.9/latest_chromedriver/chrome_info.py`

 * *Files identical despite different names*

### Comparing `latest-chromedriver-2023.8.8/latest_chromedriver/download_driver.py` & `latest-chromedriver-2023.8.9/latest_chromedriver/download_driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,44 +75,72 @@
     if system_name == 'Linux':
         return "chromedriver"
     if system_name == 'Darwin':
         return "chromedriver"
     return None
 
 
+def _offset_max_scale_list(chrome_version, json_cft):
+    chrome_version_list = [int(x) for x in chrome_version.split('.')]
+    no_of_items = len(chrome_version_list)
+    min_version = chrome_version_list.copy()
+    max_version = chrome_version_list.copy()
+
+    for item in json_cft["versions"]:
+        item_version_list = [int(x) for x in item["version"].split('.')]
+        for i, value in enumerate(item_version_list):
+            min_version[i] = min(min_version[i], value)
+            max_version[i] = max(max_version[i], value)
+
+    version_size = [max_version[i]-min_version[i] for i in range(no_of_items)]
+    current_offset = [chrome_version_list[i]-min_version[i]
+                      for i in range(no_of_items)]
+
+    result = []
+    scale = 1
+    for i in reversed(range(no_of_items)):
+        item = (current_offset[i], version_size[i], scale)
+        scale *= version_size[i] + 1
+        result.insert(0, item)
+
+    return result
+
+
 def get_chromedriver_version_cft(chrome_version, platform_system):
     """Find which is the latest chromedriver using 
     the Chrome for Testing availability JSON endpoints."""
     selected_version = None
     selected_url = None
     chrome_version_list = [int(x) for x in chrome_version.split('.')]
-    max_version_size = max([len(x) for x in chrome_version.split('.')])
-    order_of_score = 10**max_version_size
-    #max_eligible_version = [-1 for _x in range(chrome_version_list)]
-    max_score = float('-inf')
+    max_score = -1
+
+    response = requests.get(CFT_JSON_ENDPOINT, timeout=HTTP_TIMEOUT)
+    data = response.json()
+
+    oms_list = _offset_max_scale_list(chrome_version, data)
 
-    r = requests.get(CFT_JSON_ENDPOINT, timeout=HTTP_TIMEOUT)
-    data = r.json()
     for item in data["versions"]:
         item_version_list = [int(x) for x in item["version"].split('.')]
 
         compatibility_score = 0
-        max_magnitude_size = len(chrome_version_list)
-        for i in range(max_magnitude_size):
-            magnitude_size = order_of_score**(max_magnitude_size - i)
-            if item_version_list[i] == chrome_version_list[i]:
-                compatibility_score += magnitude_size
-            elif item_version_list[i] < chrome_version_list[i]:
-                version_mismatch = int(
-                    (1.0 - (item_version_list[i]/chrome_version_list[i]))*magnitude_size)
-                compatibility_score += magnitude_size - version_mismatch
-            else:
-                compatibility_score -= magnitude_size
+        no_of_items = len(chrome_version_list)
+        temp_score = [0, 0, 0, 0]
+        for i in range(no_of_items):
+            diff = chrome_version_list[i] - item_version_list[i]
+            (offset, max_diff, scale) = oms_list[i]
+
+            # If the version is newer is penalized.
+            # Newer version are getting behind older ones.
+            if diff < 0:
+                diff = offset - diff
+
+            temp_score[i] = max_diff - diff
+            compatibility_score += (max_diff - diff) * scale
 
-        if compatibility_score > max_score:
+        if compatibility_score >= max_score:
             if "chromedriver" in item["downloads"]:
                 for download in item["downloads"]["chromedriver"]:
                     if download["platform"] == platform_system:
                         max_score = compatibility_score
                         selected_version = item["version"]
                         selected_url = download["url"]
     logger.info("ChromeDriver version needed: %s", selected_version)
```

### Comparing `latest-chromedriver-2023.8.8/latest_chromedriver/enviroment.py` & `latest-chromedriver-2023.8.9/latest_chromedriver/enviroment.py`

 * *Files identical despite different names*

### Comparing `latest-chromedriver-2023.8.8/latest_chromedriver.egg-info/PKG-INFO` & `latest-chromedriver-2023.8.9/latest_chromedriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latest-chromedriver
-Version: 2023.8.8
+Version: 2023.8.9
 Summary: A small package to find the correct chromedriver version in windows machines
 Home-page: https://github.com/hargikas/auto-chromedriver/
 Author: Charalampos Gkikas
 Author-email: hargikas@gmail.com
 License: MIT
 Project-URL: Say Thanks!, https://saythanks.io/to/hargikas
 Project-URL: Source, https://github.com/hargikas/auto-chromedriver/
```

### Comparing `latest-chromedriver-2023.8.8/setup.py` & `latest-chromedriver-2023.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 import datetime
 
-__version__ = '2023.08.08'
+__version__ = '2023.08.09'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="latest-chromedriver",
     version=__version__,
```

