# Comparing `tmp/kolena_client-0.80.1.tar.gz` & `tmp/kolena_client-0.81.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.80.1.tar", max compression
+gzip compressed data, was "kolena_client-0.81.0.tar", max compression
```

## Comparing `kolena_client-0.80.1.tar` & `kolena_client-0.81.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0    11346 2023-08-04 15:19:56.981036 kolena_client-0.80.1/LICENSE
--rw-r--r--   0        0        0      556 2023-08-04 15:19:56.981036 kolena_client-0.80.1/LICENSE_HEADER
--rw-r--r--   0        0        0     1993 2023-08-04 15:19:56.981036 kolena_client-0.80.1/README.md
--rw-r--r--   0        0        0     1356 2023-08-04 15:28:10.678513 kolena_client-0.80.1/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     5111 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5880 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/classification/__init__.py
--rw-r--r--   0        0        0     9888 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/classification/utils.py
--rw-r--r--   0        0        0     1553 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0     5165 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator.py
--rw-r--r--   0        0        0    18050 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator_multiclass.py
--rw-r--r--   0        0        0    11891 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator_single_class.py
--rw-r--r--   0        0        0    14344 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0     7238 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/object_detection/workflow.py
--rw-r--r--   0        0        0      674 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/search/__init__.py
--rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/search/_internal/__init__.py
--rw-r--r--   0        0        0     1198 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/search/_internal/datatypes.py
--rw-r--r--   0        0        0     3015 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_experimental/search/embeddings.py
--rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      785 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/cli.py
--rw-r--r--   0        0        0      955 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     3337 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     5033 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0     1164 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1272 2023-08-04 15:19:57.081036 kolena_client-0.80.1/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1475 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3512 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3573 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3185 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2694 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2372 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4480 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6013 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_run.py
--rw-r--r--   0        0        0     3180 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1477 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6825 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1928 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1035 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5470 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8995 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    14122 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1201 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     1761 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13804 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     5867 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5435 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/inference.py
--rw-r--r--   0        0        0     1460 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/metadata.py
--rw-r--r--   0        0        0     3210 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/model.py
--rw-r--r--   0        0        0     2387 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3199 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5967 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5405 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2854 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2681 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20984 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/datatypes.py
--rw-r--r--   0        0        0    10274 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/model.py
--rw-r--r--   0        0        0    14952 2023-08-04 15:19:57.085036 kolena_client-0.80.1/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12237 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16943 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/fr/test_run.py
--rw-r--r--   0        0        0    16329 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3880 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/initialize.py
--rw-r--r--   0        0        0     2493 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13948 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6281 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/_validators.py
--rw-r--r--   0        0        0    10397 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     4926 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3469 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    13854 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    11232 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4421 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4334 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/inference.py
--rw-r--r--   0        0        0     1150 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     3931 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/metrics/_formula.py
--rw-r--r--   0        0        0    16014 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     8459 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/model.py
--rw-r--r--   0        0        0    10261 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/plot.py
--rw-r--r--   0        0        0    18319 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    23730 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    11006 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    15455 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0      841 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/visualization/__init__.py
--rw-r--r--   0        0        0     6145 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/visualization/_activation_map.py
--rw-r--r--   0        0        0     1910 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/visualization/_utils.py
--rw-r--r--   0        0        0     9419 2023-08-04 15:19:57.089036 kolena_client-0.80.1/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3032 2023-08-04 15:28:10.678513 kolena_client-0.80.1/pyproject.toml
--rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 kolena_client-0.80.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-08-08 23:55:34.022797 kolena_client-0.81.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-08-08 23:55:34.022797 kolena_client-0.81.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1993 2023-08-08 23:55:34.022797 kolena_client-0.81.0/README.md
+-rw-r--r--   0        0        0     1356 2023-08-09 00:03:06.473553 kolena_client-0.81.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     5111 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5880 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-08-08 23:55:34.114803 kolena_client-0.81.0/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/classification/__init__.py
+-rw-r--r--   0        0        0    13449 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/classification/utils.py
+-rw-r--r--   0        0        0     1553 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0     5165 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/object_detection/evaluator.py
+-rw-r--r--   0        0        0    18050 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/object_detection/evaluator_multiclass.py
+-rw-r--r--   0        0        0    11891 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/object_detection/evaluator_single_class.py
+-rw-r--r--   0        0        0    14344 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0     7238 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/object_detection/workflow.py
+-rw-r--r--   0        0        0      674 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/search/__init__.py
+-rw-r--r--   0        0        0      579 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/search/_internal/__init__.py
+-rw-r--r--   0        0        0     1198 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/search/_internal/datatypes.py
+-rw-r--r--   0        0        0     3015 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_experimental/search/embeddings.py
+-rw-r--r--   0        0        0      579 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      785 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      955 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     3337 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     5033 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0     1164 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6825 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1928 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8995 2023-08-08 23:55:34.118803 kolena_client-0.81.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    14122 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13804 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20984 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10274 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14952 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16329 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3880 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/initialize.py
+-rw-r--r--   0        0        0     2493 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13958 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    11487 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13854 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0     1150 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     3931 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/metrics/_formula.py
+-rw-r--r--   0        0        0    16014 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8459 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10261 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    18319 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    23730 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    11006 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15455 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0      841 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/visualization/__init__.py
+-rw-r--r--   0        0        0     6145 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/visualization/_activation_map.py
+-rw-r--r--   0        0        0     1910 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/visualization/_utils.py
+-rw-r--r--   0        0        0     9419 2023-08-08 23:55:34.122804 kolena_client-0.81.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3032 2023-08-09 00:03:06.473553 kolena_client-0.81.0/pyproject.toml
+-rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 kolena_client-0.81.0/PKG-INFO
```

### Comparing `kolena_client-0.80.1/LICENSE` & `kolena_client-0.81.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/LICENSE_HEADER` & `kolena_client-0.81.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/README.md` & `kolena_client-0.81.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/__init__.py` & `kolena_client-0.81.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/__init__.py` & `kolena_client-0.81.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/__init__.py` & `kolena_client-0.81.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/batched_load.py` & `kolena_client-0.81.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/client_log.py` & `kolena_client-0.81.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/core.py` & `kolena_client-0.81.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/detection.py` & `kolena_client-0.81.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/fr.py` & `kolena_client-0.81.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/generic.py` & `kolena_client-0.81.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/repository.py` & `kolena_client-0.81.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/token.py` & `kolena_client-0.81.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_api/v1/workflow.py` & `kolena_client-0.81.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/__init__.py` & `kolena_client-0.81.0/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/classification/__init__.py` & `kolena_client-0.81.0/kolena/_experimental/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/classification/utils.py` & `kolena_client-0.81.0/kolena/_experimental/classification/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,23 +18,26 @@
 from typing import Tuple
 
 import numpy as np
 
 from kolena._utils import log
 from kolena.workflow.annotation import ClassificationLabel
 from kolena.workflow.annotation import ScoredClassificationLabel
+from kolena.workflow.metrics import f1_score
+from kolena.workflow.metrics import precision
+from kolena.workflow.metrics import recall
 from kolena.workflow.plot import ConfusionMatrix
 from kolena.workflow.plot import Curve
 from kolena.workflow.plot import CurvePlot
 from kolena.workflow.plot import Histogram
 
 
 def get_label_confidence(label: str, inference_labels: List[ScoredClassificationLabel]) -> float:
     """
-    Returns the confidence score of the specified `label`.
+    Returns the confidence score of the specified `label` from a list of confidence scores for each label.
 
     :param label: The label whose confidence score to return.
     :param inference_labels: The list of confidence scores for each label. For `N`-class problem, expected to have
         `N` entries, one for each class.
     :return: The confidence score of the specified `label`. If the `label` doesn't exist in `inference_labels`
         then returns 0.
     """
@@ -200,15 +203,15 @@
 ) -> Optional[CurvePlot]:
     """
     Computes OvR (one-vs-rest) ROC (receiver operating characteristic) curves for each class appears in `ground_truths`
     if not specified.
 
     :param ground_truths: The list of ground truth
         [`ClassificationLabel`][kolena.workflow.annotation.ClassificationLabel]. For binary classification, the negative
-        class is `None`.
+        class can be `None`.
     :param inferences: The list of inference
         [`ScoredClassificationLabel`][kolena.workflow.annotation.ScoredClassificationLabel]. For `N`-class problems,
         each inference is expected to contain `N` entries, one for each class and its associated confidence score.
     :param labels: The labels to plot. If not specified, classes appear in `ground_truths` are used. Use `labels` to
         specify the evaluating classes especially if `ground_truths` only have negative classes.
     :param title: The title of the plot.
     :return: A [`CurvePlot`][kolena.workflow.plot.CurvePlot] if there is any valid `Curve` computed; otherwise, `None`.
@@ -247,7 +250,84 @@
         return CurvePlot(
             title=title,
             x_label="False Positive Rate (FPR)",
             y_label="True Positive Rate (TPR)",
             curves=curves,
         )
     return None
+
+
+def compute_threshold_curves(
+    ground_truths: List[Optional[ClassificationLabel]],
+    inferences: List[ScoredClassificationLabel],
+    thresholds: Optional[List[float]] = None,
+) -> Optional[List[CurvePlot]]:
+    """
+    Computes scores (i.e. [Precision][kolena.workflow.metrics.precision], [Recall][kolena.workflow.metrics.recall]
+    and [F1-score][kolena.workflow.metrics.f1_score]) vs. threshold curves for a **single** class presented in
+    `inferences`.
+
+    Expects `ground_truths` and `inferences` correspond to the same sample for the same given index.
+
+    :param ground_truths: The list of ground truth
+        [`ClassificationLabel`][kolena.workflow.annotation.ClassificationLabel]s. For binary classification, the
+        negative class can be `None`.
+    :param inferences: The list of inference
+        [`ScoredClassificationLabel`][kolena.workflow.annotation.ScoredClassificationLabel]s. The length of `inferences`
+        must match the length of `ground_truths`. The list should only include inferences of a specific class to plot
+        the threshold curves for.
+    :param thresholds: The list of thresholds to plot with. If not specified, all the unique confidence scores are used
+        as thresholds, including evenly spaced thresholds from 0 to 1 with 0.1 step.
+    :return: A list of [`CurvePlot`][kolena.workflow.plot.CurvePlot]s if there is any valid `Curve` computed;
+        otherwise, `None`.
+
+    """
+    if len(ground_truths) != len(inferences):
+        log.warn(f"ground_truths ({len(ground_truths)}) and inferences ({len(inferences)}) differ in length")
+        return None
+
+    if len(ground_truths) == 0 or len(inferences) == 0:
+        log.warn(
+            "insufficient # of samples to compute threshold curves — need at least 1 but received "
+            f"{len(ground_truths)}",
+        )
+        return None
+
+    inference_label_list = list({inf.label for inf in inferences})
+    if len(inference_label_list) > 1:
+        log.warn(
+            f"more than one class passed in as inferences: {inference_label_list} — expecting inferences belonging to "
+            "a single class",
+        )
+        return None
+
+    inference_label = inference_label_list[0]
+    gts = [gt.label == inference_label if gt else False for gt in ground_truths]
+
+    if thresholds is None:
+        unique_scores = list({inf.score for inf in inferences})
+        initial_thresholds = list(np.linspace(0, 1, 11))
+        thresholds = [0.0]
+        for threshold in sorted(set(initial_thresholds + unique_scores)):
+            if abs(threshold - thresholds[-1]) >= 1e-2:
+                thresholds.append(threshold)
+    else:
+        thresholds = sorted(set(thresholds))
+
+    precisions = []
+    recalls = []
+    f1s = []
+    for threshold in thresholds:
+        infs = [inf.score >= threshold for inf in inferences]
+        tp = len([True for gt, inf in zip(gts, infs) if gt and inf])
+        fp = len([True for gt, inf in zip(gts, infs) if not gt and inf])
+        fn = len([True for gt, inf in zip(gts, infs) if gt and not inf])
+
+        precisions.append(precision(tp, fp))
+        recalls.append(recall(tp, fn))
+        f1s.append(f1_score(tp, fp, fn))
+
+    return [
+        Curve(x=thresholds, y=precisions, label="Precision"),
+        Curve(x=thresholds, y=recalls, label="Recall"),
+        Curve(x=thresholds, y=f1s, label="F1"),
+    ]
```

### Comparing `kolena_client-0.80.1/kolena/_experimental/object_detection/__init__.py` & `kolena_client-0.81.0/kolena/_experimental/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator.py` & `kolena_client-0.81.0/kolena/_experimental/object_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator_multiclass.py` & `kolena_client-0.81.0/kolena/_experimental/object_detection/evaluator_multiclass.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/object_detection/evaluator_single_class.py` & `kolena_client-0.81.0/kolena/_experimental/object_detection/evaluator_single_class.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/object_detection/utils.py` & `kolena_client-0.81.0/kolena/_experimental/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/object_detection/workflow.py` & `kolena_client-0.81.0/kolena/_experimental/object_detection/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/search/__init__.py` & `kolena_client-0.81.0/kolena/_experimental/search/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/search/_internal/__init__.py` & `kolena_client-0.81.0/kolena/_experimental/search/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/search/_internal/datatypes.py` & `kolena_client-0.81.0/kolena/_experimental/search/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_experimental/search/embeddings.py` & `kolena_client-0.81.0/kolena/_experimental/search/embeddings.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_extras/__init__.py` & `kolena_client-0.81.0/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_extras/metrics/__init__.py` & `kolena_client-0.81.0/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_extras/metrics/sklearn.py` & `kolena_client-0.81.0/kolena/_extras/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/__init__.py` & `kolena_client-0.81.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.81.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/batched_load.py` & `kolena_client-0.81.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/cli.py` & `kolena_client-0.81.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/consts.py` & `kolena_client-0.81.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.81.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/dataframes/validators.py` & `kolena_client-0.81.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/datatypes.py` & `kolena_client-0.81.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/endpoints.py` & `kolena_client-0.81.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/frozen.py` & `kolena_client-0.81.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/geometry.py` & `kolena_client-0.81.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/inference_validators.py` & `kolena_client-0.81.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/instrumentation.py` & `kolena_client-0.81.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/krequests.py` & `kolena_client-0.81.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/log.py` & `kolena_client-0.81.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/repository.py` & `kolena_client-0.81.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/serde.py` & `kolena_client-0.81.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/serializable.py` & `kolena_client-0.81.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/state.py` & `kolena_client-0.81.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/uninstantiable.py` & `kolena_client-0.81.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/_utils/validators.py` & `kolena_client-0.81.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/__init__.py` & `kolena_client-0.81.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/metadata.py` & `kolena_client-0.81.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/model.py` & `kolena_client-0.81.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/multiclass/__init__.py` & `kolena_client-0.81.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/multiclass/_utils.py` & `kolena_client-0.81.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.81.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/multiclass/test_run.py` & `kolena_client-0.81.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/multiclass/workflow.py` & `kolena_client-0.81.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/test_case.py` & `kolena_client-0.81.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/test_config.py` & `kolena_client-0.81.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/test_image.py` & `kolena_client-0.81.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/test_run.py` & `kolena_client-0.81.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/classification/test_suite.py` & `kolena_client-0.81.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/__init__.py` & `kolena_client-0.81.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_datatypes.py` & `kolena_client-0.81.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/__init__.py` & `kolena_client-0.81.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/datatypes.py` & `kolena_client-0.81.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.81.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/inference.py` & `kolena_client-0.81.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/metadata.py` & `kolena_client-0.81.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/model.py` & `kolena_client-0.81.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/test_case.py` & `kolena_client-0.81.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/test_config.py` & `kolena_client-0.81.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/test_image.py` & `kolena_client-0.81.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/test_run.py` & `kolena_client-0.81.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/_internal/test_suite.py` & `kolena_client-0.81.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/ground_truth.py` & `kolena_client-0.81.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/inference.py` & `kolena_client-0.81.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/metadata.py` & `kolena_client-0.81.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/model.py` & `kolena_client-0.81.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/test_case.py` & `kolena_client-0.81.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/test_config.py` & `kolena_client-0.81.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/test_image.py` & `kolena_client-0.81.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/test_run.py` & `kolena_client-0.81.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/detection/test_suite.py` & `kolena_client-0.81.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/errors.py` & `kolena_client-0.81.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/fr/__init__.py` & `kolena_client-0.81.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/fr/_utils.py` & `kolena_client-0.81.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/fr/datatypes.py` & `kolena_client-0.81.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/fr/model.py` & `kolena_client-0.81.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/fr/test_case.py` & `kolena_client-0.81.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/fr/test_images.py` & `kolena_client-0.81.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/fr/test_run.py` & `kolena_client-0.81.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/fr/test_suite.py` & `kolena_client-0.81.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/initialize.py` & `kolena_client-0.81.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/__init__.py` & `kolena_client-0.81.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/_datatypes.py` & `kolena_client-0.81.0/kolena/workflow/_datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             if attempt_cast and not issubclass(field_type, type(None)):
                 return field_type(field_value)
 
             raise ValueError(
                 f"cast=False, not casting field '{field.name}' to type '{field_type}' with value '{field_value}'",
             )
 
-        items = {f.name: deserialize_field(f, obj_dict.get(f.name, None)) for f in dataclasses.fields(cls)}
+        items = {f.name: deserialize_field(f, obj_dict.get(f.name, None)) for f in dataclasses.fields(cls) if f.init}
         return cls(**items)
 
 
 class DataType(str, Enum):
     @staticmethod
     def _data_category() -> str:
         raise NotImplementedError
```

### Comparing `kolena_client-0.80.1/kolena/workflow/_validators.py` & `kolena_client-0.81.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/annotation.py` & `kolena_client-0.81.0/kolena/workflow/annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 
 For example, when viewing images in the Studio, any annotations (such as lists of
 [`BoundingBox`][kolena.workflow.annotation.BoundingBox] objects) present in the
 [`TestSample`][kolena.workflow.TestSample], [`GroundTruth`][kolena.workflow.GroundTruth],
 [`Inference`][kolena.workflow.Inference], or [`MetricsTestSample`][kolena.workflow.MetricsTestSample] objects are
 rendered on top of the image.
 """
+import dataclasses
 from abc import ABCMeta
+from functools import reduce
 from typing import Dict
 from typing import List
 from typing import Tuple
 
 from pydantic.dataclasses import dataclass
 
 from kolena._utils.validators import ValidatorConfig
@@ -61,26 +63,42 @@
 @dataclass(frozen=True, config=ValidatorConfig)
 class Annotation(TypedDataObject[_AnnotationType], metaclass=ABCMeta):
     """The base class for all annotation types."""
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class BoundingBox(Annotation):
-    """Rectangular bounding box specified with pixel coordinates of the top left and bottom right vertices."""
+    """
+    Rectangular bounding box specified with pixel coordinates of the top left and bottom right vertices.
+
+    The reserved fields `width`, `height`, `area`, and `aspect_ratio` are automatically populated with values derived
+    from the provided coordinates.
+    """
 
     top_left: Tuple[float, float]
-    """The top left vertex (in `(x, y)` image coordinates) of this bounding box."""
+    """The top left vertex (in `(x, y)` pixel coordinates) of this bounding box."""
 
     bottom_right: Tuple[float, float]
-    """The bottom right vertex (in `(x, y)` image coordinates) of this bounding box."""
+    """The bottom right vertex (in `(x, y)` pixel coordinates) of this bounding box."""
+
+    width: float = dataclasses.field(init=False)
+    height: float = dataclasses.field(init=False)
+    area: float = dataclasses.field(init=False)
+    aspect_ratio: float = dataclasses.field(init=False)
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.BOUNDING_BOX
 
+    def __post_init__(self) -> None:
+        object.__setattr__(self, "width", self.bottom_right[0] - self.top_left[0])
+        object.__setattr__(self, "height", self.bottom_right[1] - self.top_left[1])
+        object.__setattr__(self, "area", self.width * self.height)
+        object.__setattr__(self, "aspect_ratio", self.width / self.height if self.height != 0 else 0)
+
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class LabeledBoundingBox(BoundingBox):
     """
     Rectangular bounding box specified with pixel coordinates of the top left and bottom right vertices and a string
     label.
     """
@@ -115,15 +133,15 @@
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Polygon(Annotation):
     """Arbitrary polygon specified by three or more pixel coordinates."""
 
     points: List[Tuple[float, float]]
-    """The sequence of `(x, y)` points comprising the boundary of this polygon."""
+    """The sequence of `(x, y)` pixel coordinates comprising the boundary of this polygon."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.POLYGON
 
     def __post_init__(self) -> None:
         if len(self.points) < 3:
@@ -162,55 +180,62 @@
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Keypoints(Annotation):
     """Array of any number of keypoints specified in pixel coordinates."""
 
     points: List[Tuple[float, float]]
-    """The sequence of discrete `(x, y)` points comprising this keypoints annotation."""
+    """The sequence of discrete `(x, y)` pixel coordinates comprising this keypoints annotation."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.KEYPOINTS
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class Polyline(Annotation):
     """Polyline with any number of vertices specified in pixel coordinates."""
 
     points: List[Tuple[float, float]]
-    """The sequence of connected `(x, y)` points comprising this polyline."""
+    """The sequence of connected `(x, y)` pixel coordinates comprising this polyline."""
 
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.POLYLINE
 
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class BoundingBox3D(Annotation):
     """
     Three-dimensional cuboid bounding box in a right-handed coordinate system.
 
     Specified by `(x, y, z)` coordinates for the `center` of the cuboid, `(x, y, z)` `dimensions`, and a `rotation`
     parameter specifying the degrees of rotation about each axis `(x, y, z)` ranging `[-π, π]`.
+
+    The reserved field `volume` is automatically derived from the provided `dimensions`.
     """
 
     center: Tuple[float, float, float]
     """`(x, y, z)` coordinates specifying the center of the bounding box."""
 
     dimensions: Tuple[float, float, float]
     """`(x, y, z)` measurements specifying the dimensions of the bounding box."""
 
     rotations: Tuple[float, float, float]
     """Rotations in degrees about each `(x, y, z)` axis."""
 
+    volume: float = dataclasses.field(init=False)
+
     @staticmethod
     def _data_type() -> _AnnotationType:
         return _AnnotationType.BOUNDING_BOX_3D
 
+    def __post_init__(self) -> None:
+        object.__setattr__(self, "volume", reduce(lambda a, b: a * b, self.dimensions))
+
 
 @dataclass(frozen=True, config=ValidatorConfig)
 class LabeledBoundingBox3D(BoundingBox3D):
     """[`BoundingBox3D`][kolena.workflow.annotation.BoundingBox3D] with an additional string label."""
 
     label: str
     """The label associated with this 3D bounding box."""
```

### Comparing `kolena_client-0.80.1/kolena/workflow/asset.py` & `kolena_client-0.81.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/define_workflow.py` & `kolena_client-0.81.0/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/evaluator.py` & `kolena_client-0.81.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/evaluator_function.py` & `kolena_client-0.81.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/ground_truth.py` & `kolena_client-0.81.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/inference.py` & `kolena_client-0.81.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/metrics/__init__.py` & `kolena_client-0.81.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/metrics/_formula.py` & `kolena_client-0.81.0/kolena/workflow/metrics/_formula.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.81.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/model.py` & `kolena_client-0.81.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/plot.py` & `kolena_client-0.81.0/kolena/workflow/plot.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/test_case.py` & `kolena_client-0.81.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/test_run.py` & `kolena_client-0.81.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/test_sample.py` & `kolena_client-0.81.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/test_suite.py` & `kolena_client-0.81.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/visualization/__init__.py` & `kolena_client-0.81.0/kolena/workflow/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/visualization/_activation_map.py` & `kolena_client-0.81.0/kolena/workflow/visualization/_activation_map.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/visualization/_utils.py` & `kolena_client-0.81.0/kolena/workflow/visualization/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/kolena/workflow/workflow.py` & `kolena_client-0.81.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.80.1/pyproject.toml` & `kolena_client-0.81.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.80.1"  # version is automatically set to latest git tag during release process
+version = "0.81.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning testing platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena_client-0.80.1/PKG-INFO` & `kolena_client-0.81.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.80.1
+Version: 0.81.0
 Summary: Client for Kolena's machine learning testing platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.80.1 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.81.0 Summary: Client for
 Kolena's machine learning testing platform. Home-page: https://kolena.io
 License: Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena Engineering
 Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

