# Comparing `tmp/autogluon.bench-0.2.1.tar.gz` & `tmp/autogluon.bench-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.bench-0.2.1.tar", last modified: Thu Jul 27 22:25:26 2023, max compression
+gzip compressed data, was "autogluon.bench-0.2.2.tar", last modified: Tue Aug  8 23:23:35 2023, max compression
```

## Comparing `autogluon.bench-0.2.1.tar` & `autogluon.bench-0.2.2.tar`

### file list

```diff
@@ -1,137 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/.github/workflows/continuous_integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/.github/workflows/pypi_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/sample_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/sample_configs/amlb_configs/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/amlb_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/amlb_configs/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/amlb_configs/constraints.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/amlb_configs/frameworks_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/multimodal_cloud_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/multimodal_local_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/tabular_cloud_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/sample_configs/tabular_local_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.252851 autogluon.bench-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/amlb_configs/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/amlb_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18378 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/default_config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1803 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/destroy.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/stack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/src/autogluon/bench/custom_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon/bench/custom_configs/amlb_configs/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/custom_configs/amlb_configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/dataset_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/multimodal_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/object_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/datasets/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/aggregate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/aggregate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/aggregate/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/output_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/output_suite_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/evaluate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/evaluate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/run_evaluation_openml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.264852 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/exec.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      928 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/runbenchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/src/autogluon/bench/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/scripts/generate_cloud_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/src/autogluon/bench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/utils/general_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      559 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/src/autogluon/bench/utils/gpu_utilization.sh
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon/bench/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.260851 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 22:25:26.000000 autogluon.bench-0.2.1/src/autogluon.bench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/tests/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/tests/unittests/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/benchmark/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/benchmark/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/benchmark/test_runbenchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.256852 autogluon.bench-0.2.1/tests/unittests/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/tests/unittests/cloud/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/cloud/aws/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/cloud/aws/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/cloud/aws/test_stack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/tests/unittests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/datasets/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:25:26.268852 autogluon.bench-0.2.1/tests/unittests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/utils/test_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-27 22:25:06.000000 autogluon.bench-0.2.1/tests/unittests/utils/test_general_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.204184 autogluon.bench-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.188183 autogluon.bench-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.188183 autogluon.bench-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/.github/workflows/continuous_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/.github/workflows/pypi_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28225 2023-08-08 23:23:35.204184 autogluon.bench-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.188183 autogluon.bench-0.2.2/sample_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.188183 autogluon.bench-0.2.2/sample_configs/amlb_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/amlb_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/amlb_configs/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/amlb_configs/constraints.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/amlb_configs/frameworks_example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.188183 autogluon.bench-0.2.2/sample_configs/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/dataloaders/text_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/dataloaders/text_datasets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/dataloaders/vision_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/dataloaders/vision_datasets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/multimodal_cloud_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/multimodal_local_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/tabular_cloud_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/sample_configs/tabular_local_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 23:23:35.204184 autogluon.bench-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.184183 autogluon.bench-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.184183 autogluon.bench-0.2.2/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon/bench/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/lambdas/amlb_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/lambdas/amlb_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/default_config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1803 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/deploy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/destroy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/stack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.184183 autogluon.bench-0.2.2/src/autogluon/bench/custom_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon/bench/custom_configs/amlb_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/custom_configs/amlb_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/custom_configs/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/custom_configs/dataloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/datasets/dataset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19885 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/datasets/multimodal_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/datasets/object_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/datasets/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/eval/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/aggregate/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/eval/benchmark_context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/benchmark_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/benchmark_context/output_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14343 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/benchmark_context/output_suite_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/benchmark_context/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/evaluate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/evaluate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.196184 autogluon.bench-0.2.2/src/autogluon/bench/eval/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15468 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/scripts/run_evaluation_openml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/multimodal/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1698 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/multimodal/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/tabular/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/tabular/exec.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      939 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/tabular/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19317 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/runbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/src/autogluon/bench/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/scripts/generate_cloud_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/src/autogluon/bench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/utils/general_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/src/autogluon/bench/utils/hardware_utilization.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 23:23:35.000000 autogluon.bench-0.2.2/src/autogluon/bench/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.192183 autogluon.bench-0.2.2/src/autogluon.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28225 2023-08-08 23:23:35.000000 autogluon.bench-0.2.2/src/autogluon.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-08-08 23:23:35.000000 autogluon.bench-0.2.2/src/autogluon.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:23:35.000000 autogluon.bench-0.2.2/src/autogluon.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 23:23:35.000000 autogluon.bench-0.2.2/src/autogluon.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-08 23:23:35.000000 autogluon.bench-0.2.2/src/autogluon.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 23:23:35.000000 autogluon.bench-0.2.2/src/autogluon.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.188183 autogluon.bench-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.188183 autogluon.bench-0.2.2/tests/unittests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/tests/unittests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/benchmark/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/benchmark/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15502 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/benchmark/test_runbenchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.188183 autogluon.bench-0.2.2/tests/unittests/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/tests/unittests/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/cloud/aws/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/cloud/aws/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/cloud/aws/test_stack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/tests/unittests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/datasets/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:23:35.200183 autogluon.bench-0.2.2/tests/unittests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/utils/test_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-08 23:23:14.000000 autogluon.bench-0.2.2/tests/unittests/utils/test_general_utils.py
```

### Comparing `autogluon.bench-0.2.1/.github/workflows/continuous_integration.yml` & `autogluon.bench-0.2.2/.github/workflows/continuous_integration.yml`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/.github/workflows/pypi_release.yml` & `autogluon.bench-0.2.2/.github/workflows/pypi_release.yml`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/.gitignore` & `autogluon.bench-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/LICENSE` & `autogluon.bench-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/PKG-INFO` & `autogluon.bench-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.bench
-Version: 0.2.1
+Version: 0.2.2
 Summary: A benchmarking tool for AutoML
 Author: AutoGluon Community
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -303,15 +303,22 @@
 For more customizations, please follow the [example custom configuration folder](https://github.com/openml/automlbenchmark/tree/master/examples/custom) provided by AMLB and their [documentation](https://github.com/openml/automlbenchmark/blob/master/docs/HOWTO.md#custom-configuration). 
 
 
 ### Multimodal Benchmark
 
 For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
 
-You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
+You can add more datasets to your benchmarking jobs. We support custom datasets with custom defined data loaders. Follow these steps:
+  1. Create a folder under the working directory, e.g. `custom_dataloader/`
+  2. Create a dataset yaml file, `custom_dataloader/datasets.yaml` which includes all required properties for your problem type, please refer to the [function](https://github.com/autogluon/autogluon-bench/blob/52eee491018f6281236416f4b1bece14b88610e8/src/autogluon/bench/frameworks/multimodal/exec.py#L100-L201).
+  3. Create a dataset loader class, `custom_dataloader/dataloader.py`, which downloads and loads the dataset as a dataframe. Please set the required properties as mentioned above.
+  4. Add `custom_dataloader` in the `agbench run` configuration, where `dataloader_file`, `class_name` and `dataset_config_file` are required. 
+  5. Make sure you have the proper permission to download the dataset. If running in `AWS mode`, we support downloading from the S3 bucket specified as `DATA_BUCKET` in the `agbench run` configuration under the same AWS Batch deployment account.
+
+  Please refer to `sample_configs/dataloaders` for more examples.
 
 ## Run benchmarks on AWS
 
 AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
 
 To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
 
@@ -415,15 +422,15 @@
 ### Monitoring metrics for your instances on AWS
 
 A variety of metrics are available for the EC2 instances that are launched during benchmarking. These can be accessed through the AWS Console by following this navigation path: `CloudWatch` -> `All metrics` -> `AWS namespaces` -> `EC2`. For a comprehensive list of these metrics, refer to the [official AWS documentation](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/viewing_metrics_with_cloudwatch.html).
 
 In addition to the standard metrics, we also provide a custom metric for `GPUUtilization`. This can be found in the `CloudWatch` section under `All metrics` -> `Custom namespaces` -> `EC2`. Please note that the `GPUUtilization` metric is also updated every five minutes.
 
 
-## Evaluating bechmark runs
+## Evaluating benchmark runs
 
 Tabular benchmark results can be evaluated using the tools in `src/autogluon/bench/eval/`. The evaluation logic will aggregate, clean, and produce evaluation results for runs stored in S3.
 In a future release, we intend to add evaluation support for multimodal benchmark results.
 
 
 ### Evaluation Steps
```

### Comparing `autogluon.bench-0.2.1/README.md` & `autogluon.bench-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -69,15 +69,22 @@
 For more customizations, please follow the [example custom configuration folder](https://github.com/openml/automlbenchmark/tree/master/examples/custom) provided by AMLB and their [documentation](https://github.com/openml/automlbenchmark/blob/master/docs/HOWTO.md#custom-configuration). 
 
 
 ### Multimodal Benchmark
 
 For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
 
-You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
+You can add more datasets to your benchmarking jobs. We support custom datasets with custom defined data loaders. Follow these steps:
+  1. Create a folder under the working directory, e.g. `custom_dataloader/`
+  2. Create a dataset yaml file, `custom_dataloader/datasets.yaml` which includes all required properties for your problem type, please refer to the [function](https://github.com/autogluon/autogluon-bench/blob/52eee491018f6281236416f4b1bece14b88610e8/src/autogluon/bench/frameworks/multimodal/exec.py#L100-L201).
+  3. Create a dataset loader class, `custom_dataloader/dataloader.py`, which downloads and loads the dataset as a dataframe. Please set the required properties as mentioned above.
+  4. Add `custom_dataloader` in the `agbench run` configuration, where `dataloader_file`, `class_name` and `dataset_config_file` are required. 
+  5. Make sure you have the proper permission to download the dataset. If running in `AWS mode`, we support downloading from the S3 bucket specified as `DATA_BUCKET` in the `agbench run` configuration under the same AWS Batch deployment account.
+
+  Please refer to `sample_configs/dataloaders` for more examples.
 
 ## Run benchmarks on AWS
 
 AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
 
 To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
 
@@ -181,15 +188,15 @@
 ### Monitoring metrics for your instances on AWS
 
 A variety of metrics are available for the EC2 instances that are launched during benchmarking. These can be accessed through the AWS Console by following this navigation path: `CloudWatch` -> `All metrics` -> `AWS namespaces` -> `EC2`. For a comprehensive list of these metrics, refer to the [official AWS documentation](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/viewing_metrics_with_cloudwatch.html).
 
 In addition to the standard metrics, we also provide a custom metric for `GPUUtilization`. This can be found in the `CloudWatch` section under `All metrics` -> `Custom namespaces` -> `EC2`. Please note that the `GPUUtilization` metric is also updated every five minutes.
 
 
-## Evaluating bechmark runs
+## Evaluating benchmark runs
 
 Tabular benchmark results can be evaluated using the tools in `src/autogluon/bench/eval/`. The evaluation logic will aggregate, clean, and produce evaluation results for runs stored in S3.
 In a future release, we intend to add evaluation support for multimodal benchmark results.
 
 
 ### Evaluation Steps
```

### Comparing `autogluon.bench-0.2.1/pyproject.toml` & `autogluon.bench-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     "fsspec >=2023.5.0,<=2023.6.0",
     "matplotlib >=3.4,<3.7",
     "pandas >=1.2.5,<2.0",
     "pydantic>=1.10.4,<2.0", # https://github.com/ray-project/ray/issues/36990
     "pyyaml >=5.4,<=6.0",
     "ray[default] >=2.3.0,<2.4.0",
     "s3fs >=2023.5.0,<=2023.6.0",
+    "tqdm >=4.64.0,<=4.65.0",
     "typer >=0.9.0,<1.0.0",
     "wheel >0.38.0,<=0.40.0",
 ]
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-mock", "tox", "black>=23.1.9, <=23.7.0", "isort>=5.11.0, <=5.12.0"]
```

### Comparing `autogluon.bench-0.2.1/sample_configs/amlb_configs/config.yaml` & `autogluon.bench-0.2.2/sample_configs/amlb_configs/config.yaml`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/sample_configs/multimodal_cloud_configs.yaml` & `autogluon.bench-0.2.2/sample_configs/multimodal_cloud_configs.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -20,18 +20,24 @@
 module_configs:
   # Multimodal specific
   multimodal:
     git_uri#branch: # required
       - https://github.com/autogluon/autogluon#master
     dataset_name:  # required
       - shopee
-      - stanford_online
+      # - stanford_online
+    # custom_dataloader:
+    #   dataloader_file: sample_configs/dataloaders/text_dataloader.py   # required, relative path to WORKDIR
+    #   class_name: TextDataLoaer  # required
+    #   lang: en
+    #   dataset_config_file: sample_configs/dataloaders/text_datasets.yaml  # required, dataset definition yaml
+
     presets:  # optional
       - medium_quality
-      - high_quality
+      # - high_quality
     time_limit:  # optional
       - 10
     hyperparameters:  # optional
       - optimization.max_epochs: 2
         optimization.learning_rate: 0.005
-      - optimization.max_epochs: 5
-        optimization.learning_rate: 0.0005
+      # - optimization.max_epochs: 5
+      #   optimization.learning_rate: 0.0005
```

### Comparing `autogluon.bench-0.2.1/sample_configs/multimodal_local_configs.yaml` & `autogluon.bench-0.2.2/sample_configs/multimodal_local_configs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -3,13 +3,19 @@
 mode: local  # required
 benchmark_name: ag_bench  # required
 root_dir: ag_bench_runs  # optional, default = "ag_bench_runs"
 # METRICS_BUCKET: autogluon-benchmark-metrics  # optional, required only if you want to upload metrics to S3
 
 # Multimodal specific
 git_uri#branch: https://github.com/autogluon/autogluon#master  # required
-dataset_name: melbourne_airbnb  # required
+dataset_name: 
+  melbourne_airbnb  # required
+# custom_dataloader:
+#     dataloader_file: sample_configs/dataloaders/text_dataloader.py   # relative path to WORKDIR
+#     class_name: TextDataLoaer
+#     lang: en
+#     dataset_config_file: sample_configs/dataloaders/text_datasets.yaml 
 presets: medium_quality  # optional
 hyperparameters:  # optional
   optimization.learning_rate: 0.0005
   optimization.max_epochs: 5
 time_limit: 10  # optional
```

### Comparing `autogluon.bench-0.2.1/sample_configs/tabular_cloud_configs.yaml` & `autogluon.bench-0.2.2/sample_configs/tabular_cloud_configs.yaml`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/sample_configs/tabular_local_configs.yaml` & `autogluon.bench-0.2.2/sample_configs/tabular_local_configs.yaml`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/Dockerfile` & `autogluon.bench-0.2.2/src/autogluon/bench/Dockerfile`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,70 @@
-FROM 763104351884.dkr.ecr.us-east-1.amazonaws.com/pytorch-training:1.13.1-gpu-py39-cu117-ubuntu20.04-ec2
+ARG AG_BENCH_BASE_IMAGE
+FROM $AG_BENCH_BASE_IMAGE
+
+ENV DEBIAN_FRONTEND=noninteractive
+
+# Install essential packages and Python 3.9
+RUN apt-get update && \
+    apt-get install -y software-properties-common build-essential && \
+    add-apt-repository ppa:deadsnakes/ppa && \
+    apt-get update && \
+    apt-get install -y python3.9 python3.9-dev python3.9-distutils python3.9-venv && \
+    update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.9 1
+
+# Install utilities and AWS CLI
+RUN apt-get install -y python3-pip unzip curl git pciutils && \
+    curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" && \
+    unzip -q awscliv2.zip && \
+    ./aws/install && \
+    rm awscliv2.zip && \
+    python3 -m pip install --upgrade pip && \
+    apt-get clean && \
+    rm -rf /var/lib/apt/lists/* /usr/local/aws
+
+# Application-specific steps
 ARG AG_BENCH_DEV_URL
 ARG AG_BENCH_VERSION
 ARG CDK_DEPLOY_REGION
 ARG FRAMEWORK_PATH
 ARG GIT_URI
 ARG GIT_BRANCH
 ARG BENCHMARK_DIR
 ARG AMLB_FRAMEWORK
 ARG AMLB_USER_DIR
 
 WORKDIR /app/
-COPY entrypoint.sh utils/gpu_utilization.sh $FRAMEWORK_PATH/setup.sh custom_configs/ /app/
-
-RUN apt-get update && apt-get install -y --no-install-recommends cron unzip curl && rm -rf /var/lib/apt/lists/* \
-    && rm -rf /var/lib/apt/lists/* \
-    && mkdir -p /var/spool/cron/crontabs \
-    && touch /var/log/cron.log \
-    && curl "https://d1vvhvl2y92vvt.cloudfront.net/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" \
-    && unzip -q awscliv2.zip \
-    && ./aws/install \
-    && rm awscliv2.zip \
-    && pip install --upgrade pip
 
 RUN if [ -n "$AG_BENCH_DEV_URL" ]; then \
         echo "Cloning: $AG_BENCH_DEV_URL" \
         && AG_BENCH_DEV_REPO=$(echo "$AG_BENCH_DEV_URL" | cut -d "#" -f 1) \
         && AG_BENCH_DEV_BRANCH=$(echo "$AG_BENCH_DEV_URL" | cut -d "#" -f 2) \
         && git clone --branch "$AG_BENCH_DEV_BRANCH" --single-branch "$AG_BENCH_DEV_REPO" /app/autogluon-bench \
-        && pip install -e /app/autogluon-bench; \
+        && python3 -m pip install -e /app/autogluon-bench; \
     else \
         output=$(pip install autogluon.bench==$AG_BENCH_VERSION 2>&1) || true; \
         if echo $output | grep -q "No matching distribution"; then \
             echo -e "ERROR: No matching distribution found for autogluon.bench==$AG_BENCH_VERSION\n\
             To resolve the issue, try 'agbench run <config_file> --dev-branch <autogluon_bench_fork_uri>#<git_branch>'"; \
             exit 1; \
         fi; \
     fi
 
-RUN chmod +x setup.sh entrypoint.sh /app/gpu_utilization.sh \
+COPY entrypoint.sh utils/hardware_utilization.sh $FRAMEWORK_PATH/setup.sh custom_configs/ /app/
+
+RUN chmod +x setup.sh entrypoint.sh hardware_utilization.sh \
     && if echo "$FRAMEWORK_PATH" | grep -q "tabular"; then \
         if [ -n "$AMLB_USER_DIR" ]; then \
             bash setup.sh $GIT_URI $GIT_BRANCH $BENCHMARK_DIR $AMLB_FRAMEWORK $AMLB_USER_DIR; \
         else \
             bash setup.sh $GIT_URI $GIT_BRANCH $BENCHMARK_DIR $AMLB_FRAMEWORK; \
         fi; \
     elif echo "$FRAMEWORK_PATH" | grep -q "multimodal"; then \
         if [ -n "$AG_BENCH_DEV_URL" ]; then \
             bash setup.sh $GIT_URI $GIT_BRANCH $BENCHMARK_DIR --AGBENCH_DEV_URL=$AG_BENCH_DEV_URL; \
         else \
             bash setup.sh $GIT_URI $GIT_BRANCH $BENCHMARK_DIR --AG_BENCH_VER=$AG_BENCH_VERSION; \
         fi; \
     fi \
-    && echo "*/5 * * * * /app/gpu_utilization.sh >> /var/log/cron.log 2>&1" > /var/spool/cron/crontabs/root \
-    && chmod 600 /var/spool/cron/crontabs/root \
     && echo "CDK_DEPLOY_REGION=$CDK_DEPLOY_REGION" >> /etc/environment
 
 ENTRYPOINT ["./entrypoint.sh"]
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/app.py` & `autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/app.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py` & `autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py` & `autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py` & `autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,14 +282,16 @@
         )
     )
 
     for combo in specific_value_combinations:
         new_config = {key: config[key] for key in common_keys}
         new_config.update(dict(zip(specific_keys, combo)))
 
+        if "custom_dataloader" in config["module_configs"]["multimodal"]:
+            new_config["custom_dataloader"] = config["module_configs"]["multimodal"]["custom_dataloader"]
         job_id, config_s3_path = process_combination(new_config, metrics_bucket, batch_job_queue, batch_job_definition)
         job_configs[job_id] = config_s3_path
 
     return job_configs
 
 
 def generate_tabular_config_combinations(config, metrics_bucket, batch_job_queue, batch_job_definition):
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/batch_stack/stack.py` & `autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/batch_stack/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
         # TODO: use https://github.com/cdklabs/cdk-docker-image-deployment
         docker_image_asset = ecr_assets.DockerImageAsset(
             self,
             f"{prefix}-ecr-docker-image-asset",
             directory=docker_base_dir,
             follow_symlinks=core.SymlinkFollowMode.ALWAYS,
             build_args={
+                "AG_BENCH_BASE_IMAGE": os.environ["AG_BENCH_BASE_IMAGE"],
                 "AG_BENCH_VERSION": os.getenv("AG_BENCH_VERSION", "latest"),
                 "AG_BENCH_DEV_URL": os.getenv("AG_BENCH_DEV_URL", ""),
                 "CDK_DEPLOY_REGION": os.environ["CDK_DEPLOY_REGION"],
                 "FRAMEWORK_PATH": os.environ["FRAMEWORK_PATH"],
                 "GIT_URI": os.environ["GIT_URI"],
                 "GIT_BRANCH": os.environ["GIT_BRANCH"],
                 "BENCHMARK_DIR": os.environ["BENCHMARK_DIR"],
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/deploy.sh` & `autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/deploy.sh`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/destroy.sh` & `autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/destroy.sh`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/cloud/aws/stack_handler.py` & `autogluon.bench-0.2.2/src/autogluon/bench/cloud/aws/stack_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 def get_instance_type_specs(instance_type, region):
     ec2_client = boto3.client("ec2", region_name=region)
     response = ec2_client.describe_instance_types(InstanceTypes=[instance_type])
 
     instance_type_info = response["InstanceTypes"][0]
 
-    gpu_info_list = instance_type_info.get("GpuInfo", [])
-    gpu_count = sum(gpu_info.get("Count", 0) for gpu_info in gpu_info_list["Gpus"])
+    gpu_info_list = instance_type_info.get("GpuInfo", {}).get("Gpus", [{}])
+    gpu_count = sum(gpu_info.get("Count", 0) for gpu_info in gpu_info_list)
 
     vcpu_info = instance_type_info.get("VCpuInfo", {})
     vcpu_count = vcpu_info.get("DefaultVCpus", 0)
 
     memory_info = instance_type_info.get("MemoryInfo", {})
     memory = memory_info.get("SizeInMiB", 0)
 
@@ -116,14 +116,19 @@
 
     Returns:
         dict: A dictionary containing the CDK context settings used for the deployment.
     """
     cdk_path = _get_temp_cdk_app_path()
     custom_infra_configs = custom_configs.get("cdk_context", {})
     infra_configs = construct_context(custom_configs=custom_infra_configs)
+    instance_type: str = infra_configs["INSTANCE_TYPES"][0]
+    os.environ["AG_BENCH_BASE_IMAGE"] = "nvidia/cuda:12.2.0-runtime-ubuntu20.04"
+    if not instance_type.startswith(("p", "g")):
+        # CPU instances
+        os.environ["AG_BENCH_BASE_IMAGE"] = "ubuntu:20.04"
     command = [
         os.path.join(module_base_dir, "deploy.sh"),
         infra_configs["STACK_NAME_PREFIX"],
         infra_configs["STACK_NAME_TAG"],
         infra_configs["STATIC_RESOURCE_STACK_NAME"],
         infra_configs["BATCH_STACK_NAME"],
         str(infra_configs["CONTAINER_MEMORY"]),
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/datasets/multimodal_dataset.py` & `autogluon.bench-0.2.2/src/autogluon/bench/datasets/multimodal_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import logging
 import os
 
 import pandas as pd
 
-from autogluon.bench.utils.dataset_utils import get_data_home_dir, get_repo_url
+from autogluon.bench.utils.dataset_utils import get_data_home_dir, get_repo_url, path_expander
 from autogluon.common.loaders import load_zip
 from autogluon.common.loaders._utils import download
 
 from .constants import (
     _BINARY,
     _CATEGORICAL,
     _IMAGE_SIMILARITY,
@@ -36,19 +36,14 @@
     "NewsPopularity",
     "NewsChannel",
 ]
 
 logger = logging.getLogger(__name__)
 
 
-def _path_expander(path, base_folder):
-    path_l = path.split(";")
-    return ";".join([os.path.abspath(os.path.join(base_folder, path)) for path in path_l])
-
-
 class BaseMultiModalDataset(abc.ABC):
     def __init__(self, split: str, dataset_name: str, data_info: dict):
         """
         Initializes the class.
 
         Args:
             split (str): Specifies the dataset split. It should be one of the following options: 'train', 'val', 'test'.
@@ -134,15 +129,15 @@
         self._path = os.path.join(get_data_home_dir(), "shopee")
         load_zip.unzip(self._INFO["data"]["url"], unzip_dir=self._path, sha1sum=self._INFO["data"]["sha1sum"])
         self._base_folder = os.path.join(self._path, "shopee")
         try:
             data_path = os.path.join(self._base_folder, f"{self._split}.csv")
             self._data = pd.read_csv(data_path)
             self._data["image"] = self._data["image"].apply(
-                lambda ele: _path_expander(ele, base_folder=self._base_folder)
+                lambda ele: path_expander(ele, base_folder=self._base_folder)
             )
         except FileNotFoundError as e:
             logger.warn(f"The data split {self._split} is not available.")
             self._data = None
 
     @property
     def base_folder(self):
@@ -191,15 +186,15 @@
         load_zip.unzip(self._INFO["data"]["url"], unzip_dir=self._path, sha1sum=self._INFO["data"]["sha1sum"])
         self._base_folder = os.path.join(self._path, "Stanford_Online_Products")
         try:
             self._data = pd.read_csv(os.path.join(self._base_folder, f"{self._split}.csv"), index_col=0)
             self._image_columns = ["Image1", "Image2"]
             for image_col in self._image_columns:
                 self._data[image_col] = self._data[image_col].apply(
-                    lambda ele: _path_expander(ele, base_folder=self._base_folder)
+                    lambda ele: path_expander(ele, base_folder=self._base_folder)
                 )
         except FileNotFoundError as e:
             logger.warn(f"The data split {self._split} is not available.")
             self._data = None
 
     @property
     def image_columns(self):
@@ -246,15 +241,15 @@
 
         try:
             self._data = pd.read_csv(os.path.join(self._base_folder, f"{self._split}.csv"), index_col=0)
             self._image_col = "image"
             self._text_col = "caption"
 
             self._data[self._image_col] = self._data[self._image_col].apply(
-                lambda ele: _path_expander(ele, base_folder=self._base_folder)
+                lambda ele: path_expander(ele, base_folder=self._base_folder)
             )
             self._label_col = "relevance"
             self._data[self._label_col] = [1] * len(self._data)
         except FileNotFoundError as e:
             logger.warn(f"The data split {self._split} is not available.")
             self._data = None
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/datasets/object_detection_dataset.py` & `autogluon.bench-0.2.2/src/autogluon/bench/datasets/object_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/datasets/registry.py` & `autogluon.bench-0.2.2/src/autogluon/bench/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/aggregate/results.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/aggregate/results.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/output_context.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/benchmark_context/output_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Set
+from typing import Optional, Set, Union
 
 import boto3
 import numpy as np
 import pandas as pd
 
 from autogluon.common.loaders import load_pd, load_pkl
 from autogluon.common.utils.s3_utils import s3_path_to_bucket_prefix
@@ -44,14 +44,18 @@
         return self.path + "scores/results.csv"
 
     @property
     def path_leaderboard(self):
         return self.path + "leaderboard.csv"
 
     @property
+    def path_model_failures(self):
+        return self.path + "model_failures.csv"
+
+    @property
     def path_infer_speed(self):
         return self.path + "infer_speed.csv"
 
     @property
     def path_logs(self):
         return self.path + "logs.zip"
 
@@ -89,14 +93,18 @@
             except FileNotFoundError:
                 return None
         return results
 
     def load_leaderboard(self) -> pd.DataFrame:
         return load_pd.load(self.path_leaderboard)
 
+    def load_model_failures(self) -> pd.DataFrame:
+        """Load and return the raw model failures file"""
+        return load_pd.load(self.path_model_failures)
+
     def load_infer_speed(self) -> pd.DataFrame:
         return load_pd.load(self.path_infer_speed)
 
     def load_zeroshot_metadata(self, max_size_mb: float = None) -> dict:
         s3_bucket = self.get_s3_bucket()
         s3_prefix = self.get_s3_prefix(path=self.path_zeroshot_metadata)
         s3 = boto3.client("s3")
@@ -204,14 +212,32 @@
             combined_full["duration"] = combined_full["fit_time"]
             # combined_full['predict_duration'] = combined_full['pred_time_test']
 
             # print(combined_full)
             print(f"SUCCESS: {print_msg}")
             return combined_full
 
+    def get_model_failures(self) -> Union[pd.DataFrame, None]:
+        """
+        Load and return the model failures CSV as a pandas DataFrame if it exists, else return None.
+
+        Will merge with the results to get additional information, akin to the leaderboard output.
+        """
+        results = self.load_results()
+        try:
+            model_failures_df = self.load_model_failures()
+        except Exception as e:
+            print(f"FAILURE:\n" f"\t{e.__class__.__name__}: {e}")
+            return None
+        else:
+            results = results.rename(columns={"framework": "framework_parent"})
+            model_failures_df["id"] = results["id"][0]
+            model_failures_full_df = pd.merge(model_failures_df, results, on="id", how="left")
+            return model_failures_full_df
+
     def _merge_leaderboard_with_infer_speed(self, leaderboard: pd.DataFrame) -> pd.DataFrame:
         infer_speed_df = self.load_infer_speed()
         infer_speed_df = infer_speed_df[["model", "batch_size", "pred_time_test_with_transform"]]
         infer_speed_m_df = infer_speed_df.set_index(["model", "batch_size"], drop=True)
         a = infer_speed_m_df.to_dict()
         b = a["pred_time_test_with_transform"]
         c = dict()
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/benchmark_context/output_suite_context.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/benchmark_context/output_suite_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,14 +180,31 @@
         return result
 
     def aggregate_leaderboards(self) -> pd.DataFrame:
         leaderboards_list = self.load_leaderboards()
         leaderboards_df = pd.concat(leaderboards_list, ignore_index=True)
         return leaderboards_df
 
+    def load_model_failures(self) -> List[pd.DataFrame]:
+        return self._loop_func(
+            func=OutputContext.get_model_failures, input_list=self.output_contexts, allow_exception=True
+        )
+
+    def aggregate_model_failures(self) -> pd.DataFrame:
+        model_failures_list = self.load_model_failures()
+        none_count = 0
+        for e in model_failures_list:
+            if e is None:
+                none_count += 1
+        if none_count == len(model_failures_list):
+            return pd.DataFrame()
+        else:
+            model_failures_df = pd.concat(model_failures_list, ignore_index=True)
+            return model_failures_df
+
     def get_amlb_info(self) -> List[str]:
         return self._loop_func(func=OutputContext.get_amlb_info, input_list=self.output_contexts)
 
     def get_benchmark_failures(self):
         amlb_info_dict = dict()
 
         amlb_info_list = self.get_amlb_info()
@@ -225,25 +242,22 @@
         result = [r for r in result if r is not None]
         return result
 
     @staticmethod
     def _aggregate_leaderboards_seq(output_contexts, columns_to_keep, with_infer_speed):
         print("starting sequential...")
         num_contexts = len(output_contexts)
-        if not ray.is_initialized():
-            ray.init()
         results = []
         for i, output_context in enumerate(output_contexts):
             results.append(
                 get_single_leaderboard_seq(output_context, columns_to_keep, with_infer_speed, i, num_contexts)
             )
-        result = ray.get(results)
         print("finished sequential...")
-        result = [r for r in result if r is not None]
-        return result
+        results = [r for r in results if r is not None]
+        return results
 
     def construct_zs_dict(self, results_lst=None, zeroshot_metadata_list=None):
         if results_lst is None:
             results_lst = self.load_results()
         if zeroshot_metadata_list is None:
             zeroshot_metadata_list = self.load_zeroshot_metadata()
         output_contexts = self.output_contexts
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/benchmark_evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/constants.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/evaluate_results.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/evaluate_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,70 @@
+import copy
 import logging
 import os
+from typing import Tuple
 
 import pandas as pd
 
 from autogluon.common.savers import save_pd
 
 from . import evaluate_utils
 from .constants import *
 from .preprocess import preprocess_utils
 
 logger = logging.getLogger(__name__)
 
 
+def compute_vs_diff(
+    results_ranked_by_dataset: pd.DataFrame, framework_1: str, framework_2: str
+) -> Tuple[float, float]:
+    """
+    Compare two frameworks across a suite of datasets and calculate mean_diff and median_diff.
+
+    Parameters
+    ----------
+    results_ranked_by_dataset: pd.DataFrame
+        The ranked results by dataset containing only the two frameworks.
+    framework_1: str
+        The name of the first framework to compare.
+    framework_2: str
+        The name of the second framework to compare.
+
+    Returns
+    -------
+    A tuple of (mean_diff, median_diff).
+
+    mean_diff: float
+        The proportional mean difference in the metric error of framework_1 to framework_2, normalized per dataset.
+        As an example, if the value is 0.05, then the metric error is on average 5% lower on framework_1 compared to framework_2.
+            Example: framework_2 has a metric_error of 0.1, then framework_1 would have a metric_error of 0.095.
+        Conversely, if the value is -0.05, then the metric error is on average 5% lower on framework_2 compared to framework_1.
+        The maximum and minimum possible value is 1.0 and -1.0.
+    median_diff: float
+        The proportional median difference in the metric error of framework_1 to framework_2, normalized per dataset.
+        The maximum and minimum possible value is 1.0 and -1.0.
+    """
+    assert framework_1 != framework_2
+    assert set(results_ranked_by_dataset[FRAMEWORK].unique()) == {framework_1, framework_2}
+
+    results_ranked_by_dataset = copy.deepcopy(results_ranked_by_dataset)
+
+    results_ranked_by_dataset.loc[results_ranked_by_dataset[FRAMEWORK] == framework_1, "sign"] = -1
+    results_ranked_by_dataset.loc[results_ranked_by_dataset[FRAMEWORK] == framework_2, "sign"] = 1
+
+    results_ranked_by_dataset = results_ranked_by_dataset.sort_values(by=[BESTDIFF], ascending=False)
+    results_ranked_by_dataset = results_ranked_by_dataset.drop_duplicates(subset=[DATASET], keep="first")
+    results_ranked_by_dataset[BESTDIFF] = results_ranked_by_dataset[BESTDIFF] * results_ranked_by_dataset["sign"]
+
+    mean_diff = results_ranked_by_dataset[BESTDIFF].mean()
+    median_diff = results_ranked_by_dataset[BESTDIFF].median()
+
+    return mean_diff, median_diff
+
+
 def evaluate(
     results_raw,
     frameworks=None,
     banned_datasets=None,
     folds_to_keep=None,
     columns_to_agg_extra=None,
     frameworks_compare_vs_all=None,
@@ -79,70 +128,118 @@
     ideal_rows = num_folds * num_datasets * num_frameworks
     actual_rows = len(results_raw)
     errors = ideal_rows - actual_rows
     print("num_datasets:", num_datasets)
     print("num_folds:", num_folds)
     print("errors:", errors)
 
+    print("################################################")
     for framework in total_frameworks:
         results_framework = results_raw[results_raw[FRAMEWORK] == framework]
         num_rows_framework = len(results_framework)
         datasets_framework = results_framework[DATASET].unique()
         datasets_framework_errors = [dataset for dataset in total_datasets if dataset not in datasets_framework]
         datasets_framework_errors_count = len(datasets_framework_errors)
         framework_fold_errors = num_datasets * num_folds - num_rows_framework
-        print("################################################")
         print("framework:", framework)
-        print("\tdatasets_framework_errors:", datasets_framework_errors)
-        print("\tdatasets_framework_errors_count:", datasets_framework_errors_count)
-        print("\tframework_fold_errors:", framework_fold_errors)
+        print(
+            f"\tdatasets_errors: {datasets_framework_errors_count}"
+            f"\tfold_errors: {framework_fold_errors}"
+            f"\tdatasets_framework_errors: {datasets_framework_errors}"
+        )
+    print("################################################")
+    print("%s VS %s" % ("all", "all"))
+    print("\tAll datasets regardless of failures")
+    results_ranked_all, results_ranked_by_dataset_all = evaluate_utils.compare_frameworks(
+        results_raw=results_raw,
+        banned_datasets=banned_datasets,
+        folds_to_keep=folds_to_keep,
+        filter_errors=False,
+        columns_to_agg_extra=columns_to_agg_extra,
+        datasets=total_datasets,
+    )
+
+    if output_dir:
+        path_ranked_all = os.path.join(output_dir, "results_ranked_all.csv")
+        save_pd.save(path=path_ranked_all, df=results_ranked_all)
+        logger.info(f"{path_ranked_all} saved.")
+
+        path_ranked_by_dataset_all = os.path.join(output_dir, "results_ranked_by_dataset_all.csv")
+        save_pd.save(path=path_ranked_by_dataset_all, df=results_ranked_by_dataset_all)
+        logger.info(f"{path_ranked_by_dataset_all} saved.")
+
+    print("################################################")
+    print("%s VS %s" % ("all", "all"))
+    print("\tOnly datasets where all frameworks succeeded")
+    results_ranked_valid, results_ranked_by_dataset_valid = evaluate_utils.compare_frameworks(
+        results_raw=results_raw,
+        frameworks=frameworks,
+        banned_datasets=banned_datasets,
+        folds_to_keep=folds_to_keep,
+        columns_to_agg_extra=columns_to_agg_extra,
+        datasets=total_datasets,
+    )
+
+    if output_dir:
+        path_ranked_valid = os.path.join(output_dir, "results_ranked_valid.csv")
+        save_pd.save(path=path_ranked_valid, df=results_ranked_valid)
+        logger.info(f"{path_ranked_valid} saved.")
+
+        path_ranked_by_dataset_valid = os.path.join(output_dir, "results_ranked_by_dataset_valid.csv")
+        save_pd.save(path=path_ranked_by_dataset_valid, df=results_ranked_by_dataset_valid)
+        logger.info(f"{path_ranked_by_dataset_valid} saved.")
 
-    calc_inf_diff = False
+    calc_inf_diff = TIME_INFER_S in columns_to_agg_extra
+    time_infer_s_rescaled = TIME_INFER_S + "_rescaled"
 
     all_results_pairs = {}
     for framework_2 in frameworks_compare_vs_all:
+        print(f"Computing comparison vs '{framework_2}'")
         results_list = []
 
         for framework_1 in total_frameworks:
             if framework_1 == framework_2:
                 results_ranked, results_ranked_by_dataset = evaluate_utils.compare_frameworks(
                     results_raw=results_raw,
                     frameworks=[framework_2],
                     banned_datasets=banned_datasets,
                     folds_to_keep=folds_to_keep,
                     columns_to_agg_extra=columns_to_agg_extra,
                     datasets=total_datasets,
                     verbose=False,
                 )
                 ties = len(results_ranked_by_dataset)
-                results_list.append([framework_1, 0.5, 0, 0, ties, 0])
+                out = [framework_1, 0.5, 0, 0, ties, 0, 0]
+                if calc_inf_diff:
+                    out.append(0)
+                results_list.append(out)
                 continue
 
             results_ranked, results_ranked_by_dataset = evaluate_utils.compare_frameworks(
                 results_raw=results_raw,
                 frameworks=[framework_1, framework_2],
                 banned_datasets=banned_datasets,
                 folds_to_keep=folds_to_keep,
                 columns_to_agg_extra=columns_to_agg_extra,
                 datasets=total_datasets,
                 verbose=False,
             )
 
-            bestdiff_1 = results_ranked[results_ranked[FRAMEWORK] == framework_1][BESTDIFF].iloc[0]
-            bestdiff_2 = results_ranked[results_ranked[FRAMEWORK] == framework_2][BESTDIFF].iloc[0]
+            mean_diff, median_diff = compute_vs_diff(
+                results_ranked_by_dataset=results_ranked_by_dataset, framework_1=framework_1, framework_2=framework_2
+            )
 
-            avg_diff = (bestdiff_2 - bestdiff_1) * 100
+            # Convert proportion to percentile
+            mean_diff *= 100
+            median_diff *= 100
 
             datasets_pair = results_ranked_by_dataset[DATASET].unique()
             framework_1_wins = 0
             framework_2_wins = 0
             ties = 0
-            time_infer_s_rescaled = TIME_INFER_S + "_rescaled"
-            if time_infer_s_rescaled in results_ranked_by_dataset:
-                calc_inf_diff = True
             avg_inf_diffs = 0
             for dataset in datasets_pair:
                 results_isolated = results_ranked_by_dataset[results_ranked_by_dataset[DATASET] == dataset]
 
                 if len(results_isolated) != 2:
                     print(f"Found invalid results_isolated! Printing:")
                     with pd.option_context("display.max_columns", None, "display.width", 1000):
@@ -171,58 +268,25 @@
                     framework_2_wins += 1
                 elif results_isolated_rank == 1.5:
                     ties += 1
                 else:
                     raise AssertionError("Rank not valid: %s" % results_isolated_rank)
             winrate = (framework_1_wins + 0.5 * ties) / (framework_1_wins + framework_2_wins + ties)
 
-            out = [framework_1, winrate, framework_1_wins, framework_2_wins, ties, avg_diff]
+            out = [framework_1, winrate, framework_1_wins, framework_2_wins, ties, mean_diff, median_diff]
             if calc_inf_diff:
                 avg_inf_diffs = avg_inf_diffs / len(datasets_pair)
                 out.append(avg_inf_diffs)
             results_list.append(out)
-        out_col_names = [FRAMEWORK, "winrate", ">", "<", "=", "% Less Avg. Errors"]
+        out_col_names = [FRAMEWORK, "winrate", ">", "<", "=", "% Less Avg. Errors", "% Less Errors (median)"]
         if calc_inf_diff:
             out_col_names.append("Avg Inf Speed Diff")
         results_pairs = pd.DataFrame(data=results_list, columns=out_col_names)
         all_results_pairs[framework_2] = results_pairs
 
-    print("################################################")
-    print("%s VS %s" % ("all", "all"))
-    print("\tAll datasets regardless of failures")
-    results_ranked_all, results_ranked_by_dataset_all = evaluate_utils.compare_frameworks(
-        results_raw=results_raw,
-        banned_datasets=banned_datasets,
-        folds_to_keep=folds_to_keep,
-        filter_errors=False,
-        columns_to_agg_extra=columns_to_agg_extra,
-        datasets=total_datasets,
-    )
-
-    if output_dir:
-        path_ranked_all = os.path.join(output_dir, "results_ranked_all.csv")
-        save_pd.save(path=path_ranked_all, df=results_ranked_all)
-        logger.info(f"{path_ranked_all} saved.")
-
-        path_ranked_by_dataset_all = os.path.join(output_dir, "results_ranked_by_dataset_all.csv")
-        save_pd.save(path=path_ranked_by_dataset_all, df=results_ranked_by_dataset_all)
-        logger.info(f"{path_ranked_by_dataset_all} saved.")
-
-    print("################################################")
-    print("%s VS %s" % ("all", "all"))
-    print("\tOnly datasets where all frameworks succeeded")
-    results_ranked_valid, results_ranked_by_dataset_valid = evaluate_utils.compare_frameworks(
-        results_raw=results_raw,
-        frameworks=frameworks,
-        banned_datasets=banned_datasets,
-        folds_to_keep=folds_to_keep,
-        columns_to_agg_extra=columns_to_agg_extra,
-        datasets=total_datasets,
-    )
-
     results_pairs_merged_dict = {}
     for framework in frameworks_compare_vs_all:
         columns_to_get_from_all = [RANK_1, "rank=2_count", "rank=3_count", "rank>3_count", ERROR_COUNT]
         results_pairs = all_results_pairs[framework]
         results_pairs_merged = pd.merge(results_pairs, results_ranked_valid, on=FRAMEWORK, how="left")
         results_pairs_merged = results_pairs_merged.drop(columns_to_get_from_all, axis=1)
         results_pairs_merged = pd.merge(
@@ -230,39 +294,21 @@
         )
         results_pairs_merged = results_pairs_merged.sort_values(by=RANK)
         print("################################################")
         print("%s VS %s" % (framework, "all"))
         with pd.option_context("display.max_rows", None, "display.max_columns", None, "display.width", 1000):
             results_pairs_merged_print = results_pairs_merged.drop(["bestdiff", "metric_error"], axis=1)
             results_pairs_merged_print = results_pairs_merged_print.reset_index(drop=True)
-            # results_pairs_merged_print = results_pairs_merged_print.rename(
-            #     {
-            #         '> AutoGluon_bestquality_1h_2021_01_04': '>AG',
-            #         '< AutoGluon_bestquality_1h_2021_01_04': '<AG',
-            #         '= AutoGluon_bestquality_1h_2021_01_04': '=AG',
-            #         '% Less Avg. Errors Than AutoGluon_bestquality_1h_2021_01_04': '% Less Err vs AG',
-            #     }
-            # , axis=1)
-            # results_pairs_merged_print = results_pairs_merged_print.drop(columns=['metric_error', ])
             print(results_pairs_merged_print)
         if output_dir:
             path_pairwise = os.path.join(output_dir, "pairwise", framework + ".csv")
             save_pd.save(path=path_pairwise, df=results_pairs_merged)
             logger.info(f"{path_pairwise} saved.")
         results_pairs_merged_dict[framework] = results_pairs_merged
 
-    if output_dir:
-        path_ranked_valid = os.path.join(output_dir, "results_ranked_valid.csv")
-        save_pd.save(path=path_ranked_valid, df=results_ranked_valid)
-        logger.info(f"{path_ranked_valid} saved.")
-
-        path_ranked_by_dataset_valid = os.path.join(output_dir, "results_ranked_by_dataset_valid.csv")
-        save_pd.save(path=path_ranked_by_dataset_valid, df=results_ranked_by_dataset_valid)
-        logger.info(f"{path_ranked_by_dataset_valid} saved.")
-
     return (
         results_ranked_valid,
         results_ranked_by_dataset_valid,
         results_ranked_all,
         results_ranked_by_dataset_all,
         results_pairs_merged_dict,
     )
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/evaluate_utils.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/evaluate_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/metadata/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/preprocess/preprocess_openml.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/evaluation/preprocess/preprocess_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/scripts/aggregate_amlb_results.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/run_evaluation_openml.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/scripts/run_evaluation_openml.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py` & `autogluon.bench-0.2.2/src/autogluon/bench/eval/scripts/run_generate_clean_openml.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/benchmark.py` & `autogluon.bench-0.2.2/src/autogluon/bench/frameworks/benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py` & `autogluon.bench-0.2.2/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,78 @@
-import json
 import logging
 import os
 import subprocess
 import sys
-from typing import Optional
+from typing import List
 
-from autogluon.bench import __version__ as agbench_version
 from autogluon.bench.frameworks.benchmark import Benchmark
 
 logger = logging.getLogger(__name__)
 
 
-class MultiModalBenchmark(Benchmark):
-    """
-    A benchmark class for AutoGluon MultiModal.
-
-    Attributes:
-        benchmark_name (str): The name of the benchmark.
-        root_dir (str): The root directory for the benchmark.
-        module (str): The name of the module being benchmarked (multimodal).
-
-    Methods:
-        setup(): Sets up the virtual environment for running the benchmark.
-        run(): Runs the benchmark on a given dataset.
-    """
-
+class TabularBenchmark(Benchmark):
     def setup(
         self,
-        git_uri: str = "https://github.com/autogluon/autogluon.git",
-        git_branch: str = "master",
-        agbench_dev_url: str = None,
+        git_uri: str = "https://github.com/openml/automlbenchmark.git",
+        git_branch: str = "stable",
+        framework: str = "AutoGluon:stable",
+        user_dir: str = None,
     ):
-        """
-        Sets up the virtual environment for running the benchmark.
-
-        Args:
-            git_uri (str): The URI of the Git repository to clone (default: "https://github.com/autogluon/autogluon.git").
-            git_branch (str): The branch of the Git repository to clone (default: "master").
-
-        Returns:
-            None
-        """
+        """Sets up the virtual environment for tabular benchmark."""
         setup_script_path = os.path.abspath(os.path.dirname(__file__)) + "/setup.sh"
-        command = [setup_script_path, git_uri, git_branch, self.benchmark_dir]
-        if agbench_dev_url is not None:
-            command.append(f"--AGBENCH_DEV_URL={agbench_dev_url}")
-        else:
-            command.append(f"--AG_BENCH_VER={agbench_version}")
+        command = [setup_script_path, git_uri, git_branch, self.benchmark_dir, framework]
+        if user_dir is not None:
+            command.append(user_dir)
         result = subprocess.run(command)
         if result.returncode != 0:
+            logger.error(result.stderr)
             sys.exit(1)
         else:
+            logger.info(result.stdout)
             logger.info("Successfully set up the environment under %s/.venv.", self.benchmark_dir)
 
     def run(
         self,
-        dataset_name: str,
         framework: str,
-        presets: Optional[str] = None,
-        hyperparameters: Optional[dict] = None,
-        time_limit: Optional[int] = None,
+        benchmark: str,
+        constraint: str,
+        task: str = None,
+        fold: int = None,
+        user_dir: str = None,
     ):
-        """
-        Runs the benchmark on a given dataset.
+        """Runs the tabular benchmark.
 
         Args:
-            dataset_name (str): Dataset that has been registered with multimodal_dataset_registry.
+            benchmark (str): The name of the benchmark to run (default: "test").
+            constraint (str): The name of the constraint to use (default: "test").
+            task (List[str]): The name of the task to run (default: None).
+            framework (str): The name of the framework to use (default: None). Examples: "AutoGluon:latest", "AutoGluon:stable".
+            user_dir (str): Path to custom configs to use (default: None).
 
-                                To get a list of datasets:
-
-                                from autogluon.bench.datasets.dataset_registry import multimodal_dataset_registry
-                                multimodal_dataset_registry.list_keys()
         Returns:
             None
         """
-        PY_EXC_PATH = self.benchmark_dir + "/.venv/bin/python"
-        exec_path = os.path.abspath(os.path.dirname(__file__)) + "/exec.py"
+
+        exec_script_path = os.path.abspath(os.path.dirname(__file__)) + "/exec.sh"
         command = [
-            PY_EXC_PATH,
-            exec_path,
-            "--dataset_name",
-            dataset_name,
-            "--framework",
+            exec_script_path,
             framework,
-            "--benchmark_dir",
+            benchmark,
+            constraint,
             self.benchmark_dir,
-            "--metrics_dir",
             self.metrics_dir,
         ]
-        if presets is not None and len(presets) > 0:
-            command += ["--presets", presets]
-        if hyperparameters is not None:
-            command += ["--hyperparameters", json.dumps(hyperparameters)]
-        if time_limit is not None:
-            command += ["--time_limit", str(time_limit)]
+
+        if task is not None:
+            command += ["-t", task]
+
+        if fold is not None:
+            command += ["-f", str(fold)]
+
+        if user_dir is not None:
+            command += ["-u", user_dir]
+
         result = subprocess.run(command)
         if result.returncode != 0:
             sys.exit(1)
         else:
-            logger.info(f"Benchmark {self.benchmark_name} on dataset {dataset_name} is complete.")
+            logger.info(f"Benchmark {self.benchmark_name} is complete.")
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/multimodal/setup.sh` & `autogluon.bench-0.2.2/src/autogluon/bench/frameworks/multimodal/setup.sh`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/exec.sh` & `autogluon.bench-0.2.2/src/autogluon/bench/frameworks/tabular/exec.sh`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/frameworks/tabular/setup.sh` & `autogluon.bench-0.2.2/src/autogluon/bench/frameworks/tabular/setup.sh`

 * *Files 17% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 echo "Cloning $GIT_URI#$BRANCH..."
 repo_name=$(basename -s .git $(echo $GIT_URI))
 git clone --depth 1 --branch ${BRANCH} ${GIT_URI} $DIR/$repo_name
 
 python3 -m pip install --upgrade pip
 python3 -m pip install --upgrade setuptools wheel
-pip install -r $DIR/automlbenchmark/requirements.txt
+python3 -m pip install -r $DIR/automlbenchmark/requirements.txt
 
 # install amlb framework only
 echo "Installing framework $AMLB_FRAMEWORK"
 amlb_args="$AMLB_FRAMEWORK -s only"
 
 if [ -n "$AMLB_USER_DIR" ]; then
     echo "using user_dir $AMLB_USER_DIR"
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/main.py` & `autogluon.bench-0.2.2/src/autogluon/bench/main.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/runbenchmark.py` & `autogluon.bench-0.2.2/src/autogluon/bench/runbenchmark.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,14 +49,15 @@
             },
             "run_kwargs": {
                 "dataset_name": configs["dataset_name"],
                 "framework": configs["git_uri#branch"].split("/")[-1],
                 "presets": configs.get("presets"),
                 "hyperparameters": configs.get("hyperparameters"),
                 "time_limit": configs.get("time_limit"),
+                "custom_dataloader": configs.get("custom_dataloader"),
             },
         }
     elif module == "tabular":
         return {
             "setup_kwargs": {
                 "git_uri": git_uri,
                 "git_branch": git_branch,
@@ -187,37 +188,41 @@
         job = response["jobs"][0]
         status_dict[job_id] = job["status"]
 
     logger.info(status_dict)
     return status_dict
 
 
-def wait_for_jobs_to_complete(
-    config_file: Optional[str] = None, job_ids: Optional[List[str]] = None, aws_region: Optional[str] = None
+def wait_for_jobs(
+    config_file: Optional[str] = None,
+    job_ids: Optional[List[str]] = None,
+    aws_region: Optional[str] = None,
+    quit_statuses: Optional[list] = ["SUCCEEDED", "FAILED"],
+    frequency: Optional[int] = 120,
 ):
     while True:
         all_jobs_completed = True
         failed_jobs = []
 
         try:
             job_status = get_job_status(job_ids=job_ids, cdk_deploy_region=aws_region, config_file=config_file)
 
             for job_id, job_status in job_status.items():
                 if job_status == "FAILED":
                     failed_jobs.append(job_id)
-                elif job_status not in ["SUCCEEDED", "FAILED"]:
+                elif job_status not in quit_statuses:
                     all_jobs_completed = False
         except botocore.exceptions.ClientError as e:
             logger.error(f"An error occurred: {e}.")
             return
 
         if all_jobs_completed:
             break
         else:
-            time.sleep(120)  # Poll job statuses every 60 seconds
+            time.sleep(frequency)  # Poll job statuses every 60 seconds
 
     return failed_jobs
 
 
 def _get_split_id(file_name: str):
     if "split" in file_name:
         file_name = os.path.basename(file_name)
@@ -278,16 +283,19 @@
     subprocess.run(["sudo", "mount", "--bind", orig_path, new_path])
 
 
 @app.command()
 def run(
     config_file: str = typer.Argument(..., help="Path to custom config file."),
     remove_resources: bool = typer.Option(False, help="Remove resources after run."),
-    wait: bool = typer.Option(False, help="Whether to block and wait for the benchmark to finish."),
+    wait: bool = typer.Option(False, help="Whether to block and wait for the benchmark to finish, default to False."),
     dev_branch: Optional[str] = typer.Option(None, help="Path to a development AutoGluon-Bench branch."),
+    skip_setup: bool = typer.Option(
+        False, help="Whether to skip setting up framework in local mode, default to False."
+    ),
 ):
     """Main function that runs the benchmark based on the provided configuration options."""
     configs = {}
     if config_file.startswith("s3"):
         config_file = download_file_from_s3(s3_path=config_file)
     with open(config_file, "r") as f:
         configs = yaml.safe_load(f)
@@ -300,17 +308,15 @@
     root_dir = configs.get("root_dir", "ag_bench_runs")
     module = configs["module"]
     benchmark_dir = os.path.join(root_dir, module, benchmark_name)
     tmpdir = None
 
     if configs["mode"] == "aws":
         current_path = os.path.dirname(os.path.abspath(__file__))
-        custom_configs_path = os.path.join(current_path, "custom_configs/amlb_configs")
-        lambda_custom_configs_path = os.path.join(current_path, "cloud/aws/batch_stack/lambdas/amlb_configs")
-        paths = [custom_configs_path, lambda_custom_configs_path]
+        paths = []
         try:
             configs["benchmark_name"] = benchmark_name
             # setting environment variables for docker build ARG
             if dev_branch is not None:
                 os.environ["AG_BENCH_DEV_URL"] = dev_branch  # pull dev branch from GitHub
             else:
                 os.environ[
@@ -341,22 +347,51 @@
 
                     if amlb_user_dir[0].startswith("s3://"):
                         tmpdir = tempfile.TemporaryDirectory()
                         amlb_user_dir_local = download_dir_from_s3(s3_path=amlb_user_dir[0], local_path=tmpdir.name)
                     else:
                         amlb_user_dir_local = amlb_user_dir[0]
 
-                    for path in paths:
-                        _umount_if_needed(path)
-                        _mount_dir(orig_path=amlb_user_dir_local, new_path=path)
-
-                    # after mounting to custom_configs_path, custom_configs_path is copied to $WORKDIR in Dockerfile.
-                    # Contents under AMLB_USER_DIR will be seen in $WORKDIR/amlb_configs
+                    custom_configs_path = os.path.join(current_path, "custom_configs/amlb_configs")
+                    lambda_custom_configs_path = os.path.join(
+                        current_path, "cloud/aws/batch_stack/lambdas/amlb_configs"
+                    )
+                    original_path = amlb_user_dir_local
+                    paths += [custom_configs_path, lambda_custom_configs_path]
                     os.environ["AMLB_USER_DIR"] = "amlb_configs"
                     configs["module_configs"]["tabular"]["amlb_user_dir"] = ["amlb_configs"]
+            elif module == "multimodal":
+                if configs["module_configs"]["multimodal"].get("custom_dataloader") is not None:
+                    custom_dataloader_file = configs["module_configs"]["multimodal"]["custom_dataloader"][
+                        "dataloader_file"
+                    ]
+                    original_path = os.path.dirname(custom_dataloader_file)
+                    custom_dataset_config = configs["module_configs"]["multimodal"]["custom_dataloader"][
+                        "dataset_config_file"
+                    ]
+                    if original_path != os.path.dirname(custom_dataset_config):
+                        raise ValueError(
+                            "Custom dataloader dataset definition <config_file> and dataloader definition <file_path> need to be placed under the same parent directory."
+                        )
+                    dataloader_file_name = os.path.basename(custom_dataloader_file)
+                    dataset_config_file_name = os.path.basename(custom_dataset_config)
+                    custom_dataloader_file = os.path.join(current_path, "custom_configs/dataloaders")
+                    paths.append(custom_dataloader_file)
+                    configs["module_configs"]["multimodal"]["custom_dataloader"][
+                        "dataloader_file"
+                    ] = f"dataloaders/{dataloader_file_name}"
+                    configs["module_configs"]["multimodal"]["custom_dataloader"][
+                        "dataset_config_file"
+                    ] = f"dataloaders/{dataset_config_file_name}"
+
+            for path in paths:
+                # mounting custom directory to a predefined directory in the package
+                # to make it available for Docker build
+                _umount_if_needed(path)
+                _mount_dir(orig_path=original_path, new_path=path)
 
             infra_configs = deploy_stack(custom_configs=configs)
 
             cloud_config_path = _dump_configs(
                 benchmark_dir=benchmark_dir, configs=configs, file_name=os.path.basename(config_file)
             )
             config_s3_path = upload_to_s3(
@@ -380,15 +415,15 @@
                 if remove_resources:
                     logger.info(
                         "Resources will be deleted after the jobs are finished. You can also call \n"
                         f"`agbench destroy-stack --config-file {aws_config_path}` "
                         "to delete the stack after jobs have run to completion if you choose to quit now."
                     )
 
-                failed_jobs = wait_for_jobs_to_complete(config_file=aws_config_path)
+                failed_jobs = wait_for_jobs(config_file=aws_config_path)
                 if len(failed_jobs) > 0:
                     logger.warning("Some jobs have failed: %s.", failed_jobs)
                     if remove_resources:
                         logger.warning("Resources will be kept so error logs can be accessed")
                 elif failed_jobs is None:
                     if remove_resources:
                         logger.error("Resources are not being removed due to errors.")
@@ -407,18 +442,16 @@
         finally:
             for path in paths:
                 _umount_if_needed(path)
 
     elif configs["mode"] == "local":
         split_id = _get_split_id(config_file)
         benchmark_dir_s3 = f"{module}/{benchmark_name}"
-        skip_setup = False
         if split_id is not None:
             benchmark_dir_s3 += f"/{benchmark_name}_{split_id}"
-            skip_setup = True
 
         if module == "tabular":
             amlb_user_dir = configs.get("amlb_user_dir")
             if amlb_user_dir and amlb_user_dir.startswith("s3://"):
                 tmpdir = tempfile.TemporaryDirectory()
                 configs["amlb_user_dir"] = download_dir_from_s3(s3_path=amlb_user_dir, local_path=tmpdir.name)
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/scripts/generate_cloud_configs.py` & `autogluon.bench-0.2.2/src/autogluon/bench/scripts/generate_cloud_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/utils/dataset_utils.py` & `autogluon.bench-0.2.2/src/autogluon/bench/utils/dataset_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,7 +18,12 @@
 def get_repo_url():
     """Return the base URL for dataset repository"""
     default_repo = "https://automl-mm-bench.s3.amazonaws.com"
     repo_url = os.environ.get("AUTOGLUON_BENCH_REPO", default_repo)
     if repo_url[-1] != "/":
         repo_url = repo_url + "/"
     return repo_url
+
+
+def path_expander(path, base_folder):
+    path_l = path.split(";")
+    return ";".join([os.path.abspath(os.path.join(base_folder, path)) for path in path_l])
```

### Comparing `autogluon.bench-0.2.1/src/autogluon/bench/utils/general_utils.py` & `autogluon.bench-0.2.2/src/autogluon/bench/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/src/autogluon.bench.egg-info/PKG-INFO` & `autogluon.bench-0.2.2/src/autogluon.bench.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.bench
-Version: 0.2.1
+Version: 0.2.2
 Summary: A benchmarking tool for AutoML
 Author: AutoGluon Community
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -303,15 +303,22 @@
 For more customizations, please follow the [example custom configuration folder](https://github.com/openml/automlbenchmark/tree/master/examples/custom) provided by AMLB and their [documentation](https://github.com/openml/automlbenchmark/blob/master/docs/HOWTO.md#custom-configuration). 
 
 
 ### Multimodal Benchmark
 
 For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
 
-You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
+You can add more datasets to your benchmarking jobs. We support custom datasets with custom defined data loaders. Follow these steps:
+  1. Create a folder under the working directory, e.g. `custom_dataloader/`
+  2. Create a dataset yaml file, `custom_dataloader/datasets.yaml` which includes all required properties for your problem type, please refer to the [function](https://github.com/autogluon/autogluon-bench/blob/52eee491018f6281236416f4b1bece14b88610e8/src/autogluon/bench/frameworks/multimodal/exec.py#L100-L201).
+  3. Create a dataset loader class, `custom_dataloader/dataloader.py`, which downloads and loads the dataset as a dataframe. Please set the required properties as mentioned above.
+  4. Add `custom_dataloader` in the `agbench run` configuration, where `dataloader_file`, `class_name` and `dataset_config_file` are required. 
+  5. Make sure you have the proper permission to download the dataset. If running in `AWS mode`, we support downloading from the S3 bucket specified as `DATA_BUCKET` in the `agbench run` configuration under the same AWS Batch deployment account.
+
+  Please refer to `sample_configs/dataloaders` for more examples.
 
 ## Run benchmarks on AWS
 
 AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
 
 To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
 
@@ -415,15 +422,15 @@
 ### Monitoring metrics for your instances on AWS
 
 A variety of metrics are available for the EC2 instances that are launched during benchmarking. These can be accessed through the AWS Console by following this navigation path: `CloudWatch` -> `All metrics` -> `AWS namespaces` -> `EC2`. For a comprehensive list of these metrics, refer to the [official AWS documentation](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/viewing_metrics_with_cloudwatch.html).
 
 In addition to the standard metrics, we also provide a custom metric for `GPUUtilization`. This can be found in the `CloudWatch` section under `All metrics` -> `Custom namespaces` -> `EC2`. Please note that the `GPUUtilization` metric is also updated every five minutes.
 
 
-## Evaluating bechmark runs
+## Evaluating benchmark runs
 
 Tabular benchmark results can be evaluated using the tools in `src/autogluon/bench/eval/`. The evaluation logic will aggregate, clean, and produce evaluation results for runs stored in S3.
 In a future release, we intend to add evaluation support for multimodal benchmark results.
 
 
 ### Evaluation Steps
```

### Comparing `autogluon.bench-0.2.1/src/autogluon.bench.egg-info/SOURCES.txt` & `autogluon.bench-0.2.2/src/autogluon.bench.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 sample_configs/multimodal_local_configs.yaml
 sample_configs/tabular_cloud_configs.yaml
 sample_configs/tabular_local_configs.yaml
 sample_configs/amlb_configs/__init__.py
 sample_configs/amlb_configs/config.yaml
 sample_configs/amlb_configs/constraints.yaml
 sample_configs/amlb_configs/frameworks_example.yaml
+sample_configs/dataloaders/text_dataloader.py
+sample_configs/dataloaders/text_datasets.yaml
+sample_configs/dataloaders/vision_dataloader.py
+sample_configs/dataloaders/vision_datasets.yaml
 src/autogluon.bench.egg-info/PKG-INFO
 src/autogluon.bench.egg-info/SOURCES.txt
 src/autogluon.bench.egg-info/dependency_links.txt
 src/autogluon.bench.egg-info/entry_points.txt
 src/autogluon.bench.egg-info/requires.txt
 src/autogluon.bench.egg-info/top_level.txt
 src/autogluon/bench/Dockerfile
@@ -39,14 +43,15 @@
 src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
 src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/amlb_configs/__init__.py
 src/autogluon/bench/custom_configs/amlb_configs/__init__.py
+src/autogluon/bench/custom_configs/dataloaders/__init__.py
 src/autogluon/bench/datasets/__init__.py
 src/autogluon/bench/datasets/constants.py
 src/autogluon/bench/datasets/dataset_registry.py
 src/autogluon/bench/datasets/multimodal_dataset.py
 src/autogluon/bench/datasets/object_detection_dataset.py
 src/autogluon/bench/datasets/registry.py
 src/autogluon/bench/eval/__init__.py
@@ -82,15 +87,15 @@
 src/autogluon/bench/frameworks/tabular/setup.sh
 src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
 src/autogluon/bench/scripts/__init__.py
 src/autogluon/bench/scripts/generate_cloud_configs.py
 src/autogluon/bench/utils/__init__.py
 src/autogluon/bench/utils/dataset_utils.py
 src/autogluon/bench/utils/general_utils.py
-src/autogluon/bench/utils/gpu_utilization.sh
+src/autogluon/bench/utils/hardware_utilization.sh
 tests/unittests/benchmark/conftest.py
 tests/unittests/benchmark/test_benchmark.py
 tests/unittests/benchmark/test_runbenchmarks.py
 tests/unittests/cloud/aws/conftest.py
 tests/unittests/cloud/aws/test_stack.py
 tests/unittests/cloud/aws/test_stack_handler.py
 tests/unittests/datasets/test_registry.py
```

### Comparing `autogluon.bench-0.2.1/tests/unittests/benchmark/test_benchmark.py` & `autogluon.bench-0.2.2/tests/unittests/benchmark/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/tests/unittests/benchmark/test_runbenchmarks.py` & `autogluon.bench-0.2.2/tests/unittests/benchmark/test_runbenchmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 import os
 
 from autogluon.bench.runbenchmark import get_job_status, get_kwargs, invoke_lambda, run, run_benchmark
 
 
-def setup_mock(mocker, tmp_path):
+def setup_mock(mocker, tmp_path, module="tabular"):
     config_file = tmp_path / "config.yaml"
     config_file.touch()
     mock_open = mocker.patch("builtins.open", new_callable=mocker.mock_open)
     mocker.patch("re.search", return_value=False)
     cdk_context = {
         "METRICS_BUCKET": "test_bucket",
     }
@@ -21,27 +21,40 @@
         "STATIC_RESOURCE_STACK_NAME": "test_static_stack",
         "BATCH_STACK_NAME": "test_batch_stack",
         "CDK_DEPLOY_ACCOUNT": "test_account",
         "CDK_DEPLOY_REGION": "test_region",
         "METRICS_BUCKET": "test_bucket",
     }
 
-    module_configs = {
-        "tabular": {
-            "git_uri#branch": "https://github.com/openml/automlbenchmark.git#master",
-            "framework": "AutoGluon:stable",
-            "amlb_benchmark": "small",
-            "amlb_user_dir": "sample_configs/amlb_configs",
+    if module == "tabular":
+        module_configs = {
+            module: {
+                "git_uri#branch": "https://github.com/openml/automlbenchmark.git#master",
+                "framework": "AutoGluon:stable",
+                "amlb_benchmark": "small",
+                "amlb_user_dir": "sample_configs/amlb_configs",
+            }
+        }
+    elif module == "multimodal":
+        module_configs = {
+            module: {
+                "git_uri#branch": "https://github.com/openml/automlbenchmark.git#master",
+                "dataset_name": "data",
+                "custom_dataloader": {
+                    "dataloader_file": "path_to/dataset.py",
+                    "class_name": "CustomDataset",
+                    "dataset_config_file": "path_to/datasets.yaml",
+                },
+            }
         }
-    }
 
     mock_yaml = mocker.patch("yaml.safe_load")
     yaml_value = {
         "mode": "aws",
-        "module": "tabular",
+        "module": module,
         "cdk_context": cdk_context,
         "job_configs": job_configs,
         "module_configs": module_configs,
     }
     yaml_value.update(infra_configs)
     mock_yaml.return_value = yaml_value
     mocker.patch("autogluon.bench.runbenchmark._get_benchmark_name", return_value="test_benchmark")
@@ -49,15 +62,15 @@
     mocker.patch("autogluon.bench.runbenchmark._dump_configs", return_value="test_dump")
     mocker.patch("os.environ.__setitem__")
 
     mock_deploy_stack = mocker.patch("autogluon.bench.runbenchmark.deploy_stack", return_value=infra_configs)
     mock_upload_to_s3 = mocker.patch("autogluon.bench.runbenchmark.upload_to_s3", return_value="test_s3_path")
     mock_invoke_lambda = mocker.patch("autogluon.bench.runbenchmark.invoke_lambda", return_value={})
 
-    mock_wait_for_jobs = mocker.patch("autogluon.bench.runbenchmark.wait_for_jobs_to_complete", return_value=[])
+    mock_wait_for_jobs = mocker.patch("autogluon.bench.runbenchmark.wait_for_jobs", return_value=[])
     mock_destroy_stack = mocker.patch("autogluon.bench.runbenchmark.destroy_stack")
 
     return {
         "config_file": str(config_file),
         "infra_configs": infra_configs,
         "mock_deploy_stack": mock_deploy_stack,
         "mock_upload_to_s3": mock_upload_to_s3,
@@ -89,14 +102,15 @@
         },
         "run_kwargs": {
             "dataset_name": "dataset",
             "framework": "project#master",
             "presets": "preset1",
             "hyperparameters": {},
             "time_limit": 3600,
+            "custom_dataloader": None,
         },
     }
 
     assert get_kwargs(module, configs, agbench_dev_url) == expected_result
 
 
 def test_get_kwargs_tabular():
@@ -152,29 +166,29 @@
         Payload='{"config_file": "test_config_file"}',
     )
 
 
 def test_run_aws_mode(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
 
-    run(setup["config_file"], remove_resources=False, wait=False, dev_branch=None)
+    run(setup["config_file"], remove_resources=False, wait=False, dev_branch=None, skip_setup=True)
 
     setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["custom_configs"])
     setup["mock_upload_to_s3"].assert_called_once_with(
         s3_bucket="test_bucket", s3_dir="configs/test_benchmark_test_time", local_path="test_dump"
     )
     setup["mock_invoke_lambda"].assert_called_once_with(configs=setup["infra_configs"], config_file="test_s3_path")
     setup["mock_wait_for_jobs"].assert_not_called()
     setup["mock_destroy_stack"].assert_not_called()
 
 
 def test_run_aws_mode_remove_resources(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
 
-    run(setup["config_file"], remove_resources=True, wait=False, dev_branch=None)
+    run(setup["config_file"], remove_resources=True, wait=False, dev_branch=None, skip_setup=True)
 
     setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["custom_configs"])
     setup["mock_upload_to_s3"].assert_called_once_with(
         s3_bucket="test_bucket", s3_dir="configs/test_benchmark_test_time", local_path="test_dump"
     )
     setup["mock_invoke_lambda"].assert_called_once_with(configs=setup["infra_configs"], config_file="test_s3_path")
 
@@ -187,30 +201,30 @@
         config_file=None,
     )
 
 
 def test_run_aws_mode_wait(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
 
-    run(setup["config_file"], remove_resources=False, wait=True, dev_branch=None)
+    run(setup["config_file"], remove_resources=False, wait=True, dev_branch=None, skip_setup=True)
 
     setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["custom_configs"])
     setup["mock_upload_to_s3"].assert_called_once_with(
         s3_bucket="test_bucket", s3_dir="configs/test_benchmark_test_time", local_path="test_dump"
     )
     setup["mock_invoke_lambda"].assert_called_once_with(configs=setup["infra_configs"], config_file="test_s3_path")
 
     setup["mock_wait_for_jobs"].assert_called_once_with(config_file="test_dump")
 
 
 def test_run_aws_mode_dev_branch(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
     dev_branch = "dev_branch_url"
 
-    run(setup["config_file"], remove_resources=False, wait=False, dev_branch=dev_branch)
+    run(setup["config_file"], remove_resources=False, wait=False, dev_branch=dev_branch, skip_setup=True)
 
     assert os.environ["AG_BENCH_DEV_URL"] == dev_branch
     setup["mock_deploy_stack"].assert_called_once_with(custom_configs=setup["custom_configs"])
     setup["mock_upload_to_s3"].assert_called_once_with(
         s3_bucket="test_bucket", s3_dir="configs/test_benchmark_test_time", local_path="test_dump"
     )
     setup["mock_invoke_lambda"].assert_called_once_with(configs=setup["infra_configs"], config_file="test_s3_path")
@@ -219,28 +233,58 @@
 def test_run_aws_tabular_user_dir(mocker, tmp_path):
     setup = setup_mock(mocker, tmp_path)
     temp_dir_mock = mocker.patch("tempfile.TemporaryDirectory")
     s3_mock = mocker.patch("autogluon.bench.utils.general_utils.download_dir_from_s3")
     mount_mock = mocker.patch("autogluon.bench.runbenchmark._mount_dir")
     umount_mock = mocker.patch("autogluon.bench.runbenchmark._umount_if_needed")
 
-    run(setup["config_file"], remove_resources=False, wait=False, dev_branch="https://git_url#git_branch")
+    run(
+        setup["config_file"],
+        remove_resources=False,
+        wait=False,
+        dev_branch="https://git_url#git_branch",
+        skip_setup=True,
+    )
     assert os.environ["AG_BENCH_DEV_URL"] == "https://git_url#git_branch"
     assert os.environ["FRAMEWORK_PATH"] == "frameworks/tabular"
     assert os.environ["BENCHMARK_DIR"] == "ag_bench_runs/tabular/test_benchmark_test_time"
     assert os.environ["GIT_URI"] == "https://github.com/openml/automlbenchmark.git"
     assert os.environ["GIT_BRANCH"] == "master"
     assert os.environ["AMLB_FRAMEWORK"] == "AutoGluon:stable"
     assert os.environ["AMLB_USER_DIR"] == "amlb_configs"
     temp_dir_mock.assert_not_called()
     s3_mock.assert_not_called()
     assert umount_mock.call_count == 4
     assert mount_mock.call_count == 2
 
 
+def test_run_aws_multimodal_custom_dataloader(mocker, tmp_path):
+    setup = setup_mock(mocker, tmp_path, module="multimodal")
+    mount_mock = mocker.patch("autogluon.bench.runbenchmark._mount_dir")
+    umount_mock = mocker.patch("autogluon.bench.runbenchmark._umount_if_needed")
+
+    run(
+        setup["config_file"],
+        remove_resources=False,
+        wait=False,
+        dev_branch="https://git_url#git_branch",
+        skip_setup=True,
+    )
+    assert (
+        setup["custom_configs"]["module_configs"]["multimodal"]["custom_dataloader"]["dataloader_file"]
+        == "dataloaders/dataset.py"
+    )
+    assert (
+        setup["custom_configs"]["module_configs"]["multimodal"]["custom_dataloader"]["dataset_config_file"]
+        == "dataloaders/datasets.yaml"
+    )
+    assert umount_mock.call_count == 2
+    assert mount_mock.call_count == 1
+
+
 def test_run_local_mode(mocker, tmp_path):
     config_file = tmp_path / "config_split_test.yaml"
     config_file.touch()
     mock_open = mocker.patch("builtins.open", new_callable=mocker.mock_open)
 
     configs = {
         "mode": "local",
@@ -249,15 +293,15 @@
     }
     mock_yaml = mocker.patch("yaml.safe_load")
     mock_yaml.return_value = configs
     mocker.patch("autogluon.bench.runbenchmark._get_benchmark_name", return_value="test_benchmark")
     mocker.patch("autogluon.bench.runbenchmark.formatted_time", return_value="test_time")
     mock_run_benchmark = mocker.patch("autogluon.bench.runbenchmark.run_benchmark")
 
-    run(str(config_file), remove_resources=False, wait=False, dev_branch=None)
+    run(str(config_file), remove_resources=False, wait=False, dev_branch=None, skip_setup=False)
 
     mock_open.assert_called_with(str(config_file), "r")
     mock_run_benchmark.assert_called_with(
         benchmark_name="test_benchmark_test_time",
         benchmark_dir="ag_bench_runs/tabular/test_benchmark_test_time",
         configs=configs,
         benchmark_dir_s3="tabular/test_benchmark_test_time",
```

### Comparing `autogluon.bench-0.2.1/tests/unittests/cloud/aws/conftest.py` & `autogluon.bench-0.2.2/tests/unittests/cloud/aws/conftest.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/tests/unittests/cloud/aws/test_stack.py` & `autogluon.bench-0.2.2/tests/unittests/cloud/aws/test_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 @patch.dict("os.environ", {"CDK_DEPLOY_REGION": "dummy_region", "CDK_DEPLOY_ACCOUNT": "dummy_account"}, clear=True)
 def test_batch_job_stack():
     app = App()
     for key, value in context_values.items():
         app.node.set_context(key, value)
 
+    os.environ["AG_BENCH_BASE_IMAGE"] = "dummy_base_image"
     os.environ["FRAMEWORK_PATH"] = "frameworks/tabular"
     os.environ["GIT_URI"] = "https://github.com/openml/automlbenchmark.git"
     os.environ["GIT_BRANCH"] = "master"
     os.environ["BENCHMARK_DIR"] = "benchmark_name_20230725"
 
     with patch.object(
         StaticResourceStack,
```

### Comparing `autogluon.bench-0.2.1/tests/unittests/cloud/aws/test_stack_handler.py` & `autogluon.bench-0.2.2/tests/unittests/cloud/aws/test_stack_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     infra_configs_dict = {
         "STACK_NAME_PREFIX": "test-prefix",
         "STACK_NAME_TAG": "benchmark",
         "STATIC_RESOURCE_STACK_NAME": "test-prefix-static-resource-stack",
         "BATCH_STACK_NAME": "test-prefix-batch-stack",
         "CONTAINER_MEMORY": 10000,
         "CDK_DEPLOY_REGION": "us-west-2",
+        "INSTANCE_TYPES": ["m5.2xlarge"],
     }
     custom_configs = {
         "cdk_context": {
             "METRICS_BUCKET": "test-metrics-bucket",
             "DATA_BUCKET": "test-data-bucket",
         },
     }
```

### Comparing `autogluon.bench-0.2.1/tests/unittests/datasets/test_registry.py` & `autogluon.bench-0.2.2/tests/unittests/datasets/test_registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/tests/unittests/utils/test_dataset_utils.py` & `autogluon.bench-0.2.2/tests/unittests/utils/test_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.2.1/tests/unittests/utils/test_general_utils.py` & `autogluon.bench-0.2.2/tests/unittests/utils/test_general_utils.py`

 * *Files identical despite different names*

