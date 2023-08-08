# Comparing `tmp/bareunpy-1.6.2.tar.gz` & `tmp/bareunpy-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bareunpy-1.6.2.tar", max compression
+gzip compressed data, was "bareunpy-1.6.3.tar", max compression
```

## Comparing `bareunpy-1.6.2.tar` & `bareunpy-1.6.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1547 2023-01-30 00:41:12.108840 bareunpy-1.6.2/LICENSE
--rw-r--r--   0        0        0     4119 2023-03-24 00:58:50.777709 bareunpy-1.6.2/README.md
--rw-r--r--   0        0        0     1432 2023-06-16 07:55:52.795277 bareunpy-1.6.2/bareunpy/__init__.py
--rw-r--r--   0        0        0     7475 2023-06-05 09:39:16.952459 bareunpy-1.6.2/bareunpy/_custom_dict.py
--rw-r--r--   0        0        0     6006 2023-06-05 09:39:16.952459 bareunpy-1.6.2/bareunpy/_custom_dict_client.py
--rw-r--r--   0        0        0     3427 2023-03-24 00:58:50.781709 bareunpy-1.6.2/bareunpy/_lang_service_client.py
--rw-r--r--   0        0        0     9452 2023-06-16 07:55:52.795277 bareunpy-1.6.2/bareunpy/_tagger.py
--rw-r--r--   0        0        0     9633 2023-03-24 00:58:50.781709 bareunpy-1.6.2/bareunpy/_tokenizer.py
--rw-r--r--   0        0        0     1379 2023-06-16 07:55:52.795277 bareunpy-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     5903 1970-01-01 00:00:00.000000 bareunpy-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1547 2023-01-30 00:41:12.108840 bareunpy-1.6.3/LICENSE
+-rw-r--r--   0        0        0     4119 2023-03-24 00:58:50.777709 bareunpy-1.6.3/README.md
+-rw-r--r--   0        0        0     1432 2023-08-08 23:35:09.910044 bareunpy-1.6.3/bareunpy/__init__.py
+-rw-r--r--   0        0        0     7475 2023-06-05 09:39:16.952459 bareunpy-1.6.3/bareunpy/_custom_dict.py
+-rw-r--r--   0        0        0     6006 2023-06-05 09:39:16.952459 bareunpy-1.6.3/bareunpy/_custom_dict_client.py
+-rw-r--r--   0        0        0     4988 2023-08-08 23:35:09.910044 bareunpy-1.6.3/bareunpy/_lang_service_client.py
+-rw-r--r--   0        0        0    10541 2023-08-08 23:35:09.910044 bareunpy-1.6.3/bareunpy/_tagger.py
+-rw-r--r--   0        0        0     9633 2023-03-24 00:58:50.781709 bareunpy-1.6.3/bareunpy/_tokenizer.py
+-rw-r--r--   0        0        0     1379 2023-08-08 23:35:09.910044 bareunpy-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5903 1970-01-01 00:00:00.000000 bareunpy-1.6.3/PKG-INFO
```

### Comparing `bareunpy-1.6.2/LICENSE` & `bareunpy-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.2/README.md` & `bareunpy-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.2/bareunpy/__init__.py` & `bareunpy-1.6.3/bareunpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,9 +51,9 @@
 
 from bareunpy._tagger import Tagger, Tagged
 from bareunpy._tokenizer import Tokenizer, Tokenized
 from bareunpy._custom_dict import CustomDict
 from bareunpy._custom_dict_client import CustomDictionaryServiceClient
 from bareunpy._lang_service_client import BareunLanguageServiceClient
 
-version = "1.6.2"
+version = "1.6.3"
 bareun_version = "1.8.0"
```

### Comparing `bareunpy-1.6.2/bareunpy/_custom_dict.py` & `bareunpy-1.6.3/bareunpy/_custom_dict.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.2/bareunpy/_custom_dict_client.py` & `bareunpy-1.6.3/bareunpy/_custom_dict_client.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.2/bareunpy/_lang_service_client.py` & `bareunpy-1.6.3/bareunpy/_lang_service_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import grpc
+from typing import List
 
 import bareun.language_service_pb2 as pb
 import bareun.language_service_pb2_grpc as ls
 
 MAX_MESSAGE_LENGTH = 100 * 1024 * 1024
 
 
@@ -24,25 +25,25 @@
                 ('api-key', self.apikey),
                 )
         self.stub = ls.LanguageServiceStub(self.channel)
 
     def analyze_syntax(self, content: str,
         domain: str = "",
         auto_split=False,
-        auto_spacing=True, 
+        auto_spacing=True,
         auto_jointing=False) -> pb.AnalyzeSyntaxResponse:
         """
         형태소 분석을 수행합니다.
 
         Args:
             content (str): 형태소 분석할 원문, 여러 문장일 경우에 개행문자로 줄바꿈을 하면 됩니다.
             domain (str, optional): 사용사 사전의 이름. 기본값은 "".
             auto_split (bool, optional): 문장 자동 분리 여부, 기본값은 사용하지 않음.
             auto_spacing (bool, optional): 띄어쓰기 보정 기능, 기본값은 사용하도록 함.
-            auto_jointing (bool, optional): 붙여쓰기 보정 기능, 기본값은 사용하도록 함.
+            auto_jointing (bool, optional): 붙여쓰기 보정 기능, 기본값은 사용하지 않음.
 
         Raises:
             e: grpc.Error, 원격 호출시 예외가 발생할 수 있습니다.
 
         Returns:
             pb.AnalyzeSyntaxResponse: 형태소 분석 결과
         """
@@ -52,24 +53,64 @@
         req.document.language = "ko_KR"
         req.encoding_type = pb.EncodingType.UTF32
         req.auto_split_sentence = auto_split
         req.auto_spacing = auto_spacing
         req.auto_jointing = auto_jointing
         if domain:
             req.custom_domain = domain
-        try:            
+        try:
             res, c = self.stub.AnalyzeSyntax.with_call(
                 request=req, metadata=self.metadata)
             return res
         except grpc.RpcError as e:
             raise e
         except Exception as e2:
             import traceback
             traceback.print_exc()
             raise e2
+        
+    def analyze_syntax_list(self, content: List[str],
+        domain: str = "",
+        auto_spacing=True,
+        auto_jointing=False) -> pb.AnalyzeSyntaxListResponse:
+        """
+        형태소 분석을 수행하되, 입력된 문장 단위가 일치하도록 반환됩니다.
+        문장 분할 기능을 사용하지 않습니다.
+
+        Args:
+            content (List[str]): 형태소 분석할 원문의 리스트
+            domain (str, optional): 사용사 사전의 이름. 기본값은 "".
+            auto_spacing (bool, optional): 띄어쓰기 보정 기능, 기본값은 사용하도록 함.
+            auto_jointing (bool, optional): 붙여쓰기 보정 기능, 기본값은 사용하지 않음.
+
+        Raises:
+            e: grpc.Error, 원격 호출시 예외가 발생할 수 있습니다.
+
+        Returns:
+            pb.AnalyzeSyntaxListResponse: 형태소 분석 결과
+        """
+        req = pb.AnalyzeSyntaxListRequest()
+        req.sentences.extend(content)
+        req.language = "ko_KR"
+        req.encoding_type = pb.EncodingType.UTF32
+        req.auto_spacing = auto_spacing
+        req.auto_jointing = auto_jointing
+        if domain:
+            req.custom_domain = domain
+        try:
+            res, c = self.stub.AnalyzeSyntaxList.with_call(
+                request=req, metadata=self.metadata)
+            return res
+        except grpc.RpcError as e:
+            raise e
+        except Exception as e2:
+            import traceback
+            traceback.print_exc()
+            raise e2
+
 
     def tokenize(self, content: str, auto_split=False) -> pb.TokenizeResponse:
         """
         형태소 분석을 수행합니다.
 
         Args:
             content (str): 형태소 분석할 원문, 여러 문장일 경우에 개행문자로 줄바꿈을 하면 됩니다.
```

### Comparing `bareunpy-1.6.2/bareunpy/_tagger.py` & `bareunpy-1.6.3/bareunpy/_tagger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # -*- coding: utf-8 -*-
 import json
 from sys import stdout
-from typing import IO, List, Any
+from typing import IO, List, Any, Union
 
 from google.protobuf.json_format import MessageToDict
 import grpc
 from bareunpy._custom_dict import CustomDict
 from bareunpy._lang_service_client import BareunLanguageServiceClient, MAX_MESSAGE_LENGTH
-from bareun.language_service_pb2 import AnalyzeSyntaxResponse, Morpheme, Sentence, Token
+from bareun.language_service_pb2 import AnalyzeSyntaxResponse, AnalyzeSyntaxListResponse, Morpheme, Sentence, Token
 
 
 class Tagged:
     """
     Tagged result.
     It has various output manipulations.
     """
 
-    def __init__(self, phrase: str, res: AnalyzeSyntaxResponse):
+    def __init__(self, phrase: Union[str, List[str]], res: Union[AnalyzeSyntaxResponse, AnalyzeSyntaxListResponse]):
         """
         constructor, which is used internally.
         :param phrase: requested sentences.
         :param res:
         """
         super().__init__()
         self.phrase = phrase
         self.r = res
 
         # 빈 응답이 있는 경우를 대비해서 값이 없지 않도록 처리한다.
         if self.r is None:
             self.r = AnalyzeSyntaxResponse()
             self.phrase = ''
 
-    def msg(self) -> AnalyzeSyntaxResponse:
+    def msg(self) -> Union[AnalyzeSyntaxResponse, AnalyzeSyntaxListResponse]:
         """
         Protobuf message object containing all of NLP engine.
         """
         return self.r
 
     def sentences(self) -> List[Sentence]:
         """
@@ -227,14 +227,32 @@
         p = '\n'.join(phrase)
         try:
             res = self.client.analyze_syntax(p, self.domain, auto_split=auto_split, auto_spacing=auto_spacing, auto_jointing=auto_jointing)
             return Tagged(p, res)
         except Exception as e:
             raise e
 
+    def taglist(self, phrase: List[str], auto_spacing: bool = True, auto_jointing: bool = True) -> Tagged:
+        """
+        the array is not being split and the input value is being returned as-is.
+        :param phrase: array of string
+        :param auto_split(bool, optional): Whether to automatically perform sentence split
+        :param auto_spacing(bool, optional): Whether to automatically perform space insertion for typo correction
+        :param auto_jointing(bool, optional): Whether to automatically perform word joining for typo correction
+        :return: Tagged result instance
+        """
+        if len(phrase) == 0:
+            print("OOPS, no sentences.")
+            return Tagged('', AnalyzeSyntaxListResponse())
+        try:
+            res = self.client.analyze_syntax_list(phrase, self.domain, auto_spacing=auto_spacing, auto_jointing=auto_jointing)
+            return Tagged(phrase, res)
+        except Exception as e:
+            raise e
+
     def pos(self, phrase: str, flatten: bool = True, join: bool = False, detail: bool = False) -> List:
         """
         POS tagger.
         :param phrase  : string to analyse
         :param flatten : If False, returns original morphs.
         :param join    : If True, returns joined sets of morph and tag.
         :param detail  : if True, returns every things of morph result
```

### Comparing `bareunpy-1.6.2/bareunpy/_tokenizer.py` & `bareunpy-1.6.3/bareunpy/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `bareunpy-1.6.2/pyproject.toml` & `bareunpy-1.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bareunpy"
-version = "1.6.2"
+version = "1.6.3"
 description = "The bareun python library using grpc"
 authors = ["Gihyun YUN <gih2yun@baikal.ai>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://bareun.ai/"
 repository = "https://github.com/bareun-nlp/bareunpy"
 keywords = [ "NLP", "Korean", "Deep Learning", "POS tagger", "bareun"]
```

### Comparing `bareunpy-1.6.2/PKG-INFO` & `bareunpy-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bareunpy
-Version: 1.6.2
+Version: 1.6.3
 Summary: The bareun python library using grpc
 Home-page: https://bareun.ai/
 License: BSD-3-Clause
 Keywords: NLP,Korean,Deep Learning,POS tagger,bareun
 Author: Gihyun YUN
 Author-email: gih2yun@baikal.ai
 Requires-Python: >=3.6,<4.0
```

