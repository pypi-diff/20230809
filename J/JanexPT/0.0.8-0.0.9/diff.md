# Comparing `tmp/JanexPT-0.0.8.tar.gz` & `tmp/JanexPT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanexPT-0.0.8.tar", last modified: Tue Aug  8 19:19:17 2023, max compression
+gzip compressed data, was "JanexPT-0.0.9.tar", last modified: Tue Aug  8 19:23:35 2023, max compression
```

## Comparing `JanexPT-0.0.8.tar` & `JanexPT-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:19:17.425964 JanexPT-0.0.8/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:19:17.409964 JanexPT-0.0.8/JanexPT/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:19:17.425964 JanexPT-0.0.8/JanexPT/JanexSub/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/JanexSub/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/JanexSub/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     4411 2023-08-07 22:19:53.000000 JanexPT-0.0.8/JanexPT/main.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-07 14:45:22.000000 JanexPT-0.0.8/JanexPT/train.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:19:17.425964 JanexPT-0.0.8/JanexPT.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-08 19:19:16.000000 JanexPT-0.0.8/JanexPT.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-08 19:19:17.000000 JanexPT-0.0.8/JanexPT.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-08 19:19:16.000000 JanexPT-0.0.8/JanexPT.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       17 2023-08-08 19:19:16.000000 JanexPT-0.0.8/JanexPT.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-08 19:19:16.000000 JanexPT-0.0.8/JanexPT.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-07 14:45:22.000000 JanexPT-0.0.8/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-08 19:19:17.425964 JanexPT-0.0.8/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1580 2023-08-07 22:20:23.000000 JanexPT-0.0.8/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-08 19:19:17.425964 JanexPT-0.0.8/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1320 2023-08-08 19:19:09.000000 JanexPT-0.0.8/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:23:35.787741 JanexPT-0.0.9/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:23:35.783741 JanexPT-0.0.9/JanexPT/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:23:35.787741 JanexPT-0.0.9/JanexPT/JanexSub/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.9/JanexPT/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-07 14:45:22.000000 JanexPT-0.0.9/JanexPT/JanexSub/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-07 14:45:22.000000 JanexPT-0.0.9/JanexPT/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-07 14:45:22.000000 JanexPT-0.0.9/JanexPT/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     4311 2023-08-08 19:23:10.000000 JanexPT-0.0.9/JanexPT/main.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-07 14:45:22.000000 JanexPT-0.0.9/JanexPT/train.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-08 19:23:35.783741 JanexPT-0.0.9/JanexPT.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-08 19:23:35.000000 JanexPT-0.0.9/JanexPT.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-08 19:23:35.000000 JanexPT-0.0.9/JanexPT.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-08 19:23:35.000000 JanexPT-0.0.9/JanexPT.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       17 2023-08-08 19:23:35.000000 JanexPT-0.0.9/JanexPT.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-08 19:23:35.000000 JanexPT-0.0.9/JanexPT.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-07 14:45:22.000000 JanexPT-0.0.9/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1972 2023-08-08 19:23:35.787741 JanexPT-0.0.9/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1580 2023-08-07 22:20:23.000000 JanexPT-0.0.9/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-08 19:23:35.787741 JanexPT-0.0.9/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1320 2023-08-08 19:23:29.000000 JanexPT-0.0.9/setup.py
```

### Comparing `JanexPT-0.0.8/JanexPT/main.py` & `JanexPT-0.0.9/JanexPT/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         return self.n_samples
 
 class JanexPT:
     def __init__(self, intents_file_path, thesaurus_file_path, UIName):
         self.intents_file_path = intents_file_path
         self.thesaurus_file_path = thesaurus_file_path
         self.FILE = "data.pth"
-        self.model = NeuralNet(self.input_size, self.hidden_size, self.output_size).to(self.device)
         self.UIName = UIName
         self.IntentMatcher = IntentMatcher(intents_file_path, thesaurus_file_path)
         self.intents = self.IntentMatcher.train()
 
     def SayToAI(self, input_string, user):
         try:
             self.data = torch.load(self.FILE)
```

### Comparing `JanexPT-0.0.8/JanexPT/train.py` & `JanexPT-0.0.9/JanexPT/train.py`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.8/JanexPT.egg-info/PKG-INFO` & `JanexPT-0.0.9/JanexPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `JanexPT-0.0.8/LICENSE` & `JanexPT-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.8/PKG-INFO` & `JanexPT-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `JanexPT-0.0.8/README.md` & `JanexPT-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.8/setup.py` & `JanexPT-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="JanexPT",
 
     # version of the module
-    version="0.0.8",
+    version="0.0.9",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex-Pytorch',
 
     # your Email address
```

