# Comparing `tmp/ml-compiler-opt-0.0.1.dev202308080007.tar.gz` & `tmp/ml-compiler-opt-0.0.1.dev202308090007.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-compiler-opt-0.0.1.dev202308080007.tar", last modified: Tue Aug  8 00:07:24 2023, max compression
+gzip compressed data, was "ml-compiler-opt-0.0.1.dev202308090007.tar", last modified: Wed Aug  9 00:07:10 2023, max compression
```

## Comparing `ml-compiler-opt-0.0.1.dev202308080007.tar` & `ml-compiler-opt-0.0.1.dev202308090007.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.680422 ml-compiler-opt-0.0.1.dev202308080007/
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-08 00:07:24.680422 ml-compiler-opt-0.0.1.dev202308080007/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.656422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.660422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_chromium.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_llvm_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_report_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_report_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmarking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/filter_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/gtest_executable_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/list_gtests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.660422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/buffered_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/buffered_scheduler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.660422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/local/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/local/local_worker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/local/local_worker_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/worker_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.660422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48871 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/blackbox_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/blackbox_optimizers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/gradient_ascent_optimization_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/policy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/policy_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/package_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.672422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/agent_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/best_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/best_trajectory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/compilation_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/compilation_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/constant_value_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/constant_value_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/data_collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/data_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/data_reader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.672422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_collect_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_eval_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_reverb_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_reverb_server_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_train_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/env_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/feature_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/feature_ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/gin_external_configurables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.672422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/inlining_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/local_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/local_data_collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/log_reader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/policy_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/policy_saver_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/problem_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/random_net_distillation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/random_net_distillation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.676422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/regalloc_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/regalloc_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/regalloc_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.676422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc_priority/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc_priority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc_priority/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/train_bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/train_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.680422 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/combine_training_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/combine_training_corpus_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/combine_training_corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/extract_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/extract_ir_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/extract_ir_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/feature_importance_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/feature_importance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/feature_importance_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_default_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_default_trace_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_test_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/make_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/make_corpus_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/make_corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/merge_best_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:07:24.680422 ml-compiler-opt-0.0.1.dev202308080007/ml_compiler_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-08 00:07:24.000000 ml-compiler-opt-0.0.1.dev202308080007/ml_compiler_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-08-08 00:07:24.000000 ml-compiler-opt-0.0.1.dev202308080007/ml_compiler_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 00:07:24.000000 ml-compiler-opt-0.0.1.dev202308080007/ml_compiler_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-08 00:07:24.000000 ml-compiler-opt-0.0.1.dev202308080007/ml_compiler_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 00:07:24.000000 ml-compiler-opt-0.0.1.dev202308080007/ml_compiler_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 00:07:00.000000 ml-compiler-opt-0.0.1.dev202308080007/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 00:07:24.680422 ml-compiler-opt-0.0.1.dev202308080007/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.465743 ml-compiler-opt-0.0.1.dev202308090007/
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-09 00:07:10.465743 ml-compiler-opt-0.0.1.dev202308090007/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.449742 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.449742 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_chromium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_llvm_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_report_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_report_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmarking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/filter_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/gtest_executable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/list_gtests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.449742 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/buffered_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/buffered_scheduler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.449742 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/local/local_worker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/local/local_worker_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/worker_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.453743 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48712 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/blackbox_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/blackbox_optimizers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/gradient_ascent_optimization_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/policy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/policy_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/package_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.457743 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/agent_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/best_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/best_trajectory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/compilation_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/compilation_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/constant_value_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/constant_value_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/data_collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/data_reader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.457743 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_collect_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_eval_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_reverb_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_reverb_server_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_train_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/env_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/feature_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/feature_ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/gin_external_configurables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.457743 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/inlining_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/local_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/local_data_collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/log_reader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/policy_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/policy_saver_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/problem_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/random_net_distillation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/random_net_distillation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.461743 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/regalloc_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/regalloc_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/regalloc_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.461743 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc_priority/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc_priority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc_priority/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/train_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/train_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.461743 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/combine_training_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/combine_training_corpus_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/combine_training_corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/extract_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/extract_ir_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/extract_ir_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/feature_importance_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/feature_importance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/feature_importance_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_default_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_default_trace_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_test_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/make_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/make_corpus_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/make_corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/merge_best_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 00:07:10.465743 ml-compiler-opt-0.0.1.dev202308090007/ml_compiler_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-09 00:07:10.000000 ml-compiler-opt-0.0.1.dev202308090007/ml_compiler_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-08-09 00:07:10.000000 ml-compiler-opt-0.0.1.dev202308090007/ml_compiler_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 00:07:10.000000 ml-compiler-opt-0.0.1.dev202308090007/ml_compiler_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-09 00:07:10.000000 ml-compiler-opt-0.0.1.dev202308090007/ml_compiler_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-09 00:07:10.000000 ml-compiler-opt-0.0.1.dev202308090007/ml_compiler_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-09 00:06:53.000000 ml-compiler-opt-0.0.1.dev202308090007/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 00:07:10.465743 ml-compiler-opt-0.0.1.dev202308090007/setup.cfg
```

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/LICENSE` & `ml-compiler-opt-0.0.1.dev202308090007/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/PKG-INFO` & `ml-compiler-opt-0.0.1.dev202308090007/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-compiler-opt
-Version: 0.0.1.dev202308080007
+Version: 0.0.1.dev202308090007
 Summary: Tooling for ML in LLVM
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Infrastructure for MLGO - a Machine Learning Guided Compiler Optimizations Framework.
```

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/README.md` & `ml-compiler-opt-0.0.1.dev202308090007/README.md`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_chromium.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_chromium.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_llvm_test_suite.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_llvm_test_suite.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_report.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_report.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_report_converter.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_report_converter.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmark_report_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmark_report_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/benchmarking_utils.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/benchmarking_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/filter_tests.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/filter_tests.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/gtest_executable_utils.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/gtest_executable_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/benchmark/list_gtests.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/benchmark/list_gtests.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/buffered_scheduler.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/buffered_scheduler.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/buffered_scheduler_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/buffered_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/local/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/local/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/local/local_worker_manager.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/local/local_worker_manager.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/local/local_worker_manager_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/local/local_worker_manager_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/worker.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/worker.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/distributed/worker_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/distributed/worker_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/blackbox_optimizers.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/blackbox_optimizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,64 +50,81 @@
 Library of stateful blackbox optimization algorithms taking as input the values
 of the blackbox function in the neighborhood of a given point and outputting new
 point obtained after conducting one optimization step.
 """
 
 import abc
 import enum
+import gin
 import math
 
 import numpy as np
 import numpy.typing as npt
 import scipy.optimize as sp_opt
 from sklearn import linear_model
 from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 from compiler_opt.es import gradient_ascent_optimization_algorithms
 
-SequenceOfFloats = Union[Sequence[float], npt.NDArray[np.float32]]
+FloatArray = npt.NDArray[np.float32]
+
+# should specifically be a 2d numpy array of floats
+# but numpy.typing does not allow for that indication
+FloatArray2D = Sequence[FloatArray]
+
+SequenceOfFloats = Union[Sequence[float], FloatArray]
 
 LinearModel = Union[linear_model.Ridge, linear_model.Lasso,
                     linear_model.LinearRegression]
 
 
 class CurrentPointEstimate(enum.Enum):
   CURRENT = 1
   AVERAGE = 2
 
 
+@gin.constants_from_enum(module='blackbox_optimizers')
+class Algorithm(enum.Enum):
+  MONTE_CARLO = 1
+  TRUST_REGION = 2
+  SKLEARN_REGRESSION = 3
+
+
+@gin.constants_from_enum(module='blackbox_optimizers')
 class EstimatorType(enum.Enum):
   FORWARD_FD = 1
   ANTITHETIC = 2
 
 
+@gin.constants_from_enum(module='blackbox_optimizers')
 class GradientType(enum.Enum):
   MC = 1
   REGRESSION = 2
 
 
+@gin.constants_from_enum(module='blackbox_optimizers')
 class RegressionType(enum.Enum):
   LASSO = 1
   RIDGE = 2
   LINEAR = 3
 
 
+@gin.constants_from_enum(module='blackbox_optimizers')
 class UpdateMethod(enum.Enum):
   STATE_NORMALIZATION = 1
   NO_METHOD = 2
 
 
 DEFAULT_ARMIJO = 1e-4
 
 
 def filter_top_directions(
-    perturbations: npt.NDArray[np.float32],
-    function_values: npt.NDArray[np.float32], est_type: EstimatorType,
-    num_top_directions: int
-) -> Tuple[npt.NDArray[np.float32], npt.NDArray[np.float32]]:
+    perturbations: FloatArray2D, function_values: FloatArray,
+    est_type: EstimatorType,
+    num_top_directions: int) -> Tuple[FloatArray, FloatArray]:
   """Select the subset of top-performing perturbations.
 
   Args:
     perturbations: np array of perturbations
                    For antithetic, it is assumed that the input puts the pair of
                    p, -p in the even/odd entries, so the directions p_1,...,p_n
                    will be ordered (p_1, -p_1, p_2, -p_2,...)
@@ -147,18 +164,16 @@
 class BlackboxOptimizer(metaclass=abc.ABCMeta):
   """Abstract class for general blackbox optimization.
 
   Class is responsible for encoding different blackbox optimization techniques.
   """
 
   @abc.abstractmethod
-  def run_step(self, perturbations: npt.NDArray[np.float32],
-               function_values: npt.NDArray[np.float32],
-               current_input: npt.NDArray[np.float32],
-               current_value: float) -> npt.NDArray[np.float32]:
+  def run_step(self, perturbations: FloatArray2D, function_values: FloatArray,
+               current_input: FloatArray, current_value: float) -> FloatArray:
     """Conducts a single step of blackbox optimization procedure.
 
     Conducts a single step of blackbox optimization procedure, given values of
     the blackox function in the neighborhood of the current input.
 
     Args:
       perturbations: perturbation directions encoded as 1D numpy arrays
@@ -328,18 +343,17 @@
 
     self.precision_parameter = precision_parameter
     self.num_top_directions = num_top_directions
     self.gradient_ascent_optimizer = gradient_ascent_optimizer
     super().__init__(est_type, normalize_fvalues, hyperparameters_update_method,
                      extra_params)
 
-  def run_step(self, perturbations: npt.NDArray[np.float32],
-               function_values: npt.NDArray[np.float32],
-               current_input: npt.NDArray[np.float32],
-               current_value: float) -> npt.NDArray[np.float32]:
+  # TODO: Issue #285
+  def run_step(self, perturbations: FloatArray2D, function_values: FloatArray,
+               current_input: FloatArray, current_value: float) -> FloatArray:
     dim = len(current_input)
     if self.normalize_fvalues:
       values = function_values.tolist()
       values.append(current_value)
       mean = sum(values) / float(len(values))
       stdev = np.std(np.array(values))
       normalized_values = [(x - mean) / stdev for x in values]
@@ -409,18 +423,16 @@
       self.clf = linear_model.LinearRegression()
     else:
       raise ValueError('Optimization procedure option not available')
     self.gradient_ascent_optimizer = gradient_ascent_optimizer
     super().__init__(est_type, normalize_fvalues, hyperparameters_update_method,
                      extra_params)
 
-  def run_step(self, perturbations: npt.NDArray[np.float32],
-               function_values: npt.NDArray[np.float32],
-               current_input: npt.NDArray[np.float32],
-               current_value: float) -> npt.NDArray[np.float32]:
+  def run_step(self, perturbations: FloatArray2D, function_values: FloatArray,
+               current_input: FloatArray, current_value: float) -> FloatArray:
     dim = len(current_input)
     if self.normalize_fvalues:
       values = function_values.tolist()
       values.append(current_value)
       mean = sum(values) / float(len(values))
       stdev = np.std(np.array(values))
       normalized_values = [(x - mean) / stdev for x in values]
@@ -470,31 +482,30 @@
 
 Implemented: monte_carlo_gradient
              sklearn_regression_gradient
 """
 
 
 def normalize_function_values(
-    function_values: npt.NDArray[np.float32],
-    current_value: float) -> Tuple[npt.NDArray[np.float32], List[float]]:
+    function_values: FloatArray,
+    current_value: float) -> Tuple[FloatArray, List[float]]:
   values = function_values.tolist()
   values.append(current_value)
   mean = sum(values) / float(len(values))
   stdev = np.std(np.array(values))
   normalized_values = [(x - mean) / stdev for x in values]
   return (np.array(normalized_values[:-1]), normalized_values[-1])
 
 
-def monte_carlo_gradient(
-    precision_parameter: float,
-    est_type: EstimatorType,
-    perturbations: npt.NDArray[np.float32],
-    function_values: npt.NDArray[np.float32],
-    current_value: float,
-    energy: Optional[float] = 0) -> npt.NDArray[np.float32]:
+def monte_carlo_gradient(precision_parameter: float,
+                         est_type: EstimatorType,
+                         perturbations: FloatArray2D,
+                         function_values: FloatArray,
+                         current_value: float,
+                         energy: Optional[float] = 0) -> FloatArray:
   """Calculates Monte Carlo gradient.
 
   There are several ways of estimating the gradient. This is specified by the
   attribute self.est_type. Currently, forward finite difference (FFD) and
   antithetic are supported.
 
   Args:
@@ -526,19 +537,18 @@
       np.exp(adj_function_values), sum(np.exp(adj_function_values)))
   gradient = np.zeros(dim)
   for i in range(len(perturbations)):
     gradient += softmax_weights[i] * b_vector[i] * perturbations[i]
   return gradient
 
 
-def sklearn_regression_gradient(
-    clf: LinearModel, est_type: EstimatorType,
-    perturbations: npt.NDArray[np.float32],
-    function_values: npt.NDArray[np.float32],
-    current_value: float) -> npt.NDArray[np.float32]:
+def sklearn_regression_gradient(clf: LinearModel, est_type: EstimatorType,
+                                perturbations: FloatArray2D,
+                                function_values: FloatArray,
+                                current_value: float) -> FloatArray:
   """Calculates gradient by function difference regression.
 
   Args:
     clf: an object (SkLearn linear model) which fits Ax = b
     est_type: 'forward_fd' (FFD) or 'antithetic'
     perturbations: the simulated perturbations
     function_values: reward from perturbations (possibly normalized)
@@ -599,41 +609,41 @@
   Presents an interface for evaluating functions of the form
   f(x) = 1/2x^TAx + b^Tx + c
   """
 
   # pylint: disable=invalid-name
   # argument Av should be capitalized as such for mathematical convention
   def __init__(self,
-               Av: Callable[[npt.NDArray[np.float32]], npt.NDArray[np.float32]],
-               b: npt.NDArray[np.float32],
+               Av: Callable[[FloatArray], FloatArray],
+               b: FloatArray,
                c: Optional[float] = 0):
     """Initialize quadratic function.
 
     Args:
       Av: a function of one argument which returns the matrix-vector product
           A @ v.
       b: the vector b
       c (optional): a constant which is added when evaluating f.
     """
     self.quad_v = Av
     self.b = b
     self.c = c
 
   # pylint: enable=invalid-name
-  def f(self, x: npt.NDArray[np.float32]) -> float:
+  def f(self, x: FloatArray) -> float:
     """Evaluate the quadratic function.
 
     Args:
       x: numpy vector
     Returns:
       Scalar f(x)
     """
     return 0.5 * np.dot(x, self.quad_v(x)) + np.dot(x, self.b) + self.c
 
-  def grad(self, x: npt.NDArray[np.float32]) -> npt.NDArray[np.float32]:
+  def grad(self, x: FloatArray) -> FloatArray:
     """Evaluate the gradient of the quadratic, Ax + b.
 
     Args:
       x: input vector
     Returns:
       A vector of the same dimension as x, the gradient of the quadratic at x.
     """
@@ -649,17 +659,16 @@
    operator onto a closed set.
 
    The functions in this class are non-destructive,
    i.e. the input variables will not be mutated.
   """
 
   def __init__(self, function_object: QuadraticModel,
-               projection_operator: Callable[[npt.NDArray[np.float32]],
-                                             npt.NDArray[np.float32]],
-               pgd_params: Mapping[str, Any], x_init: npt.NDArray[np.float32]):
+               projection_operator: Callable[[FloatArray], FloatArray],
+               pgd_params: Mapping[str, Any], x_init: FloatArray):
     self.f = function_object
     self.proj = projection_operator
     if pgd_params is not None:
       self.params = pgd_params
     else:
       self.params = {}
     self.x = np.copy(x_init)
@@ -694,36 +703,34 @@
     # project step onto feasible set
     x_next = self.proj(self.x + step_size * search_direction)
     # record the size of x^+ - x
     self.x_diff_norm = np.linalg.norm(x_next - self.x, 2)
     self.x = x_next
     self.k += 1
 
-  def get_solution(self) -> npt.NDArray[np.float32]:
+  def get_solution(self) -> FloatArray:
     return self.x
 
   def get_x_diff_norm(self) -> float:
     return self.x_diff_norm
 
   def get_iterations(self) -> int:
     return self.k
 
 
-def make_projector(
-    radius: float
-) -> Callable[[npt.NDArray[np.float32]], npt.NDArray[np.float32]]:
+def make_projector(radius: float) -> Callable[[FloatArray], FloatArray]:
   """Makes an L2 projector function centered at origin.
 
   Args:
     radius: the radius to project on
   Returns:
     A function of one argument that projects onto L2 ball.
   """
 
-  def projector(w: npt.NDArray[np.float32]) -> npt.NDArray[np.float32]:
+  def projector(w: FloatArray) -> FloatArray:
     w_norm = np.linalg.norm(w, 2)
     if w_norm > radius:
       return radius / w_norm * w
     else:
       return w
 
   return projector
@@ -744,15 +751,15 @@
 
    [1] Except for one `bad' case which does not occur almost surely.
   """
 
   def __init__(self,
                model_function: QuadraticModel,
                trust_region_params: Dict[str, Any],
-               x_init: Optional[npt.NDArray[np.float32]] = None):
+               x_init: Optional[FloatArray] = None):
     self.mf = model_function
     self.params = trust_region_params
     self.center = x_init
     self.radius = self.params['radius']
     self.dim = self.params['problem_dim']
     self.params['const_step_size'] = 0.1 * self.radius
     if x_init is not None:
@@ -779,15 +786,15 @@
         pgd_solver.run_step()
         if (pgd_solver.get_x_diff_norm() < self.params['sub_terminate_stable']
             or pgd_solver.get_iterations() > self.params['subproblem_maxiter']):
           inner_loop_termination = True
 
       self.x = pgd_solver.get_solution()
 
-  def get_solution(self) -> npt.NDArray[np.float32]:
+  def get_solution(self) -> FloatArray:
     return self.x
 
 
 """Blackbox Optimization Algorithms
 1. Second Order Trust Region
 """
 
@@ -909,15 +916,15 @@
     if self.params['grad_type'] == GradientType.REGRESSION:
       if self.params['grad_reg_type'] == RegressionType.RIDGE:
         self.clf = linear_model.Ridge(alpha=self.params['grad_reg_alpha'])
       elif self.params['grad_reg_type'] == RegressionType.LASSO:
         self.clf = linear_model.Lasso(alpha=self.params['grad_reg_alpha'])
     self.is_returned_step = False
 
-  def trust_region_test(self, current_input: npt.NDArray[np.float32],
+  def trust_region_test(self, current_input: FloatArray,
                         current_value: float) -> bool:
     """Test the next step to determine how to update the trust region.
 
     The possible outcomes:
       0) If the previous step was rejected and the current point was previously
          accepted, then we can skip the test and immediately return TRUE.
       1) REJECT step
@@ -977,17 +984,17 @@
         elif should_grow:
           self.radius *= self.params['grow_factor']
           print('Grow: ' + str(self.radius) + log_message)
         else:
           print('Unchanged: ' + str(self.radius) + log_message)
     return True
 
-  def update_hessian_part(self, perturbations: npt.NDArray[np.float32],
-                          function_values: npt.NDArray[np.float32],
-                          current_value: float, is_update: bool) -> None:
+  def update_hessian_part(self, perturbations: FloatArray2D,
+                          function_values: FloatArray, current_value: float,
+                          is_update: bool) -> None:
     """Updates the internal state which stores Hessian information.
 
     Recall that the Hessian is given by
     1/s^2 ( EX[f(x+sg)gg^T] - gs(x) I )
     Note that each perturbation passed in is actually s*g, so we have to scale
     down by 1/s^2 /twice/ on the perturbation. This function performs scaling
     by 1/s^2 /once/, and a second scaling is done in create_hessv_function.
@@ -1042,21 +1049,20 @@
         self.saved_function_values = function_values
       else:
         self.saved_perturbations = np.append(
             self.saved_perturbations, perturbations, axis=0)
         self.saved_function_values = np.append(self.saved_function_values,
                                                function_values)
 
-  def create_hessv_function(
-      self) -> Callable[[npt.NDArray[np.float32]], npt.NDArray[np.float32]]:
+  def create_hessv_function(self) -> Callable[[FloatArray], FloatArray]:
     """Returns a function of one argument that evaluates Hessian-vector product.
     """
     if self.params['dense_hessian']:
 
-      def hessv_func(x: npt.NDArray[np.float32]) -> npt.NDArray[np.float32]:
+      def hessv_func(x: FloatArray) -> FloatArray:
         """Calculates Hessian-vector product from dense Hessian.
 
         Args:
           x: the direction to evaluate the product, i.e Hx
         Returns:
           Hessian-vector product.
         """
@@ -1064,15 +1070,15 @@
         # Reminder:
         # If not using sensing-subspace Hessian, also subract diagonal gs(x)*I
         hessv /= np.power(self.precision_parameter, 2)
         hessv *= -1
         return hessv
     else:
 
-      def hessv_func(x: npt.NDArray[np.float32]) -> npt.NDArray[np.float32]:
+      def hessv_func(x: FloatArray) -> FloatArray:
         """Calculates Hessian-vector product from perturbation/value pairs.
 
         Args:
           x: the direction to evaluate the product, i.e Hx
         Returns:
           Hessian-vector product.
         """
@@ -1091,17 +1097,16 @@
         # If not using sensing-subspace Hessian, also subract diagonal gs(x)*I
         hessv /= np.power(self.precision_parameter, 2)
         hessv *= -1
         return hessv
 
     return hessv_func
 
-  def update_quadratic_model(self, perturbations: npt.NDArray[np.float32],
-                             function_values: npt.NDArray[np.float32],
-                             current_value: float,
+  def update_quadratic_model(self, perturbations: FloatArray2D,
+                             function_values: FloatArray, current_value: float,
                              is_update: bool) -> QuadraticModel:
     """Updates the internal state of the optimizer with new perturbations.
 
     The gradient here is the standard Monte Carlo gradient, but could
     be replaced by any other method of gradient estimation.
 
     When performing an update on the same point, we just average the
@@ -1141,18 +1146,16 @@
     else:
       self.saved_gradient = 0.5 * new_gradient + 0.5 * self.saved_gradient
 
     self.update_hessian_part(perturbations, function_values, current_value,
                              is_update)
     return QuadraticModel(self.create_hessv_function(), self.saved_gradient)
 
-  def run_step(self, perturbations: npt.NDArray[np.float32],
-               function_values: npt.NDArray[np.float32],
-               current_input: npt.NDArray[np.float32],
-               current_value: float) -> npt.NDArray[np.float32]:
+  def run_step(self, perturbations: FloatArray2D, function_values: FloatArray,
+               current_input: FloatArray, current_value: float) -> FloatArray:
     """Run a single step of trust region optimizer.
 
     Args:
       perturbations: list of numpy vectors, the perturbations
       function_values: list of scalars, reward corresponding to perturbation
       current_input: numpy vector, current model weights
       current_value: scalar, reward of current model
```

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/blackbox_optimizers_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/blackbox_optimizers_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/gradient_ascent_optimization_algorithms.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/gradient_ascent_optimization_algorithms.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/policy_utils.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/policy_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/es/policy_utils_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/es/policy_utils_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/package_config.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/package_config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/agent_config.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/agent_config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/agent_config_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/agent_config_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/best_trajectory.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/best_trajectory.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/best_trajectory_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/best_trajectory_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/compilation_runner.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/compilation_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/compilation_runner_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/compilation_runner_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/constant.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/constant.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/constant_value_network.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/constant_value_network.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/constant_value_network_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/constant_value_network_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/corpus.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/corpus.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/corpus_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/corpus_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/data_collector.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/data_collector.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/data_collector_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/data_collector_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/data_reader.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/data_reader.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/data_reader_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/data_reader_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/agent.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/agent.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/learner.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/learner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_collect.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_collect.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_collect_lib.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_collect_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_eval.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_eval.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_eval_lib.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_eval_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_reverb_server.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_reverb_server.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_reverb_server_lib.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_reverb_server_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_train.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_train.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/distributed/ppo_train_lib.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/distributed/ppo_train_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/env.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/env.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/env_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/env_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/feature_ops.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/feature_ops.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/feature_ops_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/feature_ops_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/gin_external_configurables.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/gin_external_configurables.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/config.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/env.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/env.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/inlining/inlining_runner.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/inlining/inlining_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/local_data_collector.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/local_data_collector.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/local_data_collector_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/local_data_collector_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/log_reader.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/log_reader.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/log_reader_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/log_reader_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/policy_saver.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/policy_saver.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/policy_saver_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/policy_saver_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/problem_configuration.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/problem_configuration.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/random_net_distillation.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/random_net_distillation.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/random_net_distillation_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/random_net_distillation_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/config.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/regalloc_network.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/regalloc_network.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/regalloc_network_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/regalloc_network_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc/regalloc_runner.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc/regalloc_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc_priority/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc_priority/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc_priority/config.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc_priority/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/registry.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/registry.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/train_bc.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/train_bc.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/train_locally.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/train_locally.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/trainer.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/trainer.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/rl/trainer_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/rl/trainer_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/__init__.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/combine_training_corpus.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/combine_training_corpus.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/combine_training_corpus_lib.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/combine_training_corpus_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/combine_training_corpus_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/combine_training_corpus_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/extract_ir.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/extract_ir.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/extract_ir_lib.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/extract_ir_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/extract_ir_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/extract_ir_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/feature_importance.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/feature_importance.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/feature_importance_graphs.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/feature_importance_graphs.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/feature_importance_utils.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/feature_importance_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/feature_importance_utils_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/feature_importance_utils_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_default_trace.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_default_trace.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_default_trace_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_default_trace_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_test_model.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_test_model.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_test_model_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_test_model_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/generate_vocab.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/generate_vocab.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/make_corpus.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/make_corpus.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/make_corpus_lib.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/make_corpus_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/make_corpus_test.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/make_corpus_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/compiler_opt/tools/merge_best_trajectory.py` & `ml-compiler-opt-0.0.1.dev202308090007/compiler_opt/tools/merge_best_trajectory.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/ml_compiler_opt.egg-info/PKG-INFO` & `ml-compiler-opt-0.0.1.dev202308090007/ml_compiler_opt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-compiler-opt
-Version: 0.0.1.dev202308080007
+Version: 0.0.1.dev202308090007
 Summary: Tooling for ML in LLVM
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Infrastructure for MLGO - a Machine Learning Guided Compiler Optimizations Framework.
```

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/ml_compiler_opt.egg-info/SOURCES.txt` & `ml-compiler-opt-0.0.1.dev202308090007/ml_compiler_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202308080007/pyproject.toml` & `ml-compiler-opt-0.0.1.dev202308090007/pyproject.toml`

 * *Files identical despite different names*

