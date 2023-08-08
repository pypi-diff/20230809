# Comparing `tmp/whatstk-0.6.0.tar.gz` & `tmp/whatstk-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatstk-0.6.0.tar", last modified: Sat Apr  1 19:19:48 2023, max compression
+gzip compressed data, was "whatstk-0.6.1.tar", last modified: Tue Aug  8 23:38:14 2023, max compression
```

## Comparing `whatstk-0.6.0.tar` & `whatstk-0.6.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.618401 whatstk-0.6.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2023-04-01 19:18:11.000000 whatstk-0.6.0/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)      738 2023-04-01 19:18:11.000000 whatstk-0.6.0/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    35148 2023-04-01 19:18:11.000000 whatstk-0.6.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      312 2023-04-01 19:18:11.000000 whatstk-0.6.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5775 2023-04-01 19:19:48.614400 whatstk-0.6.0/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4690 2023-04-01 19:18:11.000000 whatstk-0.6.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      533 2023-04-01 19:18:11.000000 whatstk-0.6.0/SECURITY.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      220 2023-04-01 19:18:11.000000 whatstk-0.6.0/requirements-docs.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2023-04-01 19:18:11.000000 whatstk-0.6.0/requirements-flake.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2023-04-01 19:18:11.000000 whatstk-0.6.0/requirements-test.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2023-04-01 19:18:11.000000 whatstk-0.6.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-01 19:19:48.618401 whatstk-0.6.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2826 2023-04-01 19:18:11.000000 whatstk-0.6.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.602399 whatstk-0.6.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.602399 whatstk-0.6.0/tests/analysis/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/analysis/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9018 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/analysis/test_interventions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2557 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/analysis/test_responses.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.602399 whatstk-0.6.0/tests/graph/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/graph/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/graph/test_figures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/test_chat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      158 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/test_data.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.602399 whatstk-0.6.0/tests/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/utils/test_chat_merge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2870 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/utils/test_gdrive.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.602399 whatstk-0.6.0/tests/whatsapp/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/whatsapp/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2441 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/whatsapp/test_generation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      896 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/whatsapp/test_hformat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3013 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/whatsapp/test_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4120 2023-04-01 19:18:11.000000 whatstk-0.6.0/tests/whatsapp/test_parser.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.606400 whatstk-0.6.0/whatstk/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      453 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6008 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/_chat.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.606400 whatstk-0.6.0/whatstk/analysis/
--rw-rw-r--   0 travis    (2000) travis    (2000)      213 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/analysis/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6070 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/analysis/interventions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4722 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/analysis/responses.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      796 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/data.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.606400 whatstk-0.6.0/whatstk/graph/
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/graph/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9983 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/graph/base.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.606400 whatstk-0.6.0/whatstk/graph/figures/
--rw-rw-r--   0 travis    (2000) travis    (2000)       39 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/graph/figures/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1569 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/graph/figures/boxplot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      805 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/graph/figures/heatmap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2157 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/graph/figures/sankey.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/graph/figures/scatter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/graph/figures/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.606400 whatstk-0.6.0/whatstk/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/scripts/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1666 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/scripts/generate_chats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2468 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/scripts/graph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      952 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/scripts/txt_to_csv.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.610400 whatstk-0.6.0/whatstk/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)       29 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/utils/chat_merge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      211 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/utils/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3895 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/utils/gdrive.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1334 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/utils/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.610400 whatstk-0.6.0/whatstk/whatsapp/
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/whatsapp/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.610400 whatstk-0.6.0/whatstk/whatsapp/assets/
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/whatsapp/assets/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/whatsapp/assets/header_format_support.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     7982 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/whatsapp/auto_header.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8353 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/whatsapp/generation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3880 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/whatsapp/hformat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7479 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/whatsapp/objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11625 2023-04-01 19:18:11.000000 whatstk-0.6.0/whatstk/whatsapp/parser.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-01 19:19:48.614400 whatstk-0.6.0/whatstk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5775 2023-04-01 19:19:48.000000 whatstk-0.6.0/whatstk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1912 2023-04-01 19:19:48.000000 whatstk-0.6.0/whatstk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-01 19:19:48.000000 whatstk-0.6.0/whatstk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      170 2023-04-01 19:19:48.000000 whatstk-0.6.0/whatstk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-01 19:19:48.000000 whatstk-0.6.0/whatstk.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      655 2023-04-01 19:19:48.000000 whatstk-0.6.0/whatstk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2023-04-01 19:19:48.000000 whatstk-0.6.0/whatstk.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.707281 whatstk-0.6.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2023-08-08 23:36:00.000000 whatstk-0.6.1/.coveragerc
+-rw-rw-r--   0 travis    (2000) travis    (2000)      738 2023-08-08 23:36:00.000000 whatstk-0.6.1/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35148 2023-08-08 23:36:00.000000 whatstk-0.6.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      312 2023-08-08 23:36:00.000000 whatstk-0.6.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5775 2023-08-08 23:38:14.707281 whatstk-0.6.1/PKG-INFO
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4690 2023-08-08 23:36:00.000000 whatstk-0.6.1/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      533 2023-08-08 23:36:00.000000 whatstk-0.6.1/SECURITY.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      220 2023-08-08 23:36:00.000000 whatstk-0.6.1/requirements-docs.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      174 2023-08-08 23:36:00.000000 whatstk-0.6.1/requirements-flake.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2023-08-08 23:36:00.000000 whatstk-0.6.1/requirements-test.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2023-08-08 23:36:00.000000 whatstk-0.6.1/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-08-08 23:38:14.707281 whatstk-0.6.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2826 2023-08-08 23:36:00.000000 whatstk-0.6.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.695280 whatstk-0.6.1/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.695280 whatstk-0.6.1/tests/analysis/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/analysis/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9018 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/analysis/test_interventions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2557 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/analysis/test_responses.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.695280 whatstk-0.6.1/tests/graph/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/graph/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/graph/test_figures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/test_chat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      158 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/test_data.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.695280 whatstk-0.6.1/tests/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/utils/test_chat_merge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2870 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/utils/test_gdrive.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.695280 whatstk-0.6.1/tests/whatsapp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/whatsapp/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2441 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/whatsapp/test_generation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      896 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/whatsapp/test_hformat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3013 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/whatsapp/test_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4120 2023-08-08 23:36:00.000000 whatstk-0.6.1/tests/whatsapp/test_parser.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.695280 whatstk-0.6.1/whatstk/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      453 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6008 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/_chat.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.699281 whatstk-0.6.1/whatstk/analysis/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      213 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/analysis/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6070 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/analysis/interventions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4722 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/analysis/responses.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      796 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/data.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.699281 whatstk-0.6.1/whatstk/graph/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/graph/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9983 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/graph/base.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.699281 whatstk-0.6.1/whatstk/graph/figures/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       39 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/graph/figures/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1569 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/graph/figures/boxplot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      805 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/graph/figures/heatmap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2157 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/graph/figures/sankey.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/graph/figures/scatter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      520 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/graph/figures/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.699281 whatstk-0.6.1/whatstk/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       31 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/scripts/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1666 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/scripts/generate_chats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2468 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/scripts/graph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      952 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/scripts/txt_to_csv.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.703281 whatstk-0.6.1/whatstk/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       29 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/utils/chat_merge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      211 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/utils/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3895 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/utils/gdrive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1334 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/utils/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.703281 whatstk-0.6.1/whatstk/whatsapp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/whatsapp/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.703281 whatstk-0.6.1/whatstk/whatsapp/assets/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/whatsapp/assets/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/whatsapp/assets/header_format_support.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7982 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/whatsapp/auto_header.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8353 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/whatsapp/generation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3880 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/whatsapp/hformat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7479 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/whatsapp/objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11625 2023-08-08 23:36:00.000000 whatstk-0.6.1/whatstk/whatsapp/parser.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-08-08 23:38:14.703281 whatstk-0.6.1/whatstk.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5775 2023-08-08 23:38:14.000000 whatstk-0.6.1/whatstk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1912 2023-08-08 23:38:14.000000 whatstk-0.6.1/whatstk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-08-08 23:38:14.000000 whatstk-0.6.1/whatstk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      170 2023-08-08 23:38:14.000000 whatstk-0.6.1/whatstk.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-08-08 23:38:14.000000 whatstk-0.6.1/whatstk.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      654 2023-08-08 23:38:14.000000 whatstk-0.6.1/whatstk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2023-08-08 23:38:14.000000 whatstk-0.6.1/whatstk.egg-info/top_level.txt
```

### Comparing `whatstk-0.6.0/CONTRIBUTING.md` & `whatstk-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/LICENSE` & `whatstk-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/PKG-INFO` & `whatstk-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatstk
-Version: 0.6.0
+Version: 0.6.1
 Summary: Parser and analytics tools for WhatsApp group chats
 Home-page: http://github.com/lucasrodes/whatstk
 Author: Lucas Rodes-Guirao
 License: GPL-v3
 Project-URL: Documentation, https://whatstk.readthedocs.io/en/stable/
 Project-URL: Github, http://github.com/lucasrodes/whatstk
 Project-URL: Bug Tracker, https://github.com/lucasrodes/whatstk/issues
@@ -29,15 +29,15 @@
 <div align="left">
   <img src="https://raw.githubusercontent.com/lucasrodes/whatstk/develop/assets/logo.svg" width="70%">
 </div>
 <h1 align="left" style="border-bottom: none;"> whatstk: analyze WhatsApp chats with python
 </h1>
 <p align="left">
   <a href="#">
-    <img alt="Package version" src="https://img.shields.io/badge/pypi-0.6.0-blue.svg?&color=25D366&logo=whatsapp&">
+    <img alt="Package version" src="https://img.shields.io/badge/pypi-0.6.1-blue.svg?&color=25D366&logo=whatsapp&">
   </a>
 </p>
 <!-- style=for-the-badge -->
 
 <p align="left">
   <a href="https://travis-ci.com/lucasrodes/whatstk">
     <img alt="Build Status" src="https://travis-ci.com/lucasrodes/whatstk.svg?branch=develop">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: whatstk Version: 0.6.0 Summary: Parser and
+Metadata-Version: 2.1 Name: whatstk Version: 0.6.1 Summary: Parser and
 analytics tools for WhatsApp group chats Home-page: http://github.com/
 lucasrodes/whatstk Author: Lucas Rodes-Guirao License: GPL-v3 Project-URL:
 Documentation, https://whatstk.readthedocs.io/en/stable/ Project-URL: Github,
 http://github.com/lucasrodes/whatstk Project-URL: Bug Tracker, https://
 github.com/lucasrodes/whatstk/issues Keywords: whatsapp analysis parser chat
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `whatstk-0.6.0/README.md` & `whatstk-0.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div align="left">
   <img src="https://raw.githubusercontent.com/lucasrodes/whatstk/develop/assets/logo.svg" width="70%">
 </div>
 <h1 align="left" style="border-bottom: none;"> whatstk: analyze WhatsApp chats with python
 </h1>
 <p align="left">
   <a href="#">
-    <img alt="Package version" src="https://img.shields.io/badge/pypi-0.6.0-blue.svg?&color=25D366&logo=whatsapp&">
+    <img alt="Package version" src="https://img.shields.io/badge/pypi-0.6.1-blue.svg?&color=25D366&logo=whatsapp&">
   </a>
 </p>
 <!-- style=for-the-badge -->
 
 <p align="left">
   <a href="https://travis-ci.com/lucasrodes/whatstk">
     <img alt="Build Status" src="https://travis-ci.com/lucasrodes/whatstk.svg?branch=develop">
```

### Comparing `whatstk-0.6.0/SECURITY.md` & `whatstk-0.6.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/setup.py` & `whatstk-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "full": requirements_full,
     "dev": requirements_test + requirements_flake + requirements_docs,
 }
 
 
 setup(
     name='whatstk',
-    version="0.6.0",
+    version="0.6.1",
     description="Parser and analytics tools for WhatsApp group chats",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='http://github.com/lucasrodes/whatstk',
     author='Lucas Rodes-Guirao',
     license='GPL-v3',
     install_requires=requirements,
```

### Comparing `whatstk-0.6.0/tests/analysis/test_interventions.py` & `whatstk-0.6.1/tests/analysis/test_interventions.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/analysis/test_responses.py` & `whatstk-0.6.1/tests/analysis/test_responses.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/graph/test_figures.py` & `whatstk-0.6.1/tests/graph/test_figures.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/test_chat.py` & `whatstk-0.6.1/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/utils/test_chat_merge.py` & `whatstk-0.6.1/tests/utils/test_chat_merge.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/utils/test_gdrive.py` & `whatstk-0.6.1/tests/utils/test_gdrive.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/whatsapp/test_generation.py` & `whatstk-0.6.1/tests/whatsapp/test_generation.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/whatsapp/test_hformat.py` & `whatstk-0.6.1/tests/whatsapp/test_hformat.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/whatsapp/test_objects.py` & `whatstk-0.6.1/tests/whatsapp/test_objects.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/tests/whatsapp/test_parser.py` & `whatstk-0.6.1/tests/whatsapp/test_parser.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/_chat.py` & `whatstk-0.6.1/whatstk/_chat.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/analysis/interventions.py` & `whatstk-0.6.1/whatstk/analysis/interventions.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/analysis/responses.py` & `whatstk-0.6.1/whatstk/analysis/responses.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/data.py` & `whatstk-0.6.1/whatstk/data.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/graph/base.py` & `whatstk-0.6.1/whatstk/graph/base.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/graph/figures/boxplot.py` & `whatstk-0.6.1/whatstk/graph/figures/boxplot.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/graph/figures/heatmap.py` & `whatstk-0.6.1/whatstk/graph/figures/heatmap.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/graph/figures/sankey.py` & `whatstk-0.6.1/whatstk/graph/figures/sankey.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/graph/figures/scatter.py` & `whatstk-0.6.1/whatstk/graph/figures/scatter.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/graph/figures/utils.py` & `whatstk-0.6.1/whatstk/graph/figures/utils.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/scripts/generate_chats.py` & `whatstk-0.6.1/whatstk/scripts/generate_chats.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/scripts/graph.py` & `whatstk-0.6.1/whatstk/scripts/graph.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/scripts/txt_to_csv.py` & `whatstk-0.6.1/whatstk/scripts/txt_to_csv.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/utils/chat_merge.py` & `whatstk-0.6.1/whatstk/utils/chat_merge.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/utils/gdrive.py` & `whatstk-0.6.1/whatstk/utils/gdrive.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/utils/utils.py` & `whatstk-0.6.1/whatstk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/whatsapp/assets/header_format_support.json` & `whatstk-0.6.1/whatstk/whatsapp/assets/header_format_support.json`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/whatsapp/auto_header.py` & `whatstk-0.6.1/whatstk/whatsapp/auto_header.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/whatsapp/generation.py` & `whatstk-0.6.1/whatstk/whatsapp/generation.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/whatsapp/hformat.py` & `whatstk-0.6.1/whatstk/whatsapp/hformat.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/whatsapp/objects.py` & `whatstk-0.6.1/whatstk/whatsapp/objects.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk/whatsapp/parser.py` & `whatstk-0.6.1/whatstk/whatsapp/parser.py`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk.egg-info/PKG-INFO` & `whatstk-0.6.1/whatstk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatstk
-Version: 0.6.0
+Version: 0.6.1
 Summary: Parser and analytics tools for WhatsApp group chats
 Home-page: http://github.com/lucasrodes/whatstk
 Author: Lucas Rodes-Guirao
 License: GPL-v3
 Project-URL: Documentation, https://whatstk.readthedocs.io/en/stable/
 Project-URL: Github, http://github.com/lucasrodes/whatstk
 Project-URL: Bug Tracker, https://github.com/lucasrodes/whatstk/issues
@@ -29,15 +29,15 @@
 <div align="left">
   <img src="https://raw.githubusercontent.com/lucasrodes/whatstk/develop/assets/logo.svg" width="70%">
 </div>
 <h1 align="left" style="border-bottom: none;"> whatstk: analyze WhatsApp chats with python
 </h1>
 <p align="left">
   <a href="#">
-    <img alt="Package version" src="https://img.shields.io/badge/pypi-0.6.0-blue.svg?&color=25D366&logo=whatsapp&">
+    <img alt="Package version" src="https://img.shields.io/badge/pypi-0.6.1-blue.svg?&color=25D366&logo=whatsapp&">
   </a>
 </p>
 <!-- style=for-the-badge -->
 
 <p align="left">
   <a href="https://travis-ci.com/lucasrodes/whatstk">
     <img alt="Build Status" src="https://travis-ci.com/lucasrodes/whatstk.svg?branch=develop">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: whatstk Version: 0.6.0 Summary: Parser and
+Metadata-Version: 2.1 Name: whatstk Version: 0.6.1 Summary: Parser and
 analytics tools for WhatsApp group chats Home-page: http://github.com/
 lucasrodes/whatstk Author: Lucas Rodes-Guirao License: GPL-v3 Project-URL:
 Documentation, https://whatstk.readthedocs.io/en/stable/ Project-URL: Github,
 http://github.com/lucasrodes/whatstk Project-URL: Bug Tracker, https://
 github.com/lucasrodes/whatstk/issues Keywords: whatsapp analysis parser chat
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `whatstk-0.6.0/whatstk.egg-info/SOURCES.txt` & `whatstk-0.6.1/whatstk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whatstk-0.6.0/whatstk.egg-info/requires.txt` & `whatstk-0.6.1/whatstk.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 emoji~=2.2.0
 numpy~=1.24.0
 pandas~=1.5.0
-plotly~=4.14.3
+plotly~=5.0.0
 seaborn~=0.12.0
 
 [dev]
 pytest~=7.2.0
 pytest-cov~=4.0.0
 coverage~=7.2.2
 codecov~=2.1.0
```

