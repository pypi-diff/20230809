# Comparing `tmp/whylogs-1.2.7.dev0.tar.gz` & `tmp/whylogs-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.2.7.dev0.tar", max compression
+gzip compressed data, was "whylogs-1.2.8.tar", max compression
```

## Comparing `whylogs-1.2.7.dev0.tar` & `whylogs-1.2.8.tar`

### file list

```diff
@@ -1,224 +1,216 @@
--rw-r--r--   0        0        0     3166 2023-07-18 18:56:53.619279 whylogs-1.2.7.dev0/DESCRIPTION.md
--rw-r--r--   0        0        0     6251 2023-08-02 22:20:31.814458 whylogs-1.2.7.dev0/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2023-06-02 03:53:10.537055 whylogs-1.2.7.dev0/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/annotations.py
--rw-r--r--   0        0        0      120 2023-08-01 23:16:01.723078 whylogs-1.2.7.dev0/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0     8157 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/__init__.py
--rw-r--r--   0        0        0     7167 2023-08-01 22:40:10.749895 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/actor.py
--rw-r--r--   0        0        0     2102 2023-08-01 22:41:57.701954 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/data_logger.py
--rw-r--r--   0        0        0      530 2023-08-01 23:40:56.835782 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/future_util.py
--rw-r--r--   0        0        0      650 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/list_util.py
--rw-r--r--   0        0        0     3065 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/process_actor.py
--rw-r--r--   0        0        0    20225 2023-08-01 23:43:19.879837 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
--rw-r--r--   0        0        0     8364 2023-08-01 23:53:21.051980 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
--rw-r--r--   0        0        0      358 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/signal_util.py
--rw-r--r--   0        0        0      579 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/string_util.py
--rw-r--r--   0        0        0     2604 2023-08-01 23:14:48.335040 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
--rw-r--r--   0        0        0    17714 2023-08-01 23:42:37.127827 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
--rw-r--r--   0        0        0     4008 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/time_util.py
--rw-r--r--   0        0        0     4770 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    19765 2023-07-31 20:42:55.305648 whylogs-1.2.7.dev0/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9549 2023-07-31 21:40:30.741870 whylogs-1.2.7.dev0/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2023-07-28 04:07:12.661347 whylogs-1.2.7.dev0/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     6333 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6168 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7663 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0     7497 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      329 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3813 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0    11105 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0      656 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      947 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     2726 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     1169 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2084 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     3408 2023-07-18 18:56:53.631278 whylogs-1.2.7.dev0/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    41758 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0     1217 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0     1090 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3391 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2023-05-10 04:45:16.168865 whylogs-1.2.7.dev0/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30661 2023-08-01 21:48:03.367254 whylogs-1.2.7.dev0/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11486 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4230 2023-07-31 21:40:30.741870 whylogs-1.2.7.dev0/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/errors.py
--rw-r--r--   0        0        0     2560 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     1740 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0     7615 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0     9253 2023-07-31 21:40:30.741870 whylogs-1.2.7.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14608 2023-07-31 21:40:30.741870 whylogs-1.2.7.dev0/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0     7466 2023-08-02 22:21:00.178464 whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2023-08-02 22:20:59.526464 whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    11272 2023-08-02 22:20:59.526464 whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2023-08-02 22:20:59.526464 whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0     9469 2023-08-02 22:21:00.234464 whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2023-08-02 22:20:59.526464 whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0     9516 2023-08-02 22:20:59.426464 whylogs-1.2.7.dev0/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2023-08-02 22:20:59.426464 whylogs-1.2.7.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/relations.py
--rw-r--r--   0        0        0    11357 2023-07-31 21:40:30.741870 whylogs-1.2.7.dev0/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10029 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2118 2023-07-31 21:40:30.741870 whylogs-1.2.7.dev0/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     1602 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      210 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4760 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0      508 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    17663 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     8747 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2023-05-10 04:45:16.172865 whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    14261 2023-07-31 21:40:30.741870 whylogs-1.2.7.dev0/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0     8861 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1554 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    10031 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15367 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/migration/converters.py
--rw-r--r--   0        0        0     6959 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    21751 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2502 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2023-05-10 04:45:16.176864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2023-05-10 04:45:16.180864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2023-05-10 04:45:16.184864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2023-05-10 04:45:16.188864 whylogs-1.2.7.dev0/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2023-05-10 04:45:16.192864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2023-05-10 04:45:16.192864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2023-05-10 04:45:16.192864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2023-05-10 04:45:16.192864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2023-05-10 04:45:16.192864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2023-05-10 04:45:16.192864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    21376 2023-07-28 04:08:05.321355 whylogs-1.2.7.dev0/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1060 2023-07-18 18:56:53.635279 whylogs-1.2.7.dev0/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2023-05-10 04:45:16.196864 whylogs-1.2.7.dev0/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     6759 1970-01-01 00:00:00.000000 whylogs-1.2.7.dev0/PKG-INFO
+-rw-r--r--   0        0        0     3166 2023-08-09 02:29:09.647214 whylogs-1.2.8/DESCRIPTION.md
+-rw-r--r--   0        0        0     5846 2023-08-09 02:29:38.779373 whylogs-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1801 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      120 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0     8157 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
+-rw-r--r--   0        0        0      468 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
+-rw-r--r--   0        0        0     2119 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
+-rw-r--r--   0        0        0    15693 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
+-rw-r--r--   0        0        0     3964 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
+-rw-r--r--   0        0        0     4770 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    19765 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9549 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     6333 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6168 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7663 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0     7497 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      329 2023-08-09 02:29:09.691216 whylogs-1.2.8/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3813 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0    10646 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0      666 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      947 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     2726 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     1169 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2084 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     3408 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    42962 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0     1217 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0     1090 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3391 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30671 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11486 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4230 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/errors.py
+-rw-r--r--   0        0        0     2560 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     1740 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0     7615 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0     9252 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14608 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2023-08-09 02:29:42.279416 whylogs-1.2.8/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2023-08-09 02:29:41.023400 whylogs-1.2.8/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2023-08-09 02:29:41.023400 whylogs-1.2.8/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2023-08-09 02:29:41.023400 whylogs-1.2.8/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2023-08-09 02:29:42.427418 whylogs-1.2.8/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2023-08-09 02:29:41.023400 whylogs-1.2.8/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2023-08-09 02:29:40.923399 whylogs-1.2.8/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2023-08-09 02:29:40.923399 whylogs-1.2.8/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11357 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10029 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2118 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     1602 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      210 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4760 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0      508 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    17663 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     8747 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2023-08-09 02:29:09.695216 whylogs-1.2.8/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0     3530 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    14261 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0     8861 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1554 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    10031 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15367 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     6959 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    21751 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2502 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2023-08-09 02:29:09.699216 whylogs-1.2.8/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2023-08-09 02:29:09.703216 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2023-08-09 02:29:09.707217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2023-08-09 02:29:09.711217 whylogs-1.2.8/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2023-08-09 02:29:09.715217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    21376 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1060 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2023-08-09 02:29:09.719217 whylogs-1.2.8/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     6558 1970-01-01 00:00:00.000000 whylogs-1.2.8/PKG-INFO
```

### Comparing `whylogs-1.2.7.dev0/DESCRIPTION.md` & `whylogs-1.2.8/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/pyproject.toml` & `whylogs-1.2.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.2.7-dev0"
+version = "1.2.8"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
 
@@ -53,18 +53,14 @@
 mlflow-skinny = {version = "^1.26.1", optional = true}
 google-cloud-storage = {version = "^2.5.0", optional = true}
 
 # Pyspark related dependencies
 pyarrow = {version = ">=8.0.0, <13", optional = true}
 pyspark = {version = "^3.0.0", optional = true}
 
-# process logging dependencies
-faster-fifo = {version = "^1.4.5", optional = true}
-orjson = {version = "^3.8.10", optional = true}
-
 # Image support related dependencies
 Pillow = {version = "^9.2.0", optional = true}
 
 # Embeddings support related dependencies
 scikit-learn = [
   { version = "^1.0.2", python = "<3.11", optional = true },
   { version = ">=1.1.2, <2", python = ">=3.11", optional = true }
@@ -143,35 +139,28 @@
 fugue = [
   "fugue",
 ]
 embeddings = [
   "numpy",
   "scikit-learn",
 ]
-proc = [
-  "faster-fifo",  # For much better queue performance than mp.Queue and bulk retrieval
-  "orjson",  # For faster json parsing when serializing data between processes
-  "pandas",  # For merging dataframes during batch processing
-]
 all = [
   "scikit-learn",
   "fugue",
   "Pillow",
   "mlflow-skinny",
   "boto3",
   "google-cloud-storage",
   "pandas",
   "pyarrow",
   "pyspark",
   "ipython",
   "pybars3",
   "numpy",
   "scipy",
-  "faster-fifo",
-  "orjson",
 ]
 
 [tool.poetry.group.dev.dependencies]
 types-urllib3 = "^1.26.25.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `whylogs-1.2.7.dev0/whylogs/__init__.py` & `whylogs-1.2.8/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/annotations.py` & `whylogs-1.2.8/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/fugue/profiler.py` & `whylogs-1.2.8/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/fugue/registry.py` & `whylogs-1.2.8/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/__init__.py` & `whylogs-1.2.8/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/thread_actor.py` & `whylogs-1.2.8/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,91 +1,67 @@
-import queue
-import threading as th
-from typing import Generic, List, Optional, TypeVar
-
-from whylogs.api.logger.experimental.logger.actor.actor import (
-    Actor,
-    QueueConfig,
-    QueueWrapper,
-)
-
-DefaultQueueWrapperType = TypeVar("DefaultQueueWrapperType")
-
-
-class ThreadQueueWrapper(QueueWrapper, Generic[DefaultQueueWrapperType]):
-    """
-    Implementation of QueueWrapper sufficient for use in the threaded actor.
-    """
+import logging
+from abc import ABC, abstractmethod
+from queue import Empty, Full, Queue
+from threading import Event, Thread
+from typing import Generic, TypeVar, Union
 
-    def __init__(self) -> None:
-        self._queue: queue.Queue[DefaultQueueWrapperType] = queue.Queue(100_000)
-
-    def send(self, message: DefaultQueueWrapperType, timeout: float = 0.1) -> None:
-        self._queue.put(message, timeout=timeout)
-
-    def send_many(self, messages: List[DefaultQueueWrapperType], timeout: float = 0.1) -> None:
-        for message in messages:
-            self._queue.put(message, timeout=timeout)
-
-    def get(self, timeout: float = 0.1) -> Optional[DefaultQueueWrapperType]:
-        return self._queue.get(timeout=timeout)
-
-    def get_many(self, timeout: float = 0.1, max: Optional[int] = None) -> List[DefaultQueueWrapperType]:
-        if max is None or max < 1:
-            return []
-
-        messages: List[DefaultQueueWrapperType] = []
-
-        while True:
-            if len(messages) >= max:
-                break
-
-            try:
-                messages.append(self._queue.get(timeout=timeout))
-            except queue.Empty:
-                if len(messages) == 0:
-                    raise queue.Empty
-                else:
-                    break
-
-        return messages
 
-    def size(self) -> int:
-        return self._queue.qsize()
+class CloseMessage:
+    pass
 
 
-ThreadMessageType = TypeVar("ThreadMessageType")
+MessageType = TypeVar("MessageType")
 
 
-class ThreadActor(Actor, th.Thread, Generic[ThreadMessageType]):
-    """
-    Subclass of Actor that uses a thread to process messages.
-    """
-
-    def __init__(self, queue_config: QueueConfig = QueueConfig()) -> None:
-        # our mypy version has a false positive on this super call
-        super().__init__(ThreadQueueWrapper[ThreadMessageType](), queue_config)  # type: ignore
-        self._event = th.Event()
-        self._is_closed = th.Event()
+class MessageProcessor(ABC, Generic[MessageType], Thread):
+    def __init__(self) -> None:
+        super().__init__()
+        self._logger = logging.getLogger(f"{type(self).__name__}_{id(self)}")
+        self._queue: Queue[Union[MessageType, CloseMessage]] = Queue(100_000)
         self.daemon = True
+        self._is_done = Event()
+        self._closed = False
         self.start()
 
     def run(self) -> None:
-        super().run()
+        self._process_messages()
 
-    def is_done(self) -> bool:
-        return self._event.is_set()
-
-    def set_done(self) -> None:
-        self._event.set()
-
-    def done_wait(self) -> None:
-        self._event.wait()
+    def _process_messages(self) -> None:
+        while not self._is_done.is_set():
+            try:
+                message = self._queue.get(timeout=0.1)
+                self._logger.debug(f"Handling message {type(message).__name__}")
+                self._process_message(message)
+            except Empty:
+                if self._closed:
+                    self._logger.info("Done processing message queue")
+                    self._is_done.set()
+            except Full:
+                self._logger.warning("Message queue full")
+            except Exception as e:
+                self._logger.exception(e)
+
+    @abstractmethod
+    def _process_message(self, message: Union[MessageType, CloseMessage]) -> None:
+        pass
+
+    def send(self, message: Union[MessageType, CloseMessage]) -> None:
+        if self._closed:
+            raise Exception("Logger is closed")
 
-    def set_closed(self) -> None:
-        self._is_closed.set()
+        if isinstance(message, CloseMessage):
+            self._closed = True
 
-    def is_closed(self) -> bool:
-        return self._is_closed.is_set()
+        done = False
+        while not done:
+            try:
+                self._queue.put(message, timeout=0.1)
+                done = True
+            except Full:
+                self._logger.warn("Message queue full, trying again")
 
     def close(self) -> None:
-        super().close()
+        self.send(CloseMessage())
+        self._logger.info("Waiting for message processing to finish")
+        self._is_done.wait()
+        self._logger.info("Message processing finished")
+        self.join()
```

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py` & `whylogs-1.2.8/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-import os
 from concurrent.futures import Future
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Any, Callable, Dict, List, Optional, Type, Union, cast
+from typing import Any, Dict, List, Optional, Union
 
+import pandas as pd
 from dateutil import tz
 
-from whylogs.api.logger.experimental.logger.actor.actor import CloseMessage, QueueConfig
-from whylogs.api.logger.experimental.logger.actor.data_logger import (
-    DataLogger,
-    TrackData,
-)
-from whylogs.api.logger.experimental.logger.actor.future_util import wait_result
-from whylogs.api.logger.experimental.logger.actor.thread_actor import ThreadActor
-from whylogs.api.logger.experimental.logger.actor.time_util import (
-    FunctionTimer,
-    Schedule,
-    TimeGranularity,
-    current_time_ms,
-    truncate_time_ms,
-)
 from whylogs.api.logger.result_set import ProfileResultSet, ResultSet
 from whylogs.api.logger.segment_cache import SegmentCache
 from whylogs.api.logger.segment_processing import segment_processing
 from whylogs.api.store import ProfileStore
 from whylogs.api.writer import Writer
 from whylogs.api.writer.writer import Writable
 from whylogs.core import DatasetProfile, DatasetProfileView, DatasetSchema
-from whylogs.core.stubs import pd
+
+from .future_util import wait_result
+from .message_processor import CloseMessage, MessageProcessor
+from .time_util import (
+    FunctionTimer,
+    Schedule,
+    TimeGranularity,
+    current_time_ms,
+    truncate_time_ms,
+)
 
 Row = Dict[str, Any]
+TrackData = Union[pd.DataFrame, Row, List[Row]]
 
 
 class DatasetProfileContainer:
     """
     A container that abstracts over different types of profiles.
 
     This does the work of deciding how to track data and how to create profiles given a DatasetSchema.
@@ -127,27 +123,29 @@
         timestamp_ms: The time in milliseconds when the data occurred.
         result: an optional Future that is fulfilled when the track has completed. It will either
             be a success (None) or a failure (Exception).
     """
 
     data: TrackData
     timestamp_ms: int
-    result: Optional["Future[None]"]
+    result: Optional[Future[None]]
 
 
 @dataclass
 class FlushMessage:
     """
     Trigger a flush, converting all managed profiles to result sets and attempt to write them if there are writers.
     """
 
+    pass
+
 
 @dataclass
 class GetResultsMessage:
-    result: "Future[Dict[int, List[DatasetProfileView]]]"
+    result: Future[Dict[int, List[DatasetProfileView]]]
 
 
 @dataclass
 class LoggerStatus:
     """
     Various status metrics.
 
@@ -173,27 +171,27 @@
 
 @dataclass
 class StatusMessage:
     """
     Get various status metrics.
     """
 
-    result: "Future[LoggerStatus]"
+    result: Future[LoggerStatus]
 
 
 @dataclass
 class PendingWritable:
     attempts: int
     writable: Writable
 
 
-LoggerMessage = Union[TrackMessage, FlushMessage, StatusMessage, GetResultsMessage, CloseMessage]
+LoggerMessage = Union[TrackMessage, FlushMessage, StatusMessage, GetResultsMessage]
 
 
-class ThreadRollingLogger(ThreadActor[LoggerMessage], DataLogger[LoggerStatus]):
+class MultiDatasetRollingLogger(MessageProcessor[LoggerMessage]):
     """
     A logger that manages profiles and segments for various dataset timestamps.
 
     This logger manages a map of dataset timestamp to dataset profile/segment and handles proper
     logging to each type. Given a TimeGranularity to aggregate by, for each call to track(), roughly
     the following will happen:
 
@@ -211,74 +209,63 @@
 
     def __init__(
         self,
         aggregate_by: TimeGranularity = TimeGranularity.Hour,
         write_schedule: Optional[Schedule] = Schedule(cadence=TimeGranularity.Minute, interval=10),
         schema: Optional[DatasetSchema] = None,
         writers: List[Writer] = [],
-        current_time_fn: Optional[Callable[[], int]] = None,
-        queue_config: QueueConfig = QueueConfig(),
     ) -> None:
-        super().__init__(queue_config=queue_config)
         self._aggregate_by = aggregate_by
-        self.current_time_ms = current_time_fn or current_time_ms
         self._cache: Dict[int, DatasetProfileContainer] = {}
-        self._timer: Optional[FunctionTimer] = None
         self._writers: Dict[Writer, List[PendingWritable]] = {}
+        # TODO support stores as well after its updated to be able to handle Writable. This tracks segments
+        # as well as profiles and I would have to manually convert the SegmentCache into a compatible type.
         for writer in writers:
             self._writers[writer] = []
         self._schema: Optional[DatasetSchema] = schema
         self._store_list: List[ProfileStore] = []
 
         if write_schedule is not None:
-            if write_schedule.cadence == TimeGranularity.Second and write_schedule.interval <= 300:
+            if write_schedule.cadence == TimeGranularity.Second:
                 raise Exception("Minimum write schedule is five minutes.")
 
             if write_schedule.cadence == TimeGranularity.Minute and write_schedule.interval < 5:
                 raise Exception("Minimum write schedule is five minutes.")
 
             self._timer = FunctionTimer(write_schedule, self.flush)
         else:
             self._logger.warning(
                 "No write schedule defined for logger. Profiles will only be written after calls to flush()."
             )
 
-        self._logger.debug(f"Created thread logger, pid {os.getpid()}")
+        super().__init__()
 
-    def process_batch(self, batch: List[LoggerMessage], batch_type: Type) -> None:
-        if batch_type == TrackMessage:
-            self._process_track_messages(cast(List[TrackMessage], batch))
-        elif batch_type == FlushMessage:
-            self._process_flush_messages(cast(List[FlushMessage], batch))
-        elif batch_type == CloseMessage:
-            self._process_close_messages(cast(List[CloseMessage], batch))
-        elif batch_type == StatusMessage:
-            self._process_status_messages(cast(List[StatusMessage], batch))
-        elif batch_type == GetResultsMessage:
-            self._process_get_results_messages(cast(List[GetResultsMessage], batch))
+    def _process_message(self, message: Union[LoggerMessage, CloseMessage]) -> None:
+        if isinstance(message, TrackMessage):
+            self._process_track_message(message)
+        elif isinstance(message, FlushMessage):
+            self._process_flush_message(message)
+        elif isinstance(message, CloseMessage):
+            self._process_close_message(message)
+        elif isinstance(message, StatusMessage):
+            self._process_status_message(message)
+        elif isinstance(message, GetResultsMessage):
+            self._process_get_results_message(message)
         else:
             # Safe guard for forgetting to handle a message in development
-            raise Exception(f"Don't know how to handle message {batch_type}")
-
-    def _process_get_results_messages(self, messages: List[GetResultsMessage]) -> None:
-        for message in messages:
-            self._process_get_results_message(message)
+            raise Exception(f"Don't know how to handle message {message}")
 
     def _process_get_results_message(self, message: GetResultsMessage) -> None:
         items: Dict[int, List[DatasetProfileView]] = {}
         for dataset_timestamp, container in self._cache.items():
             self._logger.debug(f"Generating views for dataset timestamp {dataset_timestamp}")
             items[dataset_timestamp] = container.to_views()
 
         message.result.set_result(items)
 
-    def _process_status_messages(self, messages: List[StatusMessage]) -> None:
-        for message in messages:
-            self._process_status_message(message)
-
     def _process_status_message(self, message: StatusMessage) -> None:
         profiles = 0
         segment_caches = 0
         for ts, container in self._cache.items():
             if container._has_segments():
                 segment_caches += 1
             else:
@@ -295,38 +282,28 @@
             dataset_profiles=profiles,
             segment_caches=segment_caches,
             writers=writers,
             pending_writables=writables,
         )
         message.result.set_result(status)
 
-    def _process_close_messages(self, messages: List[CloseMessage]) -> None:
-        for message in messages:
-            self._process_close_message(message)
-
     def _process_close_message(self, message: CloseMessage) -> None:
+        if self._timer is not None:
+            self._timer.stop()
         # Force wait for all writers to handle their pending items
         self._process_flush_message(FlushMessage())
         while self._has_pending():
             self._process_flush_message(FlushMessage())
 
     def _has_pending(self) -> bool:
         has_pending = False
         for writer, pending in self._writers.items():
             has_pending = len(pending) > 0
         return has_pending
 
-    def _process_track_messages(self, messages: List[TrackMessage]) -> None:
-        for message in messages:
-            self._process_track_message(message)
-
-    def _process_flush_messages(self, messages: List[FlushMessage]) -> None:
-        for message in messages:
-            self._process_flush_message(message)
-
     def _process_flush_message(self, message: FlushMessage) -> None:
         for dataset_timestamp, container in self._cache.items():
             self._logger.debug(f"Generating result set for dataset timestamp {dataset_timestamp}")
 
             result_set = container.to_result_set()
             for writable in result_set.get_writables() or []:
                 for pending in self._writers.values():
@@ -369,71 +346,58 @@
         return self._cache[dataset_timestamp]
 
     def _process_track_message(self, message: TrackMessage) -> None:
         try:
             timestamp_ms = message.timestamp_ms
             data = message.data
 
-            ts = timestamp_ms or self.current_time_ms()
+            ts = timestamp_ms or current_time_ms()
             dataset_timestamp = truncate_time_ms(ts, self._aggregate_by)
             profile_container = self._get_profile_container(dataset_timestamp)
-            # TODO consider porting out the aggregation logic that the process rolling logger uses to batch up
-            # data and minimize the amount of track calls. It makes a really big difference.
             profile_container.track(data)
             if message.result is not None:
                 message.result.set_result(None)
         except Exception as e:
             if message.result is not None:
                 message.result.set_exception(e)
 
-    def status(self, timeout: Optional[float] = 1.0) -> LoggerStatus:
-        result: "Future[LoggerStatus]" = Future()
+    def _status(self) -> LoggerStatus:
+        result: Future[LoggerStatus] = Future()
         self.send(StatusMessage(result))
-        return wait_result(result, timeout=timeout)
-
-    def _validate_data(self, data: TrackData) -> None:
-        if not isinstance(data, pd.DataFrame) and not isinstance(data, list) and not isinstance(data, dict):
-            raise Exception(f"Unsupported data type {type(data)}")
+        return wait_result(result)
 
     def log(
         self,
         data: TrackData,
-        timestamp_ms: Optional[int] = None,  # The timestamp that the data happened at
+        timestamp_ms: Optional[int] = None,  # Not the dataset timestamp, but the timestamp of the data
         sync: bool = False,
     ) -> None:
         """
         Log some data.
 
         Parameters:
             data: The data to log. This can either be a pandas data frame, a row (dictionary of str to str/int/float/etc),
                 or a list of rows.
             timestamp_ms: The timestamp of the data. If this isn't supplied then it is assumed to have happened now.
             sync: Whether or not to perform this action synchronously. By default, this is an asynchronous operation.
                 You can make this synchronous in order to react to errors. Mostly useful when initially setting up
                 logging since the only errors that can be responded to are data format related.
         """
-        self._validate_data(data)
 
-        result: Optional["Future[None]"] = Future() if sync else None
-        self.send(TrackMessage(data=data, timestamp_ms=timestamp_ms or self.current_time_ms(), result=result))
+        result: Optional[Future[None]] = Future() if sync else None
+        self.send(TrackMessage(data=data, timestamp_ms=timestamp_ms or current_time_ms(), result=result))
         if result is not None:
-            self._logger.debug("Waiting for track to complete")
             wait_result(result)
 
     def flush(self) -> None:
         """
         Flush the internal state, causing everything to be written using the configured writers.
         """
         self.send(FlushMessage())
 
     def get_profile_views(self) -> Dict[int, List[DatasetProfileView]]:
         """
         Get all of the profile views for each dataset timestamp being maintained.
         """
-        result: "Future[Dict[int, List[DatasetProfileView]]]" = Future()
+        result: Future[Dict[int, List[DatasetProfileView]]] = Future()
         self.send(GetResultsMessage(result))
         return wait_result(result)
-
-    def close(self) -> None:
-        if self._timer is not None:
-            self._timer.stop()
-        super().close()
```

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/experimental/logger/actor/time_util.py` & `whylogs-1.2.8/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,12 +95,11 @@
         self._timer.start()
         self._fn()
 
     def is_alive(self) -> bool:
         return self._timer.is_alive()
 
     def stop(self) -> None:
-        self._logger.info("Stopping timer")
         if not self._running:
             raise Exception("Timer already stopped")
         self._timer.cancel()
         self._running = False
```

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/logger.py` & `whylogs-1.2.8/whylogs/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/result_set.py` & `whylogs-1.2.8/whylogs/api/logger/result_set.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/rolling.py` & `whylogs-1.2.8/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/segment_cache.py` & `whylogs-1.2.8/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/segment_processing.py` & `whylogs-1.2.8/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/logger/transient.py` & `whylogs-1.2.8/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.2.8/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.2.8/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/reader/local.py` & `whylogs-1.2.8/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/reader/reader.py` & `whylogs-1.2.8/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/reader/s3.py` & `whylogs-1.2.8/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/store/local_store.py` & `whylogs-1.2.8/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/store/profile_store.py` & `whylogs-1.2.8/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/store/query.py` & `whylogs-1.2.8/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/store/sqlite_store.py` & `whylogs-1.2.8/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/usage_stats/__init__.py` & `whylogs-1.2.8/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/whylabs/session/config.py` & `whylogs-1.2.8/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.2.8/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.2.8/whylogs/api/whylabs/session/session_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,18 +42,14 @@
 class UploadReferenceResult:
     viewing_url: str
     whylabs_response: BatchLogSessionReferenceResponse
 
 
 class Session(ABC):
     @abstractmethod
-    def get_config(self) -> SessionConfig:
-        raise NotImplementedError()
-
-    @abstractmethod
     def get_type(self) -> SessionType:
         raise NotImplementedError()
 
     @abstractmethod
     def upload_reference_profiles(
         self, profile_aliases: Dict[str, ResultSet]
     ) -> Union[UploadReferenceResult, NotSupported]:
@@ -73,17 +69,14 @@
         self._whylabs_session_api = SessionsApi(whylabs_client)
         self._user_guid = self._get_or_create_user_guid()
         self._session_id = self._get_or_create_session_id()
         config_path = config.get_config_file_path()
         emit_usage("guest_session")
         log_if_notebook(f"Initialized anonymous session with id {self._session_id} in config {config_path}")
 
-    def get_config(self) -> SessionConfig:
-        return self._config
-
     def get_type(self) -> SessionType:
         return SessionType.WHYLABS_ANONYMOUS
 
     def _validate_config_session(self) -> Optional[str]:
         """
         Look up the current config value for the session and make sure it's still valid by
         calling WhyLabs. If it's not valid, remove it from the config and return None.
@@ -185,35 +178,27 @@
             return UploadReferenceResult(viewing_url=viewing_url, whylabs_response=response)
         except ApiException as e:
             logger.error(e)
             raise e
 
 
 class LocalSession(Session):
-    def __init__(self, config: SessionConfig) -> None:
-        super().__init__()
-        self._config = config
-
-    def get_config(self) -> SessionConfig:
-        return self._config
-
     def get_type(self) -> SessionType:
         return SessionType.LOCAL
 
     def upload_reference_profiles(
         self, profile_aliases: Dict[str, ResultSet]
     ) -> Union[UploadReferenceResult, NotSupported]:
         return NotSupported()
 
 
 class ApiKeySession(Session):
     def __init__(self, config: SessionConfig) -> None:
         from whylogs.api.usage_stats import emit_usage
 
-        self._config = config
         self.api_key = config.get_api_key()
         self.org_id = config.get_org_id()
 
         if self.api_key is None and is_notebook():
             self.api_key = config.get_or_prompt_api_key(persist=True)
         else:
             logger.warning("No api key found in session or configuration, will not be able to send data to whylabs.")
@@ -222,17 +207,14 @@
             self.org_id = config.get_or_prompt_org_id(persist=True)
         else:
             logger.warning("No org id found in session or configuration, will not be able to send data to whylabs.")
         emit_usage("api_key_session")
         if is_notebook():
             log_if_notebook(f"Initialized whylabs session with for org {self.org_id}")
 
-    def get_config(self) -> SessionConfig:
-        return self._config
-
     def get_type(self) -> SessionType:
         return SessionType.WHYLABS
 
     def upload_reference_profiles(
         self, profile_aliases: Dict[str, ResultSet]
     ) -> Union[UploadReferenceResult, NotSupported]:
         # TODO support soon
```

### Comparing `whylogs-1.2.7.dev0/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.2.8/whylogs/api/whylabs/session/session_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 # This is used to indicate that a result is either a success or a failure
 class NotSupported:
     """
     Indicates that one of the session apis isn't supported for the current session type.
     """
 
+    pass
+
 
 def init_notebook_logging() -> None:
     global _is_notebook
     if is_notebook():
         _is_notebook = True
```

### Comparing `whylogs-1.2.7.dev0/whylogs/api/writer/__init__.py` & `whylogs-1.2.8/whylogs/api/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/writer/gcs.py` & `whylogs-1.2.8/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/writer/local.py` & `whylogs-1.2.8/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/writer/mlflow.py` & `whylogs-1.2.8/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/writer/s3.py` & `whylogs-1.2.8/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/api/writer/whylabs.py` & `whylogs-1.2.8/whylogs/api/writer/whylabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import tempfile
 from typing import IO, Any, Dict, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import requests  # type: ignore
 import whylabs_client  # type: ignore
-from urllib3 import PoolManager, ProxyManager
+from urllib3 import PoolManager, ProxyManager, util
 from whylabs_client import ApiClient, Configuration  # type: ignore
 from whylabs_client.api.dataset_profile_api import DatasetProfileApi
 from whylabs_client.api.feature_weights_api import FeatureWeightsApi
 from whylabs_client.api.log_api import AsyncLogResponse  # type: ignore
 from whylabs_client.api.log_api import (
     LogApi,
     LogAsyncRequest,
@@ -115,14 +115,23 @@
     if len(api_key) > 80:
         raise ValueError("API key too long")
     if api_key[10] != ".":
         raise ValueError("Invalid format. Expecting a dot at an index 10")
     return api_key[:10]
 
 
+def _get_auth_headers(proxy_url: str) -> Dict[str, str]:
+    parsed_url = urlparse(proxy_url)
+    if parsed_url.username and parsed_url.password:
+        default_headers = util.make_headers(proxy_basic_auth=f"{str(parsed_url.username)}:{str(parsed_url.password)}")
+    else:
+        default_headers = None
+    return default_headers
+
+
 class KeyRefresher(abc.ABC):
     @property
     @abc.abstractmethod
     def key_id(self) -> str:
         pass
 
     @abc.abstractmethod
@@ -225,14 +234,18 @@
         self._dataset_id = dataset_id or os.environ.get("WHYLABS_DEFAULT_DATASET_ID")
         self._feature_weights = None
         self.whylabs_api_endpoint = os.environ.get("WHYLABS_API_ENDPOINT") or "https://api.whylabsapp.com"
         self._reference_profile_name = os.environ.get("WHYLABS_REFERENCE_PROFILE_NAME")
         self._ssl_ca_cert = ssl_ca_cert
         self._api_config: Optional[Configuration] = None
 
+        _http_proxy = os.environ.get("HTTP_PROXY")
+        _https_proxy = os.environ.get("HTTPS_PROXY")
+        self._proxy = _https_proxy or _http_proxy
+
         if api_key:
             self._key_refresher = StaticKeyRefresher(api_key)
         else:
             self._key_refresher = _ENV_KEY_REFRESHER
         if api_client:
             self._api_client = api_client
         else:
@@ -257,20 +270,32 @@
         if _timeout_seconds is not None:
             self._timeout_seconds = _timeout_seconds
 
         # Using a pooler for uploading data
         pool = _UPLOAD_POOLER_CACHE.get(pooler_cache_key)
         if pool is None:
             logger.debug(f"Pooler is not available. Creating a new one for key: {pooler_cache_key}")
-            pool = PoolManager(
-                num_pools=4,
-                maxsize=10,
-                assert_hostname=self._s3_endpoint_subject,
-                server_hostname=self._s3_endpoint_subject,
-            )
+            if self._proxy:
+                proxy_url = self._proxy
+                default_headers = _get_auth_headers(proxy_url)
+                pool = ProxyManager(
+                    proxy_url,
+                    num_pools=4,
+                    maxsize=10,
+                    proxy_headers=default_headers,
+                    assert_hostname=self._s3_endpoint_subject,
+                    server_hostname=self._s3_endpoint_subject,
+                )
+            else:
+                pool = PoolManager(
+                    num_pools=4,
+                    maxsize=10,
+                    assert_hostname=self._s3_endpoint_subject,
+                    server_hostname=self._s3_endpoint_subject,
+                )
             self._s3_pool = pool
             _UPLOAD_POOLER_CACHE[pooler_cache_key] = pool
         else:
             self._s3_pool = pool
 
     @property
     def key_id(self) -> str:
@@ -289,15 +314,19 @@
             config = copy.deepcopy(self._api_client.configuration)
         else:
             config = Configuration()
         # Set an empty api key. The key refresher will refresh it
         config.api_key = {"ApiKeyAuth": ""}
         config.refresh_api_key_hook = self._key_refresher
         cache_key += str(hash(self._key_refresher))
-
+        if self._proxy:
+            config.proxy = self._proxy
+            default_header = _get_auth_headers(self._proxy)
+            if default_header:
+                config.proxy_headers = default_header
         config.discard_unknown_keys = True
         # Disable client side validation and trust the server
         config.client_side_validation = False
 
         cache_key += str(hash(config))
         if self._ssl_ca_cert:
             config.ssl_ca_cert = self._ssl_ca_cert
```

### Comparing `whylogs-1.2.7.dev0/whylogs/api/writer/writer.py` & `whylogs-1.2.8/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/__init__.py` & `whylogs-1.2.8/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/column_profile.py` & `whylogs-1.2.8/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/configs.py` & `whylogs-1.2.8/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.2.8/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.2.8/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.2.8/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.2.8/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.2.8/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.2.8/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.2.8/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.2.8/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.2.8/whylogs/core/constraints/metric_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,16 @@
 class MissingMetric(Exception):
     """
     DatasetConstraint conditions can raise this exception to indicate that
     a required metric or column could not be found in the DatasetProfileView.
     The DatasetConstraint is responsible for handling this exception.
     """
 
+    pass
+
 
 @dataclass(frozen=True)
 class DatasetComparisonConstraint:
     """
     Implements dataset-level constraints that require a reference dataset to
     be compared against. The condition Callable takes the DatasetProfileView
     of the dataset to be validated as well as the DatasetProfileView of the
```

### Comparing `whylogs-1.2.7.dev0/whylogs/core/dataset_profile.py` & `whylogs-1.2.8/whylogs/core/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/datatypes.py` & `whylogs-1.2.8/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/errors.py` & `whylogs-1.2.8/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/feature_weights.py` & `whylogs-1.2.8/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/input_resolver.py` & `whylogs-1.2.8/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metric_getters.py` & `whylogs-1.2.8/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/__init__.py` & `whylogs-1.2.8/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/aggregators.py` & `whylogs-1.2.8/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/column_metrics.py` & `whylogs-1.2.8/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/compound_metric.py` & `whylogs-1.2.8/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.2.8/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/decorators.py` & `whylogs-1.2.8/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/deserializers.py` & `whylogs-1.2.8/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/maths.py` & `whylogs-1.2.8/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/metric_components.py` & `whylogs-1.2.8/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/metrics.py` & `whylogs-1.2.8/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/multimetric.py` & `whylogs-1.2.8/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/serializers.py` & `whylogs-1.2.8/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/metrics/unicode_range.py` & `whylogs-1.2.8/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.2.8/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             doubles=DoublesMessage(count=dist.n),
         )
 
     @staticmethod
     def _numbers_to_dist(numbers: NumbersMessageV0) -> DistributionMetric:
         try:
             doubles_sk = ds.kll_doubles_sketch.deserialize(numbers.histogram)
-        except ValueError:
+        except Exception:
             # Fall back to KLL float for backward compatibility and convert it to doubles sketch
             sk = ds.kll_floats_sketch.deserialize(numbers.histogram)
             doubles_sk = ds.kll_floats_sketch.float_to_doubles(sk)
         return DistributionMetric(
             kll=KllComponent(doubles_sk),
             mean=FractionalComponent(numbers.variance.mean),
             m2=FractionalComponent(numbers.variance.sum),
```

### Comparing `whylogs-1.2.7.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.2.8/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.2.8/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/predicate_parser.py` & `whylogs-1.2.8/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/preprocessing.py` & `whylogs-1.2.8/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.2.8/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.2.8/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.2.8/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.2.8/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/relations.py` & `whylogs-1.2.8/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/resolvers.py` & `whylogs-1.2.8/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/schema.py` & `whylogs-1.2.8/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/segmentation_partition.py` & `whylogs-1.2.8/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/specialized_resolvers.py` & `whylogs-1.2.8/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/stubs.py` & `whylogs-1.2.8/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.2.8/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/utils/stats_calculations.py` & `whylogs-1.2.8/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/utils/utils.py` & `whylogs-1.2.8/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/validators/condition_validator.py` & `whylogs-1.2.8/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/view/column_profile_view.py` & `whylogs-1.2.8/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.2.8/whylogs/core/view/dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.2.8/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/base.py` & `whylogs-1.2.8/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/configs.py` & `whylogs-1.2.8/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.2.8/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/descr/employee.rst` & `whylogs-1.2.8/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/descr/weather.rst` & `whylogs-1.2.8/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/ecommerce.py` & `whylogs-1.2.8/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/employee.py` & `whylogs-1.2.8/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/utils.py` & `whylogs-1.2.8/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/datasets/weather.py` & `whylogs-1.2.8/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/api/logger/__init__.py` & `whylogs-1.2.8/whylogs/experimental/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.2.8/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.2.8/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.2.8/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.2.8/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.2.8/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.2.8/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.2.8/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.2.8/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/core/udf_schema.py` & `whylogs-1.2.8/whylogs/experimental/core/udf_schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.2.8/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.2.8/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.2.8/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.2.8/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.2.8/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.2.8/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/extras/image_metric.py` & `whylogs-1.2.8/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/migration/converters.py` & `whylogs-1.2.8/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/migration/uncompound.py` & `whylogs-1.2.8/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.2.8/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/drift/configs.py` & `whylogs-1.2.8/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/enums/enums.py` & `whylogs-1.2.8/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.2.8/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.2.8/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.2.8/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.2.8/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.2.8/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.2.8/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.2.8/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.2.8/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/js/d3.min.js` & `whylogs-1.2.8/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/js/handlebars.js` & `whylogs-1.2.8/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.2.8/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.2.8/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/html/templates/index.html` & `whylogs-1.2.8/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.2.8/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.2.8/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.2.8/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.2.8/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.2.8/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.2.8/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.2.8/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.2.8/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.7.dev0/PKG-INFO` & `whylogs-1.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.2.7.dev0
+Version: 1.2.8
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,35 +17,32 @@
 Provides-Extra: datasets
 Provides-Extra: docs
 Provides-Extra: embeddings
 Provides-Extra: fugue
 Provides-Extra: gcs
 Provides-Extra: image
 Provides-Extra: mlflow
-Provides-Extra: proc
 Provides-Extra: s3
 Provides-Extra: spark
 Provides-Extra: viz
 Requires-Dist: Pillow (>=9.2.0,<10.0.0) ; extra == "viz" or extra == "image" or extra == "all"
 Requires-Dist: boto3 (>=1.22.13,<2.0.0) ; extra == "s3" or extra == "all"
-Requires-Dist: faster-fifo (>=1.4.5,<2.0.0) ; extra == "proc" or extra == "all"
 Requires-Dist: fugue (>=0.8.1,<0.9.0) ; extra == "fugue" or extra == "all"
 Requires-Dist: furo (>=2022.3.4,<2023.0.0) ; extra == "docs"
 Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0) ; extra == "gcs" or extra == "all"
 Requires-Dist: importlib-metadata (<4.3) ; python_version < "3.8"
 Requires-Dist: ipython ; extra == "viz" or extra == "all"
 Requires-Dist: ipython_genutils (>=0.2.0,<0.3.0) ; extra == "docs"
 Requires-Dist: mlflow-skinny (>=1.26.1,<2.0.0) ; extra == "mlflow" or extra == "all"
 Requires-Dist: myst-parser[sphinx] (>=0.17.2,<0.18.0) ; extra == "docs"
 Requires-Dist: nbconvert (>=7.0.0,<8.0.0) ; extra == "docs"
 Requires-Dist: nbsphinx (>=0.8.9,<0.9.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.23.2) ; (python_version >= "3.11") and (extra == "viz" or extra == "embeddings" or extra == "all")
 Requires-Dist: numpy ; (python_version < "3.11") and (extra == "viz" or extra == "embeddings" or extra == "all")
-Requires-Dist: orjson (>=3.8.10,<4.0.0) ; extra == "proc" or extra == "all"
-Requires-Dist: pandas ; extra == "datasets" or extra == "proc" or extra == "all"
+Requires-Dist: pandas ; extra == "datasets" or extra == "all"
 Requires-Dist: platformdirs (>=3.5.0,<4.0.0)
 Requires-Dist: protobuf (>=3.19.4)
 Requires-Dist: pyarrow (>=8.0.0,<13) ; extra == "spark" or extra == "all"
 Requires-Dist: pybars3 (>=0.9,<0.10) ; extra == "viz" or extra == "all"
 Requires-Dist: pyspark (>=3.0.0,<4.0.0) ; extra == "spark" or extra == "all"
 Requires-Dist: requests (>=2.27,<3.0)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0) ; (python_version < "3.11") and (extra == "embeddings" or extra == "all")
```

#### html2text {}

```diff
@@ -1,56 +1,54 @@
-Metadata-Version: 2.1 Name: whylogs Version: 1.2.7.dev0 Summary: Profile and
-monitor your ML data pipeline end-to-end Home-page: https://docs.whylabs.ai
-License: Apache-2.0 Author: WhyLabs.ai Author-email: support@whylabs.ai
-Requires-Python: >=3.7.1,<4 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
-datasets Provides-Extra: docs Provides-Extra: embeddings Provides-Extra: fugue
-Provides-Extra: gcs Provides-Extra: image Provides-Extra: mlflow Provides-
-Extra: proc Provides-Extra: s3 Provides-Extra: spark Provides-Extra: viz
-Requires-Dist: Pillow (>=9.2.0,<10.0.0) ; extra == "viz" or extra == "image" or
-extra == "all" Requires-Dist: boto3 (>=1.22.13,<2.0.0) ; extra == "s3" or extra
-== "all" Requires-Dist: faster-fifo (>=1.4.5,<2.0.0) ; extra == "proc" or extra
-== "all" Requires-Dist: fugue (>=0.8.1,<0.9.0) ; extra == "fugue" or extra ==
-"all" Requires-Dist: furo (>=2022.3.4,<2023.0.0) ; extra == "docs" Requires-
-Dist: google-cloud-storage (>=2.5.0,<3.0.0) ; extra == "gcs" or extra == "all"
+Metadata-Version: 2.1 Name: whylogs Version: 1.2.8 Summary: Profile and monitor
+your ML data pipeline end-to-end Home-page: https://docs.whylabs.ai License:
+Apache-2.0 Author: WhyLabs.ai Author-email: support@whylabs.ai Requires-Python:
+>=3.7.1,<4 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: datasets
+Provides-Extra: docs Provides-Extra: embeddings Provides-Extra: fugue Provides-
+Extra: gcs Provides-Extra: image Provides-Extra: mlflow Provides-Extra: s3
+Provides-Extra: spark Provides-Extra: viz Requires-Dist: Pillow
+(>=9.2.0,<10.0.0) ; extra == "viz" or extra == "image" or extra == "all"
+Requires-Dist: boto3 (>=1.22.13,<2.0.0) ; extra == "s3" or extra == "all"
+Requires-Dist: fugue (>=0.8.1,<0.9.0) ; extra == "fugue" or extra == "all"
+Requires-Dist: furo (>=2022.3.4,<2023.0.0) ; extra == "docs" Requires-Dist:
+google-cloud-storage (>=2.5.0,<3.0.0) ; extra == "gcs" or extra == "all"
 Requires-Dist: importlib-metadata (<4.3) ; python_version < "3.8" Requires-
 Dist: ipython ; extra == "viz" or extra == "all" Requires-Dist:
 ipython_genutils (>=0.2.0,<0.3.0) ; extra == "docs" Requires-Dist: mlflow-
 skinny (>=1.26.1,<2.0.0) ; extra == "mlflow" or extra == "all" Requires-Dist:
 myst-parser[sphinx] (>=0.17.2,<0.18.0) ; extra == "docs" Requires-Dist:
 nbconvert (>=7.0.0,<8.0.0) ; extra == "docs" Requires-Dist: nbsphinx
 (>=0.8.9,<0.9.0) ; extra == "docs" Requires-Dist: numpy (>=1.23.2) ;
 (python_version >= "3.11") and (extra == "viz" or extra == "embeddings" or
 extra == "all") Requires-Dist: numpy ; (python_version < "3.11") and (extra ==
-"viz" or extra == "embeddings" or extra == "all") Requires-Dist: orjson
-(>=3.8.10,<4.0.0) ; extra == "proc" or extra == "all" Requires-Dist: pandas ;
-extra == "datasets" or extra == "proc" or extra == "all" Requires-Dist:
-platformdirs (>=3.5.0,<4.0.0) Requires-Dist: protobuf (>=3.19.4) Requires-Dist:
-pyarrow (>=8.0.0,<13) ; extra == "spark" or extra == "all" Requires-Dist:
-pybars3 (>=0.9,<0.10) ; extra == "viz" or extra == "all" Requires-Dist: pyspark
-(>=3.0.0,<4.0.0) ; extra == "spark" or extra == "all" Requires-Dist: requests
-(>=2.27,<3.0) Requires-Dist: scikit-learn (>=1.0.2,<2.0.0) ; (python_version <
-"3.11") and (extra == "embeddings" or extra == "all") Requires-Dist: scikit-
-learn (>=1.1.2,<2) ; (python_version >= "3.11") and (extra == "embeddings" or
-extra == "all") Requires-Dist: scipy (>=1.5) ; (python_version < "3.11") and
-(extra == "viz" or extra == "all") Requires-Dist: scipy (>=1.9.2) ;
-(python_version >= "3.11") and (extra == "viz" or extra == "all") Requires-
-Dist: sphinx ; extra == "docs" Requires-Dist: sphinx-autoapi ; extra == "docs"
-Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
-Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0) ; extra == "docs" Requires-
-Dist: sphinx-inline-tabs ; (python_version >= "3.8" and python_version < "4")
-and (extra == "docs") Requires-Dist: sphinxext-opengraph (>=0.6.3,<0.7.0) ;
-extra == "docs" Requires-Dist: types-requests (>=2.30.0.0,<3.0.0.0) Requires-
-Dist: typing-extensions (>=3.10) ; python_version < "4" Requires-Dist: whylabs-
-client (>=0.5.1,<1) Requires-Dist: whylogs-sketching (>=3.4.1.dev3)
-Description-Content-Type: text/markdown [https://static.scarf.sh/a.png?x-
-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
+"viz" or extra == "embeddings" or extra == "all") Requires-Dist: pandas ; extra
+== "datasets" or extra == "all" Requires-Dist: platformdirs (>=3.5.0,<4.0.0)
+Requires-Dist: protobuf (>=3.19.4) Requires-Dist: pyarrow (>=8.0.0,<13) ; extra
+== "spark" or extra == "all" Requires-Dist: pybars3 (>=0.9,<0.10) ; extra ==
+"viz" or extra == "all" Requires-Dist: pyspark (>=3.0.0,<4.0.0) ; extra ==
+"spark" or extra == "all" Requires-Dist: requests (>=2.27,<3.0) Requires-Dist:
+scikit-learn (>=1.0.2,<2.0.0) ; (python_version < "3.11") and (extra ==
+"embeddings" or extra == "all") Requires-Dist: scikit-learn (>=1.1.2,<2) ;
+(python_version >= "3.11") and (extra == "embeddings" or extra == "all")
+Requires-Dist: scipy (>=1.5) ; (python_version < "3.11") and (extra == "viz" or
+extra == "all") Requires-Dist: scipy (>=1.9.2) ; (python_version >= "3.11") and
+(extra == "viz" or extra == "all") Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: sphinx-autoapi ; extra == "docs" Requires-Dist: sphinx-autobuild
+(>=2021.3.14,<2022.0.0) ; extra == "docs" Requires-Dist: sphinx-copybutton
+(>=0.5.0,<0.6.0) ; extra == "docs" Requires-Dist: sphinx-inline-tabs ;
+(python_version >= "3.8" and python_version < "4") and (extra == "docs")
+Requires-Dist: sphinxext-opengraph (>=0.6.3,<0.7.0) ; extra == "docs" Requires-
+Dist: types-requests (>=2.30.0.0,<3.0.0.0) Requires-Dist: typing-extensions
+(>=3.10) ; python_version < "4" Requires-Dist: whylabs-client (>=0.5.1,<1)
+Requires-Dist: whylogs-sketching (>=3.4.1.dev3) Description-Content-Type: text/
+markdown [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-
+f711c4d35b82]
                       [https://i.imgur.com/nv33goV.png]
                ****** The open standard for data logging ******
  **** Documentation • Slack_Community • Python_Quickstart • WhyLabs_Quickstart
                                      ****
       [License] [PyPi_Version] [Code_style:_black] [PyPi_Downloads] [CI]
                                [Maintainability]
 ## What is whylogs whylogs is an open source library for logging any kind of
```

