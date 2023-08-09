# Comparing `tmp/YanShi-0.0.2.tar.gz` & `tmp/Yanshi-0.0.20230809.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YanShi-0.0.2.tar", last modified: Sun Mar 21 02:49:59 2021, max compression
+gzip compressed data, was "Yanshi-0.0.20230809.tar", last modified: Wed Aug  9 03:12:52 2023, max compression
```

## Comparing `YanShi-0.0.2.tar` & `Yanshi-0.0.20230809.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2021-03-21 02:49:59.240862 YanShi-0.0.2/
--rw-rw-rw-   0        0        0      366 2021-03-21 02:49:59.235867 YanShi-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-03-21 02:49:59.198157 YanShi-0.0.2/YanShi/
--rw-rw-rw-   0        0        0        0 2021-03-21 02:20:10.000000 YanShi-0.0.2/YanShi/__init__.py
--rw-rw-rw-   0        0        0       80 2021-03-21 02:49:09.000000 YanShi-0.0.2/YanShi/yanshi.py
-drwxrwxrwx   0        0        0        0 2021-03-21 02:49:59.226864 YanShi-0.0.2/YanShi.egg-info/
--rw-rw-rw-   0        0        0      366 2021-03-21 02:49:58.000000 YanShi-0.0.2/YanShi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2021-03-21 02:49:58.000000 YanShi-0.0.2/YanShi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-21 02:49:58.000000 YanShi-0.0.2/YanShi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-03-21 02:49:58.000000 YanShi-0.0.2/YanShi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-03-21 02:49:59.241864 YanShi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      657 2021-03-21 02:49:09.000000 YanShi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:12:52.845877 Yanshi-0.0.20230809/
+-rw-rw-rw-   0        0        0      313 2023-08-09 03:12:52.844901 Yanshi-0.0.20230809/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-09 03:12:52.829527 Yanshi-0.0.20230809/YanShi2/
+-rw-rw-rw-   0        0        0       15 2023-08-09 03:09:51.000000 Yanshi-0.0.20230809/YanShi2/Yanshi.py
+-rw-rw-rw-   0        0        0        0 2023-08-09 03:09:33.000000 Yanshi-0.0.20230809/YanShi2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:12:52.841928 Yanshi-0.0.20230809/Yanshi.egg-info/
+-rw-rw-rw-   0        0        0      313 2023-08-09 03:12:52.000000 Yanshi-0.0.20230809/Yanshi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-08-09 03:12:52.000000 Yanshi-0.0.20230809/Yanshi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 03:12:52.000000 Yanshi-0.0.20230809/Yanshi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-09 03:12:52.000000 Yanshi-0.0.20230809/Yanshi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 03:12:52.846853 Yanshi-0.0.20230809/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-08-09 03:12:16.000000 Yanshi-0.0.20230809/setup.py
```

### Comparing `YanShi-0.0.2/setup.py` & `Yanshi-0.0.20230809/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 setuptools.setup(
-    name='YanShi',#库名
-    version='0.0.2',#版本号，建议一开始取0.0.1
-    author='Dingdang Wang',#你的名字，名在前，姓在后，例：张一一 Yiyi Zhang
+    name='Yanshi',#库名
+    version='0.0.20230809',#版本号，建议一开始取0.0.1
+    author='Tim Daniel Walt',#你的名字，名在前，姓在后，例：张一一 Yiyi Zhang
     author_email='1330274738@qq.com',#你的邮箱（任何邮箱都行，只要不是假的）
-    description='演示',#库介绍
+    description='???',#库介绍
     long_descripition_content_type="text/markdown",
     url='https://github.com/',
     packages=setuptools.find_packages(),
     classifiers= [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent" ,
```

