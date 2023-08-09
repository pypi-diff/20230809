# Comparing `tmp/Caribe-0.8.9.tar.gz` & `tmp/Caribe-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Caribe-0.8.9.tar", last modified: Thu Jan 26 02:10:08 2023, max compression
+gzip compressed data, was "dist\Caribe-0.9.0.tar", last modified: Wed Aug  9 03:29:05 2023, max compression
```

## Comparing `Caribe-0.8.9.tar` & `Caribe-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 02:10:08.120148 Caribe-0.8.9/
--rw-rw-rw-   0        0        0     4229 2022-10-02 20:45:13.000000 Caribe-0.8.9/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-01-26 02:10:08.039367 Caribe-0.8.9/Caribe/
--rw-rw-rw-   0        0        0     2531 2022-08-01 21:41:23.000000 Caribe-0.8.9/Caribe/T5_Caribe.py
--rw-rw-rw-   0        0        0    25908 2023-01-26 01:59:42.000000 Caribe-0.8.9/Caribe/__init__.py
--rw-rw-rw-   0        0        0     1513 2022-07-31 06:38:53.000000 Caribe-0.8.9/Caribe/caribe_generate.py
-drwxrwxrwx   0        0        0        0 2023-01-26 02:10:08.105188 Caribe-0.8.9/Caribe/guyanese/
--rw-rw-rw-   0        0        0     5524 2022-09-28 00:46:15.000000 Caribe-0.8.9/Caribe/guyanese/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-26 02:10:08.100201 Caribe-0.8.9/Caribe.egg-info/
--rw-rw-rw-   0        0        0    21765 2023-01-26 02:10:07.000000 Caribe-0.8.9/Caribe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-01-26 02:10:07.000000 Caribe-0.8.9/Caribe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 02:10:07.000000 Caribe-0.8.9/Caribe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-01-26 02:10:07.000000 Caribe-0.8.9/Caribe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-26 02:10:07.000000 Caribe-0.8.9/Caribe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10945 2022-06-24 22:45:59.000000 Caribe-0.8.9/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2021-09-16 16:29:08.000000 Caribe-0.8.9/MANIFEST.in
--rw-rw-rw-   0        0        0    21765 2023-01-26 02:10:08.115163 Caribe-0.8.9/PKG-INFO
--rw-rw-rw-   0        0        0    16907 2022-12-26 23:48:10.000000 Caribe-0.8.9/README.md
--rw-rw-rw-   0        0        0       95 2022-07-31 04:44:30.000000 Caribe-0.8.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-26 02:10:08.121145 Caribe-0.8.9/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-01-26 02:09:54.000000 Caribe-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:29:05.440152 Caribe-0.9.0/
+-rw-rw-rw-   0        0        0     4565 2023-08-09 03:27:59.000000 Caribe-0.9.0/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 03:29:04.677735 Caribe-0.9.0/Caribe/
+-rw-rw-rw-   0        0        0     2531 2022-08-01 21:41:23.000000 Caribe-0.9.0/Caribe/T5_Caribe.py
+-rw-rw-rw-   0        0        0    25703 2023-08-09 02:40:13.000000 Caribe-0.9.0/Caribe/__init__.py
+-rw-rw-rw-   0        0        0     1513 2022-07-31 06:38:53.000000 Caribe-0.9.0/Caribe/caribe_generate.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:29:05.368245 Caribe-0.9.0/Caribe/guyanese/
+-rw-rw-rw-   0        0        0     5524 2022-09-28 00:46:15.000000 Caribe-0.9.0/Caribe/guyanese/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 03:29:05.328301 Caribe-0.9.0/Caribe.egg-info/
+-rw-rw-rw-   0        0        0    22481 2023-08-09 03:29:02.000000 Caribe-0.9.0/Caribe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-08-09 03:29:03.000000 Caribe-0.9.0/Caribe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 03:29:02.000000 Caribe-0.9.0/Caribe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-08-09 03:29:02.000000 Caribe-0.9.0/Caribe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-09 03:29:02.000000 Caribe-0.9.0/Caribe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10945 2022-06-24 22:45:59.000000 Caribe-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2021-09-16 16:29:08.000000 Caribe-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    22481 2023-08-09 03:29:05.400201 Caribe-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17287 2023-08-09 03:22:00.000000 Caribe-0.9.0/README.md
+-rw-rw-rw-   0        0        0       78 2023-08-09 02:42:42.000000 Caribe-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 03:29:05.444143 Caribe-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-08-09 02:39:10.000000 Caribe-0.9.0/setup.py
```

### Comparing `Caribe-0.8.9/CHANGELOG.txt` & `Caribe-0.9.0/CHANGELOG.txt`

 * *Files 3% similar despite different names*

```diff
@@ -138,8 +138,13 @@
 Version 0.7.8 (04/09/2022)
 - More Words Added
 
 Version 0.7.9 (26/09/2022)
 -  Introducing a NEW NLP model to directly translate Guyanese English Creole to English.
 
 Version 0.8.1 (02/10/2022)
--  Introducing a NEW NLP model to directly translate Standard English to Trinidad English Creole.
+-  Introducing a NEW NLP model to directly translate Standard English to Trinidad English Creole.
+
+Version 0.9.0 (08/08/2023)
+- Resolved dependency issues with cloud computing services where the service refused to install the latest version of package because of a missing/deleted dependency.
+- The gingerit_corrector function is deprecated from version 0.9.0 and above. 
+- Gingerit package no longer exists. Dependency removed.
```

### Comparing `Caribe-0.8.9/Caribe/T5_Caribe.py` & `Caribe-0.9.0/Caribe/T5_Caribe.py`

 * *Files identical despite different names*

### Comparing `Caribe-0.8.9/Caribe/__init__.py` & `Caribe-0.9.0/Caribe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Author: Keston Smith
 # Library: Caribe 
 # Contact: keston.smith@my.uwi.edu
-# Copyright: Apache-2.0 2021
+# Copyright: Apache-2.0 2023
 from asyncio import wait_for
-from gingerit.gingerit import GingerIt
 import re
 import nltk
 from nltk import *
 import pandas as pd
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
 import json
 import requests
@@ -917,19 +916,14 @@
     tokenizer = AutoTokenizer.from_pretrained("KES/T5-KES")
     model = AutoModelForSeq2SeqLM.from_pretrained("KES/T5-KES")
     inputs = tokenizer("grammar:"+sentence, truncation=True, return_tensors='pt')
     output = model.generate(inputs['input_ids'], num_beams=4, max_length=512)
     correction=tokenizer.batch_decode(output, skip_special_tokens=True)
     return "".join(correction)
 
-def gingerit_corrector(sentence:str):
-    parser = GingerIt()
-    sentence = parser.parse(sentence)
-    sentence = sentence['result']
-    return str (sentence)
 
 def remove_signs(sentence:str)->str:
     stop_signs = ['!', ".", "%", '"', "'", "`", "*", "&", ",", "-", "+", "/", "'\'", "?", ";", ":", "$", "%", "#", "@", "=", "-", "~", "(", ")", "[", "]", "^", "_", "|" ]
     for signs in stop_signs:
         sentence = sentence.replace(signs, "")
     return sentence
```

### Comparing `Caribe-0.8.9/Caribe/caribe_generate.py` & `Caribe-0.9.0/Caribe/caribe_generate.py`

 * *Files identical despite different names*

### Comparing `Caribe-0.8.9/Caribe/guyanese/__init__.py` & `Caribe-0.9.0/Caribe/guyanese/__init__.py`

 * *Files identical despite different names*

### Comparing `Caribe-0.8.9/Caribe.egg-info/PKG-INFO` & `Caribe-0.9.0/Caribe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Caribe
-Version: 0.8.9
+Version: 0.9.0
 Summary: Caribbean English Creoles to Standard English
 Home-page: UNKNOWN
 Author: Keston Smith
 Author-email: keston.smith@my.uwi.edu
 License: Apache License, Version 2.0
 Keywords: Translator
 Platform: UNKNOWN
@@ -195,15 +195,14 @@
 ---
 - ## Additional Information
     - `trinidad_decode()` : Decodes the sentence as a whole string.
     - `guyanese_decode()`:  Decodes the sentence as a whole string.
     - `trinidad_decode_split()`: Decodes the sentence word by word.
     - `phrase_decode()`: Decodes the sentence against known creole phrases.
     - `caribe_corrector()`: Corrects grammatical errors in a sentence using a trained NLP model.
-    - `gingerit_corrector()`: Corrects grammatical errors in a sentence using gingerit.
     - `t5_kes_corrector()`: Corrects grammatical errors in a sentence using a trained NLP model.
     - `trinidad_encode()`: Encodes a sentence to Trinidadian English Creole.
     - `guyanese_encode()`: Encodes a sentence to Guyanese English Creole.
     - `trinidad_direct_translation()`: Translates Trinidad English Creole to English.
     - `capitalize()`: Capitalize groups of sentences using an NLP model.
     - `caribe_pos()`: Generates parts of speech tagging on creole words.
     - `pos_report()`: Generates parts of speech tagging on english words.
@@ -282,15 +281,15 @@
 
 ```
 
 ---
 ## Dictionary Data
 The encoder and decoder utilises a dictionary data structure. The data for the dictionary was gathered from web-scapping social media sites among other websites and using Lise Winer Dictionary of the English Creole of Trinidad and Tobago among other scholarly resources.
 ____
-## Fine-tune a T5 model on custom datasets easier using Caribe built on HuggingFace Transformers APIs (Beta)
+## Fine-tune a T5 model on custom datasets easier using Caribe built on HuggingFace Transformers APIs 
 
 ### Training Section:
 Caribe allows any user to fine-tune a T5 model on a custom dataset.  The snippet below trains and generates a model in the "model/" folder. 
 Please ensure that your training and evaluation datasets are in the recommended format before training. For more info checkout [T5 documentation.](https://huggingface.co/docs/transformers/main/en/model_doc/t5#t5) 
 ```python
 from Caribe import T5_Caribe as t5
 
@@ -414,14 +413,17 @@
 - NLP Models and Dictionaries are continuously updated.
 - Future plans to create translations, models and datasets for Caribbean French and Spanish Creoles to their respective lexifers (Requires extensive research).
 - Some users complained of problems importing some of the dependencies. This is currently being monitored (10/06/2022).
 - New model introduced for sentence capitalization (09/06/2022) !!!
 - NEW model introduced for direct translation from Trinidad English Creole(TEC) to English(26/06/2022).
 - NEW model introduced for direct translation from Guyanese English Creole(GEC) to English(26/09/2022).
 
+- The gingerit_corrector function is deprecated on versions 0.9.0 and above of Caribe. Due to deletion of the gingerit package,   
+the gingerit_corrector function may no longer work depending on your initial date of install. To avoid dependency issues discovered on cloud computing services like Google Colab, the function and its parent dependency will be removed. Users can utilise the much better caribe_corrector function for sentence correction tasks (08/08/2023). 
+
 ---
 - ## Contact 
 For any concerns or issues with this library.
 
 Email: keston.smith@my.uwi.edu 
 
 Website: https://www.thecaribe.org/
@@ -569,7 +571,12 @@
 
 Version 0.7.9 (26/09/2022)
 -  Introducing a NEW NLP model to directly translate Guyanese English Creole to English.
 
 Version 0.8.1 (02/10/2022)
 -  Introducing a NEW NLP model to directly translate Standard English to Trinidad English Creole.
 
+Version 0.9.0 (08/08/2023)
+- Resolved dependency issues with cloud computing services where the service refused to install the latest version of package because of a missing/deleted dependency.
+- The gingerit_corrector function is deprecated from version 0.9.0 and above. 
+- Gingerit package no longer exists. Dependency removed.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Caribe Version: 0.8.9 Summary: Caribbean English
+Metadata-Version: 2.1 Name: Caribe Version: 0.9.0 Summary: Caribbean English
 Creoles to Standard English Home-page: UNKNOWN Author: Keston Smith Author-
 email: keston.smith@my.uwi.edu License: Apache License, Version 2.0 Keywords:
 Translator Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Education Classifier: Operating System
 :: Microsoft :: Windows :: Windows 10 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown License-File: LICENSE.txt [![License]
@@ -73,24 +73,23 @@
 cb.capitalize(sentence) print(capitalized_text) # Output: John is a boy. He is
  12 years old. His sister's name is Joy. ``` --- - ## Additional Information -
         `trinidad_decode()` : Decodes the sentence as a whole string. -
         `guyanese_decode()`: Decodes the sentence as a whole string. -
 `trinidad_decode_split()`: Decodes the sentence word by word. - `phrase_decode
 ()`: Decodes the sentence against known creole phrases. - `caribe_corrector()`:
     Corrects grammatical errors in a sentence using a trained NLP model. -
-    `gingerit_corrector()`: Corrects grammatical errors in a sentence using
-  gingerit. - `t5_kes_corrector()`: Corrects grammatical errors in a sentence
-    using a trained NLP model. - `trinidad_encode()`: Encodes a sentence to
-   Trinidadian English Creole. - `guyanese_encode()`: Encodes a sentence to
-Guyanese English Creole. - `trinidad_direct_translation()`: Translates Trinidad
-  English Creole to English. - `capitalize()`: Capitalize groups of sentences
-  using an NLP model. - `caribe_pos()`: Generates parts of speech tagging on
- creole words. - `pos_report()`: Generates parts of speech tagging on english
-words. - `remove_signs()`: Takes any sentence and remove punctuation marks. --
-- - ## File Encodings on NLP datasets Caribe introduces file encoding (Beta) in
+`t5_kes_corrector()`: Corrects grammatical errors in a sentence using a trained
+  NLP model. - `trinidad_encode()`: Encodes a sentence to Trinidadian English
+Creole. - `guyanese_encode()`: Encodes a sentence to Guyanese English Creole. -
+`trinidad_direct_translation()`: Translates Trinidad English Creole to English.
+    - `capitalize()`: Capitalize groups of sentences using an NLP model. -
+     `caribe_pos()`: Generates parts of speech tagging on creole words. -
+     `pos_report()`: Generates parts of speech tagging on english words. -
+  `remove_signs()`: Takes any sentence and remove punctuation marks. --- - ##
+   File Encodings on NLP datasets Caribe introduces file encoding (Beta) in
 version 0.1.0. This allows a dataset of any supported filetype to be translated
 into Trinidad English Creole. The file encoding feature only supports txt, json
 or csv files only. - ### Usage of File Encodings: ```python import Caribe as cb
 convert = cb.file_encode("test.txt", "text") # Generates a translated text file
   convert = cb.file_encode("test.json", "json") # Generates a translated json
  file convert = cb.file_encode("test.csv", "csv") # Generates a translated csv
  file ``` --- - ## First Parser for the Trinidad English Creole Language This
@@ -127,15 +126,15 @@
    import Caribe as cb text= "Dem men doh kno wat dey doing wid d money bai"
  output= cb.tec_translator(text) print(output.tec_translate()) #Output: These
 men do not know what they are doing with the money. ``` --- ## Dictionary Data
 The encoder and decoder utilises a dictionary data structure. The data for the
    dictionary was gathered from web-scapping social media sites among other
 websites and using Lise Winer Dictionary of the English Creole of Trinidad and
 Tobago among other scholarly resources. ____ ## Fine-tune a T5 model on custom
-datasets easier using Caribe built on HuggingFace Transformers APIs (Beta) ###
+    datasets easier using Caribe built on HuggingFace Transformers APIs ###
  Training Section: Caribe allows any user to fine-tune a T5 model on a custom
 dataset. The snippet below trains and generates a model in the "model/" folder.
 Please ensure that your training and evaluation datasets are in the recommended
   format before training. For more info checkout [T5 documentation.](https://
 huggingface.co/docs/transformers/main/en/model_doc/t5#t5) ```python from Caribe
        import T5_Caribe as t5 model = t5.T5_Trainer("train_dataset.csv",
       "eval_dataset.csv") connect = model.connect_datasets("csv") train =
@@ -207,16 +206,22 @@
     updated. - Future plans to create translations, models and datasets for
   Caribbean French and Spanish Creoles to their respective lexifers (Requires
 extensive research). - Some users complained of problems importing some of the
    dependencies. This is currently being monitored (10/06/2022). - New model
 introduced for sentence capitalization (09/06/2022) !!! - NEW model introduced
   for direct translation from Trinidad English Creole(TEC) to English(26/06/
   2022). - NEW model introduced for direct translation from Guyanese English
-Creole(GEC) to English(26/09/2022). --- - ## Contact For any concerns or issues
-      with this library. Email: keston.smith@my.uwi.edu Website: https://
+   Creole(GEC) to English(26/09/2022). - The gingerit_corrector function is
+   deprecated on versions 0.9.0 and above of Caribe. Due to deletion of the
+gingerit package, the gingerit_corrector function may no longer work depending
+on your initial date of install. To avoid dependency issues discovered on cloud
+ computing services like Google Colab, the function and its parent dependency
+ will be removed. Users can utilise the much better caribe_corrector function
+ for sentence correction tasks (08/08/2023). --- - ## Contact For any concerns
+ or issues with this library. Email: keston.smith@my.uwi.edu Website: https://
    www.thecaribe.org/ ___ CHANGELOG =======================================
 Version 0.0.1 (16/09/2021) - Initial Release Version 0.0.2 (16/09/2021) - Minor
  bugs fixed - More words added Version 0.0.3 (16/09/2021) - Minor bugs fixed -
   More words added - phase decode method created Version 0.0.4 (17/09/2021) -
 More words added - caribe corrector method created Version 0.0.5 (17/09/2021) -
  Minor Dependency issues resolved Version 0.0.6 (17/09/2021) - More Words and
   phrases added Version 0.0.7 (21/09/2021) - Major bug fixed where individual
@@ -261,8 +266,13 @@
  English. Version 0.6.6 (29/06/2022) - More Words Added. Version 0.6.8 (02/07/
  2022) - More Words Added - Model Updated - Entries Changed or Removed Version
 0.7.5 (31/07/2022) - Introducing an easier method to Fine-tuning a T5-model on
   custom datasets. Version 0.7.7 (14/08/2022) - Introducing Guyanese English
 Creole Version 0.7.8 (04/09/2022) - More Words Added Version 0.7.9 (26/09/2022)
 - Introducing a NEW NLP model to directly translate Guyanese English Creole to
  English. Version 0.8.1 (02/10/2022) - Introducing a NEW NLP model to directly
-            translate Standard English to Trinidad English Creole.
+ translate Standard English to Trinidad English Creole. Version 0.9.0 (08/08/
+  2023) - Resolved dependency issues with cloud computing services where the
+service refused to install the latest version of package because of a missing/
+   deleted dependency. - The gingerit_corrector function is deprecated from
+   version 0.9.0 and above. - Gingerit package no longer exists. Dependency
+                                   removed.
```

### Comparing `Caribe-0.8.9/LICENSE.txt` & `Caribe-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Caribe-0.8.9/PKG-INFO` & `Caribe-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Caribe
-Version: 0.8.9
+Version: 0.9.0
 Summary: Caribbean English Creoles to Standard English
 Home-page: UNKNOWN
 Author: Keston Smith
 Author-email: keston.smith@my.uwi.edu
 License: Apache License, Version 2.0
 Keywords: Translator
 Platform: UNKNOWN
@@ -195,15 +195,14 @@
 ---
 - ## Additional Information
     - `trinidad_decode()` : Decodes the sentence as a whole string.
     - `guyanese_decode()`:  Decodes the sentence as a whole string.
     - `trinidad_decode_split()`: Decodes the sentence word by word.
     - `phrase_decode()`: Decodes the sentence against known creole phrases.
     - `caribe_corrector()`: Corrects grammatical errors in a sentence using a trained NLP model.
-    - `gingerit_corrector()`: Corrects grammatical errors in a sentence using gingerit.
     - `t5_kes_corrector()`: Corrects grammatical errors in a sentence using a trained NLP model.
     - `trinidad_encode()`: Encodes a sentence to Trinidadian English Creole.
     - `guyanese_encode()`: Encodes a sentence to Guyanese English Creole.
     - `trinidad_direct_translation()`: Translates Trinidad English Creole to English.
     - `capitalize()`: Capitalize groups of sentences using an NLP model.
     - `caribe_pos()`: Generates parts of speech tagging on creole words.
     - `pos_report()`: Generates parts of speech tagging on english words.
@@ -282,15 +281,15 @@
 
 ```
 
 ---
 ## Dictionary Data
 The encoder and decoder utilises a dictionary data structure. The data for the dictionary was gathered from web-scapping social media sites among other websites and using Lise Winer Dictionary of the English Creole of Trinidad and Tobago among other scholarly resources.
 ____
-## Fine-tune a T5 model on custom datasets easier using Caribe built on HuggingFace Transformers APIs (Beta)
+## Fine-tune a T5 model on custom datasets easier using Caribe built on HuggingFace Transformers APIs 
 
 ### Training Section:
 Caribe allows any user to fine-tune a T5 model on a custom dataset.  The snippet below trains and generates a model in the "model/" folder. 
 Please ensure that your training and evaluation datasets are in the recommended format before training. For more info checkout [T5 documentation.](https://huggingface.co/docs/transformers/main/en/model_doc/t5#t5) 
 ```python
 from Caribe import T5_Caribe as t5
 
@@ -414,14 +413,17 @@
 - NLP Models and Dictionaries are continuously updated.
 - Future plans to create translations, models and datasets for Caribbean French and Spanish Creoles to their respective lexifers (Requires extensive research).
 - Some users complained of problems importing some of the dependencies. This is currently being monitored (10/06/2022).
 - New model introduced for sentence capitalization (09/06/2022) !!!
 - NEW model introduced for direct translation from Trinidad English Creole(TEC) to English(26/06/2022).
 - NEW model introduced for direct translation from Guyanese English Creole(GEC) to English(26/09/2022).
 
+- The gingerit_corrector function is deprecated on versions 0.9.0 and above of Caribe. Due to deletion of the gingerit package,   
+the gingerit_corrector function may no longer work depending on your initial date of install. To avoid dependency issues discovered on cloud computing services like Google Colab, the function and its parent dependency will be removed. Users can utilise the much better caribe_corrector function for sentence correction tasks (08/08/2023). 
+
 ---
 - ## Contact 
 For any concerns or issues with this library.
 
 Email: keston.smith@my.uwi.edu 
 
 Website: https://www.thecaribe.org/
@@ -569,7 +571,12 @@
 
 Version 0.7.9 (26/09/2022)
 -  Introducing a NEW NLP model to directly translate Guyanese English Creole to English.
 
 Version 0.8.1 (02/10/2022)
 -  Introducing a NEW NLP model to directly translate Standard English to Trinidad English Creole.
 
+Version 0.9.0 (08/08/2023)
+- Resolved dependency issues with cloud computing services where the service refused to install the latest version of package because of a missing/deleted dependency.
+- The gingerit_corrector function is deprecated from version 0.9.0 and above. 
+- Gingerit package no longer exists. Dependency removed.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Caribe Version: 0.8.9 Summary: Caribbean English
+Metadata-Version: 2.1 Name: Caribe Version: 0.9.0 Summary: Caribbean English
 Creoles to Standard English Home-page: UNKNOWN Author: Keston Smith Author-
 email: keston.smith@my.uwi.edu License: Apache License, Version 2.0 Keywords:
 Translator Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Education Classifier: Operating System
 :: Microsoft :: Windows :: Windows 10 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown License-File: LICENSE.txt [![License]
@@ -73,24 +73,23 @@
 cb.capitalize(sentence) print(capitalized_text) # Output: John is a boy. He is
  12 years old. His sister's name is Joy. ``` --- - ## Additional Information -
         `trinidad_decode()` : Decodes the sentence as a whole string. -
         `guyanese_decode()`: Decodes the sentence as a whole string. -
 `trinidad_decode_split()`: Decodes the sentence word by word. - `phrase_decode
 ()`: Decodes the sentence against known creole phrases. - `caribe_corrector()`:
     Corrects grammatical errors in a sentence using a trained NLP model. -
-    `gingerit_corrector()`: Corrects grammatical errors in a sentence using
-  gingerit. - `t5_kes_corrector()`: Corrects grammatical errors in a sentence
-    using a trained NLP model. - `trinidad_encode()`: Encodes a sentence to
-   Trinidadian English Creole. - `guyanese_encode()`: Encodes a sentence to
-Guyanese English Creole. - `trinidad_direct_translation()`: Translates Trinidad
-  English Creole to English. - `capitalize()`: Capitalize groups of sentences
-  using an NLP model. - `caribe_pos()`: Generates parts of speech tagging on
- creole words. - `pos_report()`: Generates parts of speech tagging on english
-words. - `remove_signs()`: Takes any sentence and remove punctuation marks. --
-- - ## File Encodings on NLP datasets Caribe introduces file encoding (Beta) in
+`t5_kes_corrector()`: Corrects grammatical errors in a sentence using a trained
+  NLP model. - `trinidad_encode()`: Encodes a sentence to Trinidadian English
+Creole. - `guyanese_encode()`: Encodes a sentence to Guyanese English Creole. -
+`trinidad_direct_translation()`: Translates Trinidad English Creole to English.
+    - `capitalize()`: Capitalize groups of sentences using an NLP model. -
+     `caribe_pos()`: Generates parts of speech tagging on creole words. -
+     `pos_report()`: Generates parts of speech tagging on english words. -
+  `remove_signs()`: Takes any sentence and remove punctuation marks. --- - ##
+   File Encodings on NLP datasets Caribe introduces file encoding (Beta) in
 version 0.1.0. This allows a dataset of any supported filetype to be translated
 into Trinidad English Creole. The file encoding feature only supports txt, json
 or csv files only. - ### Usage of File Encodings: ```python import Caribe as cb
 convert = cb.file_encode("test.txt", "text") # Generates a translated text file
   convert = cb.file_encode("test.json", "json") # Generates a translated json
  file convert = cb.file_encode("test.csv", "csv") # Generates a translated csv
  file ``` --- - ## First Parser for the Trinidad English Creole Language This
@@ -127,15 +126,15 @@
    import Caribe as cb text= "Dem men doh kno wat dey doing wid d money bai"
  output= cb.tec_translator(text) print(output.tec_translate()) #Output: These
 men do not know what they are doing with the money. ``` --- ## Dictionary Data
 The encoder and decoder utilises a dictionary data structure. The data for the
    dictionary was gathered from web-scapping social media sites among other
 websites and using Lise Winer Dictionary of the English Creole of Trinidad and
 Tobago among other scholarly resources. ____ ## Fine-tune a T5 model on custom
-datasets easier using Caribe built on HuggingFace Transformers APIs (Beta) ###
+    datasets easier using Caribe built on HuggingFace Transformers APIs ###
  Training Section: Caribe allows any user to fine-tune a T5 model on a custom
 dataset. The snippet below trains and generates a model in the "model/" folder.
 Please ensure that your training and evaluation datasets are in the recommended
   format before training. For more info checkout [T5 documentation.](https://
 huggingface.co/docs/transformers/main/en/model_doc/t5#t5) ```python from Caribe
        import T5_Caribe as t5 model = t5.T5_Trainer("train_dataset.csv",
       "eval_dataset.csv") connect = model.connect_datasets("csv") train =
@@ -207,16 +206,22 @@
     updated. - Future plans to create translations, models and datasets for
   Caribbean French and Spanish Creoles to their respective lexifers (Requires
 extensive research). - Some users complained of problems importing some of the
    dependencies. This is currently being monitored (10/06/2022). - New model
 introduced for sentence capitalization (09/06/2022) !!! - NEW model introduced
   for direct translation from Trinidad English Creole(TEC) to English(26/06/
   2022). - NEW model introduced for direct translation from Guyanese English
-Creole(GEC) to English(26/09/2022). --- - ## Contact For any concerns or issues
-      with this library. Email: keston.smith@my.uwi.edu Website: https://
+   Creole(GEC) to English(26/09/2022). - The gingerit_corrector function is
+   deprecated on versions 0.9.0 and above of Caribe. Due to deletion of the
+gingerit package, the gingerit_corrector function may no longer work depending
+on your initial date of install. To avoid dependency issues discovered on cloud
+ computing services like Google Colab, the function and its parent dependency
+ will be removed. Users can utilise the much better caribe_corrector function
+ for sentence correction tasks (08/08/2023). --- - ## Contact For any concerns
+ or issues with this library. Email: keston.smith@my.uwi.edu Website: https://
    www.thecaribe.org/ ___ CHANGELOG =======================================
 Version 0.0.1 (16/09/2021) - Initial Release Version 0.0.2 (16/09/2021) - Minor
  bugs fixed - More words added Version 0.0.3 (16/09/2021) - Minor bugs fixed -
   More words added - phase decode method created Version 0.0.4 (17/09/2021) -
 More words added - caribe corrector method created Version 0.0.5 (17/09/2021) -
  Minor Dependency issues resolved Version 0.0.6 (17/09/2021) - More Words and
   phrases added Version 0.0.7 (21/09/2021) - Major bug fixed where individual
@@ -261,8 +266,13 @@
  English. Version 0.6.6 (29/06/2022) - More Words Added. Version 0.6.8 (02/07/
  2022) - More Words Added - Model Updated - Entries Changed or Removed Version
 0.7.5 (31/07/2022) - Introducing an easier method to Fine-tuning a T5-model on
   custom datasets. Version 0.7.7 (14/08/2022) - Introducing Guyanese English
 Creole Version 0.7.8 (04/09/2022) - More Words Added Version 0.7.9 (26/09/2022)
 - Introducing a NEW NLP model to directly translate Guyanese English Creole to
  English. Version 0.8.1 (02/10/2022) - Introducing a NEW NLP model to directly
-            translate Standard English to Trinidad English Creole.
+ translate Standard English to Trinidad English Creole. Version 0.9.0 (08/08/
+  2023) - Resolved dependency issues with cloud computing services where the
+service refused to install the latest version of package because of a missing/
+   deleted dependency. - The gingerit_corrector function is deprecated from
+   version 0.9.0 and above. - Gingerit package no longer exists. Dependency
+                                   removed.
```

### Comparing `Caribe-0.8.9/README.md` & `Caribe-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,14 @@
 ---
 - ## Additional Information
     - `trinidad_decode()` : Decodes the sentence as a whole string.
     - `guyanese_decode()`:  Decodes the sentence as a whole string.
     - `trinidad_decode_split()`: Decodes the sentence word by word.
     - `phrase_decode()`: Decodes the sentence against known creole phrases.
     - `caribe_corrector()`: Corrects grammatical errors in a sentence using a trained NLP model.
-    - `gingerit_corrector()`: Corrects grammatical errors in a sentence using gingerit.
     - `t5_kes_corrector()`: Corrects grammatical errors in a sentence using a trained NLP model.
     - `trinidad_encode()`: Encodes a sentence to Trinidadian English Creole.
     - `guyanese_encode()`: Encodes a sentence to Guyanese English Creole.
     - `trinidad_direct_translation()`: Translates Trinidad English Creole to English.
     - `capitalize()`: Capitalize groups of sentences using an NLP model.
     - `caribe_pos()`: Generates parts of speech tagging on creole words.
     - `pos_report()`: Generates parts of speech tagging on english words.
@@ -264,15 +263,15 @@
 
 ```
 
 ---
 ## Dictionary Data
 The encoder and decoder utilises a dictionary data structure. The data for the dictionary was gathered from web-scapping social media sites among other websites and using Lise Winer Dictionary of the English Creole of Trinidad and Tobago among other scholarly resources.
 ____
-## Fine-tune a T5 model on custom datasets easier using Caribe built on HuggingFace Transformers APIs (Beta)
+## Fine-tune a T5 model on custom datasets easier using Caribe built on HuggingFace Transformers APIs 
 
 ### Training Section:
 Caribe allows any user to fine-tune a T5 model on a custom dataset.  The snippet below trains and generates a model in the "model/" folder. 
 Please ensure that your training and evaluation datasets are in the recommended format before training. For more info checkout [T5 documentation.](https://huggingface.co/docs/transformers/main/en/model_doc/t5#t5) 
 ```python
 from Caribe import T5_Caribe as t5
 
@@ -396,14 +395,17 @@
 - NLP Models and Dictionaries are continuously updated.
 - Future plans to create translations, models and datasets for Caribbean French and Spanish Creoles to their respective lexifers (Requires extensive research).
 - Some users complained of problems importing some of the dependencies. This is currently being monitored (10/06/2022).
 - New model introduced for sentence capitalization (09/06/2022) !!!
 - NEW model introduced for direct translation from Trinidad English Creole(TEC) to English(26/06/2022).
 - NEW model introduced for direct translation from Guyanese English Creole(GEC) to English(26/09/2022).
 
+- The gingerit_corrector function is deprecated on versions 0.9.0 and above of Caribe. Due to deletion of the gingerit package,   
+the gingerit_corrector function may no longer work depending on your initial date of install. To avoid dependency issues discovered on cloud computing services like Google Colab, the function and its parent dependency will be removed. Users can utilise the much better caribe_corrector function for sentence correction tasks (08/08/2023). 
+
 ---
 - ## Contact 
 For any concerns or issues with this library.
 
 Email: keston.smith@my.uwi.edu 
 
 Website: https://www.thecaribe.org/
```

#### html2text {}

```diff
@@ -66,24 +66,23 @@
 cb.capitalize(sentence) print(capitalized_text) # Output: John is a boy. He is
  12 years old. His sister's name is Joy. ``` --- - ## Additional Information -
         `trinidad_decode()` : Decodes the sentence as a whole string. -
         `guyanese_decode()`: Decodes the sentence as a whole string. -
 `trinidad_decode_split()`: Decodes the sentence word by word. - `phrase_decode
 ()`: Decodes the sentence against known creole phrases. - `caribe_corrector()`:
     Corrects grammatical errors in a sentence using a trained NLP model. -
-    `gingerit_corrector()`: Corrects grammatical errors in a sentence using
-  gingerit. - `t5_kes_corrector()`: Corrects grammatical errors in a sentence
-    using a trained NLP model. - `trinidad_encode()`: Encodes a sentence to
-   Trinidadian English Creole. - `guyanese_encode()`: Encodes a sentence to
-Guyanese English Creole. - `trinidad_direct_translation()`: Translates Trinidad
-  English Creole to English. - `capitalize()`: Capitalize groups of sentences
-  using an NLP model. - `caribe_pos()`: Generates parts of speech tagging on
- creole words. - `pos_report()`: Generates parts of speech tagging on english
-words. - `remove_signs()`: Takes any sentence and remove punctuation marks. --
-- - ## File Encodings on NLP datasets Caribe introduces file encoding (Beta) in
+`t5_kes_corrector()`: Corrects grammatical errors in a sentence using a trained
+  NLP model. - `trinidad_encode()`: Encodes a sentence to Trinidadian English
+Creole. - `guyanese_encode()`: Encodes a sentence to Guyanese English Creole. -
+`trinidad_direct_translation()`: Translates Trinidad English Creole to English.
+    - `capitalize()`: Capitalize groups of sentences using an NLP model. -
+     `caribe_pos()`: Generates parts of speech tagging on creole words. -
+     `pos_report()`: Generates parts of speech tagging on english words. -
+  `remove_signs()`: Takes any sentence and remove punctuation marks. --- - ##
+   File Encodings on NLP datasets Caribe introduces file encoding (Beta) in
 version 0.1.0. This allows a dataset of any supported filetype to be translated
 into Trinidad English Creole. The file encoding feature only supports txt, json
 or csv files only. - ### Usage of File Encodings: ```python import Caribe as cb
 convert = cb.file_encode("test.txt", "text") # Generates a translated text file
   convert = cb.file_encode("test.json", "json") # Generates a translated json
  file convert = cb.file_encode("test.csv", "csv") # Generates a translated csv
  file ``` --- - ## First Parser for the Trinidad English Creole Language This
@@ -120,15 +119,15 @@
    import Caribe as cb text= "Dem men doh kno wat dey doing wid d money bai"
  output= cb.tec_translator(text) print(output.tec_translate()) #Output: These
 men do not know what they are doing with the money. ``` --- ## Dictionary Data
 The encoder and decoder utilises a dictionary data structure. The data for the
    dictionary was gathered from web-scapping social media sites among other
 websites and using Lise Winer Dictionary of the English Creole of Trinidad and
 Tobago among other scholarly resources. ____ ## Fine-tune a T5 model on custom
-datasets easier using Caribe built on HuggingFace Transformers APIs (Beta) ###
+    datasets easier using Caribe built on HuggingFace Transformers APIs ###
  Training Section: Caribe allows any user to fine-tune a T5 model on a custom
 dataset. The snippet below trains and generates a model in the "model/" folder.
 Please ensure that your training and evaluation datasets are in the recommended
   format before training. For more info checkout [T5 documentation.](https://
 huggingface.co/docs/transformers/main/en/model_doc/t5#t5) ```python from Caribe
        import T5_Caribe as t5 model = t5.T5_Trainer("train_dataset.csv",
       "eval_dataset.csv") connect = model.connect_datasets("csv") train =
@@ -200,10 +199,16 @@
     updated. - Future plans to create translations, models and datasets for
   Caribbean French and Spanish Creoles to their respective lexifers (Requires
 extensive research). - Some users complained of problems importing some of the
    dependencies. This is currently being monitored (10/06/2022). - New model
 introduced for sentence capitalization (09/06/2022) !!! - NEW model introduced
   for direct translation from Trinidad English Creole(TEC) to English(26/06/
   2022). - NEW model introduced for direct translation from Guyanese English
-Creole(GEC) to English(26/09/2022). --- - ## Contact For any concerns or issues
-      with this library. Email: keston.smith@my.uwi.edu Website: https://
+   Creole(GEC) to English(26/09/2022). - The gingerit_corrector function is
+   deprecated on versions 0.9.0 and above of Caribe. Due to deletion of the
+gingerit package, the gingerit_corrector function may no longer work depending
+on your initial date of install. To avoid dependency issues discovered on cloud
+ computing services like Google Colab, the function and its parent dependency
+ will be removed. Users can utilise the much better caribe_corrector function
+ for sentence correction tasks (08/08/2023). --- - ## Contact For any concerns
+ or issues with this library. Email: keston.smith@my.uwi.edu Website: https://
                             www.thecaribe.org/ ___
```

### Comparing `Caribe-0.8.9/setup.py` & `Caribe-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,20 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: Apache Software License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='Caribe',
-  version='0.8.9',
+  version='0.9.0',
   description='Caribbean English Creoles to Standard English',
   long_description_content_type="text/markdown",
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Keston Smith',
   author_email='keston.smith@my.uwi.edu',
   license='Apache License, Version 2.0', 
   classifiers=classifiers,
   keywords='Translator', 
   packages=find_packages(),
-  install_requires=['nltk>=3.6.3', 'pandas>=1.3.4', 'gingerit==0.9.0', 'transformers>=4.15.0', 'requests>=2.25.1', 'torch', 'datasets'] 
+  install_requires=['nltk>=3.6.3', 'pandas>=1.3.4', 'transformers>=4.15.0', 'requests>=2.25.1', 'torch', 'datasets'] 
 )
```

