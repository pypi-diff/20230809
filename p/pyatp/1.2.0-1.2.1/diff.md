# Comparing `tmp/pyatp-1.2.0.tar.gz` & `tmp/pyatp-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatp-1.2.0.tar", max compression
+gzip compressed data, was "pyatp-1.2.1.tar", max compression
```

## Comparing `pyatp-1.2.0.tar` & `pyatp-1.2.1.tar`

### file list

```diff
@@ -1,517 +1,517 @@
--rw-r--r--   0        0        0    11357 2023-02-08 09:45:37.719000 pyatp-1.2.0/LICENSE
--rw-r--r--   0        0        0     1325 2023-08-08 11:02:52.690501 pyatp-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1151 2023-05-26 01:51:19.942655 pyatp-1.2.0/src/ailab/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 01:43:21.707000 pyatp-1.2.0/src/ailab/atp_dataset/__init__.py
--rw-r--r--   0        0        0     1189 2023-05-26 01:43:21.707000 pyatp-1.2.0/src/ailab/atp_dataset/ailab_api.py
--rw-r--r--   0        0        0      362 2023-07-24 02:56:17.630929 pyatp-1.2.0/src/ailab/atp_dataset/constant.py
--rw-r--r--   0        0        0     4367 2023-07-24 02:56:17.631639 pyatp-1.2.0/src/ailab/atp_dataset/dataset.py
--rw-r--r--   0        0        0     1975 2023-06-07 09:32:17.327152 pyatp-1.2.0/src/ailab/atp_dataset/huggingface_api.py
--rw-r--r--   0        0        0       98 2023-07-26 06:13:53.570112 pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/__init__.py
--rw-r--r--   0        0        0      947 2023-07-26 06:13:53.570258 pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/base.py
--rw-r--r--   0        0        0     5961 2023-08-08 11:02:41.061148 pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/ceval.py
--rw-r--r--   0        0        0     5638 2023-08-08 11:02:41.061214 pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/harness.py
--rw-r--r--   0        0        0     7518 2023-08-08 11:02:41.061313 pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/mmlu.py
--rw-r--r--   0        0        0      695 2023-08-08 11:02:41.061395 pyatp-1.2.0/src/ailab/atp_evaluation/build.py
--rw-r--r--   0        0        0     2002 2023-08-08 11:02:41.061479 pyatp-1.2.0/src/ailab/atp_evaluation/constant.py
--rw-r--r--   0        0        0     1503 2023-08-08 11:02:41.061583 pyatp-1.2.0/src/ailab/atp_evaluation/evaluator.py
--rw-r--r--   0        0        0       97 2023-07-26 06:13:53.570908 pyatp-1.2.0/src/ailab/atp_evaluation/models/__init__.py
--rw-r--r--   0        0        0     1194 2023-07-26 06:13:53.570990 pyatp-1.2.0/src/ailab/atp_evaluation/models/base.py
--rw-r--r--   0        0        0     5278 2023-08-08 11:02:41.061699 pyatp-1.2.0/src/ailab/atp_evaluation/models/chatglm.py
--rw-r--r--   0        0        0     4132 2023-08-08 11:02:41.061798 pyatp-1.2.0/src/ailab/atp_evaluation/models/llama.py
--rw-r--r--   0        0        0      155 2023-06-08 02:31:25.029113 pyatp-1.2.0/src/ailab/atp_finetuner/__init__.py
--rw-r--r--   0        0        0       41 2023-05-26 01:43:21.707000 pyatp-1.2.0/src/ailab/atp_finetuner/accelerator/__init__.py
--rw-r--r--   0        0        0     1738 2023-06-30 08:10:49.352351 pyatp-1.2.0/src/ailab/atp_finetuner/accelerator/accelerator.py
--rw-r--r--   0        0        0      766 2023-05-26 01:43:21.707000 pyatp-1.2.0/src/ailab/atp_finetuner/build.py
--rw-r--r--   0        0        0     2426 2023-08-08 11:02:41.061898 pyatp-1.2.0/src/ailab/atp_finetuner/constant.py
--rw-r--r--   0        0        0      402 2023-08-08 11:02:41.061985 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/__init__.py
--rw-r--r--   0        0        0     1650 2023-08-08 11:02:41.062638 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/datacollator.py
--rw-r--r--   0        0        0      987 2023-08-08 11:02:41.063097 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_alpaca.py
--rw-r--r--   0        0        0     1371 2023-08-08 11:02:41.063186 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_baichuan.py
--rw-r--r--   0        0        0     7762 2023-08-08 11:02:41.063836 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_chatglm.py
--rw-r--r--   0        0        0     1492 2023-08-08 11:02:41.064479 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_chinese_alpaca.py
--rw-r--r--   0        0        0     1026 2023-08-08 11:02:41.064894 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_language.py
--rw-r--r--   0        0        0      972 2023-08-08 11:02:41.064961 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_token.py
--rw-r--r--   0        0        0      922 2023-08-08 11:02:41.065028 pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_with_padding.py
--rw-r--r--   0        0        0     1721 2023-08-08 11:02:41.065582 pyatp-1.2.0/src/ailab/atp_finetuner/finetuner.py
--rw-r--r--   0        0        0       64 2023-05-26 01:43:21.708000 pyatp-1.2.0/src/ailab/atp_finetuner/metric/__init__.py
--rw-r--r--   0        0        0      627 2023-05-26 02:34:59.536185 pyatp-1.2.0/src/ailab/atp_finetuner/metric/accury.py
--rw-r--r--   0        0        0      425 2023-05-26 02:03:39.174407 pyatp-1.2.0/src/ailab/atp_finetuner/metric/metric.py
--rw-r--r--   0        0        0       62 2023-05-26 01:43:21.708000 pyatp-1.2.0/src/ailab/atp_finetuner/model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 01:43:21.708000 pyatp-1.2.0/src/ailab/atp_finetuner/model/cv/__init__.py
--rw-r--r--   0        0        0     1018 2023-06-08 07:46:32.642619 pyatp-1.2.0/src/ailab/atp_finetuner/model/model.py
--rw-r--r--   0        0        0       80 2023-06-01 08:42:34.253788 pyatp-1.2.0/src/ailab/atp_finetuner/model/multimodel/__init__.py
--rw-r--r--   0        0        0     3456 2023-06-08 07:46:32.642850 pyatp-1.2.0/src/ailab/atp_finetuner/model/multimodel/model_for_sd_lora.py
--rw-r--r--   0        0        0     1172 2023-06-08 07:46:32.642989 pyatp-1.2.0/src/ailab/atp_finetuner/model/multimodel/vilt_for_vqa.py
--rw-r--r--   0        0        0      380 2023-08-08 11:02:41.065674 pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/__init__.py
--rw-r--r--   0        0        0     4607 2023-08-08 11:02:41.065765 pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_baichuan.py
--rw-r--r--   0        0        0     3222 2023-08-08 11:02:41.065846 pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_chatglm.py
--rw-r--r--   0        0        0     1081 2023-06-20 06:18:50.439752 pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_chinese_alpaca.py
--rw-r--r--   0        0        0     1933 2023-07-11 08:36:20.383161 pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_lora.py
--rw-r--r--   0        0        0      820 2023-06-08 07:46:32.643745 pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_question_answer.py
--rw-r--r--   0        0        0      830 2023-06-08 07:46:32.643860 pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_text_classification.py
--rw-r--r--   0        0        0      830 2023-06-08 07:46:32.643967 pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_token_classification.py
--rw-r--r--   0        0        0       78 2023-05-26 01:43:21.709000 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 01:43:21.709000 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/cv/__init__.py
--rw-r--r--   0        0        0       88 2023-05-26 01:43:21.709000 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/multimodel/__init__.py
--rw-r--r--   0        0        0     3009 2023-06-08 07:46:32.644131 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_sd_lora.py
--rw-r--r--   0        0        0     3488 2023-06-08 07:46:32.644260 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_vilt_vqa.py
--rw-r--r--   0        0        0      378 2023-08-08 11:02:41.065929 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/__init__.py
--rw-r--r--   0        0        0     3150 2023-06-12 08:33:22.791142 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_alpaca.py
--rw-r--r--   0        0        0     5557 2023-08-08 11:02:41.066022 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_baichuan.py
--rw-r--r--   0        0        0     4212 2023-08-08 11:02:41.066639 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chatglm.py
--rw-r--r--   0        0        0     3601 2023-06-20 06:18:50.439972 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chinese_alpaca.py
--rw-r--r--   0        0        0     2852 2023-06-29 08:23:27.282928 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_llama_cn.py
--rw-r--r--   0        0        0     3586 2023-06-08 07:46:32.644729 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/question_answer_pc.py
--rw-r--r--   0        0        0     1184 2023-06-08 07:46:32.644837 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/text_classification_pc.py
--rw-r--r--   0        0        0     1112 2023-06-08 07:46:32.644960 pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/preprossor.py
--rw-r--r--   0        0        0       65 2023-05-26 01:43:21.710000 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 01:43:21.710000 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/cv/__init__.py
--rw-r--r--   0        0        0       88 2023-05-26 01:43:21.710000 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/multimodel/__init__.py
--rw-r--r--   0        0        0    10436 2023-06-01 08:42:34.255060 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_sd_lora.py
--rw-r--r--   0        0        0     4244 2023-06-01 08:42:34.255151 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_vilt_vqa.py
--rw-r--r--   0        0        0      387 2023-08-08 11:02:41.066738 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/__init__.py
--rw-r--r--   0        0        0      686 2023-06-20 06:18:50.440170 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/ds_zero2_no_offload.json
--rw-r--r--   0        0        0     5698 2023-07-11 08:36:20.383850 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_alpaca.py
--rw-r--r--   0        0        0     6766 2023-08-08 11:02:41.066829 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_baichuan.py
--rw-r--r--   0        0        0     5909 2023-08-08 11:02:41.069231 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chatglm.py
--rw-r--r--   0        0        0     6711 2023-07-11 08:36:20.384475 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chinese_alpaca.py
--rw-r--r--   0        0        0     5359 2023-07-11 08:36:20.384604 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_llama_cn.py
--rw-r--r--   0        0        0     4090 2023-06-01 08:42:34.255810 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_text_classification.py
--rw-r--r--   0        0        0     4041 2023-06-01 08:42:34.256415 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/traniner_for_question_answer.py
--rw-r--r--   0        0        0     1594 2023-06-01 08:42:34.256512 pyatp-1.2.0/src/ailab/atp_finetuner/trainer/trainer.py
--rw-r--r--   0        0        0     1498 2023-07-11 09:56:17.517435 pyatp-1.2.0/src/ailab/batch/__init__.py
--rw-r--r--   0        0        0     3749 2023-07-24 02:54:56.630083 pyatp-1.2.0/src/ailab/batch/entrypoint.py
--rw-r--r--   0        0        0      213 2023-07-11 03:21:15.515185 pyatp-1.2.0/src/ailab/buildkit/Makefile
--rw-r--r--   0        0        0      335 2023-06-07 06:35:49.073776 pyatp-1.2.0/src/ailab/buildkit/README.md
--rw-r--r--   0        0        0     1052 2023-07-11 02:23:25.287020 pyatp-1.2.0/src/ailab/buildkit/make.py
--rw-r--r--   0        0        0      743 2023-07-11 06:26:33.871730 pyatp-1.2.0/src/ailab/buildkit/pyproject.toml
--rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/__init__.py
--rw-r--r--   0        0        0    16684 2023-07-11 06:24:54.121544 pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/build.py
--rw-r--r--   0        0        0     1158 2023-06-29 06:47:07.874124 pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/config.py
--rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/dotdict.py
--rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/error.py
--rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/get-pip.py
--rw-r--r--   0        0        0     1457 2023-07-11 06:25:49.033583 pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/templates/Dockerfile.j2
--rw-r--r--   0        0        0     1550 2023-07-07 08:47:51.824731 pyatp-1.2.0/src/ailab/examples/__init__.py
--rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.0/src/ailab/examples/baichuan/__init__.py
--rw-r--r--   0        0        0      243 2023-07-24 02:56:17.634030 pyatp-1.2.0/src/ailab/examples/baichuan/requirements.txt
--rw-r--r--   0        0        0      438 2023-07-24 02:56:17.634648 pyatp-1.2.0/src/ailab/examples/baichuan/train.py
--rw-r--r--   0        0        0      174 2023-07-24 02:56:17.634777 pyatp-1.2.0/src/ailab/examples/baichuan/train.sh
--rw-r--r--   0        0        0     1934 2023-07-24 02:56:17.634846 pyatp-1.2.0/src/ailab/examples/baichuan/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-24 02:56:17.635076 pyatp-1.2.0/src/ailab/examples/baichuan_13b/__init__.py
--rw-r--r--   0        0        0      274 2023-07-24 02:56:17.635127 pyatp-1.2.0/src/ailab/examples/baichuan_13b/requirements.txt
--rw-r--r--   0        0        0      438 2023-07-24 02:56:17.635177 pyatp-1.2.0/src/ailab/examples/baichuan_13b/train.py
--rw-r--r--   0        0        0      174 2023-07-24 02:56:17.635246 pyatp-1.2.0/src/ailab/examples/baichuan_13b/train.sh
--rw-r--r--   0        0        0     1934 2023-07-24 02:56:17.635296 pyatp-1.2.0/src/ailab/examples/baichuan_13b/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-24 02:56:17.635403 pyatp-1.2.0/src/ailab/examples/bloomz/__init__.py
--rw-r--r--   0        0        0      244 2023-07-24 02:56:17.635455 pyatp-1.2.0/src/ailab/examples/bloomz/requirements.txt
--rw-r--r--   0        0        0      438 2023-07-24 02:56:17.635502 pyatp-1.2.0/src/ailab/examples/bloomz/train.py
--rw-r--r--   0        0        0      174 2023-07-24 02:56:17.635562 pyatp-1.2.0/src/ailab/examples/bloomz/train.sh
--rw-r--r--   0        0        0     1882 2023-07-24 02:56:17.635602 pyatp-1.2.0/src/ailab/examples/bloomz/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.0/src/ailab/examples/chatglm2_6b/__init__.py
--rw-r--r--   0        0        0      236 2023-07-24 02:56:17.635691 pyatp-1.2.0/src/ailab/examples/chatglm2_6b/requirements.txt
--rw-r--r--   0        0        0      438 2023-08-08 11:02:41.069329 pyatp-1.2.0/src/ailab/examples/chatglm2_6b/train.py
--rw-r--r--   0        0        0      174 2023-08-08 11:02:41.069377 pyatp-1.2.0/src/ailab/examples/chatglm2_6b/train.sh
--rw-r--r--   0        0        0     2005 2023-08-08 11:02:41.069432 pyatp-1.2.0/src/ailab/examples/chatglm2_6b/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280023 pyatp-1.2.0/src/ailab/examples/chatglm_6b/__init__.py
--rw-r--r--   0        0        0     1142 2023-08-08 11:02:41.069495 pyatp-1.2.0/src/ailab/examples/chatglm_6b/evaluator.py
--rw-r--r--   0        0        0      243 2023-07-24 02:56:17.636213 pyatp-1.2.0/src/ailab/examples/chatglm_6b/requirements.txt
--rw-r--r--   0        0        0      436 2023-08-08 11:02:41.070093 pyatp-1.2.0/src/ailab/examples/chatglm_6b/train.py
--rw-r--r--   0        0        0      174 2023-08-08 11:02:41.070137 pyatp-1.2.0/src/ailab/examples/chatglm_6b/train.sh
--rw-r--r--   0        0        0     2148 2023-08-08 11:02:41.070178 pyatp-1.2.0/src/ailab/examples/chatglm_6b/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/__init__.py
--rw-r--r--   0        0        0      963 2023-08-08 11:02:41.070227 pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/evaluator.py
--rw-r--r--   0        0        0      243 2023-07-24 02:56:17.636318 pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/requirements.txt
--rw-r--r--   0        0        0      469 2023-07-07 09:09:19.299389 pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/train.py
--rw-r--r--   0        0        0      175 2023-07-11 07:33:35.250007 pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/train.sh
--rw-r--r--   0        0        0     2092 2023-07-10 06:33:58.804274 pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/__init__.py
--rw-r--r--   0        0        0      937 2023-08-08 11:02:41.070276 pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/evaluator.py
--rw-r--r--   0        0        0      243 2023-07-24 02:56:17.636400 pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/requirements.txt
--rw-r--r--   0        0        0      468 2023-07-11 08:36:20.385166 pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/train.py
--rw-r--r--   0        0        0      174 2023-07-11 09:48:59.097911 pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/train.sh
--rw-r--r--   0        0        0     2207 2023-07-24 02:56:17.636756 pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-24 02:56:17.636849 pyatp-1.2.0/src/ailab/examples/falcon/__init__.py
--rw-r--r--   0        0        0      245 2023-07-24 02:56:17.636896 pyatp-1.2.0/src/ailab/examples/falcon/requirements.txt
--rw-r--r--   0        0        0      438 2023-07-24 02:56:17.636942 pyatp-1.2.0/src/ailab/examples/falcon/train.py
--rw-r--r--   0        0        0      174 2023-07-24 02:56:17.637002 pyatp-1.2.0/src/ailab/examples/falcon/train.sh
--rw-r--r--   0        0        0     1878 2023-07-24 02:56:17.637044 pyatp-1.2.0/src/ailab/examples/falcon/train_imp.py
--rw-r--r--   0        0        0      619 2023-08-08 11:02:41.070353 pyatp-1.2.0/src/ailab/examples/harness/evaluator.py
--rw-r--r--   0        0        0     1653 2023-08-08 11:02:41.070597 pyatp-1.2.0/src/ailab/examples/llama2/__init__.py
--rw-r--r--   0        0        0      245 2023-08-08 11:02:41.070652 pyatp-1.2.0/src/ailab/examples/llama2/requirements.txt
--rw-r--r--   0        0        0      434 2023-08-08 11:02:41.070700 pyatp-1.2.0/src/ailab/examples/llama2/train.py
--rw-r--r--   0        0        0      194 2023-08-08 11:02:41.070745 pyatp-1.2.0/src/ailab/examples/llama2/train.sh
--rw-r--r--   0        0        0     1842 2023-08-08 11:02:41.070788 pyatp-1.2.0/src/ailab/examples/llama2/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-24 02:56:17.637137 pyatp-1.2.0/src/ailab/examples/moss/__init__.py
--rw-r--r--   0        0        0      243 2023-07-24 02:56:17.637185 pyatp-1.2.0/src/ailab/examples/moss/requirements.txt
--rw-r--r--   0        0        0      438 2023-07-24 02:56:17.637227 pyatp-1.2.0/src/ailab/examples/moss/train.py
--rw-r--r--   0        0        0      174 2023-07-24 02:56:17.637288 pyatp-1.2.0/src/ailab/examples/moss/train.sh
--rw-r--r--   0        0        0     1918 2023-07-24 02:56:17.637332 pyatp-1.2.0/src/ailab/examples/moss/train_imp.py
--rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.0/src/ailab/examples/open_llama/__init__.py
--rw-r--r--   0        0        0      243 2023-07-24 02:56:17.637417 pyatp-1.2.0/src/ailab/examples/open_llama/requirements.txt
--rw-r--r--   0        0        0     2305 2023-07-07 02:48:41.671384 pyatp-1.2.0/src/ailab/examples/open_llama/train.py
--rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.0/src/ailab/examples/standford_alpaca/__init__.py
--rw-r--r--   0        0        0     1111 2023-08-08 11:02:41.070837 pyatp-1.2.0/src/ailab/examples/standford_alpaca/evaluator.py
--rw-r--r--   0        0        0      243 2023-07-24 02:56:17.637493 pyatp-1.2.0/src/ailab/examples/standford_alpaca/requirements.txt
--rw-r--r--   0        0        0      468 2023-07-11 08:36:20.385500 pyatp-1.2.0/src/ailab/examples/standford_alpaca/train.py
--rw-r--r--   0        0        0      174 2023-07-11 09:48:59.098039 pyatp-1.2.0/src/ailab/examples/standford_alpaca/train.sh
--rw-r--r--   0        0        0     2161 2023-07-24 02:56:17.637578 pyatp-1.2.0/src/ailab/examples/standford_alpaca/train_imp.py
--rw-r--r--   0        0        0      494 2023-06-12 09:33:01.581239 pyatp-1.2.0/src/ailab/examples/text_classification/README.md
--rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.0/src/ailab/examples/text_classification/__init__.py
--rw-r--r--   0        0        0      243 2023-07-24 02:56:17.637657 pyatp-1.2.0/src/ailab/examples/text_classification/requirements.txt
--rw-r--r--   0        0        0     2521 2023-06-30 08:10:49.356596 pyatp-1.2.0/src/ailab/examples/text_classification/train.py
--rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.750461 pyatp-1.2.0/src/ailab/inference_wrapper/__init__.py
--rw-r--r--   0        0        0      637 2023-03-02 05:17:14.587000 pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/Dockerfile
--rw-r--r--   0        0        0      198 2023-03-02 05:17:14.586000 pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/README.md
--rw-r--r--   0        0        0       53 2023-03-02 05:17:28.917000 pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/requirements.txt
--rw-r--r--   0        0        0    95827 2023-03-02 05:17:14.588000 pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.png
--rw-r--r--   0        0        0      918 2023-03-02 08:23:57.053000 pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.py
--rw-r--r--   0        0        0     6286 2023-03-02 05:21:16.095000 pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/wrapper.py
--rw-r--r--   0        0        0       85 2023-03-21 05:26:30.958000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/README.md
--rw-r--r--   0        0        0      637 2023-03-23 14:04:01.930000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/Dockerfile
--rw-r--r--   0        0        0      182 2023-03-31 02:08:50.009000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/readme.md
--rw-r--r--   0        0        0       84 2023-03-23 14:04:01.931000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/requirements.txt
--rw-r--r--   0        0        0   178529 2023-03-23 14:04:01.931000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/sketch-mountains-input.jpg
--rw-r--r--   0        0        0     2992 2023-03-31 02:08:50.009000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-23 14:04:01.932000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/Dockerfile
--rw-r--r--   0        0        0       84 2023-03-23 14:04:01.932000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-31 02:08:50.010000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-23 14:04:01.932000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/Dockerfile
--rw-r--r--   0        0        0      144 2023-03-31 02:08:50.010000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/readme.md
--rw-r--r--   0        0        0       84 2023-03-23 14:04:01.932000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/requirements.txt
--rw-r--r--   0        0        0  1333615 2023-03-23 14:04:01.933000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/horse.png
--rw-r--r--   0        0        0     3303 2023-03-31 02:08:50.010000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-23 14:04:01.934000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/Dockerfile
--rw-r--r--   0        0        0       84 2023-03-23 14:04:01.934000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-31 02:08:50.010000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-31 02:08:50.010000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/Dockerfile
--rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/Dockerfile
--rw-r--r--   0        0        0      260 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/readme.md
--rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/requirements.txt
--rw-r--r--   0        0        0     3349 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/Dockerfile
--rw-r--r--   0        0        0      232 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/readme.md
--rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/requirements.txt
--rw-r--r--   0        0        0   173131 2023-03-31 02:08:50.012000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/000000039769.jpg
--rw-r--r--   0        0        0     2997 2023-03-31 02:08:50.012000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-23 14:04:01.934000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/Dockerfile
--rw-r--r--   0        0        0      194 2023-03-31 02:08:50.012000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/readme.md
--rw-r--r--   0        0        0       84 2023-03-23 14:04:01.934000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/requirements.txt
--rw-r--r--   0        0        0   178529 2023-03-23 14:04:01.935000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/sketch-mountains-input.jpg
--rw-r--r--   0        0        0     3045 2023-03-31 02:08:50.012000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-31 02:08:50.012000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/Dockerfile
--rw-r--r--   0        0        0      213 2023-03-31 02:08:50.012000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/readme.md
--rw-r--r--   0        0        0       84 2023-03-31 02:08:50.012000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/requirements.txt
--rw-r--r--   0        0        0   404753 2023-03-31 02:08:50.014000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo.png
--rw-r--r--   0        0        0    12106 2023-03-31 02:08:50.014000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo_mask.png
--rw-r--r--   0        0        0     3375 2023-03-31 02:08:50.014000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-31 02:08:50.015000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/Dockerfile
--rw-r--r--   0        0        0      231 2023-03-31 02:08:50.015000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/readme.md
--rw-r--r--   0        0        0       84 2023-03-31 02:08:50.015000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/requirements.txt
--rw-r--r--   0        0        0   408679 2023-03-31 02:08:50.016000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/mountain.png
--rw-r--r--   0        0        0     3076 2023-03-31 02:08:50.016000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-31 02:08:50.016000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/Dockerfile
--rw-r--r--   0        0        0      319 2023-03-31 02:08:50.016000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/readme.md
--rw-r--r--   0        0        0       84 2023-03-31 02:08:50.016000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/requirements.txt
--rw-r--r--   0        0        0     3075 2023-03-31 02:08:50.016000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/wrapper/wrapper.py
--rw-r--r--   0        0        0      159 2023-03-31 02:08:50.016000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/readme.md
--rw-r--r--   0        0        0      637 2023-03-31 02:08:50.017000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/Dockerfile
--rw-r--r--   0        0        0      201 2023-03-31 02:08:50.017000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/readme.md
--rw-r--r--   0        0        0       84 2023-03-31 02:08:50.017000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/requirements.txt
--rw-r--r--   0        0        0     2958 2023-03-31 02:08:50.018000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-31 02:08:50.018000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/Dockerfile
--rw-r--r--   0        0        0      170 2023-03-31 02:08:50.018000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/readme.md
--rw-r--r--   0        0        0       84 2023-03-31 02:08:50.018000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/requirements.txt
--rw-r--r--   0        0        0    26358 2023-03-31 02:08:50.018000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/low_res_cat.png
--rw-r--r--   0        0        0     2992 2023-03-31 02:08:50.018000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-23 14:04:01.935000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/Dockerfile
--rw-r--r--   0        0        0      158 2023-03-31 02:08:50.018000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/readme.md
--rw-r--r--   0        0        0       84 2023-03-23 14:04:01.935000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/requirements.txt
--rw-r--r--   0        0        0     2947 2023-03-23 14:04:01.935000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-06-16 06:41:03.321672 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/Dockerfile
--rw-r--r--   0        0        0       35 2023-06-16 06:43:57.737553 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/requirements.txt
--rw-r--r--   0        0        0     4977 2023-07-07 03:56:36.825063 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-06-29 08:23:27.283839 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/Dockerfile
--rw-r--r--   0        0        0       29 2023-06-29 08:23:27.283891 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/requirements.txt
--rw-r--r--   0        0        0     4532 2023-07-24 02:56:17.638076 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-07-24 02:56:17.638302 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/Dockerfile
--rw-r--r--   0        0        0       29 2023-07-24 02:56:17.638370 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/requirements.txt
--rw-r--r--   0        0        0     4535 2023-07-24 02:56:17.638444 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-07-24 02:56:17.638530 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/Dockerfile
--rw-r--r--   0        0        0       29 2023-07-24 02:56:17.638575 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/requirements.txt
--rw-r--r--   0        0        0     4477 2023-07-24 02:56:17.638640 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/wrapper/wrapper.py
--rw-r--r--   0        0        0        0 2023-06-16 06:41:03.321927 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm/Dockerfile
--rw-r--r--   0        0        0       68 2023-07-07 07:54:55.874885 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm/requirements.txt
--rw-r--r--   0        0        0     4268 2023-07-07 03:56:36.837829 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-07-07 02:48:41.671637 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/Dockerfile
--rw-r--r--   0        0        0       29 2023-07-07 02:48:41.671851 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/requirements.txt
--rw-r--r--   0        0        0     4144 2023-07-07 03:56:36.834638 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-06-20 06:18:50.440549 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/Dockerfile
--rw-r--r--   0        0        0       29 2023-06-20 06:18:50.440773 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/requirements.txt
--rw-r--r--   0        0        0     5593 2023-07-07 03:56:47.748355 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-07-24 02:56:17.638728 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/Dockerfile
--rw-r--r--   0        0        0       29 2023-07-24 02:56:17.638772 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/requirements.txt
--rw-r--r--   0        0        0     4530 2023-07-24 02:56:17.638843 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-06-29 08:23:27.284109 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/Dockerfile
--rw-r--r--   0        0        0       35 2023-06-29 08:23:27.284234 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/requirements.txt
--rw-r--r--   0        0        0     5534 2023-07-07 03:57:08.083845 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-06-16 06:41:03.322232 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/Dockerfile
--rw-r--r--   0        0        0       35 2023-06-16 06:44:11.271284 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/requirements.txt
--rw-r--r--   0        0        0     5544 2023-07-07 03:57:20.980440 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/wrapper/wrapper.py
--rw-r--r--   0        0        0     2823 2023-03-21 05:26:30.958000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/README.md
--rw-r--r--   0        0        0     1151 2023-06-06 06:46:33.750578 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/__init__.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.708000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/Dockerfile
--rw-r--r--   0        0        0       63 2023-03-19 14:49:24.708000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/requirements.txt
--rw-r--r--   0        0        0   383447 2023-03-19 14:49:24.709000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/mlk.flac
--rw-r--r--   0        0        0     2360 2023-03-21 05:26:30.958000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-02 05:19:51.931000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/Dockerfile
--rw-r--r--   0        0        0       63 2023-03-02 05:19:51.931000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/requirements.txt
--rw-r--r--   0        0        0   383447 2023-03-02 05:19:51.932000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/mlk.flac
--rw-r--r--   0        0        0     2619 2023-03-19 14:49:24.710000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.710000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.710000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/requirements.txt
--rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.710000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/cat.jpg
--rw-r--r--   0        0        0    10942 2023-03-19 14:49:24.711000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/result_depth.jpeg
--rw-r--r--   0        0        0     2899 2023-03-19 14:49:24.711000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.711000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/Dockerfile
--rw-r--r--   0        0        0       64 2023-03-19 14:49:24.711000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/requirements.txt
--rw-r--r--   0        0        0   434332 2023-03-19 14:49:24.712000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/img.png
--rw-r--r--   0        0        0     2539 2023-03-19 14:49:24.712000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.713000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/Dockerfile
--rw-r--r--   0        0        0       98 2023-03-19 14:49:24.713000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/requirements.txt
--rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.713000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/cat.jpg
--rw-r--r--   0        0        0     9565 2023-03-19 14:49:24.713000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_1.jpg
--rw-r--r--   0        0        0     5000 2023-03-19 14:49:24.713000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_2.jpg
--rw-r--r--   0        0        0     4937 2023-03-19 14:49:24.713000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_3.jpg
--rw-r--r--   0        0        0    20405 2023-03-19 14:49:24.713000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_4.jpg
--rw-r--r--   0        0        0    10041 2023-03-19 14:49:24.713000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_5.jpg
--rw-r--r--   0        0        0    63187 2023-03-19 14:49:24.714000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/test_str_to_img.jpg
--rw-r--r--   0        0        0     3164 2023-03-19 14:49:24.714000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.714000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.714000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/requirements.txt
--rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.714000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/cat.jpg
--rw-r--r--   0        0        0     2433 2023-03-19 14:49:24.714000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.714000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/Dockerfile
--rw-r--r--   0        0        0       64 2023-03-21 05:26:30.959000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/requirements.txt
--rw-r--r--   0        0        0     2897 2023-03-21 05:26:30.959000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.718000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/Dockerfile
--rw-r--r--   0        0        0       63 2023-03-19 14:49:24.718000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/requirements.txt
--rw-r--r--   0        0        0   434332 2023-03-19 14:49:24.718000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/img.png
--rw-r--r--   0        0        0     2754 2023-03-19 14:49:24.718000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.718000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/Dockerfile
--rw-r--r--   0        0        0       64 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/requirements.txt
--rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/cat.jpg
--rw-r--r--   0        0        0     2914 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-21 05:26:30.959000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/Dockerfile
--rw-r--r--   0        0        0       75 2023-03-21 05:26:30.960000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/requirements.txt
--rw-r--r--   0        0        0    76876 2023-03-21 05:26:30.960000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/doc.png
--rw-r--r--   0        0        0     2747 2023-03-21 05:26:30.960000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-21 05:26:30.960000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/Dockerfile
--rw-r--r--   0        0        0       63 2023-03-21 05:26:30.961000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/requirements.txt
--rw-r--r--   0        0        0     2404 2023-03-21 05:26:30.961000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-21 05:26:30.961000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/Dockerfile
--rw-r--r--   0        0        0       75 2023-03-21 05:26:30.961000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/requirements.txt
--rw-r--r--   0        0        0   173131 2023-03-21 05:26:30.962000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/cat.jpg
--rw-r--r--   0        0        0     2454 2023-03-21 05:26:30.962000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-21 05:26:30.962000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/Dockerfile
--rw-r--r--   0        0        0       75 2023-03-21 05:26:30.962000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/requirements.txt
--rw-r--r--   0        0        0   173131 2023-03-21 05:26:30.963000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/cat.jpg
--rw-r--r--   0        0        0     2780 2023-03-21 05:26:30.963000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/requirements.txt
--rw-r--r--   0        0        0     2486 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/requirements.txt
--rw-r--r--   0        0        0     2386 2023-03-19 14:49:24.719000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/requirements.txt
--rw-r--r--   0        0        0     2641 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-02 05:19:51.937000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/Dockerfile
--rw-r--r--   0        0        0      435 2023-03-02 05:19:51.937000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/README.md
--rw-r--r--   0        0        0       63 2023-03-02 05:19:51.938000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/requirements.txt
--rw-r--r--   0        0        0     2475 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/requirements.txt
--rw-r--r--   0        0        0     3602 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/Dockerfile
--rw-r--r--   0        0        0       92 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/requirements.txt
--rw-r--r--   0        0        0     2832 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/requirements.txt
--rw-r--r--   0        0        0     2410 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-02 05:19:51.938000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/Dockerfile
--rw-r--r--   0        0        0        4 2023-06-06 06:46:33.750677 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/packages.txt
--rw-r--r--   0        0        0       64 2023-03-02 05:19:51.938000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/requirements.txt
--rw-r--r--   0        0        0     2865 2023-06-13 08:27:55.299240 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/requirements.txt
--rw-r--r--   0        0        0     2678 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/requirements.txt
--rw-r--r--   0        0        0     2523 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/requirements.txt
--rw-r--r--   0        0        0     2392 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/wrapper/wrapper.py
--rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/Dockerfile
--rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/requirements.txt
--rw-r--r--   0        0        0     2711 2023-03-19 14:49:24.722000 pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/wrapper/wrapper.py
--rw-r--r--   0        0        0        6 2023-03-06 07:33:04.130000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/requirements.txt
--rw-r--r--   0        0        0     3701 2023-03-06 08:14:31.141000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.dockerignore
--rw-r--r--   0        0        0       75 2023-03-06 08:14:31.141000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.gitattributes
--rw-r--r--   0        0        0     2938 2023-03-06 08:14:31.141000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      280 2023-03-06 08:14:31.141000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1803 2023-03-06 08:14:31.141000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1149 2023-03-06 08:14:31.141000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0        0        0      693 2023-03-06 08:14:31.141000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      441 2023-03-06 08:14:31.141000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/dependabot.yml
--rw-r--r--   0        0        0     6789 2023-03-23 14:04:01.875000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/ci-testing.yml
--rw-r--r--   0        0        0     2051 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1572 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/docker.yml
--rw-r--r--   0        0        0     5434 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/greetings.yml
--rw-r--r--   0        0        0     2014 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/stale.yml
--rw-r--r--   0        0        0      707 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/translate-readme.yml
--rwxr-xr-x   0        0        0     3998 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.gitignore
--rw-r--r--   0        0        0     1747 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      392 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/CITATION.cff
--rw-r--r--   0        0        0     4999 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/CONTRIBUTING.md
--rw-r--r--   0        0        0    35127 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/LICENSE
--rw-r--r--   0        0        0    40553 2023-03-06 08:14:31.142000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.md
--rw-r--r--   0        0        0    39592 2023-03-06 08:14:31.143000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.zh-CN.md
--rw-r--r--   0        0        0     7830 2023-03-06 08:14:31.143000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/benchmarks.py
--rw-r--r--   0        0        0    11730 2023-03-06 08:14:31.143000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/predict.py
--rw-r--r--   0        0        0    16383 2023-05-26 01:51:19.920034 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/train.py
--rw-r--r--   0        0        0   103520 2023-03-06 08:14:31.143000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/tutorial.ipynb
--rw-r--r--   0        0        0     8056 2023-03-06 08:14:31.143000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/val.py
--rw-r--r--   0        0        0     2733 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Argoverse.yaml
--rw-r--r--   0        0        0     1885 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/GlobalWheat2020.yaml
--rw-r--r--   0        0        0    18871 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/ImageNet.yaml
--rw-r--r--   0        0        0     9205 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Objects365.yaml
--rw-r--r--   0        0        0     2341 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/SKU-110K.yaml
--rw-r--r--   0        0        0     3493 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VOC.yaml
--rw-r--r--   0        0        0     2971 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VisDrone.yaml
--rw-r--r--   0        0        0     2495 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco.yaml
--rw-r--r--   0        0        0     1868 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128-seg.yaml
--rw-r--r--   0        0        0     1852 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128.yaml
--rw-r--r--   0        0        0      673 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.Objects365.yaml
--rw-r--r--   0        0        0     1156 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.VOC.yaml
--rw-r--r--   0        0        0     1684 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.no-augmentation.yaml
--rw-r--r--   0        0        0     1683 2023-03-06 08:14:31.144000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-high.yaml
--rw-r--r--   0        0        0     1691 2023-03-06 08:14:31.145000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-low.yaml
--rw-r--r--   0        0        0     1685 2023-03-06 08:14:31.145000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-med.yaml
--rw-r--r--   0        0        0   487438 2023-03-06 08:14:31.145000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/bus.jpg
--rw-r--r--   0        0        0   168949 2023-03-06 08:14:31.146000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/zidane.jpg
--rwxr-xr-x   0        0        0      640 2023-03-06 08:14:31.146000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/download_weights.sh
--rwxr-xr-x   0        0        0     1566 2023-03-06 08:14:31.146000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco.sh
--rwxr-xr-x   0        0        0      618 2023-03-06 08:14:31.146000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco128.sh
--rwxr-xr-x   0        0        0     1671 2023-03-06 08:14:31.146000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_imagenet.sh
--rw-r--r--   0        0        0     5170 2023-03-06 08:14:31.146000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/xView.yaml
--rw-r--r--   0        0        0    14292 2023-03-06 08:14:31.146000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/detect.py
--rw-r--r--   0        0        0    32063 2023-05-26 01:51:19.911068 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/export.py
--rw-r--r--   0        0        0     7767 2023-05-26 01:51:19.923788 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/hubconf.py
--rw-r--r--   0        0        0        0 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/__init__.py
--rw-r--r--   0        0        0    41702 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/common.py
--rw-r--r--   0        0        0     4319 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/experimental.py
--rw-r--r--   0        0        0     3335 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/anchors.yaml
--rw-r--r--   0        0        0     1567 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-spp.yaml
--rw-r--r--   0        0        0     1232 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-tiny.yaml
--rw-r--r--   0        0        0     1558 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3.yaml
--rw-r--r--   0        0        0     1423 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-bifpn.yaml
--rw-r--r--   0        0        0     1214 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-fpn.yaml
--rw-r--r--   0        0        0     1687 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p2.yaml
--rw-r--r--   0        0        0     1349 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p34.yaml
--rw-r--r--   0        0        0     1741 2023-03-06 08:14:31.147000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p6.yaml
--rw-r--r--   0        0        0     2122 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p7.yaml
--rw-r--r--   0        0        0     1407 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-panet.yaml
--rw-r--r--   0        0        0     1820 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5l6.yaml
--rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5m6.yaml
--rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5n6.yaml
--rw-r--r--   0        0        0     1497 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-LeakyReLU.yaml
--rw-r--r--   0        0        0     1483 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-ghost.yaml
--rw-r--r--   0        0        0     1441 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-transformer.yaml
--rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s6.yaml
--rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5x6.yaml
--rw-r--r--   0        0        0     1411 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5l-seg.yaml
--rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5m-seg.yaml
--rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5n-seg.yaml
--rw-r--r--   0        0        0     1412 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5s-seg.yaml
--rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5x-seg.yaml
--rw-r--r--   0        0        0    27032 2023-05-26 01:51:19.958775 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/tf.py
--rw-r--r--   0        0        0    17780 2023-05-26 01:51:19.931156 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolo.py
--rw-r--r--   0        0        0     1401 2023-03-06 08:14:31.149000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5l.yaml
--rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5m.yaml
--rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5n.yaml
--rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5s.yaml
--rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5x.yaml
--rw-r--r--   0        0        0     1593 2023-03-06 08:14:31.149000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/requirements.txt
--rw-r--r--   0        0        0    15743 2023-03-06 08:14:31.149000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/predict.py
--rw-r--r--   0        0        0    34678 2023-03-23 14:04:01.875000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/train.py
--rw-r--r--   0        0        0    43293 2023-03-06 08:14:31.150000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/tutorial.ipynb
--rw-r--r--   0        0        0    24005 2023-03-06 08:14:31.150000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/val.py
--rw-r--r--   0        0        0     1727 2023-03-06 08:14:31.150000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/setup.cfg
--rw-r--r--   0        0        0    33701 2023-03-06 08:14:31.150000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/train.py
--rw-r--r--   0        0        0    54258 2023-03-06 08:14:31.150000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/tutorial.ipynb
--rw-r--r--   0        0        0     2432 2023-03-06 08:14:31.150000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/__init__.py
--rw-r--r--   0        0        0     3449 2023-03-06 08:14:31.151000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/activations.py
--rw-r--r--   0        0        0    17030 2023-03-06 08:14:31.151000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/augmentations.py
--rw-r--r--   0        0        0     7420 2023-03-06 08:14:31.151000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autoanchor.py
--rw-r--r--   0        0        0     3003 2023-05-26 01:51:19.914199 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autobatch.py
--rw-r--r--   0        0        0        0 2023-03-06 08:14:31.151000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/__init__.py
--rw-r--r--   0        0        0      780 2023-03-06 08:14:31.151000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/mime.sh
--rw-r--r--   0        0        0     1198 2023-03-06 08:14:31.151000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/resume.py
--rw-r--r--   0        0        0     1247 2023-03-06 08:14:31.151000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/userdata.sh
--rw-r--r--   0        0        0     2661 2023-03-06 08:14:31.151000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/callbacks.py
--rw-r--r--   0        0        0    55779 2023-05-26 01:51:19.947412 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/dataloaders.py
--rw-r--r--   0        0        0     2709 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile
--rw-r--r--   0        0        0     1682 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-arm64
--rw-r--r--   0        0        0     1707 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-cpu
--rw-r--r--   0        0        0     4952 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/downloads.py
--rw-r--r--   0        0        0     1710 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/README.md
--rw-r--r--   0        0        0      368 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/example_request.py
--rw-r--r--   0        0        0     1439 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/restapi.py
--rw-r--r--   0        0        0    46844 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/general.py
--rw-r--r--   0        0        0      821 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/Dockerfile
--rw-r--r--   0        0        0      187 2023-03-06 08:14:31.152000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/additional_requirements.txt
--rw-r--r--   0        0        0      174 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/app.yaml
--rw-r--r--   0        0        0    16635 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/__init__.py
--rw-r--r--   0        0        0    10862 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/README.md
--rw-r--r--   0        0        0        0 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/__init__.py
--rw-r--r--   0        0        0     8034 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/clearml_utils.py
--rw-r--r--   0        0        0     5271 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/hpo.py
--rw-r--r--   0        0        0    10772 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/README.md
--rw-r--r--   0        0        0    18731 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/__init__.py
--rw-r--r--   0        0        0     4751 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/comet_utils.py
--rw-r--r--   0        0        0     6653 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/hpo.py
--rw-r--r--   0        0        0        0 2023-03-06 08:14:31.153000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/wandb/__init__.py
--rw-r--r--   0        0        0     8252 2023-03-06 08:14:31.154000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/wandb/wandb_utils.py
--rw-r--r--   0        0        0     9919 2023-03-06 08:14:31.154000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loss.py
--rw-r--r--   0        0        0    14568 2023-03-06 08:14:31.154000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/metrics.py
--rw-r--r--   0        0        0    24501 2023-05-26 01:51:19.940339 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/plots.py
--rw-r--r--   0        0        0        0 2023-03-06 08:14:31.154000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/__init__.py
--rw-r--r--   0        0        0     3756 2023-03-06 08:14:31.154000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/augmentations.py
--rw-r--r--   0        0        0    13835 2023-03-06 08:14:31.154000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/dataloaders.py
--rw-r--r--   0        0        0     5813 2023-03-23 14:04:01.876000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/general.py
--rw-r--r--   0        0        0     8591 2023-03-23 14:04:01.876000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/loss.py
--rw-r--r--   0        0        0     5457 2023-03-06 08:14:31.154000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/metrics.py
--rw-r--r--   0        0        0     6386 2023-03-23 14:04:01.876000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/plots.py
--rw-r--r--   0        0        0    19655 2023-05-26 01:51:19.900763 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/torch_utils.py
--rw-r--r--   0        0        0     3634 2023-03-06 08:14:31.155000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/triton.py
--rw-r--r--   0        0        0    20424 2023-03-06 08:14:31.155000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/val.py
--rw-r--r--   0        0        0     4932 2023-03-06 08:24:07.583000 pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/wrapper.py
--rw-r--r--   0        0        0     2460 2023-07-26 06:13:00.898000 pyatp-1.2.0/src/ailab/log.py
--rw-r--r--   0        0        0        0 2023-05-03 13:25:57.748000 pyatp-1.2.0/src/ailab/log_cycle/__init__.py
--rw-r--r--   0        0        0      531 2023-05-03 13:25:57.748000 pyatp-1.2.0/src/ailab/log_cycle/json_handler.py
--rw-r--r--   0        0        0     2007 2023-05-26 01:43:21.934000 pyatp-1.2.0/src/ailab/templates/README.md
--rw-r--r--   0        0        0      542 2023-05-26 01:43:21.934000 pyatp-1.2.0/src/ailab/templates/alpaca.json
--rw-r--r--   0        0        0      561 2023-05-26 01:43:21.934000 pyatp-1.2.0/src/ailab/templates/alpaca_legacy.json
--rw-r--r--   0        0        0      281 2023-05-26 01:43:21.934000 pyatp-1.2.0/src/ailab/templates/alpaca_short.json
--rw-r--r--   0        0        0      605 2023-05-26 01:43:21.934000 pyatp-1.2.0/src/ailab/templates/vigogne.json
--rw-r--r--   0        0        0      239 2023-05-29 01:38:01.672199 pyatp-1.2.0/src/ailab/utils/README.md
--rw-r--r--   0        0        0        0 2023-05-29 01:38:01.672232 pyatp-1.2.0/src/ailab/utils/__init__.py
--rw-r--r--   0        0        0     2384 2023-06-01 08:42:34.256596 pyatp-1.2.0/src/ailab/utils/callbacks.py
--rw-r--r--   0        0        0     3567 2023-07-07 02:48:41.672107 pyatp-1.2.0/src/ailab/utils/other.py
--rw-r--r--   0        0        0     1837 2023-06-16 06:41:03.322556 pyatp-1.2.0/src/ailab/utils/prompter.py
--rw-r--r--   0        0        0    35352 2023-06-30 08:10:49.357368 pyatp-1.2.0/src/ailab/utils/streampeft.py
--rw-r--r--   0        0        0     7901 2023-08-08 11:02:41.070938 pyatp-1.2.0/src/ailab/utils/template.py
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 pyatp-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-08 09:45:37.719000 pyatp-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1325 2023-08-09 02:30:42.833184 pyatp-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1151 2023-05-26 01:51:19.942655 pyatp-1.2.1/src/ailab/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.707000 pyatp-1.2.1/src/ailab/atp_dataset/__init__.py
+-rw-r--r--   0        0        0     1189 2023-05-26 01:43:21.707000 pyatp-1.2.1/src/ailab/atp_dataset/ailab_api.py
+-rw-r--r--   0        0        0      362 2023-07-24 02:56:17.630929 pyatp-1.2.1/src/ailab/atp_dataset/constant.py
+-rw-r--r--   0        0        0     4367 2023-07-24 02:56:17.631639 pyatp-1.2.1/src/ailab/atp_dataset/dataset.py
+-rw-r--r--   0        0        0     1975 2023-06-07 09:32:17.327152 pyatp-1.2.1/src/ailab/atp_dataset/huggingface_api.py
+-rw-r--r--   0        0        0       98 2023-07-26 06:13:53.570112 pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-26 06:13:53.570258 pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/base.py
+-rw-r--r--   0        0        0     5961 2023-08-08 11:02:41.061148 pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/ceval.py
+-rw-r--r--   0        0        0     5638 2023-08-08 11:02:41.061214 pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/harness.py
+-rw-r--r--   0        0        0     7518 2023-08-08 11:02:41.061313 pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/mmlu.py
+-rw-r--r--   0        0        0      695 2023-08-08 11:02:41.061395 pyatp-1.2.1/src/ailab/atp_evaluation/build.py
+-rw-r--r--   0        0        0     2002 2023-08-08 11:02:41.061479 pyatp-1.2.1/src/ailab/atp_evaluation/constant.py
+-rw-r--r--   0        0        0     1503 2023-08-08 11:02:41.061583 pyatp-1.2.1/src/ailab/atp_evaluation/evaluator.py
+-rw-r--r--   0        0        0       97 2023-07-26 06:13:53.570908 pyatp-1.2.1/src/ailab/atp_evaluation/models/__init__.py
+-rw-r--r--   0        0        0     1194 2023-07-26 06:13:53.570990 pyatp-1.2.1/src/ailab/atp_evaluation/models/base.py
+-rw-r--r--   0        0        0     5278 2023-08-08 11:02:41.061699 pyatp-1.2.1/src/ailab/atp_evaluation/models/chatglm.py
+-rw-r--r--   0        0        0     4132 2023-08-08 11:02:41.061798 pyatp-1.2.1/src/ailab/atp_evaluation/models/llama.py
+-rw-r--r--   0        0        0      155 2023-06-08 02:31:25.029113 pyatp-1.2.1/src/ailab/atp_finetuner/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-26 01:43:21.707000 pyatp-1.2.1/src/ailab/atp_finetuner/accelerator/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-30 08:10:49.352351 pyatp-1.2.1/src/ailab/atp_finetuner/accelerator/accelerator.py
+-rw-r--r--   0        0        0      766 2023-05-26 01:43:21.707000 pyatp-1.2.1/src/ailab/atp_finetuner/build.py
+-rw-r--r--   0        0        0     2426 2023-08-08 11:02:41.061898 pyatp-1.2.1/src/ailab/atp_finetuner/constant.py
+-rw-r--r--   0        0        0      402 2023-08-08 11:02:41.061985 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/__init__.py
+-rw-r--r--   0        0        0     1650 2023-08-08 11:02:41.062638 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/datacollator.py
+-rw-r--r--   0        0        0      987 2023-08-08 11:02:41.063097 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_alpaca.py
+-rw-r--r--   0        0        0     1371 2023-08-08 11:02:41.063186 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_baichuan.py
+-rw-r--r--   0        0        0     7762 2023-08-08 11:02:41.063836 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_chatglm.py
+-rw-r--r--   0        0        0     1492 2023-08-08 11:02:41.064479 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_chinese_alpaca.py
+-rw-r--r--   0        0        0     1026 2023-08-08 11:02:41.064894 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_language.py
+-rw-r--r--   0        0        0      972 2023-08-08 11:02:41.064961 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_token.py
+-rw-r--r--   0        0        0      922 2023-08-08 11:02:41.065028 pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_with_padding.py
+-rw-r--r--   0        0        0     1721 2023-08-08 11:02:41.065582 pyatp-1.2.1/src/ailab/atp_finetuner/finetuner.py
+-rw-r--r--   0        0        0       64 2023-05-26 01:43:21.708000 pyatp-1.2.1/src/ailab/atp_finetuner/metric/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-26 02:34:59.536185 pyatp-1.2.1/src/ailab/atp_finetuner/metric/accury.py
+-rw-r--r--   0        0        0      425 2023-05-26 02:03:39.174407 pyatp-1.2.1/src/ailab/atp_finetuner/metric/metric.py
+-rw-r--r--   0        0        0       62 2023-05-26 01:43:21.708000 pyatp-1.2.1/src/ailab/atp_finetuner/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.708000 pyatp-1.2.1/src/ailab/atp_finetuner/model/cv/__init__.py
+-rw-r--r--   0        0        0     1018 2023-06-08 07:46:32.642619 pyatp-1.2.1/src/ailab/atp_finetuner/model/model.py
+-rw-r--r--   0        0        0       80 2023-06-01 08:42:34.253788 pyatp-1.2.1/src/ailab/atp_finetuner/model/multimodel/__init__.py
+-rw-r--r--   0        0        0     3456 2023-06-08 07:46:32.642850 pyatp-1.2.1/src/ailab/atp_finetuner/model/multimodel/model_for_sd_lora.py
+-rw-r--r--   0        0        0     1172 2023-06-08 07:46:32.642989 pyatp-1.2.1/src/ailab/atp_finetuner/model/multimodel/vilt_for_vqa.py
+-rw-r--r--   0        0        0      380 2023-08-08 11:02:41.065674 pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/__init__.py
+-rw-r--r--   0        0        0     4607 2023-08-08 11:02:41.065765 pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_baichuan.py
+-rw-r--r--   0        0        0     3222 2023-08-08 11:02:41.065846 pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_chatglm.py
+-rw-r--r--   0        0        0     1081 2023-06-20 06:18:50.439752 pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_chinese_alpaca.py
+-rw-r--r--   0        0        0     1933 2023-07-11 08:36:20.383161 pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_lora.py
+-rw-r--r--   0        0        0      820 2023-06-08 07:46:32.643745 pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_question_answer.py
+-rw-r--r--   0        0        0      830 2023-06-08 07:46:32.643860 pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_text_classification.py
+-rw-r--r--   0        0        0      830 2023-06-08 07:46:32.643967 pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_token_classification.py
+-rw-r--r--   0        0        0       78 2023-05-26 01:43:21.709000 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.709000 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/cv/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-26 01:43:21.709000 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/multimodel/__init__.py
+-rw-r--r--   0        0        0     3009 2023-06-08 07:46:32.644131 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_sd_lora.py
+-rw-r--r--   0        0        0     3488 2023-06-08 07:46:32.644260 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_vilt_vqa.py
+-rw-r--r--   0        0        0      378 2023-08-08 11:02:41.065929 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/__init__.py
+-rw-r--r--   0        0        0     3150 2023-06-12 08:33:22.791142 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_alpaca.py
+-rw-r--r--   0        0        0     5557 2023-08-08 11:02:41.066022 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_baichuan.py
+-rw-r--r--   0        0        0     4212 2023-08-08 11:02:41.066639 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chatglm.py
+-rw-r--r--   0        0        0     3601 2023-06-20 06:18:50.439972 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chinese_alpaca.py
+-rw-r--r--   0        0        0     2852 2023-06-29 08:23:27.282928 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_llama_cn.py
+-rw-r--r--   0        0        0     3586 2023-06-08 07:46:32.644729 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/question_answer_pc.py
+-rw-r--r--   0        0        0     1184 2023-06-08 07:46:32.644837 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/text_classification_pc.py
+-rw-r--r--   0        0        0     1112 2023-06-08 07:46:32.644960 pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/preprossor.py
+-rw-r--r--   0        0        0       65 2023-05-26 01:43:21.710000 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 01:43:21.710000 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/cv/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-26 01:43:21.710000 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/multimodel/__init__.py
+-rw-r--r--   0        0        0    10436 2023-06-01 08:42:34.255060 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_sd_lora.py
+-rw-r--r--   0        0        0     4244 2023-06-01 08:42:34.255151 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_vilt_vqa.py
+-rw-r--r--   0        0        0      387 2023-08-08 11:02:41.066738 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-20 06:18:50.440170 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/ds_zero2_no_offload.json
+-rw-r--r--   0        0        0     5698 2023-07-11 08:36:20.383850 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_alpaca.py
+-rw-r--r--   0        0        0     6766 2023-08-08 11:02:41.066829 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_baichuan.py
+-rw-r--r--   0        0        0     5909 2023-08-08 11:02:41.069231 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chatglm.py
+-rw-r--r--   0        0        0     6711 2023-07-11 08:36:20.384475 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chinese_alpaca.py
+-rw-r--r--   0        0        0     5359 2023-07-11 08:36:20.384604 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_llama_cn.py
+-rw-r--r--   0        0        0     4090 2023-06-01 08:42:34.255810 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_text_classification.py
+-rw-r--r--   0        0        0     4041 2023-06-01 08:42:34.256415 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/traniner_for_question_answer.py
+-rw-r--r--   0        0        0     1594 2023-06-01 08:42:34.256512 pyatp-1.2.1/src/ailab/atp_finetuner/trainer/trainer.py
+-rw-r--r--   0        0        0     1498 2023-07-11 09:56:17.517435 pyatp-1.2.1/src/ailab/batch/__init__.py
+-rw-r--r--   0        0        0     3749 2023-07-24 02:54:56.630083 pyatp-1.2.1/src/ailab/batch/entrypoint.py
+-rw-r--r--   0        0        0      213 2023-07-11 03:21:15.515185 pyatp-1.2.1/src/ailab/buildkit/Makefile
+-rw-r--r--   0        0        0      335 2023-06-07 06:35:49.073776 pyatp-1.2.1/src/ailab/buildkit/README.md
+-rw-r--r--   0        0        0     1052 2023-07-11 02:23:25.287020 pyatp-1.2.1/src/ailab/buildkit/make.py
+-rw-r--r--   0        0        0      743 2023-07-11 06:26:33.871730 pyatp-1.2.1/src/ailab/buildkit/pyproject.toml
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/__init__.py
+-rw-r--r--   0        0        0    16684 2023-07-11 06:24:54.121544 pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/build.py
+-rw-r--r--   0        0        0     1158 2023-06-29 06:47:07.874124 pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/config.py
+-rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/dotdict.py
+-rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/error.py
+-rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/get-pip.py
+-rw-r--r--   0        0        0     1457 2023-07-11 06:25:49.033583 pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/templates/Dockerfile.j2
+-rw-r--r--   0        0        0     1550 2023-07-07 08:47:51.824731 pyatp-1.2.1/src/ailab/examples/__init__.py
+-rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.1/src/ailab/examples/baichuan/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-24 02:56:17.634030 pyatp-1.2.1/src/ailab/examples/baichuan/requirements.txt
+-rw-r--r--   0        0        0      438 2023-07-24 02:56:17.634648 pyatp-1.2.1/src/ailab/examples/baichuan/train.py
+-rw-r--r--   0        0        0      174 2023-07-24 02:56:17.634777 pyatp-1.2.1/src/ailab/examples/baichuan/train.sh
+-rw-r--r--   0        0        0     1934 2023-07-24 02:56:17.634846 pyatp-1.2.1/src/ailab/examples/baichuan/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-24 02:56:17.635076 pyatp-1.2.1/src/ailab/examples/baichuan_13b/__init__.py
+-rw-r--r--   0        0        0      274 2023-07-24 02:56:17.635127 pyatp-1.2.1/src/ailab/examples/baichuan_13b/requirements.txt
+-rw-r--r--   0        0        0      438 2023-07-24 02:56:17.635177 pyatp-1.2.1/src/ailab/examples/baichuan_13b/train.py
+-rw-r--r--   0        0        0      174 2023-07-24 02:56:17.635246 pyatp-1.2.1/src/ailab/examples/baichuan_13b/train.sh
+-rw-r--r--   0        0        0     1934 2023-07-24 02:56:17.635296 pyatp-1.2.1/src/ailab/examples/baichuan_13b/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-24 02:56:17.635403 pyatp-1.2.1/src/ailab/examples/bloomz/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-24 02:56:17.635455 pyatp-1.2.1/src/ailab/examples/bloomz/requirements.txt
+-rw-r--r--   0        0        0      438 2023-07-24 02:56:17.635502 pyatp-1.2.1/src/ailab/examples/bloomz/train.py
+-rw-r--r--   0        0        0      174 2023-07-24 02:56:17.635562 pyatp-1.2.1/src/ailab/examples/bloomz/train.sh
+-rw-r--r--   0        0        0     1882 2023-07-24 02:56:17.635602 pyatp-1.2.1/src/ailab/examples/bloomz/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.1/src/ailab/examples/chatglm2_6b/__init__.py
+-rw-r--r--   0        0        0      236 2023-07-24 02:56:17.635691 pyatp-1.2.1/src/ailab/examples/chatglm2_6b/requirements.txt
+-rw-r--r--   0        0        0      438 2023-08-08 11:02:41.069329 pyatp-1.2.1/src/ailab/examples/chatglm2_6b/train.py
+-rw-r--r--   0        0        0      174 2023-08-08 11:02:41.069377 pyatp-1.2.1/src/ailab/examples/chatglm2_6b/train.sh
+-rw-r--r--   0        0        0     2005 2023-08-08 11:02:41.069432 pyatp-1.2.1/src/ailab/examples/chatglm2_6b/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280023 pyatp-1.2.1/src/ailab/examples/chatglm_6b/__init__.py
+-rw-r--r--   0        0        0     1142 2023-08-08 11:02:41.069495 pyatp-1.2.1/src/ailab/examples/chatglm_6b/evaluator.py
+-rw-r--r--   0        0        0      254 2023-08-09 02:25:26.431048 pyatp-1.2.1/src/ailab/examples/chatglm_6b/requirements.txt
+-rw-r--r--   0        0        0      546 2023-08-09 02:30:36.076351 pyatp-1.2.1/src/ailab/examples/chatglm_6b/train.py
+-rw-r--r--   0        0        0      198 2023-08-09 02:28:05.884939 pyatp-1.2.1/src/ailab/examples/chatglm_6b/train.sh
+-rw-r--r--   0        0        0     2148 2023-08-08 11:02:41.070178 pyatp-1.2.1/src/ailab/examples/chatglm_6b/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/__init__.py
+-rw-r--r--   0        0        0      963 2023-08-08 11:02:41.070227 pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/evaluator.py
+-rw-r--r--   0        0        0      243 2023-07-24 02:56:17.636318 pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/requirements.txt
+-rw-r--r--   0        0        0      469 2023-07-07 09:09:19.299389 pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/train.py
+-rw-r--r--   0        0        0      175 2023-07-11 07:33:35.250007 pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/train.sh
+-rw-r--r--   0        0        0     2092 2023-07-10 06:33:58.804274 pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/__init__.py
+-rw-r--r--   0        0        0      937 2023-08-08 11:02:41.070276 pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/evaluator.py
+-rw-r--r--   0        0        0      243 2023-07-24 02:56:17.636400 pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/requirements.txt
+-rw-r--r--   0        0        0      468 2023-07-11 08:36:20.385166 pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/train.py
+-rw-r--r--   0        0        0      174 2023-07-11 09:48:59.097911 pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/train.sh
+-rw-r--r--   0        0        0     2207 2023-07-24 02:56:17.636756 pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-24 02:56:17.636849 pyatp-1.2.1/src/ailab/examples/falcon/__init__.py
+-rw-r--r--   0        0        0      245 2023-07-24 02:56:17.636896 pyatp-1.2.1/src/ailab/examples/falcon/requirements.txt
+-rw-r--r--   0        0        0      438 2023-07-24 02:56:17.636942 pyatp-1.2.1/src/ailab/examples/falcon/train.py
+-rw-r--r--   0        0        0      174 2023-07-24 02:56:17.637002 pyatp-1.2.1/src/ailab/examples/falcon/train.sh
+-rw-r--r--   0        0        0     1878 2023-07-24 02:56:17.637044 pyatp-1.2.1/src/ailab/examples/falcon/train_imp.py
+-rw-r--r--   0        0        0      619 2023-08-08 11:02:41.070353 pyatp-1.2.1/src/ailab/examples/harness/evaluator.py
+-rw-r--r--   0        0        0     1653 2023-08-08 11:02:41.070597 pyatp-1.2.1/src/ailab/examples/llama2/__init__.py
+-rw-r--r--   0        0        0      245 2023-08-08 11:02:41.070652 pyatp-1.2.1/src/ailab/examples/llama2/requirements.txt
+-rw-r--r--   0        0        0      434 2023-08-08 11:02:41.070700 pyatp-1.2.1/src/ailab/examples/llama2/train.py
+-rw-r--r--   0        0        0      194 2023-08-08 11:02:41.070745 pyatp-1.2.1/src/ailab/examples/llama2/train.sh
+-rw-r--r--   0        0        0     1842 2023-08-08 11:02:41.070788 pyatp-1.2.1/src/ailab/examples/llama2/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-24 02:56:17.637137 pyatp-1.2.1/src/ailab/examples/moss/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-24 02:56:17.637185 pyatp-1.2.1/src/ailab/examples/moss/requirements.txt
+-rw-r--r--   0        0        0      438 2023-07-24 02:56:17.637227 pyatp-1.2.1/src/ailab/examples/moss/train.py
+-rw-r--r--   0        0        0      174 2023-07-24 02:56:17.637288 pyatp-1.2.1/src/ailab/examples/moss/train.sh
+-rw-r--r--   0        0        0     1918 2023-07-24 02:56:17.637332 pyatp-1.2.1/src/ailab/examples/moss/train_imp.py
+-rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.1/src/ailab/examples/open_llama/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-24 02:56:17.637417 pyatp-1.2.1/src/ailab/examples/open_llama/requirements.txt
+-rw-r--r--   0        0        0     2305 2023-07-07 02:48:41.671384 pyatp-1.2.1/src/ailab/examples/open_llama/train.py
+-rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.1/src/ailab/examples/standford_alpaca/__init__.py
+-rw-r--r--   0        0        0     1111 2023-08-08 11:02:41.070837 pyatp-1.2.1/src/ailab/examples/standford_alpaca/evaluator.py
+-rw-r--r--   0        0        0      243 2023-07-24 02:56:17.637493 pyatp-1.2.1/src/ailab/examples/standford_alpaca/requirements.txt
+-rw-r--r--   0        0        0      468 2023-07-11 08:36:20.385500 pyatp-1.2.1/src/ailab/examples/standford_alpaca/train.py
+-rw-r--r--   0        0        0      174 2023-07-11 09:48:59.098039 pyatp-1.2.1/src/ailab/examples/standford_alpaca/train.sh
+-rw-r--r--   0        0        0     2161 2023-07-24 02:56:17.637578 pyatp-1.2.1/src/ailab/examples/standford_alpaca/train_imp.py
+-rw-r--r--   0        0        0      494 2023-06-12 09:33:01.581239 pyatp-1.2.1/src/ailab/examples/text_classification/README.md
+-rw-r--r--   0        0        0     1653 2023-07-07 03:10:16.280000 pyatp-1.2.1/src/ailab/examples/text_classification/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-24 02:56:17.637657 pyatp-1.2.1/src/ailab/examples/text_classification/requirements.txt
+-rw-r--r--   0        0        0     2521 2023-06-30 08:10:49.356596 pyatp-1.2.1/src/ailab/examples/text_classification/train.py
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.750461 pyatp-1.2.1/src/ailab/inference_wrapper/__init__.py
+-rw-r--r--   0        0        0      637 2023-03-02 05:17:14.587000 pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/Dockerfile
+-rw-r--r--   0        0        0      198 2023-03-02 05:17:14.586000 pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/README.md
+-rw-r--r--   0        0        0       53 2023-03-02 05:17:28.917000 pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/requirements.txt
+-rw-r--r--   0        0        0    95827 2023-03-02 05:17:14.588000 pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.png
+-rw-r--r--   0        0        0      918 2023-03-02 08:23:57.053000 pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.py
+-rw-r--r--   0        0        0     6286 2023-03-02 05:21:16.095000 pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/wrapper.py
+-rw-r--r--   0        0        0       85 2023-03-21 05:26:30.958000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/README.md
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.930000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/Dockerfile
+-rw-r--r--   0        0        0      182 2023-03-31 02:08:50.009000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/readme.md
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.931000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/requirements.txt
+-rw-r--r--   0        0        0   178529 2023-03-23 14:04:01.931000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/sketch-mountains-input.jpg
+-rw-r--r--   0        0        0     2992 2023-03-31 02:08:50.009000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.932000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/Dockerfile
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.932000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-31 02:08:50.010000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.932000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/Dockerfile
+-rw-r--r--   0        0        0      144 2023-03-31 02:08:50.010000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/readme.md
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.932000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/requirements.txt
+-rw-r--r--   0        0        0  1333615 2023-03-23 14:04:01.933000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/horse.png
+-rw-r--r--   0        0        0     3303 2023-03-31 02:08:50.010000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.934000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/Dockerfile
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.934000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-31 02:08:50.010000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.010000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/Dockerfile
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/requirements.txt
+-rw-r--r--   0        0        0        0 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/Dockerfile
+-rw-r--r--   0        0        0      260 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/requirements.txt
+-rw-r--r--   0        0        0     3349 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/Dockerfile
+-rw-r--r--   0        0        0      232 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.011000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-31 02:08:50.012000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/000000039769.jpg
+-rw-r--r--   0        0        0     2997 2023-03-31 02:08:50.012000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.934000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/Dockerfile
+-rw-r--r--   0        0        0      194 2023-03-31 02:08:50.012000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/readme.md
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.934000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/requirements.txt
+-rw-r--r--   0        0        0   178529 2023-03-23 14:04:01.935000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/sketch-mountains-input.jpg
+-rw-r--r--   0        0        0     3045 2023-03-31 02:08:50.012000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.012000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/Dockerfile
+-rw-r--r--   0        0        0      213 2023-03-31 02:08:50.012000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.012000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/requirements.txt
+-rw-r--r--   0        0        0   404753 2023-03-31 02:08:50.014000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo.png
+-rw-r--r--   0        0        0    12106 2023-03-31 02:08:50.014000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo_mask.png
+-rw-r--r--   0        0        0     3375 2023-03-31 02:08:50.014000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.015000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/Dockerfile
+-rw-r--r--   0        0        0      231 2023-03-31 02:08:50.015000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.015000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/requirements.txt
+-rw-r--r--   0        0        0   408679 2023-03-31 02:08:50.016000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/mountain.png
+-rw-r--r--   0        0        0     3076 2023-03-31 02:08:50.016000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.016000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/Dockerfile
+-rw-r--r--   0        0        0      319 2023-03-31 02:08:50.016000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.016000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/requirements.txt
+-rw-r--r--   0        0        0     3075 2023-03-31 02:08:50.016000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/wrapper/wrapper.py
+-rw-r--r--   0        0        0      159 2023-03-31 02:08:50.016000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/readme.md
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.017000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/Dockerfile
+-rw-r--r--   0        0        0      201 2023-03-31 02:08:50.017000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.017000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/requirements.txt
+-rw-r--r--   0        0        0     2958 2023-03-31 02:08:50.018000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-31 02:08:50.018000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/Dockerfile
+-rw-r--r--   0        0        0      170 2023-03-31 02:08:50.018000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/readme.md
+-rw-r--r--   0        0        0       84 2023-03-31 02:08:50.018000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/requirements.txt
+-rw-r--r--   0        0        0    26358 2023-03-31 02:08:50.018000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/low_res_cat.png
+-rw-r--r--   0        0        0     2992 2023-03-31 02:08:50.018000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-23 14:04:01.935000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/Dockerfile
+-rw-r--r--   0        0        0      158 2023-03-31 02:08:50.018000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/readme.md
+-rw-r--r--   0        0        0       84 2023-03-23 14:04:01.935000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/requirements.txt
+-rw-r--r--   0        0        0     2947 2023-03-23 14:04:01.935000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-06-16 06:41:03.321672 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/Dockerfile
+-rw-r--r--   0        0        0       35 2023-06-16 06:43:57.737553 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/requirements.txt
+-rw-r--r--   0        0        0     4977 2023-07-07 03:56:36.825063 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-06-29 08:23:27.283839 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/Dockerfile
+-rw-r--r--   0        0        0       29 2023-06-29 08:23:27.283891 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/requirements.txt
+-rw-r--r--   0        0        0     4532 2023-07-24 02:56:17.638076 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-07-24 02:56:17.638302 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/Dockerfile
+-rw-r--r--   0        0        0       29 2023-07-24 02:56:17.638370 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/requirements.txt
+-rw-r--r--   0        0        0     4535 2023-07-24 02:56:17.638444 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-07-24 02:56:17.638530 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/Dockerfile
+-rw-r--r--   0        0        0       29 2023-07-24 02:56:17.638575 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/requirements.txt
+-rw-r--r--   0        0        0     4477 2023-07-24 02:56:17.638640 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/wrapper/wrapper.py
+-rw-r--r--   0        0        0        0 2023-06-16 06:41:03.321927 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm/Dockerfile
+-rw-r--r--   0        0        0       68 2023-07-07 07:54:55.874885 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm/requirements.txt
+-rw-r--r--   0        0        0     4268 2023-07-07 03:56:36.837829 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-07-07 02:48:41.671637 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/Dockerfile
+-rw-r--r--   0        0        0       29 2023-07-07 02:48:41.671851 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/requirements.txt
+-rw-r--r--   0        0        0     4144 2023-07-07 03:56:36.834638 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-06-20 06:18:50.440549 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/Dockerfile
+-rw-r--r--   0        0        0       29 2023-06-20 06:18:50.440773 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/requirements.txt
+-rw-r--r--   0        0        0     5593 2023-07-07 03:56:47.748355 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-07-24 02:56:17.638728 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/Dockerfile
+-rw-r--r--   0        0        0       29 2023-07-24 02:56:17.638772 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/requirements.txt
+-rw-r--r--   0        0        0     4530 2023-07-24 02:56:17.638843 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-06-29 08:23:27.284109 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/Dockerfile
+-rw-r--r--   0        0        0       35 2023-06-29 08:23:27.284234 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/requirements.txt
+-rw-r--r--   0        0        0     5534 2023-07-07 03:57:08.083845 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-06-16 06:41:03.322232 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/Dockerfile
+-rw-r--r--   0        0        0       35 2023-06-16 06:44:11.271284 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/requirements.txt
+-rw-r--r--   0        0        0     5544 2023-07-07 03:57:20.980440 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/wrapper/wrapper.py
+-rw-r--r--   0        0        0     2823 2023-03-21 05:26:30.958000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/README.md
+-rw-r--r--   0        0        0     1151 2023-06-06 06:46:33.750578 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/__init__.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.708000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/Dockerfile
+-rw-r--r--   0        0        0       63 2023-03-19 14:49:24.708000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/requirements.txt
+-rw-r--r--   0        0        0   383447 2023-03-19 14:49:24.709000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/mlk.flac
+-rw-r--r--   0        0        0     2360 2023-03-21 05:26:30.958000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-02 05:19:51.931000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/Dockerfile
+-rw-r--r--   0        0        0       63 2023-03-02 05:19:51.931000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/requirements.txt
+-rw-r--r--   0        0        0   383447 2023-03-02 05:19:51.932000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/mlk.flac
+-rw-r--r--   0        0        0     2619 2023-03-19 14:49:24.710000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.710000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.710000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.710000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/cat.jpg
+-rw-r--r--   0        0        0    10942 2023-03-19 14:49:24.711000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/result_depth.jpeg
+-rw-r--r--   0        0        0     2899 2023-03-19 14:49:24.711000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.711000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/Dockerfile
+-rw-r--r--   0        0        0       64 2023-03-19 14:49:24.711000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/requirements.txt
+-rw-r--r--   0        0        0   434332 2023-03-19 14:49:24.712000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/img.png
+-rw-r--r--   0        0        0     2539 2023-03-19 14:49:24.712000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.713000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/Dockerfile
+-rw-r--r--   0        0        0       98 2023-03-19 14:49:24.713000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.713000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/cat.jpg
+-rw-r--r--   0        0        0     9565 2023-03-19 14:49:24.713000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_1.jpg
+-rw-r--r--   0        0        0     5000 2023-03-19 14:49:24.713000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_2.jpg
+-rw-r--r--   0        0        0     4937 2023-03-19 14:49:24.713000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_3.jpg
+-rw-r--r--   0        0        0    20405 2023-03-19 14:49:24.713000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_4.jpg
+-rw-r--r--   0        0        0    10041 2023-03-19 14:49:24.713000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_5.jpg
+-rw-r--r--   0        0        0    63187 2023-03-19 14:49:24.714000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/test_str_to_img.jpg
+-rw-r--r--   0        0        0     3164 2023-03-19 14:49:24.714000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.714000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.714000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.714000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/cat.jpg
+-rw-r--r--   0        0        0     2433 2023-03-19 14:49:24.714000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.714000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/Dockerfile
+-rw-r--r--   0        0        0       64 2023-03-21 05:26:30.959000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/requirements.txt
+-rw-r--r--   0        0        0     2897 2023-03-21 05:26:30.959000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.718000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/Dockerfile
+-rw-r--r--   0        0        0       63 2023-03-19 14:49:24.718000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/requirements.txt
+-rw-r--r--   0        0        0   434332 2023-03-19 14:49:24.718000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/img.png
+-rw-r--r--   0        0        0     2754 2023-03-19 14:49:24.718000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.718000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/Dockerfile
+-rw-r--r--   0        0        0       64 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/cat.jpg
+-rw-r--r--   0        0        0     2914 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-21 05:26:30.959000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/Dockerfile
+-rw-r--r--   0        0        0       75 2023-03-21 05:26:30.960000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/requirements.txt
+-rw-r--r--   0        0        0    76876 2023-03-21 05:26:30.960000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/doc.png
+-rw-r--r--   0        0        0     2747 2023-03-21 05:26:30.960000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-21 05:26:30.960000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/Dockerfile
+-rw-r--r--   0        0        0       63 2023-03-21 05:26:30.961000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/requirements.txt
+-rw-r--r--   0        0        0     2404 2023-03-21 05:26:30.961000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-21 05:26:30.961000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/Dockerfile
+-rw-r--r--   0        0        0       75 2023-03-21 05:26:30.961000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-21 05:26:30.962000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/cat.jpg
+-rw-r--r--   0        0        0     2454 2023-03-21 05:26:30.962000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-21 05:26:30.962000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/Dockerfile
+-rw-r--r--   0        0        0       75 2023-03-21 05:26:30.962000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/requirements.txt
+-rw-r--r--   0        0        0   173131 2023-03-21 05:26:30.963000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/cat.jpg
+-rw-r--r--   0        0        0     2780 2023-03-21 05:26:30.963000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/requirements.txt
+-rw-r--r--   0        0        0     2486 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/requirements.txt
+-rw-r--r--   0        0        0     2386 2023-03-19 14:49:24.719000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/requirements.txt
+-rw-r--r--   0        0        0     2641 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-02 05:19:51.937000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/Dockerfile
+-rw-r--r--   0        0        0      435 2023-03-02 05:19:51.937000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/README.md
+-rw-r--r--   0        0        0       63 2023-03-02 05:19:51.938000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/requirements.txt
+-rw-r--r--   0        0        0     2475 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/requirements.txt
+-rw-r--r--   0        0        0     3602 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/Dockerfile
+-rw-r--r--   0        0        0       92 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/requirements.txt
+-rw-r--r--   0        0        0     2832 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.720000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/requirements.txt
+-rw-r--r--   0        0        0     2410 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-02 05:19:51.938000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/Dockerfile
+-rw-r--r--   0        0        0        4 2023-06-06 06:46:33.750677 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/packages.txt
+-rw-r--r--   0        0        0       64 2023-03-02 05:19:51.938000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/requirements.txt
+-rw-r--r--   0        0        0     2865 2023-06-13 08:27:55.299240 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/requirements.txt
+-rw-r--r--   0        0        0     2678 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/requirements.txt
+-rw-r--r--   0        0        0     2523 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/requirements.txt
+-rw-r--r--   0        0        0     2392 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/wrapper/wrapper.py
+-rw-r--r--   0        0        0      637 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/Dockerfile
+-rw-r--r--   0        0        0       85 2023-03-19 14:49:24.721000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/requirements.txt
+-rw-r--r--   0        0        0     2711 2023-03-19 14:49:24.722000 pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/wrapper/wrapper.py
+-rw-r--r--   0        0        0        6 2023-03-06 07:33:04.130000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/requirements.txt
+-rw-r--r--   0        0        0     3701 2023-03-06 08:14:31.141000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.dockerignore
+-rw-r--r--   0        0        0       75 2023-03-06 08:14:31.141000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.gitattributes
+-rw-r--r--   0        0        0     2938 2023-03-06 08:14:31.141000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      280 2023-03-06 08:14:31.141000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1803 2023-03-06 08:14:31.141000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1149 2023-03-06 08:14:31.141000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0        0        0      693 2023-03-06 08:14:31.141000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      441 2023-03-06 08:14:31.141000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/dependabot.yml
+-rw-r--r--   0        0        0     6789 2023-03-23 14:04:01.875000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/ci-testing.yml
+-rw-r--r--   0        0        0     2051 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1572 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     5434 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/greetings.yml
+-rw-r--r--   0        0        0     2014 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/stale.yml
+-rw-r--r--   0        0        0      707 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/translate-readme.yml
+-rwxr-xr-x   0        0        0     3998 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.gitignore
+-rw-r--r--   0        0        0     1747 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      392 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/CITATION.cff
+-rw-r--r--   0        0        0     4999 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/CONTRIBUTING.md
+-rw-r--r--   0        0        0    35127 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/LICENSE
+-rw-r--r--   0        0        0    40553 2023-03-06 08:14:31.142000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.md
+-rw-r--r--   0        0        0    39592 2023-03-06 08:14:31.143000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.zh-CN.md
+-rw-r--r--   0        0        0     7830 2023-03-06 08:14:31.143000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/benchmarks.py
+-rw-r--r--   0        0        0    11730 2023-03-06 08:14:31.143000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/predict.py
+-rw-r--r--   0        0        0    16383 2023-05-26 01:51:19.920034 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/train.py
+-rw-r--r--   0        0        0   103520 2023-03-06 08:14:31.143000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/tutorial.ipynb
+-rw-r--r--   0        0        0     8056 2023-03-06 08:14:31.143000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/val.py
+-rw-r--r--   0        0        0     2733 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Argoverse.yaml
+-rw-r--r--   0        0        0     1885 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/GlobalWheat2020.yaml
+-rw-r--r--   0        0        0    18871 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/ImageNet.yaml
+-rw-r--r--   0        0        0     9205 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Objects365.yaml
+-rw-r--r--   0        0        0     2341 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/SKU-110K.yaml
+-rw-r--r--   0        0        0     3493 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VOC.yaml
+-rw-r--r--   0        0        0     2971 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VisDrone.yaml
+-rw-r--r--   0        0        0     2495 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco.yaml
+-rw-r--r--   0        0        0     1868 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128-seg.yaml
+-rw-r--r--   0        0        0     1852 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128.yaml
+-rw-r--r--   0        0        0      673 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.Objects365.yaml
+-rw-r--r--   0        0        0     1156 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.VOC.yaml
+-rw-r--r--   0        0        0     1684 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.no-augmentation.yaml
+-rw-r--r--   0        0        0     1683 2023-03-06 08:14:31.144000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-high.yaml
+-rw-r--r--   0        0        0     1691 2023-03-06 08:14:31.145000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-low.yaml
+-rw-r--r--   0        0        0     1685 2023-03-06 08:14:31.145000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-med.yaml
+-rw-r--r--   0        0        0   487438 2023-03-06 08:14:31.145000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/bus.jpg
+-rw-r--r--   0        0        0   168949 2023-03-06 08:14:31.146000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/zidane.jpg
+-rwxr-xr-x   0        0        0      640 2023-03-06 08:14:31.146000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/download_weights.sh
+-rwxr-xr-x   0        0        0     1566 2023-03-06 08:14:31.146000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco.sh
+-rwxr-xr-x   0        0        0      618 2023-03-06 08:14:31.146000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco128.sh
+-rwxr-xr-x   0        0        0     1671 2023-03-06 08:14:31.146000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_imagenet.sh
+-rw-r--r--   0        0        0     5170 2023-03-06 08:14:31.146000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/xView.yaml
+-rw-r--r--   0        0        0    14292 2023-03-06 08:14:31.146000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/detect.py
+-rw-r--r--   0        0        0    32063 2023-05-26 01:51:19.911068 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/export.py
+-rw-r--r--   0        0        0     7767 2023-05-26 01:51:19.923788 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/hubconf.py
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/__init__.py
+-rw-r--r--   0        0        0    41702 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/common.py
+-rw-r--r--   0        0        0     4319 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/experimental.py
+-rw-r--r--   0        0        0     3335 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/anchors.yaml
+-rw-r--r--   0        0        0     1567 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-spp.yaml
+-rw-r--r--   0        0        0     1232 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-tiny.yaml
+-rw-r--r--   0        0        0     1558 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3.yaml
+-rw-r--r--   0        0        0     1423 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-bifpn.yaml
+-rw-r--r--   0        0        0     1214 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-fpn.yaml
+-rw-r--r--   0        0        0     1687 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p2.yaml
+-rw-r--r--   0        0        0     1349 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p34.yaml
+-rw-r--r--   0        0        0     1741 2023-03-06 08:14:31.147000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p6.yaml
+-rw-r--r--   0        0        0     2122 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p7.yaml
+-rw-r--r--   0        0        0     1407 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-panet.yaml
+-rw-r--r--   0        0        0     1820 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5l6.yaml
+-rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5m6.yaml
+-rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5n6.yaml
+-rw-r--r--   0        0        0     1497 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-LeakyReLU.yaml
+-rw-r--r--   0        0        0     1483 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-ghost.yaml
+-rw-r--r--   0        0        0     1441 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-transformer.yaml
+-rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s6.yaml
+-rw-r--r--   0        0        0     1822 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5x6.yaml
+-rw-r--r--   0        0        0     1411 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5l-seg.yaml
+-rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5m-seg.yaml
+-rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5n-seg.yaml
+-rw-r--r--   0        0        0     1412 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5s-seg.yaml
+-rw-r--r--   0        0        0     1413 2023-03-06 08:14:31.148000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5x-seg.yaml
+-rw-r--r--   0        0        0    27032 2023-05-26 01:51:19.958775 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/tf.py
+-rw-r--r--   0        0        0    17780 2023-05-26 01:51:19.931156 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolo.py
+-rw-r--r--   0        0        0     1401 2023-03-06 08:14:31.149000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5l.yaml
+-rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5m.yaml
+-rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5n.yaml
+-rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5s.yaml
+-rw-r--r--   0        0        0     1403 2023-03-06 08:14:31.149000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5x.yaml
+-rw-r--r--   0        0        0     1593 2023-03-06 08:14:31.149000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/requirements.txt
+-rw-r--r--   0        0        0    15743 2023-03-06 08:14:31.149000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/predict.py
+-rw-r--r--   0        0        0    34678 2023-03-23 14:04:01.875000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/train.py
+-rw-r--r--   0        0        0    43293 2023-03-06 08:14:31.150000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/tutorial.ipynb
+-rw-r--r--   0        0        0    24005 2023-03-06 08:14:31.150000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/val.py
+-rw-r--r--   0        0        0     1727 2023-03-06 08:14:31.150000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/setup.cfg
+-rw-r--r--   0        0        0    33701 2023-03-06 08:14:31.150000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/train.py
+-rw-r--r--   0        0        0    54258 2023-03-06 08:14:31.150000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/tutorial.ipynb
+-rw-r--r--   0        0        0     2432 2023-03-06 08:14:31.150000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/__init__.py
+-rw-r--r--   0        0        0     3449 2023-03-06 08:14:31.151000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/activations.py
+-rw-r--r--   0        0        0    17030 2023-03-06 08:14:31.151000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/augmentations.py
+-rw-r--r--   0        0        0     7420 2023-03-06 08:14:31.151000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autoanchor.py
+-rw-r--r--   0        0        0     3003 2023-05-26 01:51:19.914199 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autobatch.py
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.151000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/__init__.py
+-rw-r--r--   0        0        0      780 2023-03-06 08:14:31.151000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/mime.sh
+-rw-r--r--   0        0        0     1198 2023-03-06 08:14:31.151000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/resume.py
+-rw-r--r--   0        0        0     1247 2023-03-06 08:14:31.151000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/userdata.sh
+-rw-r--r--   0        0        0     2661 2023-03-06 08:14:31.151000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/callbacks.py
+-rw-r--r--   0        0        0    55779 2023-05-26 01:51:19.947412 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/dataloaders.py
+-rw-r--r--   0        0        0     2709 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile
+-rw-r--r--   0        0        0     1682 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-arm64
+-rw-r--r--   0        0        0     1707 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-cpu
+-rw-r--r--   0        0        0     4952 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/downloads.py
+-rw-r--r--   0        0        0     1710 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/README.md
+-rw-r--r--   0        0        0      368 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/example_request.py
+-rw-r--r--   0        0        0     1439 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/restapi.py
+-rw-r--r--   0        0        0    46844 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/general.py
+-rw-r--r--   0        0        0      821 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/Dockerfile
+-rw-r--r--   0        0        0      187 2023-03-06 08:14:31.152000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/additional_requirements.txt
+-rw-r--r--   0        0        0      174 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/app.yaml
+-rw-r--r--   0        0        0    16635 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/__init__.py
+-rw-r--r--   0        0        0    10862 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/README.md
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/__init__.py
+-rw-r--r--   0        0        0     8034 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/clearml_utils.py
+-rw-r--r--   0        0        0     5271 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/hpo.py
+-rw-r--r--   0        0        0    10772 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/README.md
+-rw-r--r--   0        0        0    18731 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/__init__.py
+-rw-r--r--   0        0        0     4751 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/comet_utils.py
+-rw-r--r--   0        0        0     6653 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/hpo.py
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.153000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/wandb/__init__.py
+-rw-r--r--   0        0        0     8252 2023-03-06 08:14:31.154000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/wandb/wandb_utils.py
+-rw-r--r--   0        0        0     9919 2023-03-06 08:14:31.154000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loss.py
+-rw-r--r--   0        0        0    14568 2023-03-06 08:14:31.154000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/metrics.py
+-rw-r--r--   0        0        0    24501 2023-05-26 01:51:19.940339 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/plots.py
+-rw-r--r--   0        0        0        0 2023-03-06 08:14:31.154000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/__init__.py
+-rw-r--r--   0        0        0     3756 2023-03-06 08:14:31.154000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/augmentations.py
+-rw-r--r--   0        0        0    13835 2023-03-06 08:14:31.154000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/dataloaders.py
+-rw-r--r--   0        0        0     5813 2023-03-23 14:04:01.876000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/general.py
+-rw-r--r--   0        0        0     8591 2023-03-23 14:04:01.876000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/loss.py
+-rw-r--r--   0        0        0     5457 2023-03-06 08:14:31.154000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/metrics.py
+-rw-r--r--   0        0        0     6386 2023-03-23 14:04:01.876000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/plots.py
+-rw-r--r--   0        0        0    19655 2023-05-26 01:51:19.900763 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/torch_utils.py
+-rw-r--r--   0        0        0     3634 2023-03-06 08:14:31.155000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/triton.py
+-rw-r--r--   0        0        0    20424 2023-03-06 08:14:31.155000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/val.py
+-rw-r--r--   0        0        0     4932 2023-03-06 08:24:07.583000 pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/wrapper.py
+-rw-r--r--   0        0        0     2460 2023-07-26 06:13:00.898000 pyatp-1.2.1/src/ailab/log.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:25:57.748000 pyatp-1.2.1/src/ailab/log_cycle/__init__.py
+-rw-r--r--   0        0        0      531 2023-05-03 13:25:57.748000 pyatp-1.2.1/src/ailab/log_cycle/json_handler.py
+-rw-r--r--   0        0        0     2007 2023-05-26 01:43:21.934000 pyatp-1.2.1/src/ailab/templates/README.md
+-rw-r--r--   0        0        0      542 2023-05-26 01:43:21.934000 pyatp-1.2.1/src/ailab/templates/alpaca.json
+-rw-r--r--   0        0        0      561 2023-05-26 01:43:21.934000 pyatp-1.2.1/src/ailab/templates/alpaca_legacy.json
+-rw-r--r--   0        0        0      281 2023-05-26 01:43:21.934000 pyatp-1.2.1/src/ailab/templates/alpaca_short.json
+-rw-r--r--   0        0        0      605 2023-05-26 01:43:21.934000 pyatp-1.2.1/src/ailab/templates/vigogne.json
+-rw-r--r--   0        0        0      239 2023-05-29 01:38:01.672199 pyatp-1.2.1/src/ailab/utils/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 01:38:01.672232 pyatp-1.2.1/src/ailab/utils/__init__.py
+-rw-r--r--   0        0        0     2384 2023-06-01 08:42:34.256596 pyatp-1.2.1/src/ailab/utils/callbacks.py
+-rw-r--r--   0        0        0     3567 2023-07-07 02:48:41.672107 pyatp-1.2.1/src/ailab/utils/other.py
+-rw-r--r--   0        0        0     1837 2023-06-16 06:41:03.322556 pyatp-1.2.1/src/ailab/utils/prompter.py
+-rw-r--r--   0        0        0    35352 2023-06-30 08:10:49.357368 pyatp-1.2.1/src/ailab/utils/streampeft.py
+-rw-r--r--   0        0        0     7901 2023-08-08 11:02:41.070938 pyatp-1.2.1/src/ailab/utils/template.py
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 pyatp-1.2.1/PKG-INFO
```

### Comparing `pyatp-1.2.0/LICENSE` & `pyatp-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/pyproject.toml` & `pyatp-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyatp"
-version = "1.2.0"
+version = "1.2.1"
 description = "a iflytek ailab library ..."
 authors = ["mjchen <mjchen@iflytek.com>","ybyang <ybyang7@iflytek.com>", "kqxu <kqxu@iflytek.com>"]
 license = "Apache License 2"
 packages = [
     { include = "ailab", from = "src" }
 ]
```

### Comparing `pyatp-1.2.0/src/ailab/__init__.py` & `pyatp-1.2.1/src/ailab/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_dataset/ailab_api.py` & `pyatp-1.2.1/src/ailab/atp_dataset/ailab_api.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_dataset/dataset.py` & `pyatp-1.2.1/src/ailab/atp_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_dataset/huggingface_api.py` & `pyatp-1.2.1/src/ailab/atp_dataset/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/base.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/base.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/ceval.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/ceval.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/harness.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/harness.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/benchmarks/mmlu.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/benchmarks/mmlu.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/build.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/build.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/constant.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/constant.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/evaluator.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/models/base.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/models/base.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/models/chatglm.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/models/chatglm.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_evaluation/models/llama.py` & `pyatp-1.2.1/src/ailab/atp_evaluation/models/llama.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/accelerator/accelerator.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/accelerator/accelerator.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/build.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/build.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/constant.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/constant.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/datacollator.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/datacollator.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_alpaca.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_alpaca.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_baichuan.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_baichuan.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_chatglm.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_chatglm.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_chinese_alpaca.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_chinese_alpaca.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_language.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_language.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_for_token.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_for_token.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/datacollator/dc_with_padding.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/datacollator/dc_with_padding.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/finetuner.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/finetuner.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/metric/accury.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/metric/accury.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/model.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/model.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/multimodel/model_for_sd_lora.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/multimodel/model_for_sd_lora.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/multimodel/vilt_for_vqa.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/multimodel/vilt_for_vqa.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_baichuan.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_baichuan.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_chatglm.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_chatglm.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_chinese_alpaca.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_chinese_alpaca.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_lora.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_lora.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_question_answer.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_question_answer.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_text_classification.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_text_classification.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/model/nlp/model_for_token_classification.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/model/nlp/model_for_token_classification.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_sd_lora.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_sd_lora.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_vilt_vqa.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/multimodel/pc_for_vilt_vqa.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_alpaca.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_alpaca.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_baichuan.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_baichuan.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chatglm.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chatglm.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chinese_alpaca.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_chinese_alpaca.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/pc_for_llama_cn.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/pc_for_llama_cn.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/question_answer_pc.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/question_answer_pc.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/nlp/text_classification_pc.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/nlp/text_classification_pc.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/preprossor/preprossor.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/preprossor/preprossor.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_sd_lora.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_sd_lora.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_vilt_vqa.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/multimodel/trainer_for_vilt_vqa.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/ds_zero2_no_offload.json` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/ds_zero2_no_offload.json`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_alpaca.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_alpaca.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_baichuan.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_baichuan.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chatglm.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chatglm.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chinese_alpaca.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_chinese_alpaca.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_llama_cn.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_llama_cn.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/trainer_for_text_classification.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/trainer_for_text_classification.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/nlp/traniner_for_question_answer.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/nlp/traniner_for_question_answer.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/atp_finetuner/trainer/trainer.py` & `pyatp-1.2.1/src/ailab/atp_finetuner/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/batch/__init__.py` & `pyatp-1.2.1/src/ailab/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/batch/entrypoint.py` & `pyatp-1.2.1/src/ailab/batch/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/make.py` & `pyatp-1.2.1/src/ailab/buildkit/make.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/pyproject.toml` & `pyatp-1.2.1/src/ailab/buildkit/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/__init__.py` & `pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/build.py` & `pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/build.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/config.py` & `pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/config.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/dotdict.py` & `pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/error.py` & `pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/error.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/get-pip.py` & `pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/get-pip.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/buildkit/src/pyatp_buildkit/templates/Dockerfile.j2` & `pyatp-1.2.1/src/ailab/buildkit/src/pyatp_buildkit/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/__init__.py` & `pyatp-1.2.1/src/ailab/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/baichuan/__init__.py` & `pyatp-1.2.1/src/ailab/examples/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/baichuan/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/baichuan/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/baichuan_13b/__init__.py` & `pyatp-1.2.1/src/ailab/examples/baichuan_13b/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/baichuan_13b/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/baichuan_13b/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/bloomz/__init__.py` & `pyatp-1.2.1/src/ailab/examples/bloomz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/bloomz/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/bloomz/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chatglm2_6b/__init__.py` & `pyatp-1.2.1/src/ailab/examples/chatglm2_6b/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chatglm2_6b/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/chatglm2_6b/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chatglm_6b/__init__.py` & `pyatp-1.2.1/src/ailab/examples/chatglm_6b/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chatglm_6b/evaluator.py` & `pyatp-1.2.1/src/ailab/examples/chatglm_6b/evaluator.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chatglm_6b/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/chatglm_6b/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/__init__.py` & `pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/evaluator.py` & `pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/evaluator.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chinese_llama_alpaca/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/chinese_llama_alpaca/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/__init__.py` & `pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/evaluator.py` & `pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/evaluator.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/chinese_llama_vicuna/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/chinese_llama_vicuna/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/falcon/__init__.py` & `pyatp-1.2.1/src/ailab/examples/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/falcon/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/falcon/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/harness/evaluator.py` & `pyatp-1.2.1/src/ailab/examples/harness/evaluator.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/llama2/__init__.py` & `pyatp-1.2.1/src/ailab/examples/llama2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/llama2/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/llama2/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/moss/__init__.py` & `pyatp-1.2.1/src/ailab/examples/moss/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/moss/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/moss/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/open_llama/__init__.py` & `pyatp-1.2.1/src/ailab/examples/open_llama/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/open_llama/train.py` & `pyatp-1.2.1/src/ailab/examples/open_llama/train.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/standford_alpaca/__init__.py` & `pyatp-1.2.1/src/ailab/examples/standford_alpaca/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/standford_alpaca/evaluator.py` & `pyatp-1.2.1/src/ailab/examples/standford_alpaca/evaluator.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/standford_alpaca/train_imp.py` & `pyatp-1.2.1/src/ailab/examples/standford_alpaca/train_imp.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/text_classification/__init__.py` & `pyatp-1.2.1/src/ailab/examples/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/examples/text_classification/train.py` & `pyatp-1.2.1/src/ailab/examples/text_classification/train.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/__init__.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/test_data/test.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/chatgpt/chat_gpt_api_official/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/sketch-mountains-input.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/sketch-mountains-input.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/alt_diffusion/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/audio_diffusion/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/horse.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/horse.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/cycle_diffusion/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/dance_diffusion/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/latency_diffusion/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/attend_and_excite/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/000000039769.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/000000039769.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/depth_to_image/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/sketch-mountains-input.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/sketch-mountains-input.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/image_to_image/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo_mask.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/overture-creations-5sI6fQgYIuo_mask.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/inpainting/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/mountain.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/mountain.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/instruct_pix2pix/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/multi_diffusion/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/self_attention_guidance/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/low_res_cat.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/low_res_cat.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/super-resolution/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/diffusers/stable_diffusion/text_to_image/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/alpaca/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/baichuan_13b/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/bloomz/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chatglm2/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/chinese_alpaca/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/falcon/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/open_llama/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/lora/nlp/vicuna/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/README.md` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/README.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/__init__.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/mlk.flac` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/mlk.flac`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/audio_classification/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/mlk.flac` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/mlk.flac`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/audio/automatic-speech-recognition/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/cat.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/cat.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/result_depth.jpeg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/result_depth.jpeg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/depth_estimation/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/img.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/img.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_classification/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/cat.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/cat.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_1.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_1.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_2.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_2.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_3.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_3.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_4.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_4.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_5.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/result_mask_5.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/test_str_to_img.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/test_str_to_img.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/image_segmentation/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/cat.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/cat.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/object_detection/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/video_classification/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/img.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/img.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_image_classification/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/cat.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/cat.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/cv/zero_shot_object_detection/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/doc.png` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/doc.png`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/document_question_answering/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/feature_extraction/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/cat.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/cat.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/image_to_text/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/cat.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/cat.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/multimodal/visual_question_answering/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/conversational/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/fill_mask/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/question_answering/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/sentiment-analysis/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/summarization/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/table_question_answering/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text2text_generation/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_classification/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/text_generation/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/token_classification/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/translation/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/wrapper/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/huggingface/transformers/nlp/zero_shot_classification/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.dockerignore` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.dockerignore`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/bug-report.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/feature-request.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/question.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/ISSUE_TEMPLATE/question.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/PULL_REQUEST_TEMPLATE.md` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/ci-testing.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/codeql-analysis.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/docker.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/greetings.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/greetings.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/stale.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/translate-readme.yml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.github/workflows/translate-readme.yml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.gitignore` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.pre-commit-config.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/CONTRIBUTING.md` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/LICENSE` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.md` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.zh-CN.md` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/benchmarks.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/predict.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/predict.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/train.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/train.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/tutorial.ipynb` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/val.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/classify/val.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Argoverse.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/GlobalWheat2020.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/ImageNet.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Objects365.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/SKU-110K.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VOC.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VOC.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VisDrone.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128-seg.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/coco128.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.Objects365.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.Objects365.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.VOC.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.VOC.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.no-augmentation.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.no-augmentation.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-high.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-high.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-low.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-low.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-med.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/hyps/hyp.scratch-med.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/bus.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/bus.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/zidane.jpg` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/images/zidane.jpg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/download_weights.sh` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/download_weights.sh`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco.sh` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco.sh`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco128.sh` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_coco128.sh`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_imagenet.sh` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/scripts/get_imagenet.sh`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/xView.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/data/xView.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/detect.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/detect.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/export.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/export.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/hubconf.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/hubconf.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/common.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/common.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/experimental.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/experimental.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/anchors.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/anchors.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-spp.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-tiny.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-bifpn.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-bifpn.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-fpn.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-fpn.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p2.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p2.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p34.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p34.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p6.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p7.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-p7.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-panet.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5-panet.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5l6.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5l6.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5m6.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5m6.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5n6.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5n6.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-LeakyReLU.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-LeakyReLU.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-ghost.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-ghost.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-transformer.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s-transformer.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s6.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5s6.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5x6.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/hub/yolov5x6.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5l-seg.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5l-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5m-seg.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5m-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5n-seg.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5n-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5s-seg.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5s-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5x-seg.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/segment/yolov5x-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/tf.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/tf.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolo.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolo.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5l.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5m.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5n.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5s.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5x.yaml` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/models/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/requirements.txt` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/predict.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/predict.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/train.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/train.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/tutorial.ipynb` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/val.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/segment/val.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/setup.cfg` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/train.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/train.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/tutorial.ipynb` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/__init__.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/activations.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/activations.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/augmentations.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autoanchor.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autobatch.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/mime.sh` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/mime.sh`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/resume.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/resume.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/userdata.sh` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/aws/userdata.sh`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/callbacks.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/dataloaders.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-arm64` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-arm64`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-cpu` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/docker/Dockerfile-cpu`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/downloads.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/README.md` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/README.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/restapi.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/flask_rest_api/restapi.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/general.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/general.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/Dockerfile` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/google_app_engine/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/__init__.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/README.md` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/README.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/clearml_utils.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/clearml_utils.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/hpo.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/clearml/hpo.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/README.md` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/README.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/__init__.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/comet_utils.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/comet_utils.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/hpo.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/comet/hpo.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/wandb/wandb_utils.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loggers/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loss.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/metrics.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/plots.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/augmentations.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/augmentations.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/dataloaders.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/dataloaders.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/general.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/general.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/loss.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/loss.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/metrics.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/metrics.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/plots.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/segment/plots.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/torch_utils.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/triton.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/utils/triton.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/val.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/val.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/inference_wrapper/yolo/wrapper/yolov5/wrapper.py` & `pyatp-1.2.1/src/ailab/inference_wrapper/yolo/wrapper/yolov5/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/log.py` & `pyatp-1.2.1/src/ailab/log.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/log_cycle/json_handler.py` & `pyatp-1.2.1/src/ailab/log_cycle/json_handler.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/templates/README.md` & `pyatp-1.2.1/src/ailab/templates/README.md`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/templates/alpaca.json` & `pyatp-1.2.1/src/ailab/templates/alpaca.json`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/templates/alpaca_legacy.json` & `pyatp-1.2.1/src/ailab/templates/alpaca_legacy.json`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/templates/vigogne.json` & `pyatp-1.2.1/src/ailab/templates/vigogne.json`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/utils/callbacks.py` & `pyatp-1.2.1/src/ailab/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/utils/other.py` & `pyatp-1.2.1/src/ailab/utils/other.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/utils/prompter.py` & `pyatp-1.2.1/src/ailab/utils/prompter.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/utils/streampeft.py` & `pyatp-1.2.1/src/ailab/utils/streampeft.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/src/ailab/utils/template.py` & `pyatp-1.2.1/src/ailab/utils/template.py`

 * *Files identical despite different names*

### Comparing `pyatp-1.2.0/PKG-INFO` & `pyatp-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatp
-Version: 1.2.0
+Version: 1.2.1
 Summary: a iflytek ailab library ...
 License: Apache License 2
 Author: mjchen
 Author-email: mjchen@iflytek.com
 Requires-Python: >3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

