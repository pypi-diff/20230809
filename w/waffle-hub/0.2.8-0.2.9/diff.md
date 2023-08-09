# Comparing `tmp/waffle_hub-0.2.8.tar.gz` & `tmp/waffle_hub-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.8.tar", last modified: Mon Jul 24 12:49:30 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.9.tar", last modified: Thu Jul 27 02:16:50 2023, max compression
```

## Comparing `waffle_hub-0.2.8.tar` & `waffle_hub-0.2.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/
--rw-r--r--   0 lhj       (1001) lhj       (1001)    35149 2023-04-27 00:49:27.000000 waffle_hub-0.2.8/LICENSE
--rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-04-27 00:49:27.000000 waffle_hub-0.2.8/MANIFEST.in
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/PKG-INFO
--rw-r--r--   0 lhj       (1001) lhj       (1001)     3314 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/README.md
--rw-r--r--   0 lhj       (1001) lhj       (1001)      386 2023-07-24 11:38:49.000000 waffle_hub-0.2.8/requirements.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)       38 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/setup.cfg
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2935 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/setup.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/tests/
--rw-r--r--   0 lhj       (1001) lhj       (1001)     8814 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/tests/test_cli.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    20016 2023-07-24 12:49:23.000000 waffle_hub-0.2.8/tests/test_dataset.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4581 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/tests/test_ddp.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    12951 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/tests/test_hub.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2292 2023-07-24 12:49:23.000000 waffle_hub-0.2.8/waffle_hub/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/dataset/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       53 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/dataset/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/dataset/adapter/
--rw-r--r--   0 lhj       (1001) lhj       (1001)      419 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     7146 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/autocare_dlt.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     6516 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/coco.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     9006 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/transformers.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    14273 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/adapter/yolo.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      633 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/dataset/cli.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    57191 2023-07-24 12:49:23.000000 waffle_hub-0.2.8/waffle_hub/dataset/dataset.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/experimental/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/experimental/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/experimental/auto_label/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/experimental/auto_label/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     8261 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2986 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/experimental/serve.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/hub/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       39 2023-07-18 04:05:20.000000 waffle_hub-0.2.8/waffle_hub/hub/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub/hub/adapter/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/__init__.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       75 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    10199 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4515 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/config.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/
--rw-r--r--   0 lhj       (1001) lhj       (1001)      129 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1913 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     5446 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       77 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2220 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/config.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     9156 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/train_input_helper.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    10543 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/transformers_hub.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/
--rw-r--r--   0 lhj       (1001) lhj       (1001)       74 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     6999 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/config.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    13208 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      585 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/cli.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    57365 2023-07-23 12:16:26.000000 waffle_hub-0.2.8/waffle_hub/hub/hub.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/hub/model/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:27.000000 waffle_hub-0.2.8/waffle_hub/hub/model/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    13900 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/hub/model/wrapper.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/schema/
--rw-r--r--   0 lhj       (1001) lhj       (1001)      345 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/schema/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1236 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/base_schema.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1745 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/waffle_hub/schema/configs.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      954 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/waffle_hub/schema/data.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      378 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/evaluate.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/schema/fields/
--rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-04-27 00:49:50.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)    17259 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/annotation.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1722 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/base_field.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     7283 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/category.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     3137 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/fields/image.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      537 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/schema/result.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.468909 waffle_hub-0.2.8/waffle_hub/utils/
--rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-04-27 00:49:27.000000 waffle_hub-0.2.8/waffle_hub/utils/__init__.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     3462 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/base_cli.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     3694 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/callback.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     1686 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/conversion.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     8726 2023-07-18 01:37:59.000000 waffle_hub-0.2.8/waffle_hub/utils/data.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4200 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/draw.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4420 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/evaluate.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)     6049 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/metric_logger.py
--rw-r--r--   0 lhj       (1001) lhj       (1001)      631 2023-07-17 11:13:03.000000 waffle_hub-0.2.8/waffle_hub/utils/process.py
-drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-24 12:49:30.464908 waffle_hub-0.2.8/waffle_hub.egg-info/
--rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/PKG-INFO
--rw-r--r--   0 lhj       (1001) lhj       (1001)     2276 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/SOURCES.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)        1 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/dependency_links.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)      224 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/entry_points.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)      308 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/requires.txt
--rw-r--r--   0 lhj       (1001) lhj       (1001)       11 2023-07-24 12:49:30.000000 waffle_hub-0.2.8/waffle_hub.egg-info/top_level.txt
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    35149 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/LICENSE
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/MANIFEST.in
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/PKG-INFO
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3314 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/README.md
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      386 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/requirements.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       38 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/setup.cfg
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2935 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/setup.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.064741 waffle_hub-0.2.9/tests/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8814 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/tests/test_cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    20016 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/tests/test_dataset.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4581 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/tests/test_ddp.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    12951 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/tests/test_hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2292 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/dataset/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       53 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/dataset/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/dataset/adapter/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      419 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/dataset/adapter/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     7146 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/dataset/adapter/autocare_dlt.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6516 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/dataset/adapter/coco.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     9006 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/dataset/adapter/transformers.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    14317 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/dataset/adapter/yolo.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      759 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/dataset/cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    57127 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/dataset/dataset.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/experimental/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/experimental/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/experimental/auto_label/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/experimental/auto_label/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8261 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2986 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/experimental/serve.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/hub/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       39 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/hub/adapter/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/__init__.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       75 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    10199 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4515 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/config.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/configs/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      129 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1913 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     5446 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/hub/adapter/transformers/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       77 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/transformers/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2220 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/transformers/config.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     9156 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/transformers/train_input_helper.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    10543 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/transformers/transformers_hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/hub/adapter/ultralytics/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       74 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6999 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    13208 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      707 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    57365 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/hub.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/hub/model/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/model/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    13900 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/hub/model/wrapper.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/schema/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      345 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1236 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/base_schema.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1745 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/configs.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      954 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/data.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      378 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/evaluate.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/schema/fields/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      138 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/fields/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)    17259 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/fields/annotation.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1722 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/fields/base_field.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     7283 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/fields/category.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3137 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/fields/image.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      537 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/schema/result.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub/utils/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/__init__.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3462 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/base_cli.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     3694 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/callback.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     1686 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/conversion.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     8726 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/data.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4200 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/draw.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4420 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/evaluate.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     6049 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/metric_logger.py
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      631 2023-07-27 02:07:11.000000 waffle_hub-0.2.9/waffle_hub/utils/process.py
+drwxr-xr-x   0 lhj       (1001) lhj       (1001)        0 2023-07-27 02:16:50.068741 waffle_hub-0.2.9/waffle_hub.egg-info/
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     4395 2023-07-27 02:16:50.000000 waffle_hub-0.2.9/waffle_hub.egg-info/PKG-INFO
+-rw-r--r--   0 lhj       (1001) lhj       (1001)     2276 2023-07-27 02:16:50.000000 waffle_hub-0.2.9/waffle_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)        1 2023-07-27 02:16:50.000000 waffle_hub-0.2.9/waffle_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      224 2023-07-27 02:16:50.000000 waffle_hub-0.2.9/waffle_hub.egg-info/entry_points.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)      308 2023-07-27 02:16:50.000000 waffle_hub-0.2.9/waffle_hub.egg-info/requires.txt
+-rw-r--r--   0 lhj       (1001) lhj       (1001)       11 2023-07-27 02:16:50.000000 waffle_hub-0.2.9/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.8/LICENSE` & `waffle_hub-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/PKG-INFO` & `waffle_hub-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.2.8
+Version: 0.2.9
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.8 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.9 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.8/README.md` & `waffle_hub-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/setup.py` & `waffle_hub-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/tests/test_cli.py` & `waffle_hub-0.2.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/tests/test_dataset.py` & `waffle_hub-0.2.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/tests/test_ddp.py` & `waffle_hub-0.2.9/tests/test_ddp.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/tests/test_hub.py` & `waffle_hub-0.2.9/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/__init__.py` & `waffle_hub-0.2.9/waffle_hub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 import enum
 from collections import OrderedDict
 
 BACKEND_MAP = OrderedDict(
     {
         "ultralytics": {
```

### Comparing `waffle_hub-0.2.8/waffle_hub/dataset/adapter/autocare_dlt.py` & `waffle_hub-0.2.9/waffle_hub/dataset/adapter/autocare_dlt.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.2.9/waffle_hub/dataset/adapter/coco.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/dataset/adapter/transformers.py` & `waffle_hub-0.2.9/waffle_hub/dataset/adapter/transformers.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.9/waffle_hub/dataset/adapter/yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,18 +303,20 @@
         io.save_json(set_image_ids, self.set_dir / f"{set_name}.json", True)
 
     return True
 
 
 def _parse_od_label(line: str, width: int, height: int):
     """parse label file for od"""
-    category_id, x, y, w, h = map(float, line.split())
+    category_id, cx, cy, w, h = map(float, line.split())
+    x1 = cx - w / 2
+    y1 = cy - h / 2
     return {
         "category_id": int(category_id) + 1,
-        "bbox": [x * width, y * height, w * width, h * height],
+        "bbox": [x1 * width, y1 * height, w * width, h * height],
     }
 
 
 def _parse_seg_label(line: str, width: int, height: int):
     """parse label file for seg"""
     category_id, *segment = map(float, line.split())
     segment[::2] = [int(x * width) for x in segment[::2]]
```

### Comparing `waffle_hub-0.2.8/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.9/waffle_hub/dataset/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import logging
 import os
 import random
 import shutil
+import time
 import warnings
 from collections import Counter, OrderedDict, defaultdict
 from functools import cached_property
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import Union
 
@@ -300,95 +301,95 @@
     @cached_property
     def unlabeled_set_file(self) -> Path:
         return self.set_dir / Dataset.UNLABELED_SET_FILE_NAME
 
     # dataset indexes
     @property
     def image_dict(self) -> dict[int, Image]:
-        if not hasattr(self, "__image_dict"):
+        if not hasattr(self, "_image_dict"):
             self.create_index()
-        return self.__image_dict
+        return self._image_dict
 
     @property
     def unlabeled_image_dict(self) -> dict[int, Image]:
-        if not hasattr(self, "__unlabeled_image_dict"):
+        if not hasattr(self, "_unlabeled_image_dict"):
             self.create_index()
-        return self.__unlabeled_image_dict
+        return self._unlabeled_image_dict
 
     @property
     def annotation_dict(self) -> dict[int, Annotation]:
-        if not hasattr(self, "__annotation_dict"):
+        if not hasattr(self, "_annotation_dict"):
             self.create_index()
-        return self.__annotation_dict
+        return self._annotation_dict
 
     @property
     def prediction_dict(self) -> dict[int, Annotation]:
-        if not hasattr(self, "__prediction_dict"):
+        if not hasattr(self, "_prediction_dict"):
             self.create_index()
-        return self.__prediction_dict
+        return self._prediction_dict
 
     @property
     def category_dict(self) -> dict[int, Category]:
-        if not hasattr(self, "__category_dict"):
+        if not hasattr(self, "_category_dict"):
             self.create_index()
-        return self.__category_dict
+        return self._category_dict
 
     @property
     def image_to_annotations(self) -> dict[int, list[Annotation]]:
-        if not hasattr(self, "__image_to_annotations"):
+        if not hasattr(self, "_image_to_annotations"):
             self.create_index()
-        return self.__image_to_annotations
+        return self._image_to_annotations
 
     @property
     def image_to_predictions(self) -> dict[int, list[Annotation]]:
-        if not hasattr(self, "__image_to_predictions"):
+        if not hasattr(self, "_image_to_predictions"):
             self.create_index()
-        return self.__image_to_predictions
+        return self._image_to_predictions
 
     @property
     def annotation_to_image(self) -> dict[int, Image]:
-        if not hasattr(self, "__annotation_to_image"):
+        if not hasattr(self, "_annotation_to_image"):
             self.create_index()
-        return self.__annotation_to_image
+        return self._annotation_to_image
 
     @property
     def prediction_to_image(self) -> dict[int, Image]:
-        if not hasattr(self, "__prediction_to_image"):
+        if not hasattr(self, "_prediction_to_image"):
             self.create_index()
-        return self.__prediction_to_image
+        return self._prediction_to_image
 
     @property
     def category_to_images(self) -> dict[int, list[Image]]:
-        if not hasattr(self, "__category_to_images"):
+        if not hasattr(self, "_category_to_images"):
             self.create_index()
-        return self.__category_to_images
+        return self._category_to_images
 
     @property
     def category_to_unique_images(self) -> dict[int, list[Image]]:
-        if not hasattr(self, "__category_to_unique_images"):
+        if not hasattr(self, "_category_to_unique_images"):
             self.create_index()
-        return self.__category_to_unique_images
+        return self._category_to_unique_images
 
     @property
     def category_name_to_category(self) -> dict[str, Category]:
-        if not hasattr(self, "__category_name_to_category"):
+        if not hasattr(self, "_category_name_to_category"):
             self.create_index()
-        return self.__category_name_to_category
+        return self._category_name_to_category
 
     @property
     def category_to_annotations(self) -> dict[int, list[Annotation]]:
-        if not hasattr(self, "__category_to_annotations"):
+        if not hasattr(self, "_category_to_annotations"):
             self.create_index()
-        return self.__category_to_annotations
+        return self._category_to_annotations
 
     @property
     def category_to_predictions(self) -> dict[int, list[Annotation]]:
-        if not hasattr(self, "__category_to_predictions"):
+        if not hasattr(self, "_category_to_predictions"):
             self.create_index()
-        return self.__category_to_predictions
+        return self._category_to_predictions
 
     def get_category_names(self) -> list[str]:
         return [category.name for category in self.categories]
 
     # factories
     @classmethod
     def new(
@@ -1238,113 +1239,110 @@
             category_id: len(annotations)
             for category_id, annotations in self.category_to_annotations.items()
         }
         return num_annotations_per_category
 
     def create_index(self):
         """Create index for faster search."""
-        self.__image_dict = OrderedDict()
-        self.__unlabeled_image_dict = OrderedDict()
-        self.__annotation_dict = OrderedDict()
-        self.__prediction_dict = OrderedDict()
-        self.__category_dict = OrderedDict()
-        self.__image_to_annotations = OrderedDict()
-        self.__image_to_predictions = OrderedDict()
-        self.__annotation_to_image = OrderedDict()
-        self.__prediction_to_image = OrderedDict()
-        self.__category_to_images = OrderedDict()
-        self.__category_to_unique_images = OrderedDict()
-        self.__category_name_to_category = OrderedDict()
-        self.__category_to_annotations = OrderedDict()
-        self.__category_to_predictions = OrderedDict()
+        self._image_dict = OrderedDict()
+        self._unlabeled_image_dict = OrderedDict()
+        self._annotation_dict = OrderedDict()
+        self._prediction_dict = OrderedDict()
+        self._category_dict = OrderedDict()
+        self._image_to_annotations = OrderedDict()
+        self._image_to_predictions = OrderedDict()
+        self._annotation_to_image = OrderedDict()
+        self._prediction_to_image = OrderedDict()
+        self._category_to_images = OrderedDict()
+        self._category_to_unique_images = OrderedDict()
+        self._category_name_to_category = OrderedDict()
+        self._category_to_annotations = OrderedDict()
+        self._category_to_predictions = OrderedDict()
 
+        start = time.time()
         logger.info("Creating index for faster search")
 
         for image in self.get_images():
-            self.__image_dict[image.image_id] = image  # image_id: image
-            self.__image_to_annotations[image.image_id] = []
-            self.__image_to_predictions[image.image_id] = []
+            self._image_dict[image.image_id] = image  # image_id: image
+            self._image_to_annotations[image.image_id] = []
+            self._image_to_predictions[image.image_id] = []
 
         for annotation in self.get_annotations():
-            self.__annotation_dict[
-                annotation.annotation_id
-            ] = annotation  # annotation_id: annotation
-            self.__image_to_annotations[annotation.image_id].append(
+            self._annotation_dict[annotation.annotation_id] = annotation  # annotation_id: annotation
+            self._image_to_annotations[annotation.image_id].append(
                 annotation
             )  # image_id: [annotations]
-            self.__annotation_to_image[annotation.annotation_id] = self.__image_dict[
+            self._annotation_to_image[annotation.annotation_id] = self._image_dict[
                 annotation.image_id
             ]  # annotation_id: image
 
         for prediction in self.get_predictions():
-            self.__prediction_dict[
-                prediction.annotation_id
-            ] = prediction  # annotation_id: prediction
-            self.__image_to_predictions[prediction.image_id].append(
+            self._prediction_dict[prediction.annotation_id] = prediction  # annotation_id: prediction
+            self._image_to_predictions[prediction.image_id].append(
                 prediction
             )  # image_id: [predictions]
-            self.__prediction_to_image[prediction.annotation_id] = self.__image_dict[
+            self._prediction_to_image[prediction.annotation_id] = self._image_dict[
                 prediction.image_id
             ]  # prediction_id: image
 
         for category in self.get_categories():
-            self.__category_dict[category.category_id] = category  # category_id: category
-            self.__category_name_to_category[category.name] = category  # category_name: category
-            self.__category_to_unique_images[category.category_id] = []  # category_id: image
-            self.__category_to_images[category.category_id] = set()
-            self.__category_to_annotations[category.category_id] = []
+            self._category_dict[category.category_id] = category  # category_id: category
+            self._category_name_to_category[category.name] = category  # category_name: category
+            self._category_to_unique_images[category.category_id] = []  # category_id: image
+            self._category_to_images[category.category_id] = set()
+            self._category_to_annotations[category.category_id] = []
 
-        for annotation in self.__annotation_dict.values():
+        for annotation in self._annotation_dict.values():
             if self.task == TaskType.TEXT_RECOGNITION:
                 chars = set(annotation.caption)
                 for char in chars:
-                    category_id = self.__category_name_to_category[char].category_id
-                    self.__category_to_annotations[category_id].append(annotation)
-                    self.__category_to_images[category_id].add(
-                        self.__annotation_to_image[annotation.annotation_id]
+                    category_id = self._category_name_to_category[char].category_id
+                    self._category_to_annotations[category_id].append(annotation)
+                    self._category_to_images[category_id].add(
+                        self._annotation_to_image[annotation.annotation_id]
                     )
             else:
-                self.__category_to_annotations[annotation.category_id].append(
+                self._category_to_annotations[annotation.category_id].append(
                     annotation
                 )  # category_id: [annotations]
-                self.__category_to_images[annotation.category_id].add(
-                    self.__annotation_to_image[annotation.annotation_id]
+                self._category_to_images[annotation.category_id].add(
+                    self._annotation_to_image[annotation.annotation_id]
                 )  # category_id: {images}
 
-        for image_id, annotations in self.__image_to_annotations.items():
+        for image_id, annotations in self._image_to_annotations.items():
             if self.task == TaskType.TEXT_RECOGNITION:
                 most_common_category = Counter(
                     sum([list(annotation.caption) for annotation in annotations], [])
                 ).most_common(1)[0][0]
-                most_common_category_id = self.__category_name_to_category[
+                most_common_category_id = self._category_name_to_category[
                     most_common_category
                 ].category_id
-                self.__category_to_unique_images[most_common_category_id].append(
-                    self.__image_dict[image_id]
+                self._category_to_unique_images[most_common_category_id].append(
+                    self._image_dict[image_id]
                 )
             else:
                 most_common_category_id = Counter(
                     [annotation.category_id for annotation in annotations]
                 ).most_common(1)[0][0]
-                self.__category_to_unique_images[most_common_category_id].append(
-                    self.__image_dict[image_id]
+                self._category_to_unique_images[most_common_category_id].append(
+                    self._image_dict[image_id]
                 )
 
-        for category_id, images in self.__category_to_images.items():
-            self.__category_to_images[category_id] = list(images)
+        for category_id, images in self._category_to_images.items():
+            self._category_to_images[category_id] = list(images)
 
-        for prediction in self.__prediction_dict.values():
-            self.__category_to_predictions[prediction.category_id].append(
+        for prediction in self._prediction_dict.values():
+            self._category_to_predictions[prediction.category_id].append(
                 prediction
             )  # category_id: [predictions]
 
         for image in self.get_images(labeled=False):
-            self.__unlabeled_image_dict[image.image_id] = image  # unlabeled_image_id: image
+            self._unlabeled_image_dict[image.image_id] = image  # unlabeled_image_id: image
 
-        logger.info("Creating index done")
+        logger.info(f"Creating index done {time.time() - start:.2f} seconds")
 
     # add
     def add_images(self, images: Union[Image, list[Image]]):
         """Add "Image"s to dataset.
 
         Args:
             images (Union[Image, list[Image]]): list of "Image"s
@@ -1466,15 +1464,15 @@
         if method == SplitMethod.RANDOM:
             random.seed(seed)
 
             train_ids = []
             val_ids = []
             test_ids = []
 
-            for category_id, images in self.__category_to_unique_images.items():
+            for category_id, images in self.category_to_unique_images.items():
                 image_num = len(images)
                 image_ids = list(map(lambda x: x.image_id, images))
                 random.shuffle(image_ids)
 
                 # flatten images to one list [cat]
                 train_num = max(int(image_num * train_ratio), 1)
                 val_num = max(int(image_num * val_ratio), 1)
```

### Comparing `waffle_hub-0.2.8/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.9/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.9/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/config.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/config.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/transformers/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/train_input_helper.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/transformers/train_input_helper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/transformers/transformers_hub.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/transformers/transformers_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/config.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/ultralytics/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.9/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/cli.py` & `waffle_hub-0.2.9/waffle_hub/hub/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import inspect
-
 import fire
+from waffle_utils.log import initialize_logger
 
 from waffle_hub.hub import Hub
 from waffle_hub.utils.base_cli import BaseCLI, cli
 
+initialize_logger("hub.log", root_level="INFO", console_level="INFO", file_level="DEBUG")
+
 
 class HubInstance(BaseCLI):
     def __init__(self, name: str, root_dir: str = None):
         self.hub = None
         if name in Hub.get_hub_list(root_dir):
             self.hub = Hub.load(name, root_dir=root_dir)
         else:
```

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/hub.py` & `waffle_hub-0.2.9/waffle_hub/hub/hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.9/waffle_hub/hub/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.9/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/schema/configs.py` & `waffle_hub-0.2.9/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/schema/data.py` & `waffle_hub-0.2.9/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.9/waffle_hub/schema/fields/annotation.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.9/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.9/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.9/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/schema/result.py` & `waffle_hub-0.2.9/waffle_hub/schema/result.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/utils/base_cli.py` & `waffle_hub-0.2.9/waffle_hub/utils/base_cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/utils/callback.py` & `waffle_hub-0.2.9/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.9/waffle_hub/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/utils/data.py` & `waffle_hub-0.2.9/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/utils/draw.py` & `waffle_hub-0.2.9/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.9/waffle_hub/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/utils/metric_logger.py` & `waffle_hub-0.2.9/waffle_hub/utils/metric_logger.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub/utils/process.py` & `waffle_hub-0.2.9/waffle_hub/utils/process.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.8/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.9/waffle_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.2.8
+Version: 0.2.9
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.8 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.9 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.2.8/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.9/waffle_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

