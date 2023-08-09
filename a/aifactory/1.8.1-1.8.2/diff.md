# Comparing `tmp/aifactory-1.8.1.tar.gz` & `tmp/aifactory-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.8.1.tar", last modified: Thu Aug  3 11:57:30 2023, max compression
+gzip compressed data, was "aifactory-1.8.2.tar", last modified: Wed Aug  9 01:58:15 2023, max compression
```

## Comparing `aifactory-1.8.1.tar` & `aifactory-1.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-03 11:57:30.921949 aifactory-1.8.1/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-03 11:57:30.921764 aifactory-1.8.1/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-03 11:57:30.920641 aifactory-1.8.1/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.1/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.1/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.1/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.1/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.1/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)    13397 2023-08-03 11:11:47.000000 aifactory-1.8.1/aifactory/score.py
--rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.1/aifactory/train.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-03 11:57:30.921465 aifactory-1.8.1/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-03 11:57:30.000000 aifactory-1.8.1/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-03 11:57:30.000000 aifactory-1.8.1/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-03 11:57:30.000000 aifactory-1.8.1/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-03 11:57:30.000000 aifactory-1.8.1/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-03 11:57:30.000000 aifactory-1.8.1/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-03 11:57:30.922009 aifactory-1.8.1/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-08-03 11:11:10.000000 aifactory-1.8.1/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 01:58:15.285806 aifactory-1.8.2/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 01:58:15.285646 aifactory-1.8.2/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 01:58:15.284713 aifactory-1.8.2/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14001 2023-08-09 01:55:13.000000 aifactory-1.8.2/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.8.2/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-08-09 01:58:15.285355 aifactory-1.8.2/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-08-09 01:58:15.000000 aifactory-1.8.2/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-08-09 01:58:15.285857 aifactory-1.8.2/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-08-09 01:36:48.000000 aifactory-1.8.2/setup.py
```

### Comparing `aifactory-1.8.1/aifactory/api.py` & `aifactory-1.8.2/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.1/aifactory/demo.py` & `aifactory-1.8.2/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.1/aifactory/grade.py` & `aifactory-1.8.2/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.1/aifactory/make_zip.py` & `aifactory-1.8.2/aifactory/make_zip.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.8.1/aifactory/score.py` & `aifactory-1.8.2/aifactory/score.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,16 +155,38 @@
     main_name = ipynbname.name()
   except Exception as e:
     main_name = "task.py"
 
   print("file : {0}".format(main_name))
   make_zip(main_name)
   
-  # with open('./aif.zip', 'rb') as f:
-  #   data = f.read()
+  file_size = os.path.getsize("./aif.zip")
+  gsize = file_size / 1024 ** 3
+
+  print(gsize)
+  try:
+    checkData = { "key" : key }
+    res = requests.post(apiTestUrl + "/submission/getMaxSize", json=checkData)
+    if res.status_code != 200:
+      print("서버 오류")
+      return 
+    dataJson = json.loads(res.text)  
+    ct = dataJson["ct"]
+    if ct == 0 :
+      size = data_json["size"]
+      fsize = float(size)
+      if fsize > 0 and gsize > fsize: 
+        print("파일 제한 용량을 초과하였습니다.")       
+        return
+    else:
+      print(data_json["message"])       
+      return
+  except Exception as e:
+    print(str(e))
+    return   
 
   file = open('./aif.zip', 'rb')
   try:        
     submitData = {"key" : key, "modelname" : model_name, "requestID": "0", "fileName": "0"}    
     res = requests.post(serverTestUrl + "/submit", json=submitData)
     if res.status_code != 200:
       print("중계서버 오류")
```

