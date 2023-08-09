# Comparing `tmp/devchat-0.2.1.tar.gz` & `tmp/devchat-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.2.1.tar", max compression
+gzip compressed data, was "devchat-0.2.2.tar", max compression
```

## Comparing `devchat-0.2.1.tar` & `devchat-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-07-05 11:57:19.300520 devchat-0.2.1/LICENSE
--rw-r--r--   0        0        0     5267 2023-07-13 11:26:05.138364 devchat-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-05 11:57:31.893875 devchat-0.2.1/devchat/__init__.py
--rw-r--r--   0        0        0     9493 2023-08-01 05:53:42.349789 devchat-0.2.1/devchat/_cli.py
--rw-r--r--   0        0        0     4503 2023-07-21 16:39:59.449026 devchat-0.2.1/devchat/assistant.py
--rw-r--r--   0        0        0     1676 2023-07-21 16:39:59.449400 devchat-0.2.1/devchat/chat.py
--rw-r--r--   0        0        0      758 2023-07-23 12:18:04.254562 devchat-0.2.1/devchat/message.py
--rw-r--r--   0        0        0      248 2023-07-05 11:57:51.466105 devchat-0.2.1/devchat/openai/__init__.py
--rw-r--r--   0        0        0     3558 2023-07-31 23:46:29.233957 devchat-0.2.1/devchat/openai/openai_chat.py
--rw-r--r--   0        0        0     3293 2023-07-23 12:18:04.255359 devchat-0.2.1/devchat/openai/openai_message.py
--rw-r--r--   0        0        0    10686 2023-08-01 05:53:42.350169 devchat-0.2.1/devchat/openai/openai_prompt.py
--rw-r--r--   0        0        0     8953 2023-08-01 05:53:42.350409 devchat-0.2.1/devchat/prompt.py
--rw-r--r--   0        0        0     9872 2023-07-23 12:18:04.256202 devchat-0.2.1/devchat/store.py
--rw-r--r--   0        0        0     6821 2023-08-01 05:53:42.350632 devchat-0.2.1/devchat/utils.py
--rw-r--r--   0        0        0     1154 2023-08-01 05:53:42.350865 devchat-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6557 1970-01-01 00:00:00.000000 devchat-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 11:57:19.300520 devchat-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5267 2023-07-13 11:26:05.138364 devchat-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 11:57:31.893875 devchat-0.2.2/devchat/__init__.py
+-rw-r--r--   0        0        0     9493 2023-08-01 05:53:42.349789 devchat-0.2.2/devchat/_cli.py
+-rw-r--r--   0        0        0     4503 2023-07-21 16:39:59.449026 devchat-0.2.2/devchat/assistant.py
+-rw-r--r--   0        0        0     1676 2023-07-21 16:39:59.449400 devchat-0.2.2/devchat/chat.py
+-rw-r--r--   0        0        0      758 2023-07-23 12:18:04.254562 devchat-0.2.2/devchat/message.py
+-rw-r--r--   0        0        0      248 2023-07-05 11:57:51.466105 devchat-0.2.2/devchat/openai/__init__.py
+-rw-r--r--   0        0        0     3558 2023-07-31 23:46:29.233957 devchat-0.2.2/devchat/openai/openai_chat.py
+-rw-r--r--   0        0        0     3293 2023-07-23 12:18:04.255359 devchat-0.2.2/devchat/openai/openai_message.py
+-rw-r--r--   0        0        0    10712 2023-08-08 04:41:53.664236 devchat-0.2.2/devchat/openai/openai_prompt.py
+-rw-r--r--   0        0        0     8953 2023-08-01 05:53:42.350409 devchat-0.2.2/devchat/prompt.py
+-rw-r--r--   0        0        0     9872 2023-07-23 12:18:04.256202 devchat-0.2.2/devchat/store.py
+-rw-r--r--   0        0        0     6821 2023-08-01 05:53:42.350632 devchat-0.2.2/devchat/utils.py
+-rw-r--r--   0        0        0     1154 2023-08-09 03:41:35.527989 devchat-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6557 1970-01-01 00:00:00.000000 devchat-0.2.2/PKG-INFO
```

### Comparing `devchat-0.2.1/LICENSE` & `devchat-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/README.md` & `devchat-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/_cli.py` & `devchat-0.2.2/devchat/_cli.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/assistant.py` & `devchat-0.2.2/devchat/assistant.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/chat.py` & `devchat-0.2.2/devchat/chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/message.py` & `devchat-0.2.2/devchat/message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/openai/openai_chat.py` & `devchat-0.2.2/devchat/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/openai/openai_message.py` & `devchat-0.2.2/devchat/openai/openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/openai/openai_prompt.py` & `devchat-0.2.2/devchat/openai/openai_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,30 +66,30 @@
                     content = message.content.replace("<context>", "").replace("</context>", "")
                     message.content = content.strip()
                     self._history_messages[Message.CONTEXT].append(message)
                 else:
                     state = "history_chat"
 
             if state == "history_chat":
-                if message.role in ("user", "assistant"):
+                if message.role in ("user", "assistant", "function"):
                     self._history_messages[Message.CHAT].append(message)
                 else:
                     state = "new_context"
 
             if state == "new_context":
                 if message.role == "system" and message.content.startswith("<context>"):
                     content = message.content.replace("<context>", "").replace("</context>", "")
                     message.content = content.strip()
                     self._new_messages[Message.CONTEXT].append(message)
                 else:
                     logger.warning("Invalid new context message: %s", message)
 
         if not self.request:
             last_user_message = self._history_messages[Message.CHAT].pop()
-            if last_user_message.role == "user":
+            if last_user_message.role in ("user", "function"):
                 self._new_messages["request"] = last_user_message
             else:
                 logger.warning("Invalid user request: %s", last_user_message)
 
     def append_new(self, message_type: str, content: str,
                    available_tokens: int = math.inf) -> bool:
         if message_type not in (Message.INSTRUCT, Message.CONTEXT):
```

### Comparing `devchat-0.2.1/devchat/prompt.py` & `devchat-0.2.2/devchat/prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/store.py` & `devchat-0.2.2/devchat/store.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/devchat/utils.py` & `devchat-0.2.2/devchat/utils.py`

 * *Files identical despite different names*

### Comparing `devchat-0.2.1/pyproject.toml` & `devchat-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devchat"
-version = "0.2.1"
+version = "0.2.2"
 description = "DevChat is an open-source tool that helps developers write prompts to generate code and documentation."
 authors = ["DevChat Team <hello@devchat.ai>"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/devchat-ai/devchat"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `devchat-0.2.1/PKG-INFO` & `devchat-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat
-Version: 0.2.1
+Version: 0.2.2
 Summary: DevChat is an open-source tool that helps developers write prompts to generate code and documentation.
 Home-page: https://github.com/devchat-ai/devchat
 License: Apache-2.0
 Author: DevChat Team
 Author-email: hello@devchat.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

