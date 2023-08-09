# Comparing `tmp/re_edge_gpt-0.0.2.tar.gz` & `tmp/re_edge_gpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_edge_gpt-0.0.2.tar", last modified: Thu Aug  3 11:00:37 2023, max compression
+gzip compressed data, was "re_edge_gpt-0.0.3.tar", last modified: Tue Aug  8 14:02:23 2023, max compression
```

## Comparing `re_edge_gpt-0.0.2.tar` & `re_edge_gpt-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 11:00:37.945272 re_edge_gpt-0.0.2/
--rw-rw-rw-   0        0        0     1085 2023-06-22 06:27:17.000000 re_edge_gpt-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5789 2023-08-03 11:00:37.944274 re_edge_gpt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-08-02 08:31:13.000000 re_edge_gpt-0.0.2/README.md
--rw-rw-rw-   0        0        0     1103 2023-08-03 11:00:24.000000 re_edge_gpt-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-03 11:00:37.917816 re_edge_gpt-0.0.2/re_edge_gpt/
--rw-rw-rw-   0        0        0      154 2023-08-02 06:42:08.000000 re_edge_gpt-0.0.2/re_edge_gpt/__init__.py
--rw-rw-rw-   0        0        0     9541 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/chathub.py
--rw-rw-rw-   0        0        0     2453 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/constants.py
--rw-rw-rw-   0        0        0     4460 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/conversation.py
--rw-rw-rw-   0        0        0     1256 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.2/re_edge_gpt/conversation_style.py
--rw-rw-rw-   0        0        0       46 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.2/re_edge_gpt/exceptions.py
--rw-rw-rw-   0        0        0     2247 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.2/re_edge_gpt/locale.py
--rw-rw-rw-   0        0        0     7489 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/main.py
--rw-rw-rw-   0        0        0     7755 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/re_edge_gpt.py
--rw-rw-rw-   0        0        0     5792 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/request.py
--rw-rw-rw-   0        0        0      967 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.2/re_edge_gpt/utilities.py
-drwxrwxrwx   0        0        0        0 2023-08-03 11:00:37.944274 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/
--rw-rw-rw-   0        0        0     5789 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 11:00:37.000000 re_edge_gpt-0.0.2/re_edge_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 11:00:37.945272 re_edge_gpt-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 14:02:23.020793 re_edge_gpt-0.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-06-22 06:27:17.000000 re_edge_gpt-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5789 2023-08-08 14:02:23.020793 re_edge_gpt-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-08-02 08:31:13.000000 re_edge_gpt-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1103 2023-08-08 13:24:58.000000 re_edge_gpt-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-08 14:02:22.999353 re_edge_gpt-0.0.3/re_edge_gpt/
+-rw-rw-rw-   0        0        0      154 2023-08-02 06:42:08.000000 re_edge_gpt-0.0.3/re_edge_gpt/__init__.py
+-rw-rw-rw-   0        0        0     9522 2023-08-08 13:13:39.000000 re_edge_gpt-0.0.3/re_edge_gpt/chathub.py
+-rw-rw-rw-   0        0        0     2453 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.3/re_edge_gpt/constants.py
+-rw-rw-rw-   0        0        0     4460 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.3/re_edge_gpt/conversation.py
+-rw-rw-rw-   0        0        0     1256 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.3/re_edge_gpt/conversation_style.py
+-rw-rw-rw-   0        0        0       46 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.3/re_edge_gpt/exceptions.py
+-rw-rw-rw-   0        0        0     2247 2023-08-02 06:26:40.000000 re_edge_gpt-0.0.3/re_edge_gpt/locale.py
+-rw-rw-rw-   0        0        0     7489 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.3/re_edge_gpt/main.py
+-rw-rw-rw-   0        0        0     7755 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.3/re_edge_gpt/re_edge_gpt.py
+-rw-rw-rw-   0        0        0     5792 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.3/re_edge_gpt/request.py
+-rw-rw-rw-   0        0        0      967 2023-08-02 06:40:05.000000 re_edge_gpt-0.0.3/re_edge_gpt/utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:02:23.019811 re_edge_gpt-0.0.3/re_edge_gpt.egg-info/
+-rw-rw-rw-   0        0        0     5789 2023-08-08 14:02:22.000000 re_edge_gpt-0.0.3/re_edge_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-08-08 14:02:22.000000 re_edge_gpt-0.0.3/re_edge_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 14:02:22.000000 re_edge_gpt-0.0.3/re_edge_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-08 14:02:22.000000 re_edge_gpt-0.0.3/re_edge_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-08 14:02:22.000000 re_edge_gpt-0.0.3/re_edge_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 14:02:23.020793 re_edge_gpt-0.0.3/setup.cfg
```

### Comparing `re_edge_gpt-0.0.2/LICENSE` & `re_edge_gpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/PKG-INFO` & `re_edge_gpt-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re_edge_gpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Microsoft's Bing Chat AI
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integration-Automation/ReEdgeGPT
 Project-URL: Code, https://github.com/Integration-Automation/ReEdgeGPT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `re_edge_gpt-0.0.2/README.md` & `re_edge_gpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/pyproject.toml` & `re_edge_gpt-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "re_edge_gpt"
-version = "0.0.02"
+version = "0.0.03"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 dependencies = [
     "aiohttp", "certifi", "httpx", "prompt_toolkit", "requests", "rich"
 ]
 description = "Microsoft's Bing Chat AI"
```

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/chathub.py` & `re_edge_gpt-0.0.3/re_edge_gpt/chathub.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,48 +147,44 @@
                 continue
             for obj in objects:
                 if int(time()) % 6 == 0:
                     await wss.send_str(append_identifier({"type": 6}))
                 if obj is None or not obj:
                     continue
                 response = json.loads(obj)
-                # print(response)
                 if response.get("type") == 1 and response["arguments"][0].get(
                         "messages",
                 ):
-                    if (
-                            (
-                                    response["arguments"][0]["messages"][0]["contentOrigin"]
-                                    != "Apology"
-                            )
-                            and not raw
-                    ):
-                        resp_txt = result_text + response["arguments"][0][
-                            "messages"
-                        ][0]["adaptiveCards"][0]["body"][0].get("text", "")
-                        resp_txt_no_link = result_text + response["arguments"][0][
-                            "messages"
-                        ][0].get("text", "")
-                        if response["arguments"][0]["messages"][0].get(
-                                "messageType",
-                        ):
-                            resp_txt = (
-                                    resp_txt
-                                    + response["arguments"][0]["messages"][0][
-                                        "adaptiveCards"
-                                    ][0]["body"][0]["inlines"][0].get("text")
-                                    + "\n"
-                            )
-                            result_text = (
-                                    result_text
-                                    + response["arguments"][0]["messages"][0][
-                                        "adaptiveCards"
-                                    ][0]["body"][0]["inlines"][0].get("text")
-                                    + "\n"
-                            )
+                    if ((response["arguments"][0]["messages"][0]["contentOrigin"] != "Apology") and not raw):
+                        try:
+                            resp_txt = result_text + response["arguments"][0][
+                                "messages"
+                            ][0]["adaptiveCards"][0]["body"][0].get("text", "")
+                            resp_txt_no_link = result_text + response["arguments"][0][
+                                "messages"
+                            ][0].get("text", "")
+                            if response["arguments"][0]["messages"][0].get(
+                                    "messageType",
+                            ):
+                                resp_txt = (
+                                        resp_txt
+                                        + response["arguments"][0]["messages"][0][
+                                            "adaptiveCards"
+                                        ][0]["body"][0]["inlines"][0].get("text")
+                                        + "\n"
+                                )
+                                result_text = (
+                                        result_text
+                                        + response["arguments"][0]["messages"][0][
+                                            "adaptiveCards"
+                                        ][0]["body"][0]["inlines"][0].get("text")
+                                        + "\n"
+                                )
+                        except KeyError:
+                            pass
                     if not raw:
                         yield False, resp_txt
                 elif response.get("type") == 2:
                     if response["item"]["result"].get("error"):
                         await self.close()
                         raise Exception(
                             f"{response['item']['result']['value']}: {response['item']['result']['message']}",
```

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/constants.py` & `re_edge_gpt-0.0.3/re_edge_gpt/constants.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/conversation.py` & `re_edge_gpt-0.0.3/re_edge_gpt/conversation.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/conversation_style.py` & `re_edge_gpt-0.0.3/re_edge_gpt/conversation_style.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/locale.py` & `re_edge_gpt-0.0.3/re_edge_gpt/locale.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/main.py` & `re_edge_gpt-0.0.3/re_edge_gpt/main.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/re_edge_gpt.py` & `re_edge_gpt-0.0.3/re_edge_gpt/re_edge_gpt.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/request.py` & `re_edge_gpt-0.0.3/re_edge_gpt/request.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt/utilities.py` & `re_edge_gpt-0.0.3/re_edge_gpt/utilities.py`

 * *Files identical despite different names*

### Comparing `re_edge_gpt-0.0.2/re_edge_gpt.egg-info/PKG-INFO` & `re_edge_gpt-0.0.3/re_edge_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-edge-gpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Microsoft's Bing Chat AI
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Integration-Automation/ReEdgeGPT
 Project-URL: Code, https://github.com/Integration-Automation/ReEdgeGPT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

