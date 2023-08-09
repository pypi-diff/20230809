# Comparing `tmp/Zxy_Private-0.0.2.tar.gz` & `tmp/Zxy_Private-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Zxy_Private-0.0.2.tar", last modified: Tue Aug  8 13:30:46 2023, max compression
+gzip compressed data, was "dist\Zxy_Private-0.0.3.tar", last modified: Wed Aug  9 03:27:11 2023, max compression
```

## Comparing `Zxy_Private-0.0.2.tar` & `Zxy_Private-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/OhMyChat_API/
--rw-rw-rw-   0        0        0     3935 2023-08-08 03:03:17.000000 Zxy_Private-0.0.2/OhMyChat_API/Get_API.py
--rw-rw-rw-   0        0        0      425 2023-08-08 08:52:23.000000 Zxy_Private-0.0.2/OhMyChat_API/__init__.py
--rw-rw-rw-   0        0        0      366 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      470 2023-08-08 13:28:05.000000 Zxy_Private-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      366 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2023-08-08 13:30:46.000000 Zxy_Private-0.0.2/Zxy_Private.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/OhMyChat_API/
+-rw-rw-rw-   0        0        0     4023 2023-08-09 03:16:49.000000 Zxy_Private-0.0.3/OhMyChat_API/Get_API.py
+-rw-rw-rw-   0        0        0      290 2023-08-09 03:16:49.000000 Zxy_Private-0.0.3/OhMyChat_API/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-08-09 03:26:02.000000 Zxy_Private-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/Zxy_Private.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/Zxy_Private.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      411 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/Zxy_Private.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/Zxy_Private.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       13 2023-08-09 03:27:11.000000 Zxy_Private-0.0.3/Zxy_Private.egg-info/top_level.txt
```

### Comparing `Zxy_Private-0.0.2/OhMyChat_API/Get_API.py` & `Zxy_Private-0.0.3/OhMyChat_API/Get_API.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 import json
 import time
 import traceback
 
 import requests
 
 
-class Test_Class():
-    def __init__(self):
-        pass
+class GetAPI():
+    def __init__(self, api_key=""):
+        self.api_key = api_key  # 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
 
-    def timeStamp_to_datetime(self,timeStamp):
+    def timeStamp_to_datetime(self, timeStamp):
         timeStamp = float(timeStamp)
         timeArray = time.localtime(timeStamp)
         otherStyleTime = time.strftime("%Y-%m-%d %H:%M:%S", timeArray)
         return otherStyleTime
+
     def get_chat_api(self, query="", rety_num=0):
         url = "https://cfwus02.opapi.win/v1/chat/completions"
 
         payload = json.dumps({
             "model": "gpt-3.5-turbo",
             "messages": [
                 {
@@ -33,52 +34,52 @@
                     "content": query,
                 }
             ],
             "stream": True
         })
         headers = {
             'User-Agent': 'Apifox/1.0.0 (https://apifox.com)',
-            "Authorization": "Bearer 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",
+            "Authorization": "Bearer {api_key}".format(api_key=self.api_key),
             'Content-Type': 'application/json'
         }
         try:
             if query:
                 if not rety_num:
                     raise
-                response = requests.post(url, headers=headers, data=payload,stream=True)
-                for index,line in enumerate(response.iter_lines()):
-                    yield bytes.decode(line),index
+                response = requests.post(url, headers=headers, data=payload, stream=True)
+                for index, line in enumerate(response.iter_lines()):
+                    yield bytes.decode(line), index
         except:
-            if rety_num<3:
-                for line_data,index in self.get_chat_api(query,rety_num+1):
-                    yield line_data,index
+            if rety_num < 3:
+                for line_data, index in self.get_chat_api(query, rety_num + 1):
+                    yield line_data, index
         else:
             return None
 
-    def handler_api_result(self, line_data:str,index:int):
+    def handler_api_result(self, line_data: str, index: int):
         if not line_data or line_data.endswith("[DONE]"):
             return
-        data = json.loads(str(line_data).split(":",1)[-1])
+        data = json.loads(str(line_data).split(":", 1)[-1])
         if not index:
             release_time = self.timeStamp_to_datetime(data["created"])
             model = data["model"]
         else:
-            release_time,model="",""
+            release_time, model = "", ""
         for choice in data["choices"]:
             if not index:
                 username = choice["delta"]["role"]
-                start_str = f"{username}({model})({release_time}){'='*100}"
+                start_str = f"{username}({model})({release_time}){'=' * 100}"
                 print(start_str)
                 self.header_lenth = len(start_str)
             if choice["finish_reason"]:
-                equalSign_num = (self.header_lenth-14)//2
-                print(f"\n{'='*equalSign_num} divisionLine {'='*equalSign_num}")
+                equalSign_num = (self.header_lenth - 14) // 2
+                print(f"\n{'=' * equalSign_num} divisionLine {'=' * equalSign_num}")
             else:
                 content = choice["delta"]["content"]
-                print(content,end="")
+                print(content, end="")
 
     def run(self):
         while True:
             try:
                 query = input("please input your question:")
                 if not query:
                     continue
@@ -93,23 +94,18 @@
                         else:
                             print("Your input is illegal!")
                             continue
                     continue
                 else:
                     print("Please be patient and wait for a response . . .")
 
-                for line_data,index in self.get_chat_api(query):
-                    self.handler_api_result(line_data,index)
+                for line_data, index in self.get_chat_api(query):
+                    self.handler_api_result(line_data, index)
             except:
                 traceback.print_exc()
                 print("There is a problem with your API interface !!!")
                 return
 
 
-
-
-
-
-
 if __name__ == '__main__':
-    X = Test_Class()
+    X = GetAPI()
     X.run()
```

