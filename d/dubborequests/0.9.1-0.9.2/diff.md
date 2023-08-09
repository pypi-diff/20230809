# Comparing `tmp/dubborequests-0.9.1.tar.gz` & `tmp/dubborequests-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dubborequests-0.9.1.tar", last modified: Fri Feb 17 07:35:56 2023, max compression
+gzip compressed data, was "dubborequests-0.9.2.tar", last modified: Wed Aug  9 02:26:03 2023, max compression
```

## Comparing `dubborequests-0.9.1.tar` & `dubborequests-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-02-17 07:35:56.402301 dubborequests-0.9.1/
--rw-r--r--   0 fa_junjie   (501) staff       (20)     6196 2023-02-17 07:35:56.402171 dubborequests-0.9.1/PKG-INFO
--rw-r--r--   0 fa_junjie   (501) staff       (20)     4717 2023-02-02 08:06:02.000000 dubborequests-0.9.1/README.md
-drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-02-17 07:35:56.400846 dubborequests-0.9.1/dubborequests/
--rw-r--r--   0 fa_junjie   (501) staff       (20)      207 2023-02-01 14:29:05.000000 dubborequests-0.9.1/dubborequests/__init__.py
--rw-r--r--   0 fa_junjie   (501) staff       (20)     3621 2023-02-17 07:33:57.000000 dubborequests-0.9.1/dubborequests/api.py
--rw-r--r--   0 fa_junjie   (501) staff       (20)      258 2022-03-22 16:17:43.000000 dubborequests-0.9.1/dubborequests/config.py
--rw-r--r--   0 fa_junjie   (501) staff       (20)     8969 2023-02-01 14:30:38.000000 dubborequests-0.9.1/dubborequests/util.py
-drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-02-17 07:35:56.401944 dubborequests-0.9.1/dubborequests.egg-info/
--rw-r--r--   0 fa_junjie   (501) staff       (20)     6196 2023-02-17 07:35:56.000000 dubborequests-0.9.1/dubborequests.egg-info/PKG-INFO
--rw-r--r--   0 fa_junjie   (501) staff       (20)      295 2023-02-17 07:35:56.000000 dubborequests-0.9.1/dubborequests.egg-info/SOURCES.txt
--rw-r--r--   0 fa_junjie   (501) staff       (20)        1 2023-02-17 07:35:56.000000 dubborequests-0.9.1/dubborequests.egg-info/dependency_links.txt
--rw-r--r--   0 fa_junjie   (501) staff       (20)        6 2023-02-17 07:35:56.000000 dubborequests-0.9.1/dubborequests.egg-info/requires.txt
--rw-r--r--   0 fa_junjie   (501) staff       (20)       14 2023-02-17 07:35:56.000000 dubborequests-0.9.1/dubborequests.egg-info/top_level.txt
--rw-r--r--   0 fa_junjie   (501) staff       (20)       38 2023-02-17 07:35:56.402356 dubborequests-0.9.1/setup.cfg
--rw-r--r--   0 fa_junjie   (501) staff       (20)      782 2023-02-17 07:35:39.000000 dubborequests-0.9.1/setup.py
+drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-08-09 02:26:03.314663 dubborequests-0.9.2/
+-rw-r--r--   0 fa_junjie   (501) staff       (20)     6196 2023-08-09 02:26:03.314539 dubborequests-0.9.2/PKG-INFO
+-rw-r--r--   0 fa_junjie   (501) staff       (20)     4717 2023-02-02 08:06:02.000000 dubborequests-0.9.2/README.md
+drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-08-09 02:26:03.313628 dubborequests-0.9.2/dubborequests/
+-rw-r--r--   0 fa_junjie   (501) staff       (20)      207 2023-02-01 14:29:05.000000 dubborequests-0.9.2/dubborequests/__init__.py
+-rw-r--r--   0 fa_junjie   (501) staff       (20)     3654 2023-08-09 01:34:13.000000 dubborequests-0.9.2/dubborequests/api.py
+-rw-r--r--   0 fa_junjie   (501) staff       (20)      258 2023-03-24 03:07:07.000000 dubborequests-0.9.2/dubborequests/config.py
+-rw-r--r--   0 fa_junjie   (501) staff       (20)     8969 2023-06-06 06:54:17.000000 dubborequests-0.9.2/dubborequests/util.py
+drwxr-xr-x   0 fa_junjie   (501) staff       (20)        0 2023-08-09 02:26:03.314330 dubborequests-0.9.2/dubborequests.egg-info/
+-rw-r--r--   0 fa_junjie   (501) staff       (20)     6196 2023-08-09 02:26:03.000000 dubborequests-0.9.2/dubborequests.egg-info/PKG-INFO
+-rw-r--r--   0 fa_junjie   (501) staff       (20)      295 2023-08-09 02:26:03.000000 dubborequests-0.9.2/dubborequests.egg-info/SOURCES.txt
+-rw-r--r--   0 fa_junjie   (501) staff       (20)        1 2023-08-09 02:26:03.000000 dubborequests-0.9.2/dubborequests.egg-info/dependency_links.txt
+-rw-r--r--   0 fa_junjie   (501) staff       (20)        6 2023-08-09 02:26:03.000000 dubborequests-0.9.2/dubborequests.egg-info/requires.txt
+-rw-r--r--   0 fa_junjie   (501) staff       (20)       14 2023-08-09 02:26:03.000000 dubborequests-0.9.2/dubborequests.egg-info/top_level.txt
+-rw-r--r--   0 fa_junjie   (501) staff       (20)       38 2023-08-09 02:26:03.314703 dubborequests-0.9.2/setup.cfg
+-rw-r--r--   0 fa_junjie   (501) staff       (20)      782 2023-08-09 02:24:51.000000 dubborequests-0.9.2/setup.py
```

### Comparing `dubborequests-0.9.1/PKG-INFO` & `dubborequests-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dubborequests
-Version: 0.9.1
+Version: 0.9.2
 Summary: Telnet command test dubbo
 Home-page: https://github.com/JokerChat/dubbo_requests
 Author: fang
 Author-email: 664616581@qq.com
 License: MIT
 Description: ### 一、安装（python版本建议3.7以上）
```

### Comparing `dubborequests-0.9.1/README.md` & `dubborequests-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `dubborequests-0.9.1/dubborequests/api.py` & `dubborequests-0.9.2/dubborequests/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,18 @@
     通过zookeeper获取服务的ip和端口, invoke命令测试dubbo接口
     :param service_name: 服务名zk_invoke
     :param method_name: 方法名
     :param data: 参数对象
     :param version: 版本号
     :return:
     """
-    dubbo_conn, dubbo_data = __get_conn_dto(service_name, version)
-    param_type_list = dubbo_conn.ls_command(dubbo_data['interface'], method_name)[method_name]
+    dubbo_conn, service_data = __get_conn_dto(service_name, version)
+    param_type_list = dubbo_conn.ls_command(service_data['interface'], method_name)[method_name]
     invoke_data = dubbo_conn.invoke(service_name, method_name, data, param_type_list)
-    return dict(invoke_data=invoke_data, param_type_list=param_type_list)
+    return dict(invoke_data=invoke_data, param_type_list=param_type_list, service_data = service_data)
 
 def telnet_invoke(ip, port, service_name, method_name, data):
     """
     手动telnet测试dubbo接口
     :param ip: ip
     :param port: 端口
     :param service_name: 服务名
```

### Comparing `dubborequests-0.9.1/dubborequests/util.py` & `dubborequests-0.9.2/dubborequests/util.py`

 * *Files identical despite different names*

### Comparing `dubborequests-0.9.1/dubborequests.egg-info/PKG-INFO` & `dubborequests-0.9.2/dubborequests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dubborequests
-Version: 0.9.1
+Version: 0.9.2
 Summary: Telnet command test dubbo
 Home-page: https://github.com/JokerChat/dubbo_requests
 Author: fang
 Author-email: 664616581@qq.com
 License: MIT
 Description: ### 一、安装（python版本建议3.7以上）
```

### Comparing `dubborequests-0.9.1/setup.py` & `dubborequests-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dubborequests",
-    version="0.9.1",
+    version="0.9.2",
     author="fang",
     author_email="664616581@qq.com",
     description="Telnet command test dubbo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JokerChat/dubbo_requests",
     packages=setuptools.find_packages(),
```

