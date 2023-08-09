# Comparing `tmp/wyvern_ai-0.0.1.tar.gz` & `tmp/wyvern_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyvern_ai-0.0.1.tar", max compression
+gzip compressed data, was "wyvern_ai-0.0.2.tar", max compression
```

## Comparing `wyvern_ai-0.0.1.tar` & `wyvern_ai-0.0.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     3834 2023-08-07 02:53:32.202318 wyvern_ai-0.0.1/LICENSE
--rw-r--r--   0        0        0     2358 2023-08-07 02:56:54.812441 wyvern_ai-0.0.1/README.md
--rw-r--r--   0        0        0     1623 2023-08-07 14:05:28.062801 wyvern_ai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      153 2023-07-05 20:24:27.611681 wyvern_ai-0.0.1/wyvern/__init__.py
--rw-r--r--   0        0        0     8027 2023-08-07 01:55:32.283275 wyvern_ai-0.0.1/wyvern/api.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530207 wyvern_ai-0.0.1/wyvern/aws/__init__.py
--rw-r--r--   0        0        0     2892 2023-08-07 02:06:26.975932 wyvern_ai-0.0.1/wyvern/aws/kinesis.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530413 wyvern_ai-0.0.1/wyvern/clients/__init__.py
--rw-r--r--   0        0        0      524 2023-06-14 01:05:07.530485 wyvern_ai-0.0.1/wyvern/clients/snowflake.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530549 wyvern_ai-0.0.1/wyvern/components/__init__.py
--rw-r--r--   0        0        0     4638 2023-07-04 16:51:03.542637 wyvern_ai-0.0.1/wyvern/components/api_route_component.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530621 wyvern_ai-0.0.1/wyvern/components/business_logic/__init__.py
--rw-r--r--   0        0        0     6369 2023-07-26 04:10:25.144063 wyvern_ai-0.0.1/wyvern/components/business_logic/boosting_business_logic.py
--rw-r--r--   0        0        0     6134 2023-08-07 01:55:32.283625 wyvern_ai-0.0.1/wyvern/components/business_logic/business_logic.py
--rw-r--r--   0        0        0     6457 2023-07-26 04:10:25.144526 wyvern_ai-0.0.1/wyvern/components/business_logic/pinning_business_logic.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530967 wyvern_ai-0.0.1/wyvern/components/candidates/__init__.py
--rw-r--r--   0        0        0     2482 2023-08-07 01:55:32.284208 wyvern_ai-0.0.1/wyvern/components/candidates/candidate_logger.py
--rw-r--r--   0        0        0     5622 2023-08-07 02:06:27.017005 wyvern_ai-0.0.1/wyvern/components/component.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.531276 wyvern_ai-0.0.1/wyvern/components/events/__init__.py
--rw-r--r--   0        0        0      933 2023-08-07 01:55:32.284581 wyvern_ai-0.0.1/wyvern/components/events/events.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.531461 wyvern_ai-0.0.1/wyvern/components/features/__init__.py
--rw-r--r--   0        0        0     2082 2023-08-07 01:55:32.284890 wyvern_ai-0.0.1/wyvern/components/features/feature_logger.py
--rw-r--r--   0        0        0    12543 2023-08-04 04:01:02.209824 wyvern_ai-0.0.1/wyvern/components/features/feature_retrieval_pipeline.py
--rw-r--r--   0        0        0     4422 2023-08-01 03:17:03.782395 wyvern_ai-0.0.1/wyvern/components/features/feature_store.py
--rw-r--r--   0        0        0    11775 2023-07-27 15:57:04.546038 wyvern_ai-0.0.1/wyvern/components/features/realtime_features_component.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.531923 wyvern_ai-0.0.1/wyvern/components/helpers/__init__.py
--rw-r--r--   0        0        0      991 2023-07-13 02:54:34.215915 wyvern_ai-0.0.1/wyvern/components/helpers/linear_algebra.py
--rw-r--r--   0        0        0      732 2023-07-26 04:10:25.144954 wyvern_ai-0.0.1/wyvern/components/helpers/sorting.py
--rw-r--r--   0        0        0        0 2023-08-07 01:55:32.284987 wyvern_ai-0.0.1/wyvern/components/impressions/__init__.py
--rw-r--r--   0        0        0     2510 2023-08-07 01:55:32.285178 wyvern_ai-0.0.1/wyvern/components/impressions/impression_logger.py
--rw-r--r--   0        0        0      202 2023-06-14 01:05:07.532246 wyvern_ai-0.0.1/wyvern/components/index/__init__.py
--rw-r--r--   0        0        0     3735 2023-07-02 01:40:29.085733 wyvern_ai-0.0.1/wyvern/components/index/_index.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.532402 wyvern_ai-0.0.1/wyvern/components/models/__init__.py
--rw-r--r--   0        0        0     5027 2023-08-07 02:06:26.935084 wyvern_ai-0.0.1/wyvern/components/models/model_component.py
--rw-r--r--   0        0        0     4899 2023-08-07 02:06:26.988044 wyvern_ai-0.0.1/wyvern/components/models/modelbit_component.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.532554 wyvern_ai-0.0.1/wyvern/components/pagination/__init__.py
--rw-r--r--   0        0        0     4418 2023-06-18 21:45:42.922930 wyvern_ai-0.0.1/wyvern/components/pagination/pagination_component.py
--rw-r--r--   0        0        0      188 2023-06-14 01:05:07.532702 wyvern_ai-0.0.1/wyvern/components/pagination/pagination_fields.py
--rw-r--r--   0        0        0     3040 2023-08-07 02:06:26.935633 wyvern_ai-0.0.1/wyvern/components/pipeline_component.py
--rw-r--r--   0        0        0     1332 2023-08-07 02:06:26.995190 wyvern_ai-0.0.1/wyvern/config.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.532896 wyvern_ai-0.0.1/wyvern/core/__init__.py
--rw-r--r--   0        0        0      573 2023-06-29 09:00:23.099332 wyvern_ai-0.0.1/wyvern/core/compression.py
--rw-r--r--   0        0        0     1519 2023-08-07 02:06:27.027821 wyvern_ai-0.0.1/wyvern/core/httpx.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.533035 wyvern_ai-0.0.1/wyvern/entities/__init__.py
--rw-r--r--   0        0        0      715 2023-08-07 01:55:32.286505 wyvern_ai-0.0.1/wyvern/entities/candidate_entities.py
--rw-r--r--   0        0        0      584 2023-08-03 22:09:00.204204 wyvern_ai-0.0.1/wyvern/entities/feature_entities.py
--rw-r--r--   0        0        0      926 2023-07-13 02:54:34.217819 wyvern_ai-0.0.1/wyvern/entities/feature_entity_helpers.py
--rw-r--r--   0        0        0     3583 2023-08-07 02:06:26.969854 wyvern_ai-0.0.1/wyvern/entities/identifier.py
--rw-r--r--   0        0        0     7717 2023-07-28 19:11:25.921282 wyvern_ai-0.0.1/wyvern/entities/identifier_entities.py
--rw-r--r--   0        0        0      988 2023-07-11 00:04:25.624444 wyvern_ai-0.0.1/wyvern/entities/index_entities.py
--rw-r--r--   0        0        0      445 2023-07-26 02:52:04.729152 wyvern_ai-0.0.1/wyvern/entities/request.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.533510 wyvern_ai-0.0.1/wyvern/event_logging/__init__.py
--rw-r--r--   0        0        0     1316 2023-08-07 02:06:27.036174 wyvern_ai-0.0.1/wyvern/event_logging/event_logger.py
--rw-r--r--   0        0        0     2124 2023-08-07 01:55:32.286921 wyvern_ai-0.0.1/wyvern/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-04 21:57:48.400142 wyvern_ai-0.0.1/wyvern/feature_store/__init__.py
--rw-r--r--   0        0        0       86 2023-07-26 00:03:04.634471 wyvern_ai-0.0.1/wyvern/feature_store/constants.py
--rw-r--r--   0        0        0    16849 2023-08-07 02:06:27.040787 wyvern_ai-0.0.1/wyvern/feature_store/feature_server.py
--rw-r--r--   0        0        0    10150 2023-08-07 02:06:27.040958 wyvern_ai-0.0.1/wyvern/feature_store/historical_feature_util.py
--rw-r--r--   0        0        0     1028 2023-07-26 00:03:04.635404 wyvern_ai-0.0.1/wyvern/feature_store/schemas.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.533892 wyvern_ai-0.0.1/wyvern/helper/__init__.py
--rw-r--r--   0        0        0      245 2023-06-14 01:05:07.533944 wyvern_ai-0.0.1/wyvern/helper/sort.py
--rw-r--r--   0        0        0     2236 2023-07-11 00:04:25.624878 wyvern_ai-0.0.1/wyvern/index.py
--rw-r--r--   0        0        0     4614 2023-08-07 02:06:26.981918 wyvern_ai-0.0.1/wyvern/redis.py
--rw-r--r--   0        0        0      636 2023-06-14 01:05:07.534169 wyvern_ai-0.0.1/wyvern/request_context.py
--rw-r--r--   0        0        0     2925 2023-08-07 02:06:27.006136 wyvern_ai-0.0.1/wyvern/service.py
--rw-r--r--   0        0        0      233 2023-08-06 23:56:12.073476 wyvern_ai-0.0.1/wyvern/utils.py
--rw-r--r--   0        0        0        0 2023-06-14 01:05:07.534553 wyvern_ai-0.0.1/wyvern/web_frameworks/__init__.py
--rw-r--r--   0        0        0     5848 2023-08-07 02:06:27.023572 wyvern_ai-0.0.1/wyvern/web_frameworks/fastapi.py
--rw-r--r--   0        0        0      934 2023-08-07 01:02:17.981204 wyvern_ai-0.0.1/wyvern/wyvern_logging.py
--rw-r--r--   0        0        0     1367 2023-08-04 04:01:02.211270 wyvern_ai-0.0.1/wyvern/wyvern_request.py
--rw-r--r--   0        0        0      284 2023-06-14 01:05:07.534879 wyvern_ai-0.0.1/wyvern/wyvern_tracing.py
--rw-r--r--   0        0        0      837 2023-07-26 02:52:04.729381 wyvern_ai-0.0.1/wyvern/wyvern_typing.py
--rw-r--r--   0        0        0     3501 1970-01-01 00:00:00.000000 wyvern_ai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3829 2023-08-08 04:06:33.351589 wyvern_ai-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2358 2023-08-07 02:56:54.812441 wyvern_ai-0.0.2/README.md
+-rw-r--r--   0        0        0     1623 2023-08-09 01:40:17.780977 wyvern_ai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      153 2023-07-05 20:24:27.611681 wyvern_ai-0.0.2/wyvern/__init__.py
+-rw-r--r--   0        0        0     8028 2023-08-09 01:40:17.781429 wyvern_ai-0.0.2/wyvern/api.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530207 wyvern_ai-0.0.2/wyvern/aws/__init__.py
+-rw-r--r--   0        0        0     2892 2023-08-07 02:06:26.975932 wyvern_ai-0.0.2/wyvern/aws/kinesis.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530413 wyvern_ai-0.0.2/wyvern/clients/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-14 01:05:07.530485 wyvern_ai-0.0.2/wyvern/clients/snowflake.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530549 wyvern_ai-0.0.2/wyvern/components/__init__.py
+-rw-r--r--   0        0        0     4638 2023-07-04 16:51:03.542637 wyvern_ai-0.0.2/wyvern/components/api_route_component.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530621 wyvern_ai-0.0.2/wyvern/components/business_logic/__init__.py
+-rw-r--r--   0        0        0     6369 2023-07-26 04:10:25.144063 wyvern_ai-0.0.2/wyvern/components/business_logic/boosting_business_logic.py
+-rw-r--r--   0        0        0     6134 2023-08-07 01:55:32.283625 wyvern_ai-0.0.2/wyvern/components/business_logic/business_logic.py
+-rw-r--r--   0        0        0     6457 2023-07-26 04:10:25.144526 wyvern_ai-0.0.2/wyvern/components/business_logic/pinning_business_logic.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.530967 wyvern_ai-0.0.2/wyvern/components/candidates/__init__.py
+-rw-r--r--   0        0        0     2482 2023-08-07 01:55:32.284208 wyvern_ai-0.0.2/wyvern/components/candidates/candidate_logger.py
+-rw-r--r--   0        0        0     5622 2023-08-07 02:06:27.017005 wyvern_ai-0.0.2/wyvern/components/component.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.531276 wyvern_ai-0.0.2/wyvern/components/events/__init__.py
+-rw-r--r--   0        0        0      933 2023-08-07 01:55:32.284581 wyvern_ai-0.0.2/wyvern/components/events/events.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.531461 wyvern_ai-0.0.2/wyvern/components/features/__init__.py
+-rw-r--r--   0        0        0     2082 2023-08-07 01:55:32.284890 wyvern_ai-0.0.2/wyvern/components/features/feature_logger.py
+-rw-r--r--   0        0        0    12543 2023-08-04 04:01:02.209824 wyvern_ai-0.0.2/wyvern/components/features/feature_retrieval_pipeline.py
+-rw-r--r--   0        0        0     4422 2023-08-01 03:17:03.782395 wyvern_ai-0.0.2/wyvern/components/features/feature_store.py
+-rw-r--r--   0        0        0    11775 2023-07-27 15:57:04.546038 wyvern_ai-0.0.2/wyvern/components/features/realtime_features_component.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.531923 wyvern_ai-0.0.2/wyvern/components/helpers/__init__.py
+-rw-r--r--   0        0        0      991 2023-07-13 02:54:34.215915 wyvern_ai-0.0.2/wyvern/components/helpers/linear_algebra.py
+-rw-r--r--   0        0        0      732 2023-07-26 04:10:25.144954 wyvern_ai-0.0.2/wyvern/components/helpers/sorting.py
+-rw-r--r--   0        0        0        0 2023-08-07 01:55:32.284987 wyvern_ai-0.0.2/wyvern/components/impressions/__init__.py
+-rw-r--r--   0        0        0     2510 2023-08-07 01:55:32.285178 wyvern_ai-0.0.2/wyvern/components/impressions/impression_logger.py
+-rw-r--r--   0        0        0      202 2023-06-14 01:05:07.532246 wyvern_ai-0.0.2/wyvern/components/index/__init__.py
+-rw-r--r--   0        0        0     3735 2023-07-02 01:40:29.085733 wyvern_ai-0.0.2/wyvern/components/index/_index.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.532402 wyvern_ai-0.0.2/wyvern/components/models/__init__.py
+-rw-r--r--   0        0        0     5027 2023-08-07 02:06:26.935084 wyvern_ai-0.0.2/wyvern/components/models/model_component.py
+-rw-r--r--   0        0        0     4899 2023-08-07 02:06:26.988044 wyvern_ai-0.0.2/wyvern/components/models/modelbit_component.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.532554 wyvern_ai-0.0.2/wyvern/components/pagination/__init__.py
+-rw-r--r--   0        0        0     4418 2023-06-18 21:45:42.922930 wyvern_ai-0.0.2/wyvern/components/pagination/pagination_component.py
+-rw-r--r--   0        0        0      188 2023-06-14 01:05:07.532702 wyvern_ai-0.0.2/wyvern/components/pagination/pagination_fields.py
+-rw-r--r--   0        0        0     3040 2023-08-07 02:06:26.935633 wyvern_ai-0.0.2/wyvern/components/pipeline_component.py
+-rw-r--r--   0        0        0     1332 2023-08-07 02:06:26.995190 wyvern_ai-0.0.2/wyvern/config.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.532896 wyvern_ai-0.0.2/wyvern/core/__init__.py
+-rw-r--r--   0        0        0      573 2023-06-29 09:00:23.099332 wyvern_ai-0.0.2/wyvern/core/compression.py
+-rw-r--r--   0        0        0     1519 2023-08-07 02:06:27.027821 wyvern_ai-0.0.2/wyvern/core/httpx.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.533035 wyvern_ai-0.0.2/wyvern/entities/__init__.py
+-rw-r--r--   0        0        0      715 2023-08-07 01:55:32.286505 wyvern_ai-0.0.2/wyvern/entities/candidate_entities.py
+-rw-r--r--   0        0        0      584 2023-08-03 22:09:00.204204 wyvern_ai-0.0.2/wyvern/entities/feature_entities.py
+-rw-r--r--   0        0        0      926 2023-07-13 02:54:34.217819 wyvern_ai-0.0.2/wyvern/entities/feature_entity_helpers.py
+-rw-r--r--   0        0        0     3583 2023-08-07 02:06:26.969854 wyvern_ai-0.0.2/wyvern/entities/identifier.py
+-rw-r--r--   0        0        0     7717 2023-07-28 19:11:25.921282 wyvern_ai-0.0.2/wyvern/entities/identifier_entities.py
+-rw-r--r--   0        0        0      988 2023-07-11 00:04:25.624444 wyvern_ai-0.0.2/wyvern/entities/index_entities.py
+-rw-r--r--   0        0        0      445 2023-07-26 02:52:04.729152 wyvern_ai-0.0.2/wyvern/entities/request.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.533510 wyvern_ai-0.0.2/wyvern/event_logging/__init__.py
+-rw-r--r--   0        0        0     1316 2023-08-07 02:06:27.036174 wyvern_ai-0.0.2/wyvern/event_logging/event_logger.py
+-rw-r--r--   0        0        0     2124 2023-08-07 01:55:32.286921 wyvern_ai-0.0.2/wyvern/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-04 21:57:48.400142 wyvern_ai-0.0.2/wyvern/feature_store/__init__.py
+-rw-r--r--   0        0        0       86 2023-07-26 00:03:04.634471 wyvern_ai-0.0.2/wyvern/feature_store/constants.py
+-rw-r--r--   0        0        0    16849 2023-08-07 02:06:27.040787 wyvern_ai-0.0.2/wyvern/feature_store/feature_server.py
+-rw-r--r--   0        0        0    10150 2023-08-07 02:06:27.040958 wyvern_ai-0.0.2/wyvern/feature_store/historical_feature_util.py
+-rw-r--r--   0        0        0     1028 2023-07-26 00:03:04.635404 wyvern_ai-0.0.2/wyvern/feature_store/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.533892 wyvern_ai-0.0.2/wyvern/helper/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-14 01:05:07.533944 wyvern_ai-0.0.2/wyvern/helper/sort.py
+-rw-r--r--   0        0        0     2236 2023-07-11 00:04:25.624878 wyvern_ai-0.0.2/wyvern/index.py
+-rw-r--r--   0        0        0     4614 2023-08-07 02:06:26.981918 wyvern_ai-0.0.2/wyvern/redis.py
+-rw-r--r--   0        0        0      636 2023-06-14 01:05:07.534169 wyvern_ai-0.0.2/wyvern/request_context.py
+-rw-r--r--   0        0        0     2925 2023-08-07 02:06:27.006136 wyvern_ai-0.0.2/wyvern/service.py
+-rw-r--r--   0        0        0      233 2023-08-06 23:56:12.073476 wyvern_ai-0.0.2/wyvern/utils.py
+-rw-r--r--   0        0        0        0 2023-06-14 01:05:07.534553 wyvern_ai-0.0.2/wyvern/web_frameworks/__init__.py
+-rw-r--r--   0        0        0     5848 2023-08-07 02:06:27.023572 wyvern_ai-0.0.2/wyvern/web_frameworks/fastapi.py
+-rw-r--r--   0        0        0      934 2023-08-07 01:02:17.981204 wyvern_ai-0.0.2/wyvern/wyvern_logging.py
+-rw-r--r--   0        0        0     1367 2023-08-04 04:01:02.211270 wyvern_ai-0.0.2/wyvern/wyvern_request.py
+-rw-r--r--   0        0        0      284 2023-06-14 01:05:07.534879 wyvern_ai-0.0.2/wyvern/wyvern_tracing.py
+-rw-r--r--   0        0        0      837 2023-07-26 02:52:04.729381 wyvern_ai-0.0.2/wyvern/wyvern_typing.py
+-rw-r--r--   0        0        0     3501 1970-01-01 00:00:00.000000 wyvern_ai-0.0.2/PKG-INFO
```

### Comparing `wyvern_ai-0.0.1/LICENSE` & `wyvern_ai-0.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Artie Transfer uses Elastic License 2.0
+Wyvern AI uses Elastic License 2.0
 
 Elastic License 2.0 (ELv2)
 
 **Acceptance**
 By using the software, you agree to all of the terms and conditions below.
 
 **Copyright License**
```

### Comparing `wyvern_ai-0.0.1/README.md` & `wyvern_ai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/pyproject.toml` & `wyvern_ai-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wyvern-ai"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Wyvern AI <info@wyvern.ai>"]
 readme = "README.md"
 packages = [
     { include = "wyvern" },
 ]
```

### Comparing `wyvern_ai-0.0.1/wyvern/api.py` & `wyvern_ai-0.0.2/wyvern/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pandas.api.types import is_datetime64_any_dtype
 from tqdm import tqdm
 
 from wyvern.config import settings
 from wyvern.exceptions import WyvernAPIKeyMissingError, WyvernError
 
 BATCH_SIZE = 15000
-HTTP_TIMEOUT = 60
+HTTP_TIMEOUT = 180
 BATCH_SIZE_PER_GATHER = 4
 
 
 class WyvernAPI:
     def __init__(
         self,
         api_key: Optional[str] = None,
```

### Comparing `wyvern_ai-0.0.1/wyvern/aws/kinesis.py` & `wyvern_ai-0.0.2/wyvern/aws/kinesis.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/clients/snowflake.py` & `wyvern_ai-0.0.2/wyvern/clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/api_route_component.py` & `wyvern_ai-0.0.2/wyvern/components/api_route_component.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/business_logic/boosting_business_logic.py` & `wyvern_ai-0.0.2/wyvern/components/business_logic/boosting_business_logic.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/business_logic/business_logic.py` & `wyvern_ai-0.0.2/wyvern/components/business_logic/business_logic.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/business_logic/pinning_business_logic.py` & `wyvern_ai-0.0.2/wyvern/components/business_logic/pinning_business_logic.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/candidates/candidate_logger.py` & `wyvern_ai-0.0.2/wyvern/components/candidates/candidate_logger.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/component.py` & `wyvern_ai-0.0.2/wyvern/components/component.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/events/events.py` & `wyvern_ai-0.0.2/wyvern/components/events/events.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/features/feature_logger.py` & `wyvern_ai-0.0.2/wyvern/components/features/feature_logger.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/features/feature_retrieval_pipeline.py` & `wyvern_ai-0.0.2/wyvern/components/features/feature_retrieval_pipeline.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/features/feature_store.py` & `wyvern_ai-0.0.2/wyvern/components/features/feature_store.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/features/realtime_features_component.py` & `wyvern_ai-0.0.2/wyvern/components/features/realtime_features_component.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/helpers/linear_algebra.py` & `wyvern_ai-0.0.2/wyvern/components/helpers/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/helpers/sorting.py` & `wyvern_ai-0.0.2/wyvern/components/helpers/sorting.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/impressions/impression_logger.py` & `wyvern_ai-0.0.2/wyvern/components/impressions/impression_logger.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/index/_index.py` & `wyvern_ai-0.0.2/wyvern/components/index/_index.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/models/model_component.py` & `wyvern_ai-0.0.2/wyvern/components/models/model_component.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/models/modelbit_component.py` & `wyvern_ai-0.0.2/wyvern/components/models/modelbit_component.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/pagination/pagination_component.py` & `wyvern_ai-0.0.2/wyvern/components/pagination/pagination_component.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/components/pipeline_component.py` & `wyvern_ai-0.0.2/wyvern/components/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/config.py` & `wyvern_ai-0.0.2/wyvern/config.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/core/compression.py` & `wyvern_ai-0.0.2/wyvern/core/compression.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/core/httpx.py` & `wyvern_ai-0.0.2/wyvern/core/httpx.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/entities/candidate_entities.py` & `wyvern_ai-0.0.2/wyvern/entities/candidate_entities.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/entities/feature_entities.py` & `wyvern_ai-0.0.2/wyvern/entities/feature_entities.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/entities/feature_entity_helpers.py` & `wyvern_ai-0.0.2/wyvern/entities/feature_entity_helpers.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/entities/identifier.py` & `wyvern_ai-0.0.2/wyvern/entities/identifier.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/entities/identifier_entities.py` & `wyvern_ai-0.0.2/wyvern/entities/identifier_entities.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/entities/index_entities.py` & `wyvern_ai-0.0.2/wyvern/entities/index_entities.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/event_logging/event_logger.py` & `wyvern_ai-0.0.2/wyvern/event_logging/event_logger.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/exceptions.py` & `wyvern_ai-0.0.2/wyvern/exceptions.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/feature_store/feature_server.py` & `wyvern_ai-0.0.2/wyvern/feature_store/feature_server.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/feature_store/historical_feature_util.py` & `wyvern_ai-0.0.2/wyvern/feature_store/historical_feature_util.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/feature_store/schemas.py` & `wyvern_ai-0.0.2/wyvern/feature_store/schemas.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/index.py` & `wyvern_ai-0.0.2/wyvern/index.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/redis.py` & `wyvern_ai-0.0.2/wyvern/redis.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/request_context.py` & `wyvern_ai-0.0.2/wyvern/request_context.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/service.py` & `wyvern_ai-0.0.2/wyvern/service.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/web_frameworks/fastapi.py` & `wyvern_ai-0.0.2/wyvern/web_frameworks/fastapi.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/wyvern_logging.py` & `wyvern_ai-0.0.2/wyvern/wyvern_logging.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/wyvern_request.py` & `wyvern_ai-0.0.2/wyvern/wyvern_request.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/wyvern/wyvern_typing.py` & `wyvern_ai-0.0.2/wyvern/wyvern_typing.py`

 * *Files identical despite different names*

### Comparing `wyvern_ai-0.0.1/PKG-INFO` & `wyvern_ai-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyvern-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Wyvern AI
 Author-email: info@wyvern.ai
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

