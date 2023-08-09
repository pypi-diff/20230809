# Comparing `tmp/aifactory-1.8.3.tar.gz` & `tmp/aifactory-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.8.3.tar", last modified: Wed Aug  9 02:14:30 2023, max compression
+gzip compressed data, was "aifactory-1.8.4.tar", last modified: Wed Aug  9 02:20:49 2023, max compression
```

## Comparing `aifactory-1.8.3.tar` & `aifactory-1.8.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:14:30.366236 aifactory-1.8.3/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:14:30.366096 aifactory-1.8.3/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:14:30.364813 aifactory-1.8.3/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)    14001 2023-08-09 01:55:13.000000 aifactory-1.8.3/aifactory/score.py
--rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.3/aifactory/train.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:14:30.365878 aifactory-1.8.3/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-09 02:14:30.000000 aifactory-1.8.3/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-09 02:14:30.366284 aifactory-1.8.3/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-08-09 02:14:22.000000 aifactory-1.8.3/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:20:49.155355 aifactory-1.8.4/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:20:49.155176 aifactory-1.8.4/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:20:49.154172 aifactory-1.8.4/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.4/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.4/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.4/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.4/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.4/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14028 2023-08-09 02:20:05.000000 aifactory-1.8.4/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.4/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 02:20:49.154926 aifactory-1.8.4/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 02:20:49.000000 aifactory-1.8.4/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-09 02:20:49.000000 aifactory-1.8.4/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-09 02:20:49.000000 aifactory-1.8.4/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-09 02:20:49.000000 aifactory-1.8.4/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-09 02:20:49.000000 aifactory-1.8.4/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-09 02:20:49.155414 aifactory-1.8.4/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-08-09 02:20:30.000000 aifactory-1.8.4/setup.py
```

### Comparing `aifactory-1.8.3/aifactory/api.py` & `aifactory-1.8.4/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.3/aifactory/demo.py` & `aifactory-1.8.4/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.3/aifactory/grade.py` & `aifactory-1.8.4/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.3/aifactory/make_zip.py` & `aifactory-1.8.4/aifactory/make_zip.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.3/aifactory/score.py` & `aifactory-1.8.4/aifactory/score.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
   file_size = os.path.getsize("./aif.zip")
   gsize = file_size / 1024 ** 3
 
   print(gsize)
   try:
     checkData = { "key" : key }
     res = requests.post(apiTestUrl + "/submission/getMaxSize", json=checkData)
-    if res.status_code != 200:
+    if res.status_code != 200 and res.status_code != 201:
       print("서버 오류")
       return 
     dataJson = json.loads(res.text)  
     ct = dataJson["ct"]
     if ct == 0 :
       size = data_json["size"]
       fsize = float(size)
```

