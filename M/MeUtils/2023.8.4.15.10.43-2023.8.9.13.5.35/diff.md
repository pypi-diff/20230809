# Comparing `tmp/MeUtils-2023.8.4.15.10.43.tar.gz` & `tmp/MeUtils-2023.8.9.13.5.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2023.8.4.15.10.43.tar", last modified: Fri Aug  4 07:10:44 2023, max compression
+gzip compressed data, was "MeUtils-2023.8.9.13.5.35.tar", last modified: Wed Aug  9 05:05:36 2023, max compression
```

## Comparing `MeUtils-2023.8.4.15.10.43.tar` & `MeUtils-2023.8.9.13.5.35.tar`

### file list

```diff
@@ -1,585 +1,585 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.724671 MeUtils-2023.8.4.15.10.43/
--rw-r--r--   0 betterme   (501) staff       (20)     6148 2023-04-14 02:46:19.000000 MeUtils-2023.8.4.15.10.43/.DS_Store
--rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.8.4.15.10.43/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.612884 MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-08-04 07:10:44.000000 MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    19765 2023-08-04 07:10:44.000000 MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-08-04 07:10:44.000000 MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      232 2023-08-04 07:10:44.000000 MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1049 2023-08-04 07:10:44.000000 MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       17 2023-08-04 07:10:44.000000 MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-08-04 07:10:44.724504 MeUtils-2023.8.4.15.10.43/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.8.4.15.10.43/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-07-20 08:15:27.000000 MeUtils-2023.8.4.15.10.43/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/clear_git_history.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      291 2023-07-27 03:02:44.000000 MeUtils-2023.8.4.15.10.43/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.617438 MeUtils-2023.8.4.15.10.43/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.8.4.15.10.43/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.617831 MeUtils-2023.8.4.15.10.43/meutils/ai_audio/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_audio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_audio/asr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.618319 MeUtils-2023.8.4.15.10.43/meutils/ai_cv/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_cv/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_cv/ocr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.620483 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/
--rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/SplitSentence.py
--rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/Untitled-1(1).py
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/_lda.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.621232 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/_textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/_textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/_textsplitter/text_split.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/lda.py
--rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-07-25 08:50:49.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/ner.py
--rw-r--r--   0 betterme   (501) staff       (20)      963 2023-07-04 08:24:23.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/sentence_transformers.py
--rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.623666 MeUtils-2023.8.4.15.10.43/meutils/ann/
--rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/README_gensim.md
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/ann_inmemory.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/ann_qdrant.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.624098 MeUtils-2023.8.4.15.10.43/meutils/ann/examples/
--rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/examples/client.py
--rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/examples/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/ann/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.624320 MeUtils-2023.8.4.15.10.43/meutils/asyncio_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/asyncio_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8767 2023-08-04 00:52:37.000000 MeUtils-2023.8.4.15.10.43/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.626140 MeUtils-2023.8.4.15.10.43/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/nesc.py
--rw-r--r--   0 betterme   (501) staff       (20)      758 2023-08-04 07:10:42.000000 MeUtils-2023.8.4.15.10.43/meutils/clis/server.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.627043 MeUtils-2023.8.4.15.10.43/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/cmds/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.627336 MeUtils-2023.8.4.15.10.43/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)    10778 2023-08-02 00:43:22.000000 MeUtils-2023.8.4.15.10.43/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.627639 MeUtils-2023.8.4.15.10.43/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.635245 MeUtils-2023.8.4.15.10.43/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.8.4.15.10.43/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-08-04 07:10:43.000000 MeUtils-2023.8.4.15.10.43/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/data/coordinate.py
--rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.640580 MeUtils-2023.8.4.15.10.43/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/db/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     7396 2023-06-30 01:59:42.000000 MeUtils-2023.8.4.15.10.43/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/db/neo4j.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.643937 MeUtils-2023.8.4.15.10.43/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/__ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6482 2023-07-25 08:50:49.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     2741 2023-07-28 07:07:38.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.8.4.15.10.43/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.8.4.15.10.43/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.645228 MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/demo_es.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/demo_hnsw.py
--rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/in_memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/改造下hnsw.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.645657 MeUtils-2023.8.4.15.10.43/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2425 2023-08-02 06:36:30.000000 MeUtils-2023.8.4.15.10.43/meutils/easy_search/es.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.647444 MeUtils-2023.8.4.15.10.43/meutils/fileparser/
--rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/PDF抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      284 2023-07-12 04:10:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1025 2023-07-12 06:55:12.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.648849 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/
--rw-r--r--   0 betterme   (501) staff       (20)      223 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      803 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/__main__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/filetype.py
--rw-r--r--   0 betterme   (501) staff       (20)     2947 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/helpers.py
--rw-r--r--   0 betterme   (501) staff       (20)     3288 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/match.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.650838 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      498 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/application.py
--rw-r--r--   0 betterme   (501) staff       (20)    17006 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/archive.py
--rw-r--r--   0 betterme   (501) staff       (20)     4960 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     7513 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/document.py
--rw-r--r--   0 betterme   (501) staff       (20)     2924 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/font.py
--rw-r--r--   0 betterme   (501) staff       (20)     9130 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/image.py
--rw-r--r--   0 betterme   (501) staff       (20)      958 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/isobmff.py
--rw-r--r--   0 betterme   (501) staff       (20)     5371 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2089 2023-05-18 08:40:53.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      285 2023-07-15 07:06:30.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype.py
--rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4037 2023-07-17 10:15:11.000000 MeUtils-2023.8.4.15.10.43/meutils/fileparser/表格抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.8.4.15.10.43/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.651585 MeUtils-2023.8.4.15.10.43/meutils/init/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.8.4.15.10.43/meutils/init/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-07-26 06:41:28.000000 MeUtils-2023.8.4.15.10.43/meutils/init/evn.py
--rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2023.8.4.15.10.43/meutils/init/oo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.652893 MeUtils-2023.8.4.15.10.43/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.8.4.15.10.43/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.8.4.15.10.43/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2023.8.4.15.10.43/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/io/x.yml
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/jinja_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2499 2023-08-03 10:04:00.000000 MeUtils-2023.8.4.15.10.43/meutils/log_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.654177 MeUtils-2023.8.4.15.10.43/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-06-13 09:13:04.000000 MeUtils-2023.8.4.15.10.43/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     2962 2023-05-16 06:23:15.000000 MeUtils-2023.8.4.15.10.43/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.655844 MeUtils-2023.8.4.15.10.43/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.8.4.15.10.43/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1528 2023-07-25 10:06:46.000000 MeUtils-2023.8.4.15.10.43/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.8.4.15.10.43/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.8.4.15.10.43/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.656821 MeUtils-2023.8.4.15.10.43/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/office_automation/report/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/office_automation/投资管理系统O3.2_交易组.pdm
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.657693 MeUtils-2023.8.4.15.10.43/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2023.8.4.15.10.43/meutils/other/__demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/other/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.659541 MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/
--rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/__version__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/core.py
--rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/pool.py
--rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/types.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.8.4.15.10.43/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.662122 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.665420 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/
--rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/annlite.py
--rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/chunk.py
--rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/document.py
--rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/elastic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/match.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/milvus.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.669533 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/content.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.669943 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/dataloader/
--rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/dataloader/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/dataloader/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/delitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/embed.py
--rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/empty.py
--rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/getattr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/getitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/group.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.671559 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/binary.py
--rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/csv.py
--rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/dataframe.py
--rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/from_gen.py
--rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/json.py
--rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/pbar.py
--rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/pushpull.py
--rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/match.py
--rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/parallel.py
--rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/post.py
--rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/reduce.py
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/sample.py
--rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/setitem.py
--rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/traverse.py
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/opensearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/qdrant.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.672248 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/queryset/
--rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/queryset/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/queryset/lookup.py
--rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/queryset/parser.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/redis.py
--rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/sqlite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.672589 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.673517 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.674443 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.675431 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.676284 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/
--rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.677249 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/
--rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.678165 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/
--rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.679239 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.680047 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/
--rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/registry.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.680797 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/
--rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.681640 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/
--rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/weaviate.py
--rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.682554 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/enums.py
--rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/getter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/setter.py
--rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.683629 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/
--rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/data.py
--rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/generators.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.687420 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/_property.py
--rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/attribute.py
--rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/blob.py
--rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/content.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/dump.py
--rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/featurehash.py
--rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/mesh.py
--rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/multimodal.py
--rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/porting.py
--rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/protobuf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/rich_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/sugar.py
--rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/pydantic_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/strawberry_type.py
--rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/helper.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.688221 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.689221 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/
--rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/numpy.py
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/paddle.py
--rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/tensorflow.py
--rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/torch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.689599 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.689977 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/io/
--rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/io/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.690291 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/pb/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/pb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/pb/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.690613 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/pb2/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/pb2/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/pb2/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.690774 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/resources/
--rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/resources/ci-vendors.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.690944 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/resources/embedding-projector/
--rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.691675 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/data.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.692178 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/mixins/representer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.692340 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/typing/
--rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.8.4.15.10.43/meutils/other/docarray/typing/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.693569 MeUtils-2023.8.4.15.10.43/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.8.4.15.10.43/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     9319 2023-08-03 04:35:12.000000 MeUtils-2023.8.4.15.10.43/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.695243 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/embedding_plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/mecharts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/plot_utils/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.695708 MeUtils-2023.8.4.15.10.43/meutils/queues/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-07-20 02:35:53.000000 MeUtils-2023.8.4.15.10.43/meutils/queues/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1704 2023-07-20 03:22:15.000000 MeUtils-2023.8.4.15.10.43/meutils/queues/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.696863 MeUtils-2023.8.4.15.10.43/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     3375 2023-07-27 05:15:39.000000 MeUtils-2023.8.4.15.10.43/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.8.4.15.10.43/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.8.4.15.10.43/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/request_utils/公网ip.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.697374 MeUtils-2023.8.4.15.10.43/meutils/serving/
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.698607 MeUtils-2023.8.4.15.10.43/meutils/serving/celery/
--rw-r--r--   0 betterme   (501) staff       (20)      628 2023-08-04 02:38:19.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/celery/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2109 2023-08-04 05:36:36.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/celery/_conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      514 2023-08-04 06:55:40.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/celery/_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-08-04 06:55:14.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/celery/_run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      415 2023-08-04 07:01:12.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/celery/_run_fastapi.py
--rw-r--r--   0 betterme   (501) staff       (20)     1379 2023-08-04 06:59:02.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/celery/router.py
--rw-r--r--   0 betterme   (501) staff       (20)     1436 2023-08-04 06:45:49.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/celery/tasks.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.699123 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.699669 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/__demo/异步任务.py
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2106 2023-07-24 09:52:55.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.700395 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/errors/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/errors/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/errors/http_error.py
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/errors/validation_error.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.701416 MeUtils-2023.8.4.15.10.43/meutils/serving/gui/
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/gui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/gui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/gui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.701691 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.703939 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/client.py
--rw-r--r--   0 betterme   (501) staff       (20)    14055 2023-07-24 05:52:25.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/flow.svg
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-07-24 06:13:28.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/s.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-07-24 06:17:01.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/s2.py
--rw-r--r--   0 betterme   (501) staff       (20)     2113 2023-07-24 06:04:10.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/server.py
--rw-r--r--   0 betterme   (501) staff       (20)     1160 2023-07-19 06:57:16.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/test.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.704995 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/
--rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/SentenceEncoder.py
--rw-r--r--   0 betterme   (501) staff       (20)     1831 2023-07-17 10:23:25.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/SentenceEncoder_.py
--rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-07-24 06:57:00.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.705540 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/nlp_serving/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/nlp_serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/jina/nlp_serving/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.706864 MeUtils-2023.8.4.15.10.43/meutils/serving/st_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/st_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/st_utils/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/st_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/st_utils/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/st_utils/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.707935 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.708448 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/.streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/.streamlit/_config.toml
--rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/.streamlit/config.toml
--rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/_🏆_主页.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.709402 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/pages/
--rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/pages/_1_分词.py
--rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/pages/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/pages/_3_文本匹配.py
--rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.8.4.15.10.43/meutils/serving/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.709718 MeUtils-2023.8.4.15.10.43/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.710597 MeUtils-2023.8.4.15.10.43/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.8.4.15.10.43/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.711385 MeUtils-2023.8.4.15.10.43/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2023.8.4.15.10.43/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.8.4.15.10.43/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.714122 MeUtils-2023.8.4.15.10.43/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.715804 MeUtils-2023.8.4.15.10.43/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/hegui.py
--rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/markmap.html
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.715957 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.719250 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.719424 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.721398 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.721551 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.721863 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.722189 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.722647 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/x.html
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/templates/合规日报模板.docx
--rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.8.4.15.10.43/meutils/todo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.723665 MeUtils-2023.8.4.15.10.43/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/tools/monitor.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/meutils/zk_utils.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.8.4.15.10.43/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      369 2023-07-07 09:51:37.000000 MeUtils-2023.8.4.15.10.43/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/requirements_ai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/requirements_app.txt
--rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2023.8.4.15.10.43/requirements_db.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.8.4.15.10.43/requirements_fileparser.txt
--rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/requirements_office.txt
--rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/requirements_pd.txt
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/requirements_plot.txt
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/requirements_plus.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-04 07:10:44.724223 MeUtils-2023.8.4.15.10.43/scripts/
--rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/scripts/demo.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/scripts/killall.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/scripts/py_sh.sh
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.8.4.15.10.43/scripts/yum.sh
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-08-04 07:10:44.724722 MeUtils-2023.8.4.15.10.43/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2360 2023-08-04 07:09:27.000000 MeUtils-2023.8.4.15.10.43/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.012596 MeUtils-2023.8.9.13.5.35/
+-rw-r--r--   0 betterme   (501) staff       (20)     6148 2023-04-14 02:46:19.000000 MeUtils-2023.8.9.13.5.35/.DS_Store
+-rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.8.9.13.5.35/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.903839 MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1893 2023-08-09 05:05:35.000000 MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    19765 2023-08-09 05:05:35.000000 MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-08-09 05:05:35.000000 MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      232 2023-08-09 05:05:35.000000 MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1049 2023-08-09 05:05:35.000000 MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       17 2023-08-09 05:05:35.000000 MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1893 2023-08-09 05:05:36.012414 MeUtils-2023.8.9.13.5.35/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.8.9.13.5.35/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-07-20 08:15:27.000000 MeUtils-2023.8.9.13.5.35/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/clear_git_history.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      291 2023-07-27 03:02:44.000000 MeUtils-2023.8.9.13.5.35/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.908499 MeUtils-2023.8.9.13.5.35/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.8.9.13.5.35/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.908812 MeUtils-2023.8.9.13.5.35/meutils/ai_audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_audio/asr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.909194 MeUtils-2023.8.9.13.5.35/meutils/ai_cv/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_cv/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_cv/ocr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.910514 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/
+-rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/SplitSentence.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/Untitled-1(1).py
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/_lda.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.911182 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/_textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/_textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/_textsplitter/text_split.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/lda.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-07-25 08:50:49.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/ner.py
+-rw-r--r--   0 betterme   (501) staff       (20)      963 2023-07-04 08:24:23.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/sentence_transformers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.913995 MeUtils-2023.8.9.13.5.35/meutils/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/README_gensim.md
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/ann_inmemory.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/ann_qdrant.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.914361 MeUtils-2023.8.9.13.5.35/meutils/ann/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/examples/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/examples/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/ann/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.914541 MeUtils-2023.8.9.13.5.35/meutils/asyncio_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/asyncio_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8612 2023-08-07 00:40:02.000000 MeUtils-2023.8.9.13.5.35/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.916401 MeUtils-2023.8.9.13.5.35/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/nesc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      742 2023-08-04 07:25:31.000000 MeUtils-2023.8.9.13.5.35/meutils/clis/server.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.917387 MeUtils-2023.8.9.13.5.35/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/cmds/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.917852 MeUtils-2023.8.9.13.5.35/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10778 2023-08-02 00:43:22.000000 MeUtils-2023.8.9.13.5.35/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.918139 MeUtils-2023.8.9.13.5.35/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.926682 MeUtils-2023.8.9.13.5.35/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.8.9.13.5.35/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-08-09 05:05:35.000000 MeUtils-2023.8.9.13.5.35/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/data/coordinate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.930759 MeUtils-2023.8.9.13.5.35/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/db/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     7396 2023-06-30 01:59:42.000000 MeUtils-2023.8.9.13.5.35/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/db/neo4j.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.932274 MeUtils-2023.8.9.13.5.35/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/__ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6524 2023-08-09 01:31:12.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2741 2023-07-28 07:07:38.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.8.9.13.5.35/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.8.9.13.5.35/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.933021 MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/demo_es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/demo_hnsw.py
+-rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/in_memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/改造下hnsw.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.933284 MeUtils-2023.8.9.13.5.35/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2425 2023-08-02 06:36:30.000000 MeUtils-2023.8.9.13.5.35/meutils/easy_search/es.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.934172 MeUtils-2023.8.9.13.5.35/meutils/fileparser/
+-rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/PDF抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      284 2023-07-12 04:10:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1025 2023-07-12 06:55:12.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.935482 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/
+-rw-r--r--   0 betterme   (501) staff       (20)      223 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      803 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/__main__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/filetype.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2947 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/helpers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3288 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/match.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.937467 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      498 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/application.py
+-rw-r--r--   0 betterme   (501) staff       (20)    17006 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/archive.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4960 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7513 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2924 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/font.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9130 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)      958 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/isobmff.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5371 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2089 2023-05-18 08:40:53.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      285 2023-07-15 07:06:30.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4037 2023-07-17 10:15:11.000000 MeUtils-2023.8.9.13.5.35/meutils/fileparser/表格抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.8.9.13.5.35/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.938055 MeUtils-2023.8.9.13.5.35/meutils/init/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.8.9.13.5.35/meutils/init/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1588 2023-08-07 08:26:31.000000 MeUtils-2023.8.9.13.5.35/meutils/init/evn.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2023.8.9.13.5.35/meutils/init/oo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.939548 MeUtils-2023.8.9.13.5.35/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.8.9.13.5.35/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.8.9.13.5.35/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2023.8.9.13.5.35/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/io/x.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/jinja_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-08-09 01:28:38.000000 MeUtils-2023.8.9.13.5.35/meutils/log_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.940598 MeUtils-2023.8.9.13.5.35/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-06-13 09:13:04.000000 MeUtils-2023.8.9.13.5.35/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3701 2023-08-08 01:42:47.000000 MeUtils-2023.8.9.13.5.35/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.941341 MeUtils-2023.8.9.13.5.35/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.8.9.13.5.35/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1528 2023-07-25 10:06:46.000000 MeUtils-2023.8.9.13.5.35/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.8.9.13.5.35/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.8.9.13.5.35/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.941861 MeUtils-2023.8.9.13.5.35/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/office_automation/report/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/office_automation/投资管理系统O3.2_交易组.pdm
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.943048 MeUtils-2023.8.9.13.5.35/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2023.8.9.13.5.35/meutils/other/__demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/other/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.944894 MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/
+-rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/__version__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/core.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/pool.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/types.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.8.9.13.5.35/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.945834 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.949582 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/
+-rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/annlite.py
+-rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/chunk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/elastic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/milvus.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.953626 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/content.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.954032 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/dataloader/
+-rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/dataloader/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/dataloader/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/delitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/embed.py
+-rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/empty.py
+-rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/getattr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/getitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/group.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.955653 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/binary.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/csv.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/dataframe.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/from_gen.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/json.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/pbar.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/pushpull.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/parallel.py
+-rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/reduce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/sample.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/setitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/traverse.py
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/opensearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/qdrant.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.956406 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/queryset/
+-rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/queryset/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/queryset/lookup.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/queryset/parser.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/redis.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/sqlite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.956746 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.957871 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.958863 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.959825 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.960771 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/
+-rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.961662 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/
+-rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.962566 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/
+-rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.963676 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/
+-rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.964623 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/
+-rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/registry.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.965711 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.968432 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/
+-rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/weaviate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.969560 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/
+-rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/enums.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/getter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/setter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.970726 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/
+-rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/data.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/generators.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.975088 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/_property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/attribute.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/blob.py
+-rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/content.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/dump.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/featurehash.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-08-04 08:03:16.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/mesh.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/multimodal.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/porting.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/protobuf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/rich_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/sugar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/pydantic_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/strawberry_type.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/helper.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.976031 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.977058 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/
+-rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/numpy.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/paddle.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/tensorflow.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/torch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.977361 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.977700 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/io/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.977973 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/pb/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/pb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/pb/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.978259 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/pb2/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/pb2/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/pb2/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.978439 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/resources/
+-rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/resources/ci-vendors.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.978614 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/resources/embedding-projector/
+-rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/resources/embedding-projector/index.html.gz
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.979431 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/data.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.980077 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/mixins/representer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.980431 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/typing/
+-rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.8.9.13.5.35/meutils/other/docarray/typing/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.981093 MeUtils-2023.8.9.13.5.35/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.8.9.13.5.35/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9721 2023-08-09 05:05:33.000000 MeUtils-2023.8.9.13.5.35/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.982343 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/embedding_plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/mecharts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/plot_utils/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.982655 MeUtils-2023.8.9.13.5.35/meutils/queues/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-07-20 02:35:53.000000 MeUtils-2023.8.9.13.5.35/meutils/queues/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1704 2023-07-20 03:22:15.000000 MeUtils-2023.8.9.13.5.35/meutils/queues/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.983726 MeUtils-2023.8.9.13.5.35/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     3375 2023-07-27 05:15:39.000000 MeUtils-2023.8.9.13.5.35/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.8.9.13.5.35/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.8.9.13.5.35/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/request_utils/公网ip.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.984099 MeUtils-2023.8.9.13.5.35/meutils/serving/
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.984984 MeUtils-2023.8.9.13.5.35/meutils/serving/celery/
+-rw-r--r--   0 betterme   (501) staff       (20)      628 2023-08-04 02:38:19.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/celery/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2109 2023-08-04 05:36:36.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/celery/_conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      514 2023-08-04 06:55:40.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/celery/_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-08-04 06:55:14.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/celery/_run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      415 2023-08-04 07:01:12.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/celery/_run_fastapi.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1379 2023-08-04 06:59:02.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/celery/router.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1465 2023-08-04 07:31:09.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/celery/tasks.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.985548 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.986185 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/__demo/异步任务.py
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2106 2023-07-24 09:52:55.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.986941 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/errors/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/errors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/errors/http_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/errors/validation_error.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.988035 MeUtils-2023.8.9.13.5.35/meutils/serving/gui/
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/gui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/gui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/gui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.988328 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.990407 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14055 2023-07-24 05:52:25.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/flow.svg
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-07-24 06:13:28.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/s.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-07-24 06:17:01.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/s2.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2113 2023-07-24 06:04:10.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/server.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1160 2023-07-19 06:57:16.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/test.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.991492 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/
+-rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/SentenceEncoder.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1831 2023-07-17 10:23:25.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/SentenceEncoder_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-07-24 06:57:00.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.992001 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/nlp_serving/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/nlp_serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/jina/nlp_serving/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.993517 MeUtils-2023.8.9.13.5.35/meutils/serving/st_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/st_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/st_utils/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/st_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/st_utils/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/st_utils/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.994656 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.995216 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/.streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/.streamlit/_config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/.streamlit/config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/_🏆_主页.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.996111 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/pages/
+-rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/pages/_1_分词.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/pages/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/pages/_3_文本匹配.py
+-rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.8.9.13.5.35/meutils/serving/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.996445 MeUtils-2023.8.9.13.5.35/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.997054 MeUtils-2023.8.9.13.5.35/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.8.9.13.5.35/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.997962 MeUtils-2023.8.9.13.5.35/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2023.8.9.13.5.35/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      927 2023-08-07 12:04:31.000000 MeUtils-2023.8.9.13.5.35/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:35.999805 MeUtils-2023.8.9.13.5.35/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.001411 MeUtils-2023.8.9.13.5.35/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/hegui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/markmap.html
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.001612 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.006025 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.006245 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.008917 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.009104 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.009471 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.009861 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.010404 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/x.html
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/templates/合规日报模板.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.8.9.13.5.35/meutils/todo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.011427 MeUtils-2023.8.9.13.5.35/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/tools/monitor.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/meutils/zk_utils.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.8.9.13.5.35/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      369 2023-07-07 09:51:37.000000 MeUtils-2023.8.9.13.5.35/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/requirements_ai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/requirements_app.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       52 2023-06-02 06:00:11.000000 MeUtils-2023.8.9.13.5.35/requirements_db.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.8.9.13.5.35/requirements_fileparser.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/requirements_office.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/requirements_pd.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/requirements_plot.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/requirements_plus.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-08-09 05:05:36.012133 MeUtils-2023.8.9.13.5.35/scripts/
+-rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/scripts/demo.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/scripts/killall.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/scripts/py_sh.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.8.9.13.5.35/scripts/yum.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-08-09 05:05:36.012646 MeUtils-2023.8.9.13.5.35/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2360 2023-08-04 07:09:27.000000 MeUtils-2023.8.9.13.5.35/setup.py
```

### Comparing `MeUtils-2023.8.4.15.10.43/.DS_Store` & `MeUtils-2023.8.9.13.5.35/.DS_Store`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/.gitignore` & `MeUtils-2023.8.9.13.5.35/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/LICENSE` & `MeUtils-2023.8.9.13.5.35/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/PKG-INFO` & `MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.8.4.15.10.43
+Version: 2023.8.9.13.5.35
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/SOURCES.txt` & `MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/MeUtils.egg-info/requires.txt` & `MeUtils-2023.8.9.13.5.35/MeUtils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -24,47 +24,47 @@
 diskcache
 
 [ai]
 faiss-gpu
 gensim
 
 [all]
-iteration_utilities
-geopy
-thefuck
-gensim
-asyncmy
-fastapi[all]
-streamlit
-jieba
-jinja2
 cachetools
-missingno
-simplejson
-filetype
+pymongo
+seaborn
 pymupd
 pretty_errors
+redis-py-cluster
+geopy
+faiss-gpu
+dataframe_image
+iteration_utilities
+faiss-cpu
 reportlab
 thriftpy2
-pandas-profiling[notebook]
 polars
-seaborn
-pandas_summary
-dataframe_image
 uvicorn
-faiss-cpu
-faiss-gpu
-pymongo
-redis-py-cluster
-pymilvus
-pymysql
+pandas_summary
+jmespath
+missingno
+asyncmy
+gensim
 sqlalchemy
-schedule
+thefuck
+pymysql
+jieba
+streamlit
+filetype
+pymilvus
 pyarrow
-jmespath
+simplejson
+schedule
+jinja2
+fastapi[all]
+pandas-profiling[notebook]
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
 fastapi[all]
```

### Comparing `MeUtils-2023.8.4.15.10.43/PKG-INFO` & `MeUtils-2023.8.9.13.5.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.8.4.15.10.43
+Version: 2023.8.9.13.5.35
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
```

### Comparing `MeUtils-2023.8.4.15.10.43/README.md` & `MeUtils-2023.8.9.13.5.35/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/TODO.md` & `MeUtils-2023.8.9.13.5.35/TODO.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/clear_git_history.sh` & `MeUtils-2023.8.9.13.5.35/clear_git_history.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_audio/asr.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_audio/asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/SplitSentence.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/SplitSentence.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/Untitled-1(1).py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/Untitled-1(1).py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/_lda.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/_lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/_textsplitter/text_split.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/_textsplitter/text_split.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/lda.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/ner.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/ner.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/sentence_transformers.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/textsplitter.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/textsplitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ai_nlp/word_segmentation.py` & `MeUtils-2023.8.9.13.5.35/meutils/ai_nlp/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/README.md` & `MeUtils-2023.8.9.13.5.35/meutils/ann/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/README_gensim.md` & `MeUtils-2023.8.9.13.5.35/meutils/ann/README_gensim.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/ann.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/ann_faiss.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/ann_gensim.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/ann_inmemory.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/ann_inmemory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/ann_service.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/ann_v1.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/cli.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/examples/client.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/examples/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/ann/shake_demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/ann/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/cache_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/cache_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     """
     https://zhuanlan.zhihu.com/p/356447502
     https://grantjenks.com/docs/diskcache/
 
     """
     from diskcache import Cache, FanoutCache
 
-    cache = Cache(directory=location)
+    cache = FanoutCache(directory=location)
 
     raw_key = dict(filter_args(func, [], list(args), kwargs))
     raw_key = {**raw_key.pop('**', {}), **raw_key, '__tag__': tag or func.__name__}
 
     # self cls 看场景选择
     ignore = (ignore or []) + [
         'api_base', 'api_key', 'openai_api_base', 'openai_api_key',
@@ -149,29 +149,26 @@
     ]
 
     for arg in ignore:
         raw_key.pop(arg, None)
 
     key = hashing.hash(raw_key)
 
-    _ = cache.get(key, '__NO__')
+    _ = cache.get(key, '__NO__', retry=True)
     if isinstance(_, str) and _ == '__NO__':
         _ = func(*args, **kwargs)
-        if inspect.isgenerator(_):
-            _ = list(_)
-            cache.set(f"{key}_isgenerator", True, expire=ttl)
 
         cache.set(key, _, expire=ttl)  # 异步写入
 
         if verbose:
             from loguru import logger
             logger = logger.patch(lambda r: r.update(name=func.__name__))
             logger.info(f"{cache.directory}: `CacheKey: {raw_key if verbose != 1 else key}`")
 
-    return _ if not cache.get(f"{key}_isgenerator") else iter(_)
+    return _
 
 
 @decorator
 def disk_cache(func, location='cachedir', maxsize=128, ttl=np.inf, verbose=True, *args, **kwargs):
     ttl_cache = TTLCache(maxsize, ttl)  # 单例
 
     k = md5(f"cache_{func.__name__}_{args}_{kwargs}")  # uuid
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/clis/cli.py` & `MeUtils-2023.8.9.13.5.35/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/clis/conf.py` & `MeUtils-2023.8.9.13.5.35/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/clis/cron.py` & `MeUtils-2023.8.9.13.5.35/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/clis/demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/clis/gunicorn.conf.py` & `MeUtils-2023.8.9.13.5.35/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/clis/monitor.py` & `MeUtils-2023.8.9.13.5.35/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/clis/nesc.py` & `MeUtils-2023.8.9.13.5.35/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/clis/server.py` & `MeUtils-2023.8.9.13.5.35/meutils/clis/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @cli.command()  # help会覆盖docstring
 def celery_consumer(host='0.0.0.0', port: int = 8501):
     """
     # 消费者
     celery -A meutils.serving.celery.tasks worker -l info
 
     # 生产者
-    mecli-server celery-consumer --host 127.0.0.1 --port 8000
+    mecli-server --host 127.0.0.1 --port 8000
 
     """
 
     from meutils.serving.fastapi import App
     from meutils.serving.celery.router import router
 
     app = App()
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/cmds/README.md` & `MeUtils-2023.8.9.13.5.35/meutils/cmds/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/cmds/hdfs_cmd.py` & `MeUtils-2023.8.9.13.5.35/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/cmds/subprocess_demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/coding/find132.py` & `MeUtils-2023.8.9.13.5.35/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/common.py` & `MeUtils-2023.8.9.13.5.35/meutils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/comp_utils/reverse_metric.py` & `MeUtils-2023.8.9.13.5.35/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/data/SimHei.ttf` & `MeUtils-2023.8.9.13.5.35/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/data/coordinate.py` & `MeUtils-2023.8.9.13.5.35/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/date_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/db/README.md` & `MeUtils-2023.8.9.13.5.35/meutils/db/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/db/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/db/mongo.py` & `MeUtils-2023.8.9.13.5.35/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/db/neo4j.py` & `MeUtils-2023.8.9.13.5.35/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/__ai.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/__ai.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/catch.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/common.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
 @decorator
 def background_task(func, max_workers=1, *args, **kwargs):
     # pool.shutdown(wait=False)  # 不等待
     # pool.shutdown(wait=True)  # 等待
     pool = ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix='🐶')
     future = pool.submit(func, *args, **kwargs)  # pool.map(fun4, ips)
     future.add_done_callback(lambda x: logger.error(future.exception()) if future.exception() else None)
+    # 详细错误 traceback.format_exc()
     return future.running()  # future.done()
 
 
 background = background_task
 
 
 # @backend
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/decorator.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/decorator_demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/feishu.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/retry.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/decorators/scheduler.py` & `MeUtils-2023.8.9.13.5.35/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/dist_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/demo_es.py` & `MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/demo_es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/demo_hnsw.py` & `MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/demo_hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/in_memory.py` & `MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/in_memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/docarray_utils/改造下hnsw.py` & `MeUtils-2023.8.9.13.5.35/meutils/docarray_utils/改造下hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/easy_search/es.py` & `MeUtils-2023.8.9.13.5.35/meutils/easy_search/es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/PDF抽取.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/PDF抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/common.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/__main__.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/__main__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/filetype.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/filetype.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/helpers.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/helpers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/match.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/archive.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/archive.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/audio.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/base.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/document.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/font.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/font.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/image.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/isobmff.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/isobmff.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/types/video.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/types/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/filetype/utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/filetype/utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/fileparser/表格抽取.py` & `MeUtils-2023.8.9.13.5.35/meutils/fileparser/表格抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/hash_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/import_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/init/evn.py` & `MeUtils-2023.8.9.13.5.35/meutils/init/evn.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 os.environ['PROMPT_TEMPLATE'] = """
 {role}
 根据以下信息，简洁、专业地回答用户的问题。如果无法得到答案，请回复：“根据已知信息无法回答该问题”或“没有提供足够的信息”。请勿编造信息，答案必须使用中文。
 已知信息：
 {context}
 问题：
 {question}
-""".strip()
+""".strip() # Let's think step by step
+
+
 # """
 # {role}
 # 请根据以下<>中的信息简洁、专业地回答问题。
 # 信息：<{context}>
 # 问题：{question}
 # 如果无法从中得到答案，请回答“根据已知信息无法回答该问题”或“没有提供足够的信息”。请使用中文回答，不允许添加编造内容。
 # """
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/init/oo.py` & `MeUtils-2023.8.9.13.5.35/meutils/init/oo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/io/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/io/image.py` & `MeUtils-2023.8.9.13.5.35/meutils/io/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/io/tf_io.py` & `MeUtils-2023.8.9.13.5.35/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/jinja_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/log_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/log_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     )
 
 else:
     logger.remove()
     logger.add(sys.stderr, enqueue=True)
 
 
+
 # 日志采样输出：按时间 按条数
 def logger4sample(log, bins=10):
     if uniform(0, bins) < 1:
         logger.info(log)
 
 
 # todo: 起个服务配置通用logger
@@ -65,14 +66,16 @@
     return Wecom(hook_url).send_markdown(title=str(title), content=str(text))
 
 
 # todo:
 #  add zk/es/mongo/hdfs logger
 # logger = logger.patch(lambda r: r.update(name=__file__))
 logger_patch = lambda name: logger.patch(lambda r: r.update(name=name))  # main模块: 等价于 __name__=__file__
+# file_name, line, function, _, _ = inspect.getframeinfo(inspect.currentframe().f_back)
+# logger = logger.patch(lambda r: r.update(name='func_test', function=function, line=line))
 
 if __name__ == '__main__':
     logger.info("xx")
     # logger4feishu('', 'a\nb')
     logger4wecom()
 
     # 异步sink
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/notice/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/notice/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/notice/emails.py` & `MeUtils-2023.8.9.13.5.35/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/notice/feishu.py` & `MeUtils-2023.8.9.13.5.35/meutils/notice/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/notice/file_post.py` & `MeUtils-2023.8.9.13.5.35/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/notice/wechat.py` & `MeUtils-2023.8.9.13.5.35/meutils/notice/wechat.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/notice/wechat_.py` & `MeUtils-2023.8.9.13.5.35/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/notice/wecom.py` & `MeUtils-2023.8.9.13.5.35/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/notice/weekmeet.py` & `MeUtils-2023.8.9.13.5.35/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/np_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/np_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 l=[[1,2,3],[4,[5],[6,7]],[8,[9,[10]]]]*1000
 from iteration_utilities import deepflatten
 _ = list(deepflatten(l)) # 快十倍
 _ = sum(l, [])
 """
 
 
-def normalize(x):
-    if len(x.shape) > 1:
-        return x / np.clip(x ** 2, 1e-12, None).sum(axis=1).reshape((-1, 1) + x.shape[2:]) ** 0.5
-    else:
-        return x / np.clip(x ** 2, 1e-12, None).sum() ** 0.5
+# def normalize(x):
+#     if len(x.shape) > 1:
+#         return x / np.clip(x ** 2, 1e-12, None).sum(axis=1).reshape((-1, 1) + x.shape[2:]) ** 0.5
+#     else:
+#         return x / np.clip(x ** 2, 1e-12, None).sum() ** 0.5
+def normalize(v):
+    """性能提升2.5倍"""
+    return v / np.linalg.norm(np.atleast_2d(v), axis=1, keepdims=True)
 
 
 def cosine(v1, v2):  # 相似度不是距离
     """
     v1 = np.array([[1, 2], [3, 4]])
     v2 = np.array([[5, 6], [7, 8], [5, 6]])
     cosine_dist(v1, v2)
@@ -52,14 +55,34 @@
 def cosine_topk(v1, v2, topk=10):  # 相似度不是距离
     dist = - cosine(v1, v2)
     idxs = np.argsort(dist)[:, :topk]
     scores = - np.take_along_axis(dist, idxs, -1)  # 取出得分
     return idxs[0], scores[0]
 
 
+def cosine_similarity(v1, v2):
+    """先归一化再点乘，比from sklearn.metrics.pairwise import cosine_similarity 快10倍"""
+    v1, v2 = map(lambda v: v / np.linalg.norm(np.atleast_2d(v), axis=1, keepdims=True), [v1, v2])
+    return v1 @ v2.T
+
+
+def similarity_search_by_vector(v1, v2, topk=10):
+    """
+
+    :param v1:
+    :param v2:
+    :param topk:
+    :return: idxs, scores
+    """
+    dist = - cosine_similarity(v1, v2)
+    idxs = np.argsort(dist)[:, :topk]
+    scores = - np.take_along_axis(dist, idxs, -1)  # 取出得分
+    return idxs, scores
+
+
 def cooccurrence_matrix(texts, window_size=2):
     """
     构建共现矩阵
     :param texts: 文本列表
     :param window_size: 单词之间的最大距离
     :return: 共现矩阵
 
@@ -98,8 +121,10 @@
 if __name__ == "__main__":
     import time
     from sklearn.metrics.pairwise import cosine_similarity
 
     x = np.random.rand(10, 128)
     y = np.random.rand(1000000, 128)
     idxs, scores = cosine_topk(x[:1], x)
-    print(idxs[0])
+    print(idxs)
+
+    print(similarity_search_by_vector(x, y, 3)[0])
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/office_automation/pdf.py` & `MeUtils-2023.8.9.13.5.35/meutils/office_automation/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/office_automation/pdm.py` & `MeUtils-2023.8.9.13.5.35/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/office_automation/pdm_run.py` & `MeUtils-2023.8.9.13.5.35/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/office_automation/投资管理系统O3.2_交易组.pdm` & `MeUtils-2023.8.9.13.5.35/meutils/office_automation/投资管理系统O3.2_交易组.pdm`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/__demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/__demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/core.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/core.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/pool.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/pool.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/scheduler.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/aiomultiprocess/types.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/aiomultiprocess/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/besttable.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/crontab.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/annlite.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/annlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/base.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/chunk.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/chunk.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/document.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/elastic.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/elastic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/match.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/memory.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/milvus.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/milvus.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/content.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/dataloader/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/dataloader/helper.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/dataloader/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/delitem.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/delitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/embed.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/embed.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/empty.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/empty.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/evaluation.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/getattr.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/getattr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/getitem.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/getitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/group.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/group.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/binary.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/binary.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/common.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/csv.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/csv.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/dataframe.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/from_gen.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/from_gen.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/json.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/json.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/pbar.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/pbar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/io/pushpull.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/io/pushpull.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/match.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/parallel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/parallel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/plot.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/post.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/pydantic.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/reduce.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/reduce.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/sample.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/sample.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/setitem.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/setitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/strawberry.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/text.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/mixins/traverse.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/mixins/traverse.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/opensearch.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/opensearch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/qdrant.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/qdrant.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/queryset/lookup.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/queryset/lookup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/queryset/parser.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/queryset/parser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/redis.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/redis.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/sqlite.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/sqlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/helper.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/annlite/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/annlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/helper.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/base/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/base/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/elastic/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/elastic/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/memory/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/memory/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/milvus/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/milvus/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/opensearch/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/opensearch/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/qdrant/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/qdrant/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/redis/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/redis/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/helper.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/sqlite/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/sqlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/backend.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/find.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/getsetdel.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/storage/weaviate/seqlike.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/storage/weaviate/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/array/weaviate.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/array/weaviate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/base.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/enums.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/enums.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/getter.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/getter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/setter.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/setter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/dataclasses/types.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/data.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/generators.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/generators.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/_property.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/_property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/attribute.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/attribute.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/audio.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/blob.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/blob.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/content.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/convert.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/dump.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/dump.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/featurehash.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/featurehash.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/helper.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,7 +77,9 @@
         or os.access(os.path.dirname(value), os.W_OK)
     )
 
 
 def _is_datauri(value: str) -> bool:
     scheme = urllib.parse.urlparse(value).scheme
     return scheme in {'data'}
+
+
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/image.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/mesh.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/multimodal.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/multimodal.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/plot.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/porting.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/porting.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/property.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/protobuf.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/protobuf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/pydantic.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/rich_embedding.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/rich_embedding.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/strawberry.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/sugar.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/sugar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/text.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/mixins/video.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/mixins/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/pydantic_model.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/document/strawberry_type.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/document/strawberry_type.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/helper.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/numpy.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/numpy.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/paddle.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/paddle.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/tensorflow.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/tensorflow.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/distance/torch.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/distance/torch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/evaluation.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/helper.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/math/ndarray.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/math/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/io/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/io/ndarray.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/io/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/pb/docarray_pb2.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/pb/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/proto/pb2/docarray_pb2.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/proto/pb2/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/resources/ci-vendors.json` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/resources/embedding-projector/index.html.gz` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/resources/embedding-projector/index.html.gz`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/data.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/score/mixins/property.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/score/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/other/docarray/typing/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/other/docarray/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/pandas_utils/opt.py` & `MeUtils-2023.8.9.13.5.35/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/pandas_utils/pd_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/path_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/pd_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/pipe.py` & `MeUtils-2023.8.9.13.5.35/meutils/pipe.py`

 * *Files 7% similar despite different names*

```diff
@@ -243,29 +243,29 @@
 
         with ThreadPoolExecutor(max_workers) as pool, tqdm(total=total, desc=desc, unit=unit) as pbar:
             for i in pool.map(func, iterable):
                 yield i
                 pbar.update()
 
     else:
-        return map(func, iterable)
+        yield from map(func, iterable)
 
 
 @Pipe
 def xProcessPoolExecutor(iterable, func, max_workers=5, desc="Processing", unit="it"):
     if max_workers > 1:
         total = len(iterable) if hasattr(iterable, '__len__') else None
 
         with ProcessPoolExecutor(max_workers) as pool, tqdm(total=total, desc=desc, unit=unit) as pbar:
             for i in pool.map(func, iterable):
                 yield i
                 pbar.update()
 
     else:
-        return map(func, iterable)
+        yield from map(func, iterable)
 
 
 # 异步
 @Pipe
 def xAsyncio(tasks, return_exceptions=False):
     """为了从异步方式获益，一个应用程序需要有经常被 I/O 阻塞的任务，并且没有太多 CPU 工作。Web 应用程序通常非常适合，特别是当它们需要处理大量客户端请求时。
         import nest_asyncio
@@ -283,54 +283,61 @@
     """
     loop = asyncio.get_event_loop()
     _ = asyncio.gather(*tasks, return_exceptions=return_exceptions)  # asyncio.wait(tasks)
     return loop.run_until_complete(_)
 
 
 if __name__ == '__main__':
-    @Pipe
-    def xfunc1(x):
-        _ = x.split()
-        print(_)
-        return _
-
-
-    @Pipe
-    def xfunc2(x):
-        _ = '>>'.join(x)
-        print(_)
-        return _
-
-
-    def wrapper(func):
-        @functools.wraps(func)
-        def wrapped(*args, **kwargs):
-            logger.patch(lambda r: r.update(name='__file__', function=func.__name__)).info("Wrapped!")
-            return func(*args, **kwargs)
-
-        return wrapped
-
-
-    # log = 'I am very like a linux pipe' | xfunc1 | xfunc2
-    # logger.info(log)
+    # @Pipe
+    # def xfunc1(x):
+    #     _ = x.split()
+    #     print(_)
+    #     return _
+    #
+    #
+    # @Pipe
+    # def xfunc2(x):
+    #     _ = '>>'.join(x)
+    #     print(_)
+    #     return _
+    #
+    #
+    # def wrapper(func):
+    #     @functools.wraps(func)
+    #     def wrapped(*args, **kwargs):
+    #         logger.patch(lambda r: r.update(name='__file__', function=func.__name__)).info("Wrapped!")
+    #         return func(*args, **kwargs)
     #
-    # logger = logger.patch(lambda r: r.update(name=__file__, function=''))  # main:module
-    # logger.info(log)
+    #     return wrapped
     #
-    # # logger = logger.patch(wrapper(lambda x: ''))
+    #
+    # # log = 'I am very like a linux pipe' | xfunc1 | xfunc2
     # # logger.info(log)
+    # #
+    # # logger = logger.patch(lambda r: r.update(name=__file__, function=''))  # main:module
+    # # logger.info(log)
+    # #
+    # # # logger = logger.patch(wrapper(lambda x: ''))
+    # # # logger.info(log)
+    #
+    # ['aaaa', 'vvvvv'] | xprint
+    #
+    #
+    #
+    # def single(a):
+    #     """ 定义一个简单的函数  """
+    #     time.sleep(1)
+    #
+    #
+    # with timer('并行'):
+    #     range(10) | xJobs(single)
 
-    ['aaaa', 'vvvvv'] | xprint
-
-
-    def single(a):
-        """ 定义一个简单的函数  """
-        time.sleep(1)
-
+    # s = pd.DataFrame(range(10), columns=['a']).a
+    # idxs = np.where(s.isin((3, 6)))[0]
+    # ss = pd.cut(dd.a, [-np.inf, *idxs, np.inf])
+    # ss.groupby(ss).groups
 
-    with timer('并行'):
-        range(10) | xJobs(single)
+    # print(range(10) | xThreadPoolExecutor(print, 1) | xlist)
+    # print(range(10) | xThreadPoolExecutor(print, 2) | xlist)
 
-# s = pd.DataFrame(range(10), columns=['a']).a
-# idxs = np.where(s.isin((3, 6)))[0]
-# ss = pd.cut(dd.a, [-np.inf, *idxs, np.inf])
-# ss.groupby(ss).groups
+    print(range(10) | xProcessPoolExecutor(print, 1) | xlist)
+    print(range(10) | xProcessPoolExecutor(print, 2) | xlist)
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/plot_utils/demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/plot_utils/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/plot_utils/echarts.py` & `MeUtils-2023.8.9.13.5.35/meutils/plot_utils/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/plot_utils/embedding_plot.py` & `MeUtils-2023.8.9.13.5.35/meutils/plot_utils/embedding_plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/plot_utils/mecharts.py` & `MeUtils-2023.8.9.13.5.35/meutils/plot_utils/mecharts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/plot_utils/metrics.py` & `MeUtils-2023.8.9.13.5.35/meutils/plot_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/plot_utils/plot_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/plot_utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/queues/common.py` & `MeUtils-2023.8.9.13.5.35/meutils/queues/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/request_utils/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/request_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/request_utils/crawler.py` & `MeUtils-2023.8.9.13.5.35/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/request_utils/download.py` & `MeUtils-2023.8.9.13.5.35/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/request_utils/results.py` & `MeUtils-2023.8.9.13.5.35/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/request_utils/公网ip.py` & `MeUtils-2023.8.9.13.5.35/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/_fastapi.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/_fastapi.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/celery/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/celery/_conf.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/celery/_conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/celery/_demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/celery/_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/celery/router.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/celery/router.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/celery/tasks.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/celery/tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     backend=CELERY_BACKEND,
 )
 
 app.conf.update(
     result_expires=30 * 24 * 60 * 60,
     enable_utc=False,
     timezone='Asia/Shanghai',
+    task_track_started=True,
 )
 
 
 # app.config_from_envvar
 # app.config_from_cmdline
 
 @shared_task()
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/__demo/异步任务.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/__demo/异步任务.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/common.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/fastapi/errors/validation_error.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/fastapi/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/gui/bar.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/gui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/gui/demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/gui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/client.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/flow.svg` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/flow.svg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/s.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/s.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/s2.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/s2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/server.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/server.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/__demo/test.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/__demo/test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/SentenceEncoder.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/SentenceEncoder.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/SentenceEncoder_.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/SentenceEncoder_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/executors/base.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/executors/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/jina/nlp_serving/word_segmentation.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/jina/nlp_serving/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/st_utils/_test.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/st_utils/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/st_utils/common.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/st_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/webui/.streamlit/_config.toml` & `MeUtils-2023.8.9.13.5.35/meutils/serving/webui/.streamlit/_config.toml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/webui/_2_词性标注与实体识别.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/webui/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/webui/pages/_1_分词.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/webui/pages/_1_分词.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/webui/pages/_2_词性标注与实体识别.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/webui/pages/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/serving/webui/pages/_3_文本匹配.py` & `MeUtils-2023.8.9.13.5.35/meutils/serving/webui/pages/_3_文本匹配.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/sftp.py` & `MeUtils-2023.8.9.13.5.35/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/sk_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/smooth_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/spark/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/str_utils/Translator.py` & `MeUtils-2023.8.9.13.5.35/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/str_utils/__init__.py` & `MeUtils-2023.8.9.13.5.35/meutils/str_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/str_utils/__translater/tencent.py` & `MeUtils-2023.8.9.13.5.35/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/str_utils/__translater/translater.py` & `MeUtils-2023.8.9.13.5.35/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/str_utils/__translater/youdao.py` & `MeUtils-2023.8.9.13.5.35/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/str_utils/json_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/str_utils/regular_expression.py` & `MeUtils-2023.8.9.13.5.35/meutils/str_utils/regular_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,7 +27,8 @@
 
     # 使用re.finditer匹配文本并返回匹配对象迭代器
     matches = regex.finditer(text)
 
     # 遍历匹配对象迭代器，输出匹配项及其在文本中的位置
     for match in matches:  # 大数据
         yield match.start(), match.end(), match.group()
+
```

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/demo.j2` & `MeUtils-2023.8.9.13.5.35/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/demo.py` & `MeUtils-2023.8.9.13.5.35/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/demox.py` & `MeUtils-2023.8.9.13.5.35/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/df_html.j2` & `MeUtils-2023.8.9.13.5.35/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2023.8.9.13.5.35/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/hegui.py` & `MeUtils-2023.8.9.13.5.35/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/markmap.html` & `MeUtils-2023.8.9.13.5.35/meutils/templates/markmap.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2023.8.9.13.5.35/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/tpl.docx` & `MeUtils-2023.8.9.13.5.35/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/x.html` & `MeUtils-2023.8.9.13.5.35/meutils/templates/x.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/templates/合规日报模板.docx` & `MeUtils-2023.8.9.13.5.35/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/todo.py` & `MeUtils-2023.8.9.13.5.35/meutils/todo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/tools/cprint.py` & `MeUtils-2023.8.9.13.5.35/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/tools/machine_monitor.py` & `MeUtils-2023.8.9.13.5.35/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/tools/monitor.yml` & `MeUtils-2023.8.9.13.5.35/meutils/tools/monitor.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/tools/seize.py` & `MeUtils-2023.8.9.13.5.35/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/tools/service_monitor.py` & `MeUtils-2023.8.9.13.5.35/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/meutils/zk_utils.py` & `MeUtils-2023.8.9.13.5.35/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/pypi.sh` & `MeUtils-2023.8.9.13.5.35/pypi.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.8.4.15.10.43/setup.py` & `MeUtils-2023.8.9.13.5.35/setup.py`

 * *Files identical despite different names*

