# Comparing `tmp/vector_vault-2.2.1.tar.gz` & `tmp/vector_vault-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.2.1.tar", last modified: Mon Aug  7 16:34:27 2023, max compression
+gzip compressed data, was "vector_vault-2.2.2.tar", last modified: Wed Aug  9 00:49:08 2023, max compression
```

## Comparing `vector_vault-2.2.1.tar` & `vector_vault-2.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 16:34:27.791134 vector_vault-2.2.1/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.2.1/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 16:34:27.791000 vector_vault-2.2.1/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    27408 2023-08-06 20:06:54.000000 vector_vault-2.2.1/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-07 16:34:27.791174 vector_vault-2.2.1/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-07 16:34:24.000000 vector_vault-2.2.1/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 16:34:27.787185 vector_vault-2.2.1/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    28067 2023-08-07 16:34:27.000000 vector_vault-2.2.1/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-07 16:34:27.000000 vector_vault-2.2.1/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-07 16:34:27.000000 vector_vault-2.2.1/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-07 16:34:27.000000 vector_vault-2.2.1/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-07 16:34:27.000000 vector_vault-2.2.1/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-07 16:34:27.790631 vector_vault-2.2.1/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.2.1/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    14416 2023-08-07 16:34:19.000000 vector_vault-2.2.1/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.2.1/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.2.1/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.2.1/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.2.1/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.2.1/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16787 2023-08-06 19:45:14.000000 vector_vault-2.2.1/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    37296 2023-08-07 16:29:14.000000 vector_vault-2.2.1/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.2.1/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.2.1/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-09 00:49:08.084122 vector_vault-2.2.2/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.2.2/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    27954 2023-08-09 00:49:08.082914 vector_vault-2.2.2/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    27295 2023-08-07 16:48:57.000000 vector_vault-2.2.2/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-09 00:49:08.084186 vector_vault-2.2.2/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-09 00:49:03.000000 vector_vault-2.2.2/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-09 00:49:08.074134 vector_vault-2.2.2/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    27954 2023-08-09 00:49:08.000000 vector_vault-2.2.2/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-09 00:49:08.000000 vector_vault-2.2.2/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-09 00:49:08.000000 vector_vault-2.2.2/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-09 00:49:08.000000 vector_vault-2.2.2/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-09 00:49:08.000000 vector_vault-2.2.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-09 00:49:08.079415 vector_vault-2.2.2/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.2.2/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    14416 2023-08-07 16:34:19.000000 vector_vault-2.2.2/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.2.2/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.2.2/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.2.2/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.2.2/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.2.2/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16787 2023-08-06 19:45:14.000000 vector_vault-2.2.2/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    37296 2023-08-07 16:29:14.000000 vector_vault-2.2.2/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.2.2/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.2.2/vectorvault/wrap.py
```

### Comparing `vector_vault-2.2.1/LICENSE` & `vector_vault-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/PKG-INFO` & `vector_vault-2.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,14 @@
-Metadata-Version: 2.1
-Name: vector_vault
-Version: 2.2.1
-Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
-Home-page: https://github.com/John-Rood/VectorVault
-Author: VectorVault.io
-Author-email: john@johnrood.com
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a cloud-native vector database combined with OpenAI. Easily call ChatGPT or GPT4 and customize how they respond. Take any text data, vectorize it, and add it to the cloud vector database in 3 lines of code. Vector Vault enables you to quickly and securely create and interact with your vector databases - aka "Vaults". Vaults are hosted on serverless distributed cloud architecture backed by Google, making `vectorvault` scalable to any project size. 
 
-`vectorvault` takes inspiration from LangChain and integrates their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. The main value of the `vectorvault` package is how few lines of code you'll need to write to create the expirience you're goign for. It's much simpler and easier to use ChatGPT with the `vectorvault` package than OpenAI's default package. Customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (which was made using Vector Vault).
+`vectorvault` takes inspiration from LangChain, integrating their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. It's even easier to use ChatGPT with the `vectorvault` package than OpenAI's default package, and you can customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (PhilosophyGPT is powered by Vector Vault in this way).
 
-Make bots with knowledge and personalities. Create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and only limited by your imagination.
+You can bots with knowledge and personalities, create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and limited only by your imagination.
 
 Check out the tutorials in the Examples folder. You don't need a Vector Vault API key to use the tools or chat features, but you will need one to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io). While the service is paid at production scale, the first tier is free, and the following tiers are very affordable.
 
 <br>
 
 ### Full Python API:
```

### Comparing `vector_vault-2.2.1/README.md` & `vector_vault-2.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,31 @@
+Metadata-Version: 2.1
+Name: vector_vault
+Version: 2.2.2
+Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
+Home-page: https://github.com/John-Rood/VectorVault
+Author: VectorVault.io
+Author-email: john@johnrood.com
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a cloud-native vector database combined with OpenAI. Easily call ChatGPT or GPT4 and customize how they respond. Take any text data, vectorize it, and add it to the cloud vector database in 3 lines of code. Vector Vault enables you to quickly and securely create and interact with your vector databases - aka "Vaults". Vaults are hosted on serverless distributed cloud architecture backed by Google, making `vectorvault` scalable to any project size. 
 
-`vectorvault` takes inspiration from LangChain and integrates their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. The main value of the `vectorvault` package is how few lines of code you'll need to write to create the expirience you're goign for. It's much simpler and easier to use ChatGPT with the `vectorvault` package than OpenAI's default package. Customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (which was made using Vector Vault).
+`vectorvault` takes inspiration from LangChain, integrating their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. It's even easier to use ChatGPT with the `vectorvault` package than OpenAI's default package, and you can customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (PhilosophyGPT is powered by Vector Vault in this way).
 
-Make bots with knowledge and personalities. Create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and only limited by your imagination.
+You can bots with knowledge and personalities, create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and limited only by your imagination.
 
 Check out the tutorials in the Examples folder. You don't need a Vector Vault API key to use the tools or chat features, but you will need one to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io). While the service is paid at production scale, the first tier is free, and the following tiers are very affordable.
 
 <br>
 
 ### Full Python API:
```

### Comparing `vector_vault-2.2.1/setup.py` & `vector_vault-2.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.2.1",
+    version="2.2.2",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.2.1/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.2.2/vector_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.2.1
+Version: 2.2.2
 Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,17 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a cloud-native vector database combined with OpenAI. Easily call ChatGPT or GPT4 and customize how they respond. Take any text data, vectorize it, and add it to the cloud vector database in 3 lines of code. Vector Vault enables you to quickly and securely create and interact with your vector databases - aka "Vaults". Vaults are hosted on serverless distributed cloud architecture backed by Google, making `vectorvault` scalable to any project size. 
 
-`vectorvault` takes inspiration from LangChain and integrates their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. The main value of the `vectorvault` package is how few lines of code you'll need to write to create the expirience you're goign for. It's much simpler and easier to use ChatGPT with the `vectorvault` package than OpenAI's default package. Customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (which was made using Vector Vault).
+`vectorvault` takes inspiration from LangChain, integrating their most popular chat features and LLM tools. However, by combining vector databases with OpenAI's chat into one single package, `vectorvault` is able to hide most of the complexity, making it simple to build custom chat experiences. It's even easier to use ChatGPT with the `vectorvault` package than OpenAI's default package, and you can customize what ChatGPT says by adding the kind of things you want it to say to the Vault. When you call the `get_chat()` function with "get_context=True", whatever you have added to the Vault will be the way ChatGPT sounds. Check out [PhilosophyGPT](https://philbrosophy.web.app) for an example of this (PhilosophyGPT is powered by Vector Vault in this way).
 
-Make bots with knowledge and personalities. Create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and only limited by your imagination.
+You can bots with knowledge and personalities, create dynamic game characters with goals and opinions, AI support reps for a product/service, or your alter ego AI self. Use the "LLM Exclusive Tools" to create AI smart automation in code. The possibilities are endless and limited only by your imagination.
 
 Check out the tutorials in the Examples folder. You don't need a Vector Vault API key to use the tools or chat features, but you will need one to access the Vault Cloud. If you don't already have one, you can sign up for a free account at [VectorVault.io](https://vectorvault.io). While the service is paid at production scale, the first tier is free, and the following tiers are very affordable.
 
 <br>
 
 ### Full Python API:
```

### Comparing `vector_vault-2.2.1/vectorvault/ai.py` & `vector_vault-2.2.2/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/vectorvault/cloud_api.py` & `vector_vault-2.2.2/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/vectorvault/cloudmanager.py` & `vector_vault-2.2.2/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/vectorvault/creds.py` & `vector_vault-2.2.2/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/vectorvault/download.py` & `vector_vault-2.2.2/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/vectorvault/itemize.py` & `vector_vault-2.2.2/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/vectorvault/tools_gpt.py` & `vector_vault-2.2.2/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/vectorvault/vault.py` & `vector_vault-2.2.2/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.2.1/vectorvault/vecreq.py` & `vector_vault-2.2.2/vectorvault/vecreq.py`

 * *Files identical despite different names*

