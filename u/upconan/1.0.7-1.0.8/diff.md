# Comparing `tmp/upconan-1.0.7.tar.gz` & `tmp/upconan-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upconan-1.0.7.tar", last modified: Tue May 23 11:48:50 2023, max compression
+gzip compressed data, was "upconan-1.0.8.tar", last modified: Tue Aug  8 07:08:05 2023, max compression
```

## Comparing `upconan-1.0.7.tar` & `upconan-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 11:48:50.190582 upconan-1.0.7/
--rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      490 2023-05-23 11:48:50.190582 upconan-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 11:48:50.190582 upconan-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      895 2023-05-23 11:48:35.000000 upconan-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:48:50.182677 upconan-1.0.7/src/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.7/src/__init__.py
--rw-rw-rw-   0        0        0     4799 2023-05-23 06:33:57.000000 upconan-1.0.7/src/upconan.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:48:50.189582 upconan-1.0.7/upconan.egg-info/
--rw-rw-rw-   0        0        0      490 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-23 11:48:50.000000 upconan-1.0.7/upconan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 07:08:05.761012 upconan-1.0.8/
+-rw-rw-rw-   0        0        0     1062 2023-05-19 13:12:37.000000 upconan-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      490 2023-08-08 07:08:05.759941 upconan-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-05-19 13:13:20.000000 upconan-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 07:08:05.761012 upconan-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-08-08 07:06:06.000000 upconan-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:08:05.752475 upconan-1.0.8/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 upconan-1.0.8/src/__init__.py
+-rw-rw-rw-   0        0        0     4876 2023-08-08 07:04:15.000000 upconan-1.0.8/src/upconan.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:08:05.759941 upconan-1.0.8/upconan.egg-info/
+-rw-rw-rw-   0        0        0      490 2023-08-08 07:08:05.000000 upconan-1.0.8/upconan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-08-08 07:08:05.000000 upconan-1.0.8/upconan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 07:08:05.000000 upconan-1.0.8/upconan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-08-08 07:08:05.000000 upconan-1.0.8/upconan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-08 07:08:05.000000 upconan-1.0.8/upconan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-08-08 07:08:05.000000 upconan-1.0.8/upconan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-08 07:08:05.000000 upconan-1.0.8/upconan.egg-info/top_level.txt
```

### Comparing `upconan-1.0.7/LICENSE` & `upconan-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `upconan-1.0.7/setup.py` & `upconan-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='upconan',
-    version="1.0.7",
+    version="1.0.8",
     description="一个更新conanfile的便捷工具",
     long_description="""从剪贴板复制conan包信息，更新当前路径下的conanfile.py或conanfile.txt文件中对应的conan包版本""",
     long_description_content_type='text/x-rst',
     keywords='python conan',
     author='leytou',
     author_email='hi_litao@163.com',
     url='https://github.com/leytou/upconan',
```

### Comparing `upconan-1.0.7/src/upconan.py` & `upconan-1.0.8/src/upconan.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,23 +65,25 @@
         result_dict = result.groupdict()
         result_list.append(result_dict)
     return result_list
 
 
 def FindTargetPackageInfo(curent_package_info , target_package_infos):
     for target_package_info in  target_package_infos:
-        if curent_package_info['name'] == target_package_info['name'] and curent_package_info['owner'] == target_package_info['owner']:
+        if curent_package_info['name'] == target_package_info['name']:
             return target_package_info
     return None
 
 
 def UpdatePackageInfoLine(line,curent_package_info, target_package_info ):
     updated_line =  line.replace(curent_package_info['version'], target_package_info['version'])
     if curent_package_info['channel']:
         updated_line =  updated_line.replace(curent_package_info['channel'], target_package_info['channel'])
+    if curent_package_info['owner']:
+        updated_line =  updated_line.replace(curent_package_info['owner'], target_package_info['owner'])
     return updated_line
 
 is_changed = False
 def UpdatePackageInfoLines(lines, target_package_infos):
     global is_changed
     for idx, line in enumerate(lines):
         curent_package_info = ParsePackageInfoLine(line)
```

