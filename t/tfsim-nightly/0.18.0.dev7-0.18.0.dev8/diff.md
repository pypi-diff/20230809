# Comparing `tmp/tfsim-nightly-0.18.0.dev7.tar.gz` & `tmp/tfsim-nightly-0.18.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfsim-nightly-0.18.0.dev7.tar", last modified: Sun Jul  2 03:20:27 2023, max compression
+gzip compressed data, was "tfsim-nightly-0.18.0.dev8.tar", last modified: Wed Aug  9 03:12:17 2023, max compression
```

## Comparing `tfsim-nightly-0.18.0.dev7.tar` & `tfsim-nightly-0.18.0.dev8.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.124139 tfsim-nightly-0.18.0.dev7/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-07-02 03:20:27.124139 tfsim-nightly-0.18.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 03:20:27.124139 tfsim-nightly-0.18.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.100139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-02 03:20:24.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.100139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.100139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.100139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.100139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/cropping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/barlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/base_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.104139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/binary_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/classification_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/false_positive_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/negative_predictive_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/distances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.104139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/evaluators/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/evaluators/memory_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.108139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/barlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/circle_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/metric_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/multinegrank_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/multisim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/pn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/softnn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/vicreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/xbm_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.108139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/classification_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/match_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/match_nearest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.108139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39080 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/models/contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/models/similarity_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.108139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/bndcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/map_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/precision_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/retrieval_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.112139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/file_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/memory_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/tfdata_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/tfdataset_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/tfrecords_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.112139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/faiss_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/linear_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/nmslib_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.112139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/cached_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.112139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/training_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/training_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/training_metrics/distance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/training_metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.116139 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/confusion_matrix_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/neighbors_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/vizualize_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.116139 tfsim-nightly-0.18.0.dev7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.116139 tfsim-nightly-0.18.0.dev7/tests/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/architectures/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/architectures/test_resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/architectures/test_resnet50.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.116139 tfsim-nightly-0.18.0.dev7/tests/classification_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/classification_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/classification_metrics/test_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.116139 tfsim-nightly-0.18.0.dev7/tests/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/evaluators/test_memory_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.120139 tfsim-nightly-0.18.0.dev7/tests/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/losses/test_pn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/losses/test_softnn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/losses/test_triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/losses/test_xbm_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.120139 tfsim-nightly-0.18.0.dev7/tests/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/matchers/test_classification_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/matchers/test_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/matchers/test_match_nearest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.120139 tfsim-nightly-0.18.0.dev7/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/models/test_contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/models/test_similarity_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.120139 tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_bndcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_map_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_precision_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_retrieval_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.120139 tfsim-nightly-0.18.0.dev7/tests/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/samplers/test_file_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/samplers/test_memory_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/samplers/test_tfdata_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/samplers/test_tfdataset_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/samplers/test_tfrecord_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.120139 tfsim-nightly-0.18.0.dev7/tests/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/search/test_faiss_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/search/test_linear_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/search/test_nmslib_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.124139 tfsim-nightly-0.18.0.dev7/tests/stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/stores/test_cached_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/stores/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/stores/test_redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/test_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/test_schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.124139 tfsim-nightly-0.18.0.dev7/tests/training_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/training_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/training_metrics/test_distance_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.124139 tfsim-nightly-0.18.0.dev7/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/visualization/test_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-02 03:18:03.000000 tfsim-nightly-0.18.0.dev7/tests/visualization/test_neighbors_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:20:27.124139 tfsim-nightly-0.18.0.dev7/tfsim_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-07-02 03:20:26.000000 tfsim-nightly-0.18.0.dev7/tfsim_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-02 03:20:27.000000 tfsim-nightly-0.18.0.dev7/tfsim_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 03:20:26.000000 tfsim-nightly-0.18.0.dev7/tfsim_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 03:20:26.000000 tfsim-nightly-0.18.0.dev7/tfsim_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 03:20:26.000000 tfsim-nightly-0.18.0.dev7/tfsim_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.662066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-09 03:12:15.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.666066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.666066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.666066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.666066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/cropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/barlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/base_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.666066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/binary_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/classification_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/false_positive_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/negative_predictive_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.666066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/evaluators/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/evaluators/memory_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.670066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/barlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/circle_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/metric_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/multinegrank_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/multisim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/pn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/softnn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/vicreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/xbm_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.670066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/classification_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/match_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/match_nearest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.670066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39080 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/models/contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/models/similarity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.670066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/bndcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/map_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/precision_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.670066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/file_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/memory_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/tfdata_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/tfdataset_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/tfrecords_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.670066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/faiss_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/linear_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/nmslib_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.670066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/cached_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/training_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/training_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/training_metrics/distance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/training_metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/confusion_matrix_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/neighbors_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/vizualize_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tests/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/architectures/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/architectures/test_resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/architectures/test_resnet50.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tests/classification_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/classification_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/classification_metrics/test_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tests/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/evaluators/test_memory_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tests/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/losses/test_pn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/losses/test_softnn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/losses/test_triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/losses/test_xbm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tests/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/matchers/test_classification_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/matchers/test_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/matchers/test_match_nearest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.674066 tfsim-nightly-0.18.0.dev8/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/models/test_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/models/test_similarity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_bndcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_map_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_precision_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_retrieval_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/tests/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/samplers/test_file_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/samplers/test_memory_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/samplers/test_tfdata_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/samplers/test_tfdataset_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/samplers/test_tfrecord_samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/search/test_faiss_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/search/test_linear_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/search/test_nmslib_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/tests/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/stores/test_cached_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/stores/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/stores/test_redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/test_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/test_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/tests/training_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/training_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/training_metrics/test_distance_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/visualization/test_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-08-09 03:09:44.000000 tfsim-nightly-0.18.0.dev8/tests/visualization/test_neighbors_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:12:17.678066 tfsim-nightly-0.18.0.dev8/tfsim_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-08-09 03:12:17.000000 tfsim-nightly-0.18.0.dev8/tfsim_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-08-09 03:12:17.000000 tfsim-nightly-0.18.0.dev8/tfsim_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:12:17.000000 tfsim-nightly-0.18.0.dev8/tfsim_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-09 03:12:17.000000 tfsim-nightly-0.18.0.dev8/tfsim_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-09 03:12:17.000000 tfsim-nightly-0.18.0.dev8/tfsim_nightly.egg-info/top_level.txt
```

### Comparing `tfsim-nightly-0.18.0.dev7/LICENSE` & `tfsim-nightly-0.18.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/PKG-INFO` & `tfsim-nightly-0.18.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfsim-nightly
-Version: 0.18.0.dev7
+Version: 0.18.0.dev8
 Summary: Metric Learning for Humans
 Home-page: https://github.com/tensorflow/similarity
 Author: Tensorflow Similarity authors
 Author-email: tf-similarity@google.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tfsim-nightly-0.18.0.dev7/README.md` & `tfsim-nightly-0.18.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/setup.py` & `tfsim-nightly-0.18.0.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.18.0.dev7"
+__version__ = "0.18.0.dev8"
 
 
 from . import algebra  # noqa
 from . import architectures  # noqa
 from . import augmenters  # noqa
 from . import callbacks  # noqa
 from . import classification_metrics  # noqa
```

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/algebra.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/algebra.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/api/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/efficientnet.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/efficientnet.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/resnet18.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/resnet18.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/resnet50.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/resnet50.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/architectures/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/architectures/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/blur.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/blur.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/cropping.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/cropping.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/flip.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/flip.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmentation_utils/solarize.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmentation_utils/solarize.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/augmenter.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/augmenter.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/barlow.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/barlow.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/contrastive.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/contrastive.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/augmenters/simclr.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/augmenters/simclr.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/base_indexer.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/base_indexer.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/callbacks.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/callbacks.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/binary_accuracy.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/binary_accuracy.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/classification_metric.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/classification_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/f1_score.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/f1_score.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/false_positive_rate.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/false_positive_rate.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/negative_predictive_value.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/negative_predictive_value.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/precision.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/precision.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/recall.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/recall.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/classification_metrics/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/classification_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/distances.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/distances.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/evaluators/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/evaluators/evaluator.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/evaluators/evaluator.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/evaluators/memory_evaluator.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/evaluators/memory_evaluator.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/indexer.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/indexer.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/layers.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/layers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/barlow.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/barlow.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/circle_loss.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/circle_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/metric_loss.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/metric_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/multinegrank_loss.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/multinegrank_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/multisim_loss.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/multisim_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/pn_loss.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/pn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/simclr.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/simclr.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/simsiam.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/simsiam.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/softnn_loss.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/softnn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/triplet_loss.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/vicreg.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/vicreg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/losses/xbm_loss.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/losses/xbm_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/classification_match.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/classification_match.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/match_majority_vote.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/match_majority_vote.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/match_nearest.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/match_nearest.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/matchers/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/matchers/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/models/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/models/contrastive_model.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/models/contrastive_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/models/similarity_model.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/models/similarity_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/bndcg.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/bndcg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/map_at_k.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/map_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/precision_at_k.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/precision_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/recall_at_k.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/recall_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/retrieval_metric.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/retrieval_metrics/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/retrieval_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/file_samplers.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/file_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/memory_samplers.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/memory_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/samplers.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/tfdata_sampler.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/tfdata_sampler.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/tfdataset_samplers.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/tfdataset_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/tfrecords_samplers.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/tfrecords_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/samplers/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/schedules.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/schedules.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/faiss_search.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/faiss_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,28 +123,37 @@
             embedding: Batch of query embeddings as predicted by the model.
             k: Number of nearest neighboors embedding to lookup. Defaults to 5.
         """
 
         if normalize:
             faiss.normalize_L2(embeddings)
         sims, indices = self.index.search(embeddings, k)
-        return indices, sims
+        out_indices = []
+        out_sims = []
+        for i in range(len(indices)):
+            out_indices.append(list(indices[i][indices[i] != -1]))
+            out_sims.append(list(sims[i])[: len(out_indices[i])])
+        return out_indices, out_sims
 
     def lookup(self, embedding: FloatTensor, k: int = 5, normalize: bool = True) -> tuple[list[int], list[float]]:
         """Find embedding K nearest neighboors embeddings.
 
         Args:
             embedding: Query embedding as predicted by the model.
             k: Number of nearest neighboors embedding to lookup. Defaults to 5.
         """
         int_embedding = np.array([embedding], dtype=np.float32)
         if normalize:
             faiss.normalize_L2(int_embedding)
         sims, indices = self.index.search(int_embedding, k)
-        return indices[0], sims[0]
+        # FAISS might return less than k items, in which case the rest will
+        # be set to -1
+        out_indices = list(indices[0][indices[0] != -1])
+        out_sims = list(sims[0])[: len(out_indices)]
+        return out_indices, out_sims
 
     def add(self, embedding: FloatTensor, idx: int, verbose: int = 1, normalize: bool = True, **kwargs):
         """Add a single embedding to the search index.
 
         Args:
             embedding: The embedding to index as computed by the similarity model.
             idx: Embedding id as in the index table. Returned with the embedding to
```

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/linear_search.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/linear_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/nmslib_search.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/nmslib_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/search.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/search/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/search/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/cached_store.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/cached_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/memory_store.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/memory_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/redis_store.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/redis_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             data: Data associated with the embedding. Defaults to None.
 
         Returns:
             Associated record id.
         """
         num_items = int(self.__conn.incr("num_items"))
         idx = num_items - 1
-        self.__conn.set(idx, pickle.dumps((embedding, label, data)))
+        self.__conn.set(str(idx), pickle.dumps((embedding, label, data)))
 
         return idx
 
     def get_num_items(self) -> int:
         return int(self.__conn.get("num_items")) or 0
 
     def batch_add(
@@ -102,15 +102,15 @@
         Args:
             idx: Id of the record to fetch.
 
         Returns:
             record associated with the requested id.
         """
 
-        ret_bytes: bytes = self.__conn.get(idx)
+        ret_bytes: bytes = self.__conn.get(str(idx))
         ret: tuple = pickle.loads(ret_bytes)
         return (ret[0], ret[1], ret[2])
 
     def batch_get(self, idxs: Sequence[int]) -> tuple[list[FloatTensor], list[int | None], list[Tensor | None]]:
         """Get embedding records from the key value store.
 
         Args:
```

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/store.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/stores/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/stores/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/training_metrics/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/training_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/training_metrics/distance_metrics.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/training_metrics/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/training_metrics/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/training_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/types.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/types.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/utils.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/__init__.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/confusion_matrix_viz.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/confusion_matrix_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/neighbors_viz.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/neighbors_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/projector.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/projector.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tensorflow_similarity/visualization/vizualize_views.py` & `tfsim-nightly-0.18.0.dev8/tensorflow_similarity/visualization/vizualize_views.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/architectures/test_efficientnet.py` & `tfsim-nightly-0.18.0.dev8/tests/architectures/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/architectures/test_resnet18.py` & `tfsim-nightly-0.18.0.dev8/tests/architectures/test_resnet18.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/architectures/test_resnet50.py` & `tfsim-nightly-0.18.0.dev8/tests/architectures/test_resnet50.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/classification_metrics/test_classification_metrics.py` & `tfsim-nightly-0.18.0.dev8/tests/classification_metrics/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/evaluators/test_memory_evaluator.py` & `tfsim-nightly-0.18.0.dev8/tests/evaluators/test_memory_evaluator.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/losses/test_pn_loss.py` & `tfsim-nightly-0.18.0.dev8/tests/losses/test_pn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/losses/test_softnn_loss.py` & `tfsim-nightly-0.18.0.dev8/tests/losses/test_softnn_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/losses/test_triplet_loss.py` & `tfsim-nightly-0.18.0.dev8/tests/losses/test_triplet_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/losses/test_xbm_loss.py` & `tfsim-nightly-0.18.0.dev8/tests/losses/test_xbm_loss.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/losses/utils.py` & `tfsim-nightly-0.18.0.dev8/tests/losses/utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/matchers/test_classification_match.py` & `tfsim-nightly-0.18.0.dev8/tests/matchers/test_classification_match.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/matchers/test_majority_vote.py` & `tfsim-nightly-0.18.0.dev8/tests/matchers/test_majority_vote.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/matchers/test_match_nearest.py` & `tfsim-nightly-0.18.0.dev8/tests/matchers/test_match_nearest.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/models/test_contrastive_model.py` & `tfsim-nightly-0.18.0.dev8/tests/models/test_contrastive_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/models/test_similarity_model.py` & `tfsim-nightly-0.18.0.dev8/tests/models/test_similarity_model.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_bndcg.py` & `tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_bndcg.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_map_at_k.py` & `tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_map_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_precision_at_k.py` & `tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_precision_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_recall_at_k.py` & `tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_recall_at_k.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/retrieval_metrics/test_retrieval_metric.py` & `tfsim-nightly-0.18.0.dev8/tests/retrieval_metrics/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/samplers/test_file_samplers.py` & `tfsim-nightly-0.18.0.dev8/tests/samplers/test_file_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/samplers/test_memory_samplers.py` & `tfsim-nightly-0.18.0.dev8/tests/samplers/test_memory_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/samplers/test_tfdata_sampler.py` & `tfsim-nightly-0.18.0.dev8/tests/samplers/test_tfdata_sampler.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/samplers/test_tfdataset_samplers.py` & `tfsim-nightly-0.18.0.dev8/tests/samplers/test_tfdataset_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/samplers/test_tfrecord_samplers.py` & `tfsim-nightly-0.18.0.dev8/tests/samplers/test_tfrecord_samplers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/search/test_faiss_search.py` & `tfsim-nightly-0.18.0.dev8/tests/search/test_faiss_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     singles_idxs = []
     for t in targets:
         idxs, embs = search_index.lookup(t)
         singles_idxs.append(idxs)
 
     for i in range(num_targets):
         # k neigboors are the same?
-        for k in range(3):
+        for k in range(len(batch_idxs[i])):
             assert batch_idxs[i][k] == singles_idxs[i][k]
 
 
 def test_ivfpq():
     # test ivfpq ANN indexing with 100M entries
     num_targets = 10
     index_size = 10000
@@ -101,20 +101,21 @@
     last_idx = 0
     for i in range(1000):
         idxs = np.array(list(range(last_idx, last_idx + index_size)))
         embs = np.random.random((index_size, vect_dim)).astype("float32")
         last_idx += index_size
         search_index.batch_add(embs, idxs)
     found_idxs, found_dists = search_index.batch_lookup(targets, 2)
-    assert found_idxs.shape == (10, 2)
+    assert len(found_idxs) == 10
+    assert len(found_idxs[0]) == 2
 
 
 def test_reset():
     target = np.array([1, 2, 3], dtype="float32")
-    embs = np.array([[3, 2, 1], [2, 3, 4]], dtype="float32")
+    embs = np.array([[3, 2, 1], [2, 3, 4], [3, 6, 9]], dtype="float32")
 
     search_index = FaissSearch("cosine", 3, algo="flat")
     search_index.add(embs[0], 0)
     search_index.add(embs[1], 1)
 
     idxs, out_embs = search_index.lookup(target, k=2)
     print(f"idxs={idxs}, embs={out_embs}")
@@ -122,9 +123,9 @@
     assert len(out_embs) == 2
     assert list(idxs) == [1, 0]
     search_index.reset()
     # only add one
     search_index.add(embs[0], 0)
     idxs, out_embs = search_index.lookup(target, k=2)
     print(f"idxs={idxs}, embs={out_embs}")
-    assert len(out_embs) == 2
-    assert list(idxs) == [0, -1]
+    assert len(out_embs) == 1
+    assert list(idxs) == [0]
```

### Comparing `tfsim-nightly-0.18.0.dev7/tests/search/test_linear_search.py` & `tfsim-nightly-0.18.0.dev8/tests/search/test_linear_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/search/test_nmslib_search.py` & `tfsim-nightly-0.18.0.dev8/tests/search/test_nmslib_search.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/stores/test_cached_store.py` & `tfsim-nightly-0.18.0.dev8/tests/stores/test_cached_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/stores/test_memory_store.py` & `tfsim-nightly-0.18.0.dev8/tests/stores/test_memory_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/stores/test_redis_store.py` & `tfsim-nightly-0.18.0.dev8/tests/stores/test_redis_store.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/test_algebra.py` & `tfsim-nightly-0.18.0.dev8/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/test_callbacks.py` & `tfsim-nightly-0.18.0.dev8/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/test_distances.py` & `tfsim-nightly-0.18.0.dev8/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/test_indexer.py` & `tfsim-nightly-0.18.0.dev8/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/test_layers.py` & `tfsim-nightly-0.18.0.dev8/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/test_schedules.py` & `tfsim-nightly-0.18.0.dev8/tests/test_schedules.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/test_types.py` & `tfsim-nightly-0.18.0.dev8/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/test_utils.py` & `tfsim-nightly-0.18.0.dev8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/training_metrics/test_distance_metrics.py` & `tfsim-nightly-0.18.0.dev8/tests/training_metrics/test_distance_metrics.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/visualization/test_confusion_matrix.py` & `tfsim-nightly-0.18.0.dev8/tests/visualization/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tests/visualization/test_neighbors_viz.py` & `tfsim-nightly-0.18.0.dev8/tests/visualization/test_neighbors_viz.py`

 * *Files identical despite different names*

### Comparing `tfsim-nightly-0.18.0.dev7/tfsim_nightly.egg-info/PKG-INFO` & `tfsim-nightly-0.18.0.dev8/tfsim_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfsim-nightly
-Version: 0.18.0.dev7
+Version: 0.18.0.dev8
 Summary: Metric Learning for Humans
 Home-page: https://github.com/tensorflow/similarity
 Author: Tensorflow Similarity authors
 Author-email: tf-similarity@google.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tfsim-nightly-0.18.0.dev7/tfsim_nightly.egg-info/SOURCES.txt` & `tfsim-nightly-0.18.0.dev8/tfsim_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

