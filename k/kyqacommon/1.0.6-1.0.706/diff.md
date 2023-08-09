# Comparing `tmp/kyqacommon-1.0.6.tar.gz` & `tmp/kyqacommon-1.0.706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyqacommon-1.0.6.tar", last modified: Wed Aug  9 02:15:12 2023, max compression
+gzip compressed data, was "kyqacommon-1.0.706.tar", last modified: Thu Jul  6 07:56:01 2023, max compression
```

## Comparing `kyqacommon-1.0.6.tar` & `kyqacommon-1.0.706.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 02:15:12.399950 kyqacommon-1.0.6/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 kyqacommon-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      442 2023-08-09 02:15:12.398950 kyqacommon-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       67 2022-07-28 10:32:06.000000 kyqacommon-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-09 02:15:12.389387 kyqacommon-1.0.6/kyqacommon/
--rw-rw-rw-   0        0        0       67 2022-07-28 10:07:15.000000 kyqacommon-1.0.6/kyqacommon/__init__.py
--rw-rw-rw-   0        0        0     1331 2023-08-09 02:12:32.000000 kyqacommon-1.0.6/kyqacommon/getLogger.py
--rw-rw-rw-   0        0        0     2034 2022-07-29 02:54:06.000000 kyqacommon-1.0.6/kyqacommon/uiCommonMethod.py
-drwxrwxrwx   0        0        0        0 2023-08-09 02:15:12.397951 kyqacommon-1.0.6/kyqacommon.egg-info/
--rw-rw-rw-   0        0        0      442 2023-08-09 02:15:12.000000 kyqacommon-1.0.6/kyqacommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-08-09 02:15:12.000000 kyqacommon-1.0.6/kyqacommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 02:15:12.000000 kyqacommon-1.0.6/kyqacommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-09 02:15:12.000000 kyqacommon-1.0.6/kyqacommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-09 02:15:12.399950 kyqacommon-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1002 2023-08-09 02:14:48.000000 kyqacommon-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:56:01.093958 kyqacommon-1.0.706/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 kyqacommon-1.0.706/LICENSE
+-rw-rw-rw-   0        0        0      444 2023-07-06 07:56:01.093958 kyqacommon-1.0.706/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2022-07-28 10:32:06.000000 kyqacommon-1.0.706/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 07:56:01.073104 kyqacommon-1.0.706/kyqacommon/
+-rw-rw-rw-   0        0        0       67 2022-07-28 10:07:15.000000 kyqacommon-1.0.706/kyqacommon/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-02-16 08:19:41.000000 kyqacommon-1.0.706/kyqacommon/getLogger.py
+-rw-rw-rw-   0        0        0     3075 2023-02-14 06:27:53.000000 kyqacommon-1.0.706/kyqacommon/minio_handld.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:56:01.091958 kyqacommon-1.0.706/kyqacommon/tools/
+-rw-rw-rw-   0        0        0        0 2023-07-06 07:45:55.000000 kyqacommon-1.0.706/kyqacommon/tools/__init__.py
+-rw-rw-rw-   0        0        0     6283 2023-07-06 07:49:19.000000 kyqacommon-1.0.706/kyqacommon/tools/cpu_ssh.py
+-rw-rw-rw-   0        0        0     3404 2023-07-06 07:49:19.000000 kyqacommon-1.0.706/kyqacommon/tools/dataBase.py
+-rw-rw-rw-   0        0        0      444 2023-07-06 07:49:19.000000 kyqacommon-1.0.706/kyqacommon/tools/loading_ly.py
+-rw-rw-rw-   0        0        0     2126 2022-10-12 06:55:19.000000 kyqacommon-1.0.706/kyqacommon/uiCommonMethod.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:56:01.083953 kyqacommon-1.0.706/kyqacommon.egg-info/
+-rw-rw-rw-   0        0        0      444 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 07:56:00.000000 kyqacommon-1.0.706/kyqacommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-06 07:56:01.094958 kyqacommon-1.0.706/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-07-06 07:54:03.000000 kyqacommon-1.0.706/setup.py
```

### Comparing `kyqacommon-1.0.6/LICENSE` & `kyqacommon-1.0.706/LICENSE`

 * *Files identical despite different names*

### Comparing `kyqacommon-1.0.6/kyqacommon/getLogger.py` & `kyqacommon-1.0.706/kyqacommon/getLogger.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,38 +5,33 @@
 r=os.path.abspath(os.path.dirname(__file__))
 rootpath=os.path.split(r)[0]
 sys.path.append(os.path.split(r)[0])
 import logging
 from logging import handlers
 
 
-def handle_log(log_path,log_name="AutoTest"):
+def handle_log(log_path):
     '''
 
     :param log_path: 必须定义日志文件需要保存的位置；
     :return:
     '''
     log_file_name = time.strftime("%Y%m%d", time.localtime())
-    log_dir = os.path.join(log_path,'{}_ky{}.log'.format(log_file_name,log_name))
-    kyAAT = logging.getLogger(name='kyAT')
+    log_dir = os.path.join(log_path,'{}_kyuiAutoTest.log'.format(log_file_name))
+    kyAAT = logging.getLogger(name='kyAAT')
 
     pycharm = logging.StreamHandler()#控制台渠道
-
     file = handlers.TimedRotatingFileHandler( filename=log_dir, when='D', encoding='utf-8',interval=1, backupCount=10)
 
     #日志格式
-    fmt = '\033[35m'+'%(asctime)s-%(name)s-%(levelname)s-%(filename)s-%(funcName)s-[line:%(lineno)d]：'+\
-          '\033[0m\033[34m'+'%(message)s\033[0m'
-    filefmt = '%(asctime)s-%(name)s-%(levelname)s-%(filename)s-%(funcName)s-[line:%(lineno)d]：%(message)s'
+    fmt = '\033[35m%(asctime)s-%(name)s-%(levelname)s-%(filename)s-%(funcName)s-[line:%(lineno)d]：%(message)s\033[0m'
+    log_fmt = logging.Formatter(fmt=fmt)
 
     kyAAT.setLevel(logging.DEBUG)
-    log_fmt = logging.Formatter(fmt=fmt)
-    log_fmt2 = logging.Formatter(fmt=filefmt)
 
     pycharm.setFormatter(fmt=log_fmt)
-    file.setFormatter(fmt=log_fmt2)
+    file.setFormatter(fmt=log_fmt)
 
     #渠道
     kyAAT.addHandler(pycharm)
     kyAAT.addHandler(file)
     return kyAAT
-log= handle_log("./")
```

### Comparing `kyqacommon-1.0.6/kyqacommon/uiCommonMethod.py` & `kyqacommon-1.0.706/kyqacommon/uiCommonMethod.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,18 @@
         anydlg ,filePath,fileName = func(*args,**arges)
         '''
         :param anydlg: dlg
         :param filePath: 文件路径
         :param fileName: 文件名称
         '''
         action = "anydlg.print_control_identifiers()"
-        identifiersPath = os.path.join(filePath, "identifiersFile",
+        fp =os.path.join(filePath, "identifiersFile")
+        if not os.path.exists(fp):
+            os.mkdir(fp)
+        identifiersPath = os.path.join(fp,
                                        "identifiers{}_{}.txt".format(timeStr, fileName))
         with open(identifiersPath, "w", encoding="utf8") as f:
             with redirect_stdout(f):
                 eval(action)
     return __wrapper
 
 @printfiers
```

### Comparing `kyqacommon-1.0.6/setup.py` & `kyqacommon-1.0.706/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kyqacommon",  # 包名
-    version="1.0.6",  # 包版本号，便于维护版本
+    version="1.0.706",  # 包版本号，便于维护版本
     author="lyl",  # 作者
     author_email="lyulei66@163.com",  # 联系方式
     description="kyqacommon",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
+    install_requires = ["minio==7.1.13","pymysql==1.0.3","progress==1.6","paramiko==3.2.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',  # 对python的最低版本要求
 )
-'''
-Python setup.py sdist bdist_wheel
-Python -m twine upload——repository pypi dist/*
-'''
```

