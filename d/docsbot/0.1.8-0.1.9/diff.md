# Comparing `tmp/docsbot-0.1.8.tar.gz` & `tmp/docsbot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsbot-0.1.8.tar", last modified: Tue Aug  8 09:41:55 2023, max compression
+gzip compressed data, was "docsbot-0.1.9.tar", last modified: Tue Aug  8 16:53:08 2023, max compression
```

## Comparing `docsbot-0.1.8.tar` & `docsbot-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 09:41:55.296651 docsbot-0.1.8/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4892 2023-08-08 09:41:55.296550 docsbot-0.1.8/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     4654 2023-08-08 03:01:47.000000 docsbot-0.1.8/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 09:41:55.296418 docsbot-0.1.8/docsbot.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4892 2023-08-08 09:41:55.000000 docsbot-0.1.8/docsbot.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      206 2023-08-08 09:41:55.000000 docsbot-0.1.8/docsbot.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 09:41:55.000000 docsbot-0.1.8/docsbot.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       45 2023-08-08 09:41:55.000000 docsbot-0.1.8/docsbot.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       94 2023-08-08 09:41:55.000000 docsbot-0.1.8/docsbot.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 09:41:55.000000 docsbot-0.1.8/docsbot.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-08 09:41:55.296685 docsbot-0.1.8/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      747 2023-08-08 09:41:47.000000 docsbot-0.1.8/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 16:53:08.205876 docsbot-0.1.9/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4586 2023-08-08 16:53:08.205757 docsbot-0.1.9/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4348 2023-08-08 16:46:58.000000 docsbot-0.1.9/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 16:53:08.204659 docsbot-0.1.9/docsbot/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-08-08 13:46:21.000000 docsbot-0.1.9/docsbot/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5648 2023-08-08 16:42:13.000000 docsbot-0.1.9/docsbot/base.py
+-rwxr-xr-x   0 jeffrey    (501) staff       (20)     5184 2023-08-08 16:48:27.000000 docsbot-0.1.9/docsbot/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1112 2023-08-08 16:48:27.000000 docsbot-0.1.9/docsbot/config.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-08 16:53:08.205612 docsbot-0.1.9/docsbot.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4586 2023-08-08 16:53:08.000000 docsbot-0.1.9/docsbot.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      275 2023-08-08 16:53:08.000000 docsbot-0.1.9/docsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-08 16:53:08.000000 docsbot-0.1.9/docsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       45 2023-08-08 16:53:08.000000 docsbot-0.1.9/docsbot.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      119 2023-08-08 16:53:08.000000 docsbot-0.1.9/docsbot.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        8 2023-08-08 16:53:08.000000 docsbot-0.1.9/docsbot.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-08 16:53:08.205910 docsbot-0.1.9/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      810 2023-08-08 16:51:02.000000 docsbot-0.1.9/setup.py
```

### Comparing `docsbot-0.1.8/PKG-INFO` & `docsbot-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: docsbot
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple chat bot for querying information from your local private documents.
 Home-page: https://github.com/CuiJing/docsbot
 Author: Jeff
 Description-Content-Type: text/markdown
 
 # DocsBot 使用说明
 
 DocsBot 是一个简单的命令行工具，用对话的方式，快速查询本地的文档库（Word、PDF、PPT等）
 
 ## 快速开始 Quick Start
 
+### 安装：通过pip 安装
 ```shell
-$ pip install docsbot
+$ pip install docsbot -i https://pypi.tuna.tsinghua.edu.cn/simple
+```
 
+### 安装：通过Docker运行
+```shell
+docker run -ti  -e "OPENAI_PROXY=http://192.168.3.112:8001" -e "OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxx" jingstory/docsbot  bash
+```
 
+### 使用
+```
 $ docsbot
 Please enter your OpenAI Key: sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 usage: chatbase [-h] {addbase,listbase,deletebase,query} ...
 
 positional arguments:
   {addbase,listbase,deletebase,query}
 
@@ -44,17 +52,15 @@
 $ docsbot query base000x7uvrvegk9vv 什么是技术开发合同
 Using vector store:  Qdrant
 查询: 什么是技术开发合同
 结果:  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。它包括委托开发合同和合作开发合同，并且应当采用书面形式。
 来源文件：
 1. 来源：/Users/jeffrey/Downloads/laws/中华人民共和国民法典.docx
    内容1.：第八百五十一条  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。  技术开发合同包括委托开发合同和合作开发合同。  技术开发合同应当采用书面形式。  当事人之间就具有实用价值的科技成果实施转化订立的合同，参照适用技术开发合同的有关规定。
-   内容2.：第八百五十一条  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。  技术开发合同包括委托开发合同和合作开发合同。  技术开发合同应当采用书面形式。  当事人之间就具有实用价值的科技成果实施转化订立的合同，参照适用技术开发合同的有关规定。
-   内容3.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
-   内容4.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
+   内容2.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
 Queried base with ID base000x7uvrvegk9vv with query 什么是技术开发合同
 
 
 
 
 ```
 
@@ -87,24 +93,31 @@
 ### 配置文件
 第一次运行时，请根据提示设置OpenAI的Key，`docsbot`自动保存到配置文件 
 `$HOME/.docsbot/docsbot.env`中。
 
 所有的配置项如下：
 ```env
 OpenAI_KEY=xxxxxxxxx
+OPENAI_PROXY="http://192.168.3.112:8001"
 VECTOR_STORE_TYPE="Chroma"  # 索引类型，目前支持Chroma、Qdrant
 QDRANT_SERVER_URL="http://192.168.1.22:6333"
 ```
 
 
 ## FAQ
 
+### Q：由于众所周知的原因，如何设置OPENAI的代理？
+在配置文件中，增加如下配置项：
+```env
+OPENAI_PROXY="http://192.168.3.112:8001"
+```
+
 ### Q：如何更换向量数据库为Qdrant？
 
-修改配置文件，添加如下内容（修改为真实的Qdrant地址）：
+在配置文件中，增加如下配置项（修改为真实的Qdrant地址）：
 ```env
 VECTOR_STORE_TYPE="Qdrant"
 QDRANT_SERVER_URL="http://192.168.1.22:6333"
 ```
```

### Comparing `docsbot-0.1.8/README.md` & `docsbot-0.1.9/docsbot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,33 @@
+Metadata-Version: 2.1
+Name: docsbot
+Version: 0.1.9
+Summary: A simple chat bot for querying information from your local private documents.
+Home-page: https://github.com/CuiJing/docsbot
+Author: Jeff
+Description-Content-Type: text/markdown
+
 # DocsBot 使用说明
 
 DocsBot 是一个简单的命令行工具，用对话的方式，快速查询本地的文档库（Word、PDF、PPT等）
 
 ## 快速开始 Quick Start
 
+### 安装：通过pip 安装
 ```shell
-$ pip install docsbot
+$ pip install docsbot -i https://pypi.tuna.tsinghua.edu.cn/simple
+```
 
+### 安装：通过Docker运行
+```shell
+docker run -ti  -e "OPENAI_PROXY=http://192.168.3.112:8001" -e "OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxx" jingstory/docsbot  bash
+```
 
+### 使用
+```
 $ docsbot
 Please enter your OpenAI Key: sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 usage: chatbase [-h] {addbase,listbase,deletebase,query} ...
 
 positional arguments:
   {addbase,listbase,deletebase,query}
 
@@ -36,17 +52,15 @@
 $ docsbot query base000x7uvrvegk9vv 什么是技术开发合同
 Using vector store:  Qdrant
 查询: 什么是技术开发合同
 结果:  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。它包括委托开发合同和合作开发合同，并且应当采用书面形式。
 来源文件：
 1. 来源：/Users/jeffrey/Downloads/laws/中华人民共和国民法典.docx
    内容1.：第八百五十一条  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。  技术开发合同包括委托开发合同和合作开发合同。  技术开发合同应当采用书面形式。  当事人之间就具有实用价值的科技成果实施转化订立的合同，参照适用技术开发合同的有关规定。
-   内容2.：第八百五十一条  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。  技术开发合同包括委托开发合同和合作开发合同。  技术开发合同应当采用书面形式。  当事人之间就具有实用价值的科技成果实施转化订立的合同，参照适用技术开发合同的有关规定。
-   内容3.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
-   内容4.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
+   内容2.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
 Queried base with ID base000x7uvrvegk9vv with query 什么是技术开发合同
 
 
 
 
 ```
 
@@ -79,24 +93,31 @@
 ### 配置文件
 第一次运行时，请根据提示设置OpenAI的Key，`docsbot`自动保存到配置文件 
 `$HOME/.docsbot/docsbot.env`中。
 
 所有的配置项如下：
 ```env
 OpenAI_KEY=xxxxxxxxx
+OPENAI_PROXY="http://192.168.3.112:8001"
 VECTOR_STORE_TYPE="Chroma"  # 索引类型，目前支持Chroma、Qdrant
 QDRANT_SERVER_URL="http://192.168.1.22:6333"
 ```
 
 
 ## FAQ
 
+### Q：由于众所周知的原因，如何设置OPENAI的代理？
+在配置文件中，增加如下配置项：
+```env
+OPENAI_PROXY="http://192.168.3.112:8001"
+```
+
 ### Q：如何更换向量数据库为Qdrant？
 
-修改配置文件，添加如下内容（修改为真实的Qdrant地址）：
+在配置文件中，增加如下配置项（修改为真实的Qdrant地址）：
 ```env
 VECTOR_STORE_TYPE="Qdrant"
 QDRANT_SERVER_URL="http://192.168.1.22:6333"
 ```
```

### Comparing `docsbot-0.1.8/docsbot.egg-info/PKG-INFO` & `docsbot-0.1.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1
-Name: docsbot
-Version: 0.1.8
-Summary: A simple chat bot for querying information from your local private documents.
-Home-page: https://github.com/CuiJing/docsbot
-Author: Jeff
-Description-Content-Type: text/markdown
-
 # DocsBot 使用说明
 
 DocsBot 是一个简单的命令行工具，用对话的方式，快速查询本地的文档库（Word、PDF、PPT等）
 
 ## 快速开始 Quick Start
 
+### 安装：通过pip 安装
 ```shell
-$ pip install docsbot
+$ pip install docsbot -i https://pypi.tuna.tsinghua.edu.cn/simple
+```
 
+### 安装：通过Docker运行
+```shell
+docker run -ti  -e "OPENAI_PROXY=http://192.168.3.112:8001" -e "OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxx" jingstory/docsbot  bash
+```
 
+### 使用
+```
 $ docsbot
 Please enter your OpenAI Key: sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 usage: chatbase [-h] {addbase,listbase,deletebase,query} ...
 
 positional arguments:
   {addbase,listbase,deletebase,query}
 
@@ -44,17 +44,15 @@
 $ docsbot query base000x7uvrvegk9vv 什么是技术开发合同
 Using vector store:  Qdrant
 查询: 什么是技术开发合同
 结果:  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。它包括委托开发合同和合作开发合同，并且应当采用书面形式。
 来源文件：
 1. 来源：/Users/jeffrey/Downloads/laws/中华人民共和国民法典.docx
    内容1.：第八百五十一条  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。  技术开发合同包括委托开发合同和合作开发合同。  技术开发合同应当采用书面形式。  当事人之间就具有实用价值的科技成果实施转化订立的合同，参照适用技术开发合同的有关规定。
-   内容2.：第八百五十一条  技术开发合同是当事人之间就新技术、新产品、新工艺、新品种或者新材料及其系统的研究开发所订立的合同。  技术开发合同包括委托开发合同和合作开发合同。  技术开发合同应当采用书面形式。  当事人之间就具有实用价值的科技成果实施转化订立的合同，参照适用技术开发合同的有关规定。
-   内容3.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
-   内容4.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
+   内容2.：第八百四十三条  技术合同是当事人就技术开发、转让、许可、咨询或者服务订立的确立相互之间权利和义务的合同。  第八百四十四条  订立技术合同，应当有利于知识产权的保护和科学技术的进步，促进科学技术成果的研发、转化、应用和推广。
 Queried base with ID base000x7uvrvegk9vv with query 什么是技术开发合同
 
 
 
 
 ```
 
@@ -87,24 +85,31 @@
 ### 配置文件
 第一次运行时，请根据提示设置OpenAI的Key，`docsbot`自动保存到配置文件 
 `$HOME/.docsbot/docsbot.env`中。
 
 所有的配置项如下：
 ```env
 OpenAI_KEY=xxxxxxxxx
+OPENAI_PROXY="http://192.168.3.112:8001"
 VECTOR_STORE_TYPE="Chroma"  # 索引类型，目前支持Chroma、Qdrant
 QDRANT_SERVER_URL="http://192.168.1.22:6333"
 ```
 
 
 ## FAQ
 
+### Q：由于众所周知的原因，如何设置OPENAI的代理？
+在配置文件中，增加如下配置项：
+```env
+OPENAI_PROXY="http://192.168.3.112:8001"
+```
+
 ### Q：如何更换向量数据库为Qdrant？
 
-修改配置文件，添加如下内容（修改为真实的Qdrant地址）：
+在配置文件中，增加如下配置项（修改为真实的Qdrant地址）：
 ```env
 VECTOR_STORE_TYPE="Qdrant"
 QDRANT_SERVER_URL="http://192.168.1.22:6333"
 ```
```

