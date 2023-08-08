# Comparing `tmp/modular_rl-0.4.1.tar.gz` & `tmp/modular_rl-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.4.1.tar", last modified: Sat Jun 24 07:36:39 2023, max compression
+gzip compressed data, was "modular_rl-0.4.2.tar", last modified: Tue Aug  8 22:50:09 2023, max compression
```

## Comparing `modular_rl-0.4.1.tar` & `modular_rl-0.4.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.064935 modular_rl-0.4.1/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.4.1/LICENSE
--rw-rw-rw-   0        0        0      781 2023-06-24 07:36:39.063362 modular_rl-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4322 2023-06-10 03:09:21.000000 modular_rl-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:38.921813 modular_rl-0.4.1/modular_rl/
--rw-rw-rw-   0        0        0       36 2023-05-07 02:39:54.000000 modular_rl-0.4.1/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:38.984781 modular_rl-0.4.1/modular_rl/agents/
--rw-rw-rw-   0        0        0      112 2023-06-10 03:09:21.000000 modular_rl-0.4.1/modular_rl/agents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:38.988781 modular_rl-0.4.1/modular_rl/agents/_common/
--rw-rw-rw-   0        0        0       35 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/_common/__init__.py
--rw-rw-rw-   0        0        0     7265 2023-06-24 05:46:15.000000 modular_rl-0.4.1/modular_rl/agents/_common/_agents.py
--rw-rw-rw-   0        0        0     5252 2023-06-24 05:54:50.000000 modular_rl-0.4.1/modular_rl/agents/_custom.py
--rw-rw-rw-   0        0        0     2251 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/mcis.py
--rw-rw-rw-   0        0        0     2251 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/mcts.py
--rw-rw-rw-   0        0        0    23135 2023-06-24 05:35:24.000000 modular_rl-0.4.1/modular_rl/agents/mim.py
--rw-rw-rw-   0        0        0     2819 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.000270 modular_rl-0.4.1/modular_rl/agents/pytorch/
--rw-rw-rw-   0        0        0      106 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/pytorch/__init__.py
--rw-rw-rw-   0        0        0     6913 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/pytorch/_agent.py
--rw-rw-rw-   0        0        0    12241 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/pytorch/mcis.py
--rw-rw-rw-   0        0        0    12545 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/pytorch/mcts.py
--rw-rw-rw-   0        0        0    15558 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/pytorch/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.012791 modular_rl-0.4.1/modular_rl/agents/tensorflow/
--rw-rw-rw-   0        0        0      115 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/agents/tensorflow/__init__.py
--rw-rw-rw-   0        0        0     6053 2023-06-24 05:53:23.000000 modular_rl-0.4.1/modular_rl/agents/tensorflow/_agent.py
--rw-rw-rw-   0        0        0    13196 2023-06-24 05:56:47.000000 modular_rl-0.4.1/modular_rl/agents/tensorflow/mcis.py
--rw-rw-rw-   0        0        0    11894 2023-06-24 05:52:02.000000 modular_rl-0.4.1/modular_rl/agents/tensorflow/mcts.py
--rw-rw-rw-   0        0        0    11937 2023-06-24 05:52:29.000000 modular_rl-0.4.1/modular_rl/agents/tensorflow/ppo.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.017354 modular_rl-0.4.1/modular_rl/envs/
--rw-rw-rw-   0        0        0        0 2023-06-03 00:27:02.000000 modular_rl-0.4.1/modular_rl/envs/__init__.py
--rw-rw-rw-   0        0        0      133 2023-06-03 00:27:02.000000 modular_rl-0.4.1/modular_rl/envs/_custom.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.023352 modular_rl-0.4.1/modular_rl/envs/mim/
--rw-rw-rw-   0        0        0       25 2023-06-03 00:27:02.000000 modular_rl-0.4.1/modular_rl/envs/mim/__init__.py
--rw-rw-rw-   0        0        0    15402 2023-06-03 00:27:02.000000 modular_rl-0.4.1/modular_rl/envs/mim/card_evaluator.py
--rw-rw-rw-   0        0        0     4555 2023-06-24 05:35:24.000000 modular_rl-0.4.1/modular_rl/envs/mim/mim.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.025355 modular_rl-0.4.1/modular_rl/networks/
--rw-rw-rw-   0        0        0        0 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.036355 modular_rl-0.4.1/modular_rl/networks/pytorch/
--rw-rw-rw-   0        0        0      135 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/pytorch/__init__.py
--rw-rw-rw-   0        0        0     2188 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/pytorch/actor_critic.py
--rw-rw-rw-   0        0        0     2888 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/pytorch/policy.py
--rw-rw-rw-   0        0        0     2698 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/pytorch/value.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.047361 modular_rl-0.4.1/modular_rl/networks/tensorflow/
--rw-rw-rw-   0        0        0      114 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/tensorflow/__init__.py
--rw-rw-rw-   0        0        0      849 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/tensorflow/actor_critic.py
--rw-rw-rw-   0        0        0     1119 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/tensorflow/policy.py
--rw-rw-rw-   0        0        0     1022 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/networks/tensorflow/value.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.057361 modular_rl-0.4.1/modular_rl/params/
--rw-rw-rw-   0        0        0       85 2023-06-03 00:27:02.000000 modular_rl-0.4.1/modular_rl/params/__init__.py
--rw-rw-rw-   0        0        0     2198 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/params/mcis.py
--rw-rw-rw-   0        0        0     2412 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/params/mcts.py
--rw-rw-rw-   0        0        0     2975 2023-06-24 05:35:24.000000 modular_rl-0.4.1/modular_rl/params/mim.py
--rw-rw-rw-   0        0        0     2131 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/params/ppo.py
--rw-rw-rw-   0        0        0     1406 2023-06-10 03:09:21.000000 modular_rl-0.4.1/modular_rl/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:39.061363 modular_rl-0.4.1/modular_rl/util/
--rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.4.1/modular_rl/util/__init__.py
--rw-rw-rw-   0        0        0     2626 2023-06-24 05:45:12.000000 modular_rl-0.4.1/modular_rl/util/node.py
-drwxrwxrwx   0        0        0        0 2023-06-24 07:36:38.970910 modular_rl-0.4.1/modular_rl.egg-info/
--rw-rw-rw-   0        0        0      781 2023-06-24 07:36:38.000000 modular_rl-0.4.1/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1555 2023-06-24 07:36:38.000000 modular_rl-0.4.1/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 07:36:38.000000 modular_rl-0.4.1/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-06-24 07:36:38.000000 modular_rl-0.4.1/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 07:36:38.000000 modular_rl-0.4.1/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1503 2023-06-24 07:34:57.000000 modular_rl-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 07:36:39.064935 modular_rl-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-06-24 07:36:15.000000 modular_rl-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.907287 modular_rl-0.4.2/
+-rw-rw-rw-   0        0        0     1520 2023-07-05 06:30:22.000000 modular_rl-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     5728 2023-08-08 22:50:09.906279 modular_rl-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4182 2023-06-08 11:09:02.000000 modular_rl-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.838476 modular_rl-0.4.2/modular_rl/
+-rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.4.2/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.855635 modular_rl-0.4.2/modular_rl/agents/
+-rw-rw-rw-   0        0        0      108 2023-06-06 21:28:14.000000 modular_rl-0.4.2/modular_rl/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.859100 modular_rl-0.4.2/modular_rl/agents/_common/
+-rw-rw-rw-   0        0        0       35 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/_common/__init__.py
+-rw-rw-rw-   0        0        0     6320 2023-07-11 07:59:29.000000 modular_rl-0.4.2/modular_rl/agents/_common/_agents.py
+-rw-rw-rw-   0        0        0     5402 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/_custom.py
+-rw-rw-rw-   0        0        0     2251 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/mcis.py
+-rw-rw-rw-   0        0        0     2251 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/mcts.py
+-rw-rw-rw-   0        0        0    22611 2023-06-14 12:35:48.000000 modular_rl-0.4.2/modular_rl/agents/mim.py
+-rw-rw-rw-   0        0        0     2819 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/ppo.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.865634 modular_rl-0.4.2/modular_rl/agents/pytorch/
+-rw-rw-rw-   0        0        0      106 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     6913 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/pytorch/_agent.py
+-rw-rw-rw-   0        0        0    12241 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/pytorch/mcis.py
+-rw-rw-rw-   0        0        0    12545 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/pytorch/mcts.py
+-rw-rw-rw-   0        0        0    15558 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/pytorch/ppo.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.872629 modular_rl-0.4.2/modular_rl/agents/tensorflow/
+-rw-rw-rw-   0        0        0      115 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0     6102 2023-07-11 08:04:32.000000 modular_rl-0.4.2/modular_rl/agents/tensorflow/_agent.py
+-rw-rw-rw-   0        0        0    13520 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/agents/tensorflow/mcis.py
+-rw-rw-rw-   0        0        0    11968 2023-08-08 21:56:49.000000 modular_rl-0.4.2/modular_rl/agents/tensorflow/mcts.py
+-rw-rw-rw-   0        0        0    12856 2023-08-08 22:40:05.000000 modular_rl-0.4.2/modular_rl/agents/tensorflow/ppo.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.875485 modular_rl-0.4.2/modular_rl/envs/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:09:01.000000 modular_rl-0.4.2/modular_rl/envs/__init__.py
+-rw-rw-rw-   0        0        0      133 2023-06-04 21:09:01.000000 modular_rl-0.4.2/modular_rl/envs/_custom.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.880291 modular_rl-0.4.2/modular_rl/envs/mim/
+-rw-rw-rw-   0        0        0       25 2023-06-04 21:09:01.000000 modular_rl-0.4.2/modular_rl/envs/mim/__init__.py
+-rw-rw-rw-   0        0        0    15402 2023-06-04 21:09:01.000000 modular_rl-0.4.2/modular_rl/envs/mim/card_evaluator.py
+-rw-rw-rw-   0        0        0     4413 2023-06-14 12:37:11.000000 modular_rl-0.4.2/modular_rl/envs/mim/mim.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.881443 modular_rl-0.4.2/modular_rl/networks/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.888950 modular_rl-0.4.2/modular_rl/networks/pytorch/
+-rw-rw-rw-   0        0        0      135 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/pytorch/actor_critic.py
+-rw-rw-rw-   0        0        0     2888 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/pytorch/policy.py
+-rw-rw-rw-   0        0        0     2698 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/pytorch/value.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.894008 modular_rl-0.4.2/modular_rl/networks/tensorflow/
+-rw-rw-rw-   0        0        0      114 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/tensorflow/actor_critic.py
+-rw-rw-rw-   0        0        0     1119 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/tensorflow/policy.py
+-rw-rw-rw-   0        0        0     1022 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/networks/tensorflow/value.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.901999 modular_rl-0.4.2/modular_rl/params/
+-rw-rw-rw-   0        0        0       85 2023-06-04 21:09:01.000000 modular_rl-0.4.2/modular_rl/params/__init__.py
+-rw-rw-rw-   0        0        0     2198 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/params/mcis.py
+-rw-rw-rw-   0        0        0     2412 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/params/mcts.py
+-rw-rw-rw-   0        0        0     2933 2023-06-13 11:17:09.000000 modular_rl-0.4.2/modular_rl/params/mim.py
+-rw-rw-rw-   0        0        0     2131 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/params/ppo.py
+-rw-rw-rw-   0        0        0     1377 2023-06-06 22:36:03.000000 modular_rl-0.4.2/modular_rl/settings.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.904926 modular_rl-0.4.2/modular_rl/util/
+-rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.4.2/modular_rl/util/__init__.py
+-rw-rw-rw-   0        0        0     2626 2023-07-05 06:30:22.000000 modular_rl-0.4.2/modular_rl/util/node.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:50:09.847044 modular_rl-0.4.2/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     5728 2023-08-08 22:50:09.000000 modular_rl-0.4.2/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1555 2023-08-08 22:50:09.000000 modular_rl-0.4.2/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 22:50:09.000000 modular_rl-0.4.2/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-08 22:50:09.000000 modular_rl-0.4.2/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 22:50:09.000000 modular_rl-0.4.2/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1503 2023-08-08 22:48:56.000000 modular_rl-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 22:50:09.907287 modular_rl-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-08-08 22:47:47.000000 modular_rl-0.4.2/setup.py
```

### Comparing `modular_rl-0.4.1/README.md` & `modular_rl-0.4.2/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-# ModularRL
-
-ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
-
-## Installation
-
-```powershell
-pip install modular_rl
-```
-
-## Features
-
--   Implementations of various reinforcement learning algorithms,
-    such as Proximal Policy Optimization (PPO), Monte Carlo Tree Search (MCTS), Monte Carlo Information Set (MCIS), and Modular's sIMulator (MIM)
--   Customizable agent settings and network architectures
--   Modular structure for easy adaptation and extension across different algorithms
--   Model saving and loading functionality for easy reuse of trained models
-
-## Supported Algorithms
-
--   Proximal Policy Optimization (PPO)
--   Monte Carlo Tree Search (MCTS)
--   Monte Carlo Information Set (MCIS)
--   Modular's sIMulator (MIM)
-
-Refer to the respective agent classes for each algorithm:
-
--   AgentPPO (+ Modular)
--   AgentMCTS (+ Modular)
--   AgentMCIS (+ Modular)
--   AgentMIM (+ Modular)
-
-## Example Usage
-
-You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
-
-```python
-import modular_rl.tester as tester
-
-tester.init_ppo()
-# or
-tester.init_ppo_modular()
-
-tester.init_mcts()
-```
-
-As more algorithms are added, the tester functions will follow the naming convention init*[algorithm_name] or init*[algorithm_name]\_modular.
-
-Please note that not all algorithms support modular training due to the nature of their design.
-For such algorithms, you will need to use the non-modular training method provided by the respective agent class.
-You can refer to the list of supported algorithms to determine which training method is appropriate.
-
-Alternatively, you can create and train an instance of the AgentPPO(example) class directly in your code:
-
-```python
-from modular_rl.agents.agent_ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-def init():
-    env = AgentPPO(env=None, setting=AgentSettings.default)
-    env.learn()
-
-init()
-```
-
-To create and train an instance of the AgentPPO(example) class with modified settings, use the following code:
-
-```python
-from modular_rl.agents.agent_ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-def init_modular():
-    # Semi-automatic (defined record usage)
-    # Implement your environment and pass it to 'env' parameter.
-    env = AgentPPO(env=None, setting=AgentSettings.default_modular)
-    env.reset()
-    env.learn_reset()
-    action, reward, is_done = env.learn_next()
-    env.learn_check()
-    env.update()
-
-    # Proceed with the learning manually.
-    env.reset()
-    # Implement the 'reset' method in your environment.
-    '''
-    def reset(self):
-        ...
-        return initial_state
-    '''
-    env.learn_reset()
-    initial_state = env.learn_reset()
-    action, dist = env.select_action(initial_state)
-
-    '''
-    Note:
-    Please implement the resulting state of update_step in the step function of your environment.
-
-    For example:
-
-    def step(self, action):
-        ...
-        return next_state, reward, is_done, _
-    '''
-
-    env.update_step(initial_state, dist, action, -1)
-
-    env.learn_check()
-    env.update()
-
-    env.learn_close()
-
-init_modular()
-```
-
-## Saving and Loading Models
-
-Agents can save and load their models using the save_model(file_name) and load_model(file_name) methods.
-The file_name parameter should be the name of the file to save or load the model to/from.
-
-Example:
-
-```python
-agent = AgentPPO(env, setting)
-agent.train()
-
-agent.save_model("my_saved_model.pth")
-
-loaded_agent = AgentPPO(env, setting)
-loaded_agent.load_model("my_saved_model.pth")
-```
-
-## Key Classes
-
--   AgentPPO, AgentMCTS, AgentMCIS, AgentMIM: The main agent classes implementing various reinforcement learning algorithms.
--   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
--   AgentSettings: A configuration class for setting up the agents.
-
-## License
-
-MIT License
+# ModularRL
+
+ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
+
+## Installation
+
+```powershell
+pip install modular_rl
+```
+
+## Features
+
+-   Implementations of various reinforcement learning algorithms,
+    such as Proximal Policy Optimization (PPO), Monte Carlo Tree Search (MCTS), Monte Carlo Information Set (MCIS), and Modular's sIMulator (MIM)
+-   Customizable agent settings and network architectures
+-   Modular structure for easy adaptation and extension across different algorithms
+-   Model saving and loading functionality for easy reuse of trained models
+
+## Supported Algorithms
+
+-   Proximal Policy Optimization (PPO)
+-   Monte Carlo Tree Search (MCTS)
+-   Monte Carlo Information Set (MCIS)
+-   Modular's sIMulator (MIM)
+
+Refer to the respective agent classes for each algorithm:
+
+-   AgentPPO (+ Modular)
+-   AgentMCTS (+ Modular)
+-   AgentMCIS (+ Modular)
+-   AgentMIM (+ Modular)
+
+## Example Usage
+
+You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
+
+```python
+import modular_rl.tester as tester
+
+tester.init_ppo()
+# or
+tester.init_ppo_modular()
+
+tester.init_mcts()
+```
+
+As more algorithms are added, the tester functions will follow the naming convention init*[algorithm_name] or init*[algorithm_name]\_modular.
+
+Please note that not all algorithms support modular training due to the nature of their design.
+For such algorithms, you will need to use the non-modular training method provided by the respective agent class.
+You can refer to the list of supported algorithms to determine which training method is appropriate.
+
+Alternatively, you can create and train an instance of the AgentPPO(example) class directly in your code:
+
+```python
+from modular_rl.agents.agent_ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+def init():
+    env = AgentPPO(env=None, setting=AgentSettings.default)
+    env.learn()
+
+init()
+```
+
+To create and train an instance of the AgentPPO(example) class with modified settings, use the following code:
+
+```python
+from modular_rl.agents.agent_ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+def init_modular():
+    # Semi-automatic (defined record usage)
+    # Implement your environment and pass it to 'env' parameter.
+    env = AgentPPO(env=None, setting=AgentSettings.default_modular)
+    env.reset()
+    env.learn_reset()
+    action, reward, is_done = env.learn_next()
+    env.learn_check()
+    env.update()
+
+    # Proceed with the learning manually.
+    env.reset()
+    # Implement the 'reset' method in your environment.
+    '''
+    def reset(self):
+        ...
+        return initial_state
+    '''
+    env.learn_reset()
+    initial_state = env.learn_reset()
+    action, dist = env.select_action(initial_state)
+
+    '''
+    Note:
+    Please implement the resulting state of update_step in the step function of your environment.
+
+    For example:
+
+    def step(self, action):
+        ...
+        return next_state, reward, is_done, _
+    '''
+
+    env.update_step(initial_state, dist, action, -1)
+
+    env.learn_check()
+    env.update()
+
+    env.learn_close()
+
+init_modular()
+```
+
+## Saving and Loading Models
+
+Agents can save and load their models using the save_model(file_name) and load_model(file_name) methods.
+The file_name parameter should be the name of the file to save or load the model to/from.
+
+Example:
+
+```python
+agent = AgentPPO(env, setting)
+agent.train()
+
+agent.save_model("my_saved_model.pth")
+
+loaded_agent = AgentPPO(env, setting)
+loaded_agent.load_model("my_saved_model.pth")
+```
+
+## Key Classes
+
+-   AgentPPO, AgentMCTS, AgentMCIS, AgentMIM: The main agent classes implementing various reinforcement learning algorithms.
+-   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
+-   AgentSettings: A configuration class for setting up the agents.
+
+## License
+
+MIT License
```

### Comparing `modular_rl-0.4.1/modular_rl/agents/_common/_agents.py` & `modular_rl-0.4.2/modular_rl/agents/_common/_agents.py`

 * *Files 20% similar despite different names*

```diff
@@ -171,44 +171,14 @@
         """
         Update the episode-related variables to indicate the start of a new episode.
         """
 
         self.episode += 1
         self.episode_reward = 0
 
-    def convert_float_to_double(self, input_tensor):
-        """
-        Convert the input tensor from float32 to double precision if necessary.
-
-        :param input_tensor: The input tensor to be converted.
-        :type input_tensor: torch.Tensor
-        :return: The converted tensor.
-        :rtype: torch.Tensor
-        """
-
-        if input_tensor.dtype == torch.float32:
-            return input_tensor.double()
-        else:
-            return input_tensor
-
-    def ensure_float(self, input_tensor):
-        """
-        Ensure that the input tensor is of float precision by converting it from float64 if necessary.
-
-        :param input_tensor: The input tensor to be converted.
-        :type input_tensor: torch.Tensor
-        :return: The converted tensor.
-        :rtype: torch.Tensor
-        """
-
-        if input_tensor.dtype == torch.float64:
-            return input_tensor.float()
-        else:
-            return input_tensor
-
     def update(self):
         '''
         This function is a placeholder and must be implemented by the child class that extends this Agent class.
 
         update() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function is responsible for updating the agent's state, action, and policy based on the new state and reward received from the environment.
 
         No parameters are passed into this function and it does not return anything.
```

### Comparing `modular_rl-0.4.1/modular_rl/agents/_custom.py` & `modular_rl-0.4.2/modular_rl/agents/_custom.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible-gh
-
-ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms.
-The library is designed to be easily customizable and modular,
-allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
-
-"""
-
-
-from LogAssist.log import Logger
-from modular_rl.envs._custom import CustomEnv
-
-
-class AgentCustom:
-    def __init__(self, env, setting):
-        """
-        :param env: The environment for the agent to interact with. It should be an instance of a compatible environment class. If None is provided, a default CustomEnv environment will be used.
-        :type env: object
-        :param setting: The setting configuration for the agent, specifying various learning parameters and settings.
-        :type setting: dict
-        :return: None
-        """
-
-        self.env = env if env else CustomEnv()
-        self.setting = setting
-
-        # Set learn episode parameters
-        self.episode_reward = 0
-        self.total_reward = 0
-        self.prev_reward = 0
-        self.episode = 0
-        self.avg_reward = 0
-
-        # Set learn parameters (If necessary)
-        self.state = None
-        self.action = None
-        self.reward = None
-        self.done = None
-        self.reset()
-
-        # Training parameters(Common)
-        self.max_episodes = setting.get('max_episodes', 30)
-        self.max_timesteps = setting.get('max_timesteps', 100)
-
-        # Logger initialize
-        self.log_level = setting.get('log_level', 'debug')
-        self.log_init_pass = setting.get('log_init_pass', False)
-        if self.log_init_pass == False:
-            Logger.init(
-                dir_name=None,
-                file_name=None,
-                log_level=self.log_level,
-                out_console=True,
-                out_file=None,
-                prev_log_remove=None
-            )
-
-    def reset(self):
-        """
-        Reset the lists that contain information about the states, actions, rewards, and other values for the agent.
-        """
-
-        self.states = []
-        self.actions = []
-        self.rewards = []
-        self.next_states = []
-        self.dones = []
-        self.log_probs = []
-
-    def _check_state(self, state):
-        '''
-        This function takes a state parameter and returns the first element of a tuple if state has a length of 2, otherwise it simply returns the state parameter.
-
-        :param state: The state data to be checked.
-        :return: The checked state data.
-        '''
-
-        state_num = len(state)
-        if state_num == 2:
-            state, _ = state  # Unpack the tuple
-        return state
-
-    def learn_reset(self):
-        """
-        Reset the agent's state and episode reward.
-        """
-
-        self.state = self.env.reset()
-        return self._check_state(self.state)
-
-    def learn_close(self):
-        """
-        Close the environment and reset the agent's total reward, episode count, and episode reward.
-        """
-
-        self.env.close()
-        self.total_reward = 0
-        self.episode = 0
-        self.episode_reward = 0
-
-    def learn_check(self):
-        """
-        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
-        """
-
-        avg_reward = self.total_reward / (self.episode + 1)
-        Logger.debug(
-            f'Episode: {self.episode}, Previous Reward: {self.prev_reward},  Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Episode Reward: {avg_reward}')
-
-    def select_action(self, state):
-        '''
-        These functions are placeholders and must be implemented by the child class that extends this Agent class.
-
-        select_action() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function takes the current state of the environment and returns the selected action for the agent to take.
-
-        :param state: The current state of the environment.
-        :return: The selected action for the agent to take.
-        '''
-        pass
-
-    def update(self):
-        '''
-        This function is a placeholder and must be implemented by the child class that extends this Agent class.
-
-        update() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function is responsible for updating the agent's state, action, and policy based on the new state and reward received from the environment.
-
-        No parameters are passed into this function and it does not return anything.
-        '''
-        pass
-
-    def step_unpack(self, step_output):
-        step_output_num = len(step_output)
-        if step_output_num == 4:
-            next_state, reward, is_done, _ = step_output
-        elif step_output_num == 5:
-            next_state, reward, is_done, _, _ = step_output
-        return next_state, reward, is_done
-
-    def update_reward(self, reward):
-        self.episode_reward += reward
-        self.total_reward += reward
-        self.prev_reward = reward
-
-    def update_episode(self):
-        self.episode += 1
-        self.episode_reward = 0
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms.
+The library is designed to be easily customizable and modular,
+allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
+
+"""
+
+
+from LogAssist.log import Logger
+from modular_rl.envs._custom import CustomEnv
+
+
+class AgentCustom:
+    def __init__(self, env, setting):
+        """
+        :param env: The environment for the agent to interact with. It should be an instance of a compatible environment class. If None is provided, a default CustomEnv environment will be used.
+        :type env: object
+        :param setting: The setting configuration for the agent, specifying various learning parameters and settings.
+        :type setting: dict
+        :return: None
+        """
+
+        self.env = env if env else CustomEnv()
+        self.setting = setting
+
+        # Set learn episode parameters
+        self.episode_reward = 0
+        self.total_reward = 0
+        self.prev_reward = 0
+        self.episode = 0
+        self.avg_reward = 0
+
+        # Set learn parameters (If necessary)
+        self.state = None
+        self.action = None
+        self.reward = None
+        self.done = None
+        self.reset()
+
+        # Training parameters(Common)
+        self.max_episodes = setting.get('max_episodes', 30)
+        self.max_timesteps = setting.get('max_timesteps', 100)
+
+        # Logger initialize
+        self.log_level = setting.get('log_level', 'debug')
+        self.log_init_pass = setting.get('log_init_pass', False)
+        if self.log_init_pass == False:
+            Logger.init(
+                dir_name=None,
+                file_name=None,
+                log_level=self.log_level,
+                out_console=True,
+                out_file=None,
+                prev_log_remove=None
+            )
+
+    def reset(self):
+        """
+        Reset the lists that contain information about the states, actions, rewards, and other values for the agent.
+        """
+
+        self.states = []
+        self.actions = []
+        self.rewards = []
+        self.next_states = []
+        self.dones = []
+        self.log_probs = []
+
+    def _check_state(self, state):
+        '''
+        This function takes a state parameter and returns the first element of a tuple if state has a length of 2, otherwise it simply returns the state parameter.
+
+        :param state: The state data to be checked.
+        :return: The checked state data.
+        '''
+
+        state_num = len(state)
+        if state_num == 2:
+            state, _ = state  # Unpack the tuple
+        return state
+
+    def learn_reset(self):
+        """
+        Reset the agent's state and episode reward.
+        """
+
+        self.state = self.env.reset()
+        return self._check_state(self.state)
+
+    def learn_close(self):
+        """
+        Close the environment and reset the agent's total reward, episode count, and episode reward.
+        """
+
+        self.env.close()
+        self.total_reward = 0
+        self.episode = 0
+        self.episode_reward = 0
+
+    def learn_check(self):
+        """
+        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
+        """
+
+        avg_reward = self.total_reward / (self.episode + 1)
+        Logger.debug(
+            f'Episode: {self.episode}, Previous Reward: {self.prev_reward},  Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Episode Reward: {avg_reward}')
+
+    def select_action(self, state):
+        '''
+        These functions are placeholders and must be implemented by the child class that extends this Agent class.
+
+        select_action() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function takes the current state of the environment and returns the selected action for the agent to take.
+
+        :param state: The current state of the environment.
+        :return: The selected action for the agent to take.
+        '''
+        pass
+
+    def update(self):
+        '''
+        This function is a placeholder and must be implemented by the child class that extends this Agent class.
+
+        update() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function is responsible for updating the agent's state, action, and policy based on the new state and reward received from the environment.
+
+        No parameters are passed into this function and it does not return anything.
+        '''
+        pass
+
+    def step_unpack(self, step_output):
+        step_output_num = len(step_output)
+        if step_output_num == 4:
+            next_state, reward, is_done, _ = step_output
+        elif step_output_num == 5:
+            next_state, reward, is_done, _, _ = step_output
+        return next_state, reward, is_done
+
+    def update_reward(self, reward):
+        self.episode_reward += reward
+        self.total_reward += reward
+        self.prev_reward = reward
+
+    def update_episode(self):
+        self.episode += 1
+        self.episode_reward = 0
```

### Comparing `modular_rl-0.4.1/modular_rl/agents/mcis.py` & `modular_rl-0.4.2/modular_rl/agents/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/agents/mcts.py` & `modular_rl-0.4.2/modular_rl/agents/mcts.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/agents/mim.py` & `modular_rl-0.4.2/modular_rl/agents/mim.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,524 +1,524 @@
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible-gh
-
-Class AgentMIM is an implementation of the Modular's sIMulator (MIM) algorithm.
-It takes an environment and a setting configuration as inputs, initializes various simulation parameters,
-and sets various simulation elements such as fixed states, unknown spaces, simulation states, excluded states, score calculation method, and simulation number.
-
-It has methods to perform a simulation given a state, calculate skewness and kurtosis of the simulation result, rank the simulation result array, and adjust weights based on the simulation result.
-The class also keeps track of the simulation iteration count, average standard deviations, skews, and kurtosises of the simulation results.
-
-This software includes the following third-party libraries:
-NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-"""
-
-import random
-import numpy as np
-from LogAssist.log import Logger
-from modular_rl.agents._custom import AgentCustom
-from modular_rl.params.mim import ParamMIM
-
-
-class AgentMIM(AgentCustom):
-    def __init__(self, env, setting):
-        """
-        Initialize the AgentMIM class with the specified environment and settings.
-
-        :param env: The environment to use for training.
-        :type env: gym.Env or None
-        :param setting: The settings for the MIM algorithm.
-        :type setting: AgentSettings
-        """
-        super().__init__(env, setting)
-        # The name to use for the fixed states in the simulation.
-        self.fixed_states_name = 'fixed_states'
-        # The name to use for the unknown spaces in the simulation.
-        self.unknown_spaces_name = 'unknown_spaces'
-        # The name to use for the simulation states.
-        self.simulation_states_name = 'simulation_states'
-        # The name to use for the excluded states in the simulation.
-        self.excluded_states_name = 'excluded_states'
-        # The name to use for the simulation number.
-        self.my_simulation_number_name = 'my_simulation_number'
-        # The name to use for the score table.
-        self.score_table_name = 'score_table'
-        # The name to use for the score calculation callback function.
-        self.score_calculation_callback_name = 'score_calculation_callback'
-        self.score_column = setting.get(  # The name of the score column in the score table.
-            'score_column', ParamMIM.default['score_column'])
-        self.simulation_iterations = setting.get(  # The number of iterations for each simulation.
-            'simulation_iterations', ParamMIM.default['simulation_iterations'])
-        self.superior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked superior.
-            'superior_rank_adjustment_factor', ParamMIM.default['superior_rank_adjustment_factor'])
-        self.inferior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked inferior.
-            'inferior_rank_adjustment_factor', ParamMIM.default['inferior_rank_adjustment_factor'])
-        self.std_deviation_factor = setting.get(
-            'std_deviation_factor', ParamMIM.default['std_deviation_factor'])
-        self.skewness_factor = setting.get(
-            'skewness_factor', ParamMIM.default['skewness_factor'])
-        self.kurtosis_factor = setting.get(
-            'kurtosis_factor', ParamMIM.default['kurtosis_factor'])
-
-        # Counter for the number of simulation iterations.
-        self.simulation_iteration_indexes_count = 0
-        # Average of standard deviations for all simulations.
-        self.standard_deviations_avg = 0
-        self.skews_avg = 0  # Average skewness for all simulations.
-        self.kurtosises_avg = 0  # Average kurtosis for all simulations.
-        self.reset()  # Reset the simulation results.
-
-    def simulate(self, state):
-        """
-        Simulates the given state with various conditions and adjustments.
-        It extracts the required elements from the state, performs multiple simulations,
-        calculates the score, and records the statistics of each simulation.
-
-        :param state: The state to be simulated.
-        :type state: dict
-        """
-
-        required_state_elements = {
-            self.fixed_states_name: 'fixed_state',
-            self.unknown_spaces_name: 'unknown_spaces',
-            self.simulation_states_name: 'simulation_states',
-            self.excluded_states_name: 'excluded_states',
-            self.score_calculation_callback_name: 'score_calculation_callback',
-            self.my_simulation_number_name: 'my_simulation_number',
-            self.score_table_name: 'score_table',
-        }
-
-        for element_key, error_obj in required_state_elements.items():
-            if state.get(element_key) is None:
-                raise Exception(
-                    f"'{error_obj}' not found in the provided state for simulation.")
-
-        fixed_states = state[self.fixed_states_name]
-        unknown_spaces = state[self.unknown_spaces_name]
-        simulation_states = state[self.simulation_states_name]
-        excluded_states = state[self.excluded_states_name]
-        score_calculation_callback = state[self.score_calculation_callback_name]
-        self.my_simulation_number = state[self.my_simulation_number_name]
-        score_table = state[self.score_table_name]
-        self.risk_table = state.get('risk_table', None)
-        remaining_states = set(simulation_states) - set(excluded_states)
-        simulation_table = []
-
-        Logger.verb(
-            'mim:simulate', f'{self.simulation_states_name},{list(remaining_states)}, {simulation_states}')
-
-        self.reset()
-
-        if len(fixed_states) != len(unknown_spaces):
-            return simulation_table
-
-        for fixed_state in fixed_states:
-            remaining_states -= set(fixed_state)
-
-        for i, fixed_state in enumerate(fixed_states):
-            simulation_table.append([0 for _ in score_table])
-            self.simulation_iteration_indexes.append(0)
-            for _ in range(self.simulation_iterations):
-                self.simulation_iteration_indexes[i] += 1
-                # Logger.verb('mim:simulate:fixed_states,unkonwn_spaces,remaining_states ',f'{fixed_states}, {unknown_spaces}, {list(remaining_states)}, {i}')
-                sample_states = random.sample(
-                    list(remaining_states), unknown_spaces[i])
-                simulated_result = fixed_state + sample_states
-                # Logger.verb('mim:simulate',simulated_result)
-                score_obj = score_calculation_callback(simulated_result)
-                score = score_obj[self.score_column] if self.score_column else score_obj
-                for idx in range(len(score_table)-1):
-                    # Logger.verb('mim:simulate',f'{score}, {score_table}')
-                    if score_table[idx] <= score <= score_table[idx+1]:
-                        simulation_table[i][idx] += 1
-                        break
-                if unknown_spaces[i] == 0:
-                    break
-
-        Logger.verb('mim:simulation_table', simulation_table)
-        for index in range(len(simulation_table)):
-            sim_result = 0
-            for sub_index in range(len(simulation_table[index])):
-                sim_result += simulation_table[index][sub_index] * \
-                    sub_index + 0.0001
-            self.simulation_totals.append(sim_result)
-            self.simulation_averages.append(
-                sim_result / self.simulation_iteration_indexes[index])
-            self.standard_deviations.append(np.std(simulation_table[index]))
-            skewness, kurtosis = self.calc_skewness_kurtosis(
-                simulation_table[index])
-            self.skews.append(skewness)
-            self.kurtosises.append(kurtosis)
-
-        Logger.verb('simulator:simulation_totals', self.simulation_totals)
-        Logger.verb('simulator:simulation_averages', self.simulation_averages)
-        Logger.verb('simulator:standard_deviations', self.standard_deviations)
-        Logger.verb('simulator:skews', self.skews)
-        Logger.verb('simulator:kurtosises', self.kurtosises)
-
-    def calc_skewness_kurtosis(self, data):
-        """
-        Calculates the skewness and kurtosis of the given data.
-
-        :param data: The data for which to calculate skewness and kurtosis.
-        :type data: list or array-like
-        :return: The skewness and kurtosis of the data.
-        :rtype: tuple
-        """
-
-        n = len(data)
-        mean = np.mean(data)
-        std_dev = np.std(data)
-
-        skewness = (1/n) * sum((x - mean)**3 for x in data) / (std_dev**3)
-        kurtosis = (1/n) * sum((x - mean)**4 for x in data) / (std_dev**4) - 3
-
-        return skewness, kurtosis
-
-    def rank_array(self, array):
-        """
-        Ranks the elements in the array in descending order.
-
-        :param array: The array to be ranked.
-        :type array: list or array-like
-        :return: The ranks of the elements in the array.
-        :rtype: numpy.ndarray
-        """
-
-        temp = array.argsort()
-        ranks = np.empty_like(temp)
-        ranks[temp] = len(array) - (np.arange(len(array)))
-
-        return ranks
-
-    def calculate_weight_adjustment_factors(self, simulation_size):
-        """
-        Calculates the adjustment factors for the weights of the simulations.
-
-        :param simulation_size: The size of the simulation.
-        :type simulation_size: int
-        :return: The adjustment factors for the weights of the simulations.
-        :rtype: list
-        """
-
-        weight_adjustment_factors = [1] * simulation_size
-        factors = [
-            self.std_deviation_factor,
-            self.skewness_factor,
-            self.kurtosis_factor,
-        ]
-        averages = [self.standard_deviations_avg,
-                    self.skews_avg, self.kurtosises_avg]
-        values = [self.standard_deviations, self.skews, self.kurtosises]
-
-        for index in range(simulation_size):
-            for factor, average, value in zip(factors, averages, values):
-                if average < value[index]:
-                    weight_adjustment_factor = factor * average / value[index]
-                    weight_adjustment_factors[index] += weight_adjustment_factor - factor
-        return weight_adjustment_factors
-
-    def update_averages(self, total_size):
-        """
-        Updates the averages of standard deviations, skews, and kurtosises.
-
-        :param total_size: The total size of the simulations.
-        :type total_size: int
-        """
-
-        factors = [self.standard_deviations_avg,
-                   self.skews_avg, self.kurtosises_avg]
-        values = [self.standard_deviations, self.skews, self.kurtosises]
-        for factor, value in zip(factors, values):
-            factor = (
-                factor * self.simulation_iteration_indexes_count + sum(value)) / total_size
-        self.simulation_iteration_indexes_count = total_size
-
-    def calculate_action_weights(self, adjusted_averages, skip_myself):
-        """
-        Calculates the weights for each action.
-
-        :param adjusted_averages: The adjusted averages from the simulations.
-        :type adjusted_averages: list
-        :param skip_myself: Whether to skip the current instance in the calculation.
-        :type skip_myself: bool
-        :return: The weights for each action.
-        :rtype: list
-        """
-
-        Logger.verb('mim:calculate_action_weights:adjusted_averages',
-                    adjusted_averages)
-        Logger.verb('mim:calculate_action_weights:my_simulation_average',
-                    self.my_simulation_average)
-        averages_table = []
-        if skip_myself:
-            averages_table.insert(0, self.my_simulation_average)
-        averages_table.extend(adjusted_averages)
-        Logger.verb('mim:calculate_action_weights:averages_table',
-                    averages_table)
-        ranks = self.rank_array(np.array(averages_table))
-        Logger.verb('mim:calculate_action_weights:ranks', f'{ranks}')
-
-        base_weight = int(1 / self.env.action_space * 100)
-        action_scale = self.env.action_space / len(ranks)
-        action_weights = [base_weight for _ in range(self.env.action_space)]
-        check_weights = [False for _ in range(self.env.action_space)]
-
-        Logger.verb('mim:calculate_action_weights:check_base_weight',
-                    f'{base_weight},{action_scale},{action_weights}')
-
-        my_rank = ranks[0]
-        my_average = self.my_simulation_average
-        my_action_rank = my_rank
-        my_action_rank = self.env.action_space - \
-            round(my_rank * action_scale)
-        if my_rank == 1 and action_scale >= 1.5:
-            my_action_rank = self.env.action_space - 1
-        if my_action_rank < 0:
-            my_action_rank = 0
-
-        for rank_idx in range(len(ranks)):
-            Logger.verb('mim:calculate_action_weights:rank_idx',
-                        rank_idx)
-            if rank_idx != 0:
-                rank_diff = abs(my_rank - ranks[rank_idx])
-                Logger.verb('mim:calculate_action_weights:rank_diff',
-                            rank_diff)
-                if my_rank < ranks[rank_idx]:
-                    average_weight = (averages_table[rank_idx] /
-                                      my_average) * (self.superior_rank_adjustment_factor ** rank_diff)
-                else:
-                    average_weight = (my_average /
-                                      averages_table[rank_idx]) * (self.inferior_rank_adjustment_factor ** rank_diff)
-
-                Logger.verb('mim:calculate_action_weights:scale,num',
-                            f'{action_scale}, {rank_idx}, {average_weight}')
-
-                action_num = self.env.action_space - \
-                    round(ranks[rank_idx] * action_scale)
-                if ranks[rank_idx] == 1 and action_scale >= 1.5:
-                    action_num = self.env.action_space - 1
-                if action_num < 0:
-                    action_num = 0
-                Logger.verb('mim:calculate_action_weights:action_num',
-                            action_num)
-
-                if check_weights[action_num] == False:
-                    check_weights[action_num] = True
-                    expect_weight = action_weights[action_num] * \
-                        average_weight
-                    weight_diff = action_weights[action_num] - expect_weight
-                    Logger.verb('mim:calculate_action_weights:weight_diff',
-                                f'{weight_diff}, {expect_weight}')
-                    action_weights[action_num] -= weight_diff
-                    if action_weights[action_num] < 1:
-                        action_weights[action_num] = 1
-                    action_weights[my_action_rank] += weight_diff
-                    Logger.verb('mim:calculate_action_weights:scale,num',
-                                f'{action_num}, {action_weights[action_num]}, {my_action_rank}, {action_weights[my_action_rank]}, {average_weight}')
-
-        for action_num in range(len(action_weights)):
-            if action_weights[action_num] in (0, int(1 / self.env.action_space * 100)):
-                prev_action_weights = action_weights[action_num-1]
-                next_action_weights = action_weights[action_num+1]
-                middle_weight = (prev_action_weights + next_action_weights) / 2
-                action_weights[action_num] = round(middle_weight)
-
-        if self.risk_table:
-            risk_total = sum(self.risk_table)
-            if risk_total != 0:
-                action_weight_total = 0
-                action_weight = 0
-                for risk_num in range(len(self.risk_table)):
-                    action_weight += action_weights[risk_num] * \
-                        self.risk_table[risk_num]
-                    action_weights[risk_num] -= action_weight
-                    action_weight_total += action_weight
-
-                risk_weight = [risk_total-self.risk_table[risk_num]
-                               for risk_num in range(len(self.risk_table))]
-                risk_total = sum(risk_weight)
-
-                Logger.verb('mim:calculate_action_weights:risk_weight,risk_total',
-                            f'{risk_weight},{risk_total}')
-
-                for risk_num in range(len(risk_weight)):
-                    if risk_total != 0:
-                        action_weights[risk_num] += action_weight_total * \
-                            risk_weight[risk_num] / risk_total
-
-        Logger.verb('mim:calculate_action_weights:action_weights',
-                    action_weights)
-        return action_weights
-
-    def calculate_weights(self):
-        """
-        Calculates the weights for the actions based on the simulation results.
-
-        :return: The calculated weights for each action.
-        :rtype: list
-        """
-
-        skip_myself = False
-        skip_count = 0
-
-        if self.simulation_iteration_indexes[self.my_simulation_number] <= 1:
-            skip_myself = True
-            skip_count = 1
-
-        self.my_simulation_average = self.simulation_averages[self.my_simulation_number]
-
-        if skip_myself:
-            del self.simulation_iteration_indexes[self.my_simulation_number]
-            del self.simulation_averages[self.my_simulation_number]
-            del self.standard_deviations[self.my_simulation_number]
-            del self.skews[self.my_simulation_number]
-            del self.kurtosises[self.my_simulation_number]
-
-        simulation_size = len(self.simulation_averages)
-        simulation_total_size = self.simulation_iteration_indexes_count + simulation_size
-
-        self.update_averages(simulation_total_size)
-        weight_adjustment_factors = self.calculate_weight_adjustment_factors(
-            simulation_size)
-
-        adjusted_averages = [average * factor for average,
-                             factor in zip(self.simulation_averages, weight_adjustment_factors)]
-        action_weights = self.calculate_action_weights(
-            adjusted_averages, skip_myself)
-
-        return action_weights
-
-    def select_action(self, state):
-        action_list = []
-        if isinstance(self.env.action_space, int) != True:
-            raise Exception("action space be not an integer")
-        else:
-            action_table = list(range(self.env.action_space))
-        self.simulate(state)
-        action_weights = self.calculate_weights()
-        Logger.verb('mim:select_action', action_weights)
-        for action_index in range(len(action_weights)):
-            for _ in range(int(action_weights[action_index])):
-                action_list.append(action_index)
-
-        random.shuffle(action_list)
-        choice = random.choice(action_list)
-        return action_table[choice]
-
-    def update_step(self, reward, done):
-        """
-        This method updates the agent at each step in the environment.
-        It takes as input the reward from the last action and a boolean indicating if the episode has ended.
-
-        :param reward: The reward received after executing an action
-        :type reward: int/float
-        :param done: Indicates if the episode has ended
-        :type done: bool
-        """
-        self.update_reward(reward)
-        # self.states.append(state)
-        # self.actions.append(action)
-        # self.rewards.append(reward)
-        # self.dones.append(done)
-        # self.next_states.append(next_state)
-        if done:
-            self.update()
-
-    def update(self):
-        """
-        This method is intended to update the internal model or values based on the collected rewards or experiences.
-        Currently, it's just a placeholder and does nothing. Further implementation is needed.
-        """
-        pass
-
-    def reset(self):
-        """
-        This method resets the agent's internal data. It's typically called at the end of each episode.
-        It clears out various lists that store information about the simulations.
-        """
-        self.simulation_totals = []
-        self.simulation_iteration_indexes = []
-        self.simulation_averages = []
-        self.standard_deviations = []
-        self.skews = []
-        self.kurtosises = []
-
-    def train(self):
-        """
-        Train the agent.
-        """
-        self.learn()
-
-    def learn(self):
-        """
-        Train the agent.
-        """
-        self.total_reward = 0
-        for episode in range(self.max_episodes):
-            self.episode = episode
-            state = self.learn_reset()
-            for t in range(self.max_timesteps):
-                state = self._check_state(state)
-
-                # Select an action
-                action = self.select_action(state)
-                Logger.verb('agents:mim:learn:action', action)
-                # Take a step in the environment
-                next_state, reward, done = self.env.step(action)
-                # Update the agent's experience
-                self.update_step(reward, done)
-                # Update the network parameters at the end of the episode
-                if done:
-                    self.update()
-                    self.learn_check()
-                    break
-                state = next_state
-            self.episode += 1
-
-    def load(self, file_name):
-        """
-        Loads the simulation statistics from the given file.
-
-        :param file_name: The name of the file from which to load the statistics.
-        :type file_name: str
-        """
-        self.load_model(file_name)
-
-    def load_model(self, file_name):
-        """
-        Loads the simulation statistics from the given file.
-
-        :param file_name: The name of the file from which to load the statistics.
-        :type file_name: str
-        """
-        data_arr = np.load(file_name)
-        self.simulation_iteration_indexes_count = data_arr[0]
-        self.standard_deviations_avg = data_arr[1]
-        self.skews_avg = data_arr[2]
-        self.kurtosises_avg = data_arr[3]
-
-    def save(self, file_name):
-        """
-        Saves the simulation statistics to the given file.
-
-        :param file_name: The name of the file to which to save the statistics.
-        :type file_name: str
-        """
-        self.save_model(file_name)
-
-    def save_model(self, file_name):
-        """
-        Saves the simulation statistics to the given file.
-
-        :param file_name: The name of the file to which to save the statistics.
-        :type file_name: str
-        """
-        data_arr = [
-            self.simulation_iteration_indexes_count,
-            self.standard_deviations_avg,
-            self.skews_avg,
-            self.kurtosises_avg,
-        ]
-        np.save(file_name, data_arr)
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+Class AgentMIM is an implementation of the Modular's sIMulator (MIM) algorithm.
+It takes an environment and a setting configuration as inputs, initializes various simulation parameters,
+and sets various simulation elements such as fixed states, unknown spaces, simulation states, excluded states, score calculation method, and simulation number.
+
+It has methods to perform a simulation given a state, calculate skewness and kurtosis of the simulation result, rank the simulation result array, and adjust weights based on the simulation result.
+The class also keeps track of the simulation iteration count, average standard deviations, skews, and kurtosises of the simulation results.
+
+This software includes the following third-party libraries:
+NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
+"""
+
+import random
+import numpy as np
+from LogAssist.log import Logger
+from modular_rl.agents._custom import AgentCustom
+from modular_rl.params.mim import ParamMIM
+
+
+class AgentMIM(AgentCustom):
+    def __init__(self, env, setting):
+        """
+        Initialize the AgentMIM class with the specified environment and settings.
+
+        :param env: The environment to use for training.
+        :type env: gym.Env or None
+        :param setting: The settings for the MIM algorithm.
+        :type setting: AgentSettings
+        """
+        super().__init__(env, setting)
+        # The name to use for the fixed states in the simulation.
+        self.fixed_states_name = 'fixed_states'
+        # The name to use for the unknown spaces in the simulation.
+        self.unknown_spaces_name = 'unknown_spaces'
+        # The name to use for the simulation states.
+        self.simulation_states_name = 'simulation_states'
+        # The name to use for the excluded states in the simulation.
+        self.excluded_states_name = 'excluded_states'
+        # The name to use for the simulation number.
+        self.my_simulation_number_name = 'my_simulation_number'
+        # The name to use for the score table.
+        self.score_table_name = 'score_table'
+        # The name to use for the score calculation callback function.
+        self.score_calculation_callback_name = 'score_calculation_callback'
+        self.score_column = setting.get(  # The name of the score column in the score table.
+            'score_column', ParamMIM.default['score_column'])
+        self.simulation_iterations = setting.get(  # The number of iterations for each simulation.
+            'simulation_iterations', ParamMIM.default['simulation_iterations'])
+        self.superior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked superior.
+            'superior_rank_adjustment_factor', ParamMIM.default['superior_rank_adjustment_factor'])
+        self.inferior_rank_adjustment_factor = setting.get(  # The adjustment factor applied to actions that are ranked inferior.
+            'inferior_rank_adjustment_factor', ParamMIM.default['inferior_rank_adjustment_factor'])
+        self.std_deviation_factor = setting.get(
+            'std_deviation_factor', ParamMIM.default['std_deviation_factor'])
+        self.skewness_factor = setting.get(
+            'skewness_factor', ParamMIM.default['skewness_factor'])
+        self.kurtosis_factor = setting.get(
+            'kurtosis_factor', ParamMIM.default['kurtosis_factor'])
+
+        # Counter for the number of simulation iterations.
+        self.simulation_iteration_indexes_count = 0
+        # Average of standard deviations for all simulations.
+        self.standard_deviations_avg = 0
+        self.skews_avg = 0  # Average skewness for all simulations.
+        self.kurtosises_avg = 0  # Average kurtosis for all simulations.
+        self.reset()  # Reset the simulation results.
+
+    def simulate(self, state):
+        """
+        Simulates the given state with various conditions and adjustments.
+        It extracts the required elements from the state, performs multiple simulations,
+        calculates the score, and records the statistics of each simulation.
+
+        :param state: The state to be simulated.
+        :type state: dict
+        """
+
+        required_state_elements = {
+            self.fixed_states_name: 'fixed_state',
+            self.unknown_spaces_name: 'unknown_spaces',
+            self.simulation_states_name: 'simulation_states',
+            self.excluded_states_name: 'excluded_states',
+            self.score_calculation_callback_name: 'score_calculation_callback',
+            self.my_simulation_number_name: 'my_simulation_number',
+            self.score_table_name: 'score_table',
+        }
+
+        for element_key, error_obj in required_state_elements.items():
+            if state.get(element_key) is None:
+                raise Exception(
+                    f"'{error_obj}' not found in the provided state for simulation.")
+
+        fixed_states = state[self.fixed_states_name]
+        unknown_spaces = state[self.unknown_spaces_name]
+        simulation_states = state[self.simulation_states_name]
+        excluded_states = state[self.excluded_states_name]
+        score_calculation_callback = state[self.score_calculation_callback_name]
+        self.my_simulation_number = state[self.my_simulation_number_name]
+        score_table = state[self.score_table_name]
+        self.risk_table = state.get('risk_table', None)
+        remaining_states = set(simulation_states) - set(excluded_states)
+        simulation_table = []
+
+        Logger.verb(
+            'mim:simulate', f'{self.simulation_states_name},{list(remaining_states)}, {simulation_states}')
+
+        self.reset()
+
+        if len(fixed_states) != len(unknown_spaces):
+            return simulation_table
+
+        for fixed_state in fixed_states:
+            remaining_states -= set(fixed_state)
+
+        for i, fixed_state in enumerate(fixed_states):
+            simulation_table.append([0 for _ in score_table])
+            self.simulation_iteration_indexes.append(0)
+            for _ in range(self.simulation_iterations):
+                self.simulation_iteration_indexes[i] += 1
+                # Logger.verb('mim:simulate:fixed_states,unkonwn_spaces,remaining_states ',f'{fixed_states}, {unknown_spaces}, {list(remaining_states)}, {i}')
+                sample_states = random.sample(
+                    list(remaining_states), unknown_spaces[i])
+                simulated_result = fixed_state + sample_states
+                # Logger.verb('mim:simulate',simulated_result)
+                score_obj = score_calculation_callback(simulated_result)
+                score = score_obj[self.score_column] if self.score_column else score_obj
+                for idx in range(len(score_table)-1):
+                    # Logger.verb('mim:simulate',f'{score}, {score_table}')
+                    if score_table[idx] <= score <= score_table[idx+1]:
+                        simulation_table[i][idx] += 1
+                        break
+                if unknown_spaces[i] == 0:
+                    break
+
+        Logger.verb('mim:simulation_table', simulation_table)
+        for index in range(len(simulation_table)):
+            sim_result = 0
+            for sub_index in range(len(simulation_table[index])):
+                sim_result += simulation_table[index][sub_index] * \
+                    sub_index + 0.0001
+            self.simulation_totals.append(sim_result)
+            self.simulation_averages.append(
+                sim_result / self.simulation_iteration_indexes[index])
+            self.standard_deviations.append(np.std(simulation_table[index]))
+            skewness, kurtosis = self.calc_skewness_kurtosis(
+                simulation_table[index])
+            self.skews.append(skewness)
+            self.kurtosises.append(kurtosis)
+
+        Logger.verb('simulator:simulation_totals', self.simulation_totals)
+        Logger.verb('simulator:simulation_averages', self.simulation_averages)
+        Logger.verb('simulator:standard_deviations', self.standard_deviations)
+        Logger.verb('simulator:skews', self.skews)
+        Logger.verb('simulator:kurtosises', self.kurtosises)
+
+    def calc_skewness_kurtosis(self, data):
+        """
+        Calculates the skewness and kurtosis of the given data.
+
+        :param data: The data for which to calculate skewness and kurtosis.
+        :type data: list or array-like
+        :return: The skewness and kurtosis of the data.
+        :rtype: tuple
+        """
+
+        n = len(data)
+        mean = np.mean(data)
+        std_dev = np.std(data)
+
+        skewness = (1/n) * sum((x - mean)**3 for x in data) / (std_dev**3)
+        kurtosis = (1/n) * sum((x - mean)**4 for x in data) / (std_dev**4) - 3
+
+        return skewness, kurtosis
+
+    def rank_array(self, array):
+        """
+        Ranks the elements in the array in descending order.
+
+        :param array: The array to be ranked.
+        :type array: list or array-like
+        :return: The ranks of the elements in the array.
+        :rtype: numpy.ndarray
+        """
+
+        temp = array.argsort()
+        ranks = np.empty_like(temp)
+        ranks[temp] = len(array) - (np.arange(len(array)))
+
+        return ranks
+
+    def calculate_weight_adjustment_factors(self, simulation_size):
+        """
+        Calculates the adjustment factors for the weights of the simulations.
+
+        :param simulation_size: The size of the simulation.
+        :type simulation_size: int
+        :return: The adjustment factors for the weights of the simulations.
+        :rtype: list
+        """
+
+        weight_adjustment_factors = [1] * simulation_size
+        factors = [
+            self.std_deviation_factor,
+            self.skewness_factor,
+            self.kurtosis_factor,
+        ]
+        averages = [self.standard_deviations_avg,
+                    self.skews_avg, self.kurtosises_avg]
+        values = [self.standard_deviations, self.skews, self.kurtosises]
+
+        for index in range(simulation_size):
+            for factor, average, value in zip(factors, averages, values):
+                if average < value[index]:
+                    weight_adjustment_factor = factor * average / value[index]
+                    weight_adjustment_factors[index] += weight_adjustment_factor - factor
+        return weight_adjustment_factors
+
+    def update_averages(self, total_size):
+        """
+        Updates the averages of standard deviations, skews, and kurtosises.
+
+        :param total_size: The total size of the simulations.
+        :type total_size: int
+        """
+
+        factors = [self.standard_deviations_avg,
+                   self.skews_avg, self.kurtosises_avg]
+        values = [self.standard_deviations, self.skews, self.kurtosises]
+        for factor, value in zip(factors, values):
+            factor = (
+                factor * self.simulation_iteration_indexes_count + sum(value)) / total_size
+        self.simulation_iteration_indexes_count = total_size
+
+    def calculate_action_weights(self, adjusted_averages, skip_myself):
+        """
+        Calculates the weights for each action.
+
+        :param adjusted_averages: The adjusted averages from the simulations.
+        :type adjusted_averages: list
+        :param skip_myself: Whether to skip the current instance in the calculation.
+        :type skip_myself: bool
+        :return: The weights for each action.
+        :rtype: list
+        """
+
+        Logger.verb('mim:calculate_action_weights:adjusted_averages',
+                    adjusted_averages)
+        Logger.verb('mim:calculate_action_weights:my_simulation_average',
+                    self.my_simulation_average)
+        averages_table = []
+        if skip_myself:
+            averages_table.insert(0, self.my_simulation_average)
+        averages_table.extend(adjusted_averages)
+        Logger.verb('mim:calculate_action_weights:averages_table',
+                    averages_table)
+        ranks = self.rank_array(np.array(averages_table))
+        Logger.verb('mim:calculate_action_weights:ranks', f'{ranks}')
+
+        base_weight = int(1 / self.env.action_space * 100)
+        action_scale = self.env.action_space / len(ranks)
+        action_weights = [base_weight for _ in range(self.env.action_space)]
+        check_weights = [False for _ in range(self.env.action_space)]
+
+        Logger.verb('mim:calculate_action_weights:check_base_weight',
+                    f'{base_weight},{action_scale},{action_weights}')
+
+        my_rank = ranks[0]
+        my_average = self.my_simulation_average
+        my_action_rank = my_rank
+        my_action_rank = self.env.action_space - \
+            round(my_rank * action_scale)
+        if my_rank == 1 and action_scale >= 1.5:
+            my_action_rank = self.env.action_space - 1
+        if my_action_rank < 0:
+            my_action_rank = 0
+
+        for rank_idx in range(len(ranks)):
+            Logger.verb('mim:calculate_action_weights:rank_idx',
+                        rank_idx)
+            if rank_idx != 0:
+                rank_diff = abs(my_rank - ranks[rank_idx])
+                Logger.verb('mim:calculate_action_weights:rank_diff',
+                            rank_diff)
+                if my_rank < ranks[rank_idx]:
+                    average_weight = (averages_table[rank_idx] /
+                                      my_average) * (self.superior_rank_adjustment_factor ** rank_diff)
+                else:
+                    average_weight = (my_average /
+                                      averages_table[rank_idx]) * (self.inferior_rank_adjustment_factor ** rank_diff)
+
+                Logger.verb('mim:calculate_action_weights:scale,num',
+                            f'{action_scale}, {rank_idx}, {average_weight}')
+
+                action_num = self.env.action_space - \
+                    round(ranks[rank_idx] * action_scale)
+                if ranks[rank_idx] == 1 and action_scale >= 1.5:
+                    action_num = self.env.action_space - 1
+                if action_num < 0:
+                    action_num = 0
+                Logger.verb('mim:calculate_action_weights:action_num',
+                            action_num)
+
+                if check_weights[action_num] == False:
+                    check_weights[action_num] = True
+                    expect_weight = action_weights[action_num] * \
+                        average_weight
+                    weight_diff = action_weights[action_num] - expect_weight
+                    Logger.verb('mim:calculate_action_weights:weight_diff',
+                                f'{weight_diff}, {expect_weight}')
+                    action_weights[action_num] -= weight_diff
+                    if action_weights[action_num] < 1:
+                        action_weights[action_num] = 1
+                    action_weights[my_action_rank] += weight_diff
+                    Logger.verb('mim:calculate_action_weights:scale,num',
+                                f'{action_num}, {action_weights[action_num]}, {my_action_rank}, {action_weights[my_action_rank]}, {average_weight}')
+
+        for action_num in range(len(action_weights)):
+            if action_weights[action_num] in (0, int(1 / self.env.action_space * 100)):
+                prev_action_weights = action_weights[action_num-1]
+                next_action_weights = action_weights[action_num+1]
+                middle_weight = (prev_action_weights + next_action_weights) / 2
+                action_weights[action_num] = round(middle_weight)
+
+        if self.risk_table:
+            risk_total = sum(self.risk_table)
+            if risk_total != 0:
+                action_weight_total = 0
+                action_weight = 0
+                for risk_num in range(len(self.risk_table)):
+                    action_weight += action_weights[risk_num] * \
+                        self.risk_table[risk_num]
+                    action_weights[risk_num] -= action_weight
+                    action_weight_total += action_weight
+
+                risk_weight = [risk_total-self.risk_table[risk_num]
+                               for risk_num in range(len(self.risk_table))]
+                risk_total = sum(risk_weight)
+
+                Logger.verb('mim:calculate_action_weights:risk_weight,risk_total',
+                            f'{risk_weight},{risk_total}')
+
+                for risk_num in range(len(risk_weight)):
+                    if risk_total != 0:
+                        action_weights[risk_num] += action_weight_total * \
+                            risk_weight[risk_num] / risk_total
+
+        Logger.verb('mim:calculate_action_weights:action_weights',
+                    action_weights)
+        return action_weights
+
+    def calculate_weights(self):
+        """
+        Calculates the weights for the actions based on the simulation results.
+
+        :return: The calculated weights for each action.
+        :rtype: list
+        """
+
+        skip_myself = False
+        skip_count = 0
+
+        if self.simulation_iteration_indexes[self.my_simulation_number] <= 1:
+            skip_myself = True
+            skip_count = 1
+
+        self.my_simulation_average = self.simulation_averages[self.my_simulation_number]
+
+        if skip_myself:
+            del self.simulation_iteration_indexes[self.my_simulation_number]
+            del self.simulation_averages[self.my_simulation_number]
+            del self.standard_deviations[self.my_simulation_number]
+            del self.skews[self.my_simulation_number]
+            del self.kurtosises[self.my_simulation_number]
+
+        simulation_size = len(self.simulation_averages)
+        simulation_total_size = self.simulation_iteration_indexes_count + simulation_size
+
+        self.update_averages(simulation_total_size)
+        weight_adjustment_factors = self.calculate_weight_adjustment_factors(
+            simulation_size)
+
+        adjusted_averages = [average * factor for average,
+                             factor in zip(self.simulation_averages, weight_adjustment_factors)]
+        action_weights = self.calculate_action_weights(
+            adjusted_averages, skip_myself)
+
+        return action_weights
+
+    def select_action(self, state):
+        action_list = []
+        if isinstance(self.env.action_space, int) != True:
+            raise Exception("action space be not an integer")
+        else:
+            action_table = list(range(self.env.action_space))
+        self.simulate(state)
+        action_weights = self.calculate_weights()
+        Logger.verb('mim:select_action', action_weights)
+        for action_index in range(len(action_weights)):
+            for _ in range(int(action_weights[action_index])):
+                action_list.append(action_index)
+
+        random.shuffle(action_list)
+        choice = random.choice(action_list)
+        return action_table[choice]
+
+    def update_step(self, reward, done):
+        """
+        This method updates the agent at each step in the environment.
+        It takes as input the reward from the last action and a boolean indicating if the episode has ended.
+
+        :param reward: The reward received after executing an action
+        :type reward: int/float
+        :param done: Indicates if the episode has ended
+        :type done: bool
+        """
+        self.update_reward(reward)
+        # self.states.append(state)
+        # self.actions.append(action)
+        # self.rewards.append(reward)
+        # self.dones.append(done)
+        # self.next_states.append(next_state)
+        if done:
+            self.update()
+
+    def update(self):
+        """
+        This method is intended to update the internal model or values based on the collected rewards or experiences.
+        Currently, it's just a placeholder and does nothing. Further implementation is needed.
+        """
+        pass
+
+    def reset(self):
+        """
+        This method resets the agent's internal data. It's typically called at the end of each episode.
+        It clears out various lists that store information about the simulations.
+        """
+        self.simulation_totals = []
+        self.simulation_iteration_indexes = []
+        self.simulation_averages = []
+        self.standard_deviations = []
+        self.skews = []
+        self.kurtosises = []
+
+    def train(self):
+        """
+        Train the agent.
+        """
+        self.learn()
+
+    def learn(self):
+        """
+        Train the agent.
+        """
+        self.total_reward = 0
+        for episode in range(self.max_episodes):
+            self.episode = episode
+            state = self.learn_reset()
+            for t in range(self.max_timesteps):
+                state = self._check_state(state)
+
+                # Select an action
+                action = self.select_action(state)
+                Logger.verb('agents:mim:learn:action', action)
+                # Take a step in the environment
+                next_state, reward, done = self.env.step(action)
+                # Update the agent's experience
+                self.update_step(reward, done)
+                # Update the network parameters at the end of the episode
+                if done:
+                    self.update()
+                    self.learn_check()
+                    break
+                state = next_state
+            self.episode += 1
+
+    def load(self, file_name):
+        """
+        Loads the simulation statistics from the given file.
+
+        :param file_name: The name of the file from which to load the statistics.
+        :type file_name: str
+        """
+        self.load_model(file_name)
+
+    def load_model(self, file_name):
+        """
+        Loads the simulation statistics from the given file.
+
+        :param file_name: The name of the file from which to load the statistics.
+        :type file_name: str
+        """
+        data_arr = np.load(file_name)
+        self.simulation_iteration_indexes_count = data_arr[0]
+        self.standard_deviations_avg = data_arr[1]
+        self.skews_avg = data_arr[2]
+        self.kurtosises_avg = data_arr[3]
+
+    def save(self, file_name):
+        """
+        Saves the simulation statistics to the given file.
+
+        :param file_name: The name of the file to which to save the statistics.
+        :type file_name: str
+        """
+        self.save_model(file_name)
+
+    def save_model(self, file_name):
+        """
+        Saves the simulation statistics to the given file.
+
+        :param file_name: The name of the file to which to save the statistics.
+        :type file_name: str
+        """
+        data_arr = [
+            self.simulation_iteration_indexes_count,
+            self.standard_deviations_avg,
+            self.skews_avg,
+            self.kurtosises_avg,
+        ]
+        np.save(file_name, data_arr)
```

### Comparing `modular_rl-0.4.1/modular_rl/agents/ppo.py` & `modular_rl-0.4.2/modular_rl/agents/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/agents/pytorch/_agent.py` & `modular_rl-0.4.2/modular_rl/agents/pytorch/_agent.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/agents/pytorch/mcis.py` & `modular_rl-0.4.2/modular_rl/agents/pytorch/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/agents/pytorch/mcts.py` & `modular_rl-0.4.2/modular_rl/agents/pytorch/mcts.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/agents/pytorch/ppo.py` & `modular_rl-0.4.2/modular_rl/agents/pytorch/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/agents/tensorflow/_agent.py` & `modular_rl-0.4.2/modular_rl/agents/tensorflow/_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,40 +127,41 @@
         """
         Save the policy and value networks.
 
         :param file_name: The base name of the files to save the networks.
         :type file_name: str
         """
 
-        self.policy_net.save(file_name + '_policy.h5')
-        self.value_net.save(file_name + '_value.h5')
+        self.policy_net.save(file_name + '_policy', save_format='tf')
+        self.value_net.save(file_name + '_value', save_format='tf')
 
     def load_policy_value(self, file_name):
         """
         Load the policy and value networks.
 
         :param file_name: The base name of the files to load the networks.
         :type file_name: str
         """
 
-        self.policy_net = load_model(file_name + '_policy.h5')
-        self.value_net = load_model(file_name + '_value.h5')
+        self.policy_net = load_model(file_name + '_policy')
+        self.value_net = load_model(file_name + '_value')
 
     def save_actor_critic(self, file_name):
         """
         Save the actor-critic network.
 
         :param file_name: The name of the file to save the network.
         :type file_name: str
         """
 
-        self.actor_critic_net.save(file_name + '_actor_critic.h5')
+        self.actor_critic_net.save(
+            file_name + '_actor_critic', save_format='tf')
 
     def load_actor_critic(self, file_name):
         """
         Load the actor-critic network.
 
         :param file_name: The name of the file to load the network.
         :type file_name: str
         """
 
-        self.actor_critic_net = load_model(file_name + '_actor_critic.h5')
+        self.actor_critic_net = load_model(file_name + '_actor_critic')
```

### Comparing `modular_rl-0.4.1/modular_rl/agents/tensorflow/mcis.py` & `modular_rl-0.4.2/modular_rl/agents/tensorflow/mcts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,36 @@
+
+# -*- coding: utf-8 -*-
 """
 ModularRL project
 
 Copyright (c) 2023 horrible-gh
 
-Class AgentMCIS is an implementation of the Monte Carlo Importance Sampling (MCIS) algorithm.
-The algorithm is used for solving problems of sequential decision making under uncertainty.
+Class AgentMCTS is an implementation of the Monte Carlo Tree Search (MCTS) algorithm.
 It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
 and sets various learning parameters.
-This class has methods to predict an action given a state, perform a learning step, update the neural network parameters,
+It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
 save and load a checkpoint, and reset learning parameters.
 The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
 
-Importance Sampling is used to estimate the properties of a particular target distribution, given some observed data and a proposal distribution.
-This implementation makes use of Monte Carlo methods, which rely on repeated random sampling to obtain numerical results.
-
 This software includes the following third-party libraries:
 Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
 NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
 TensorFlow (Apache License 2.0): https://www.tensorflow.org/ - Copyright (c) TensorFlow Developers.
 """
 
 import tensorflow as tf
 import tensorflow_probability as tfp
 import numpy as np
 from LogAssist.log import Logger
 from modular_rl.agents.tensorflow._agent import Agent
 from modular_rl.util.node import Node
 
 
-class TensorFlowAgentMCIS(Agent):
+class TensorFlowAgentMCTS(Agent):
     def __init__(self, env, setting):
         """
         Initialize the AgentMCIS class with the specified environment and settings.
 
         :param env: The environment to use for training.
         :type env: gym.Env or None
         :param setting: The settings for the MCIS algorithm.
@@ -49,193 +47,196 @@
 
         self.device = setting.get('device', None)
         if self.device == None:
             # TensorFlow automatically uses the GPU if one is available, otherwise it uses the CPU.
             # Therefore, there is no need to manually set the device as in PyTorch.
             pass
 
-    def update_step(self, state, action, reward, done, next_state):
+    def reset(self):
+        self.state = None
+        self.action = None
+        self.reward = None
+        self.done = None
+        self.total_reward = 0
+        self.total_value = 0
+
+    def select_action(self, state):
         """
-        Updates the provided state, action, reward, done, and next_state.
+        Select an action using MCTS.
 
-        :param state: The current state of the environment.
+        :param state: The current state.
         :type state: numpy.ndarray
-        :param action: The action taken by the agent.
-        :type action: int
-        :param reward: The reward for the current step.
-        :type reward: float
-        :param done: Flag to mark if the episode is done or not.
-        :type done: bool
-        :param next_state: The next state after the current action.
-        :type next_state: numpy.ndarray
+        :return: The selected action.
+        :rtype: int
         """
+        state = self._check_state(state)
+        state_tensor = self.check_tensor(state)
+        action_probs, _ = self.actor_critic_net(state_tensor)
+        action_probs = tf.stop_gradient(action_probs)
+        m = tfp.distributions.Categorical(probs=action_probs)
+        chosen_action = m.sample().numpy().item()
 
-        self.update_reward(reward)
-
-        self.states.append(tf.squeeze(state))  # change here
-        self.actions.append(action)
-        self.rewards.append(reward)
-        self.dones.append(done)
-        self.next_states.append(tf.squeeze(next_state))  # change here
-
-        if done:
-            self.update()
+        # Use uniform prior for root node.
+        root = Node(state, [1 / self.env.action_space.n]
+                    * self.env.action_space.n)
 
-    def select_action(self, state):
-        state_tensor = tf.convert_to_tensor(
-            self.check_tensor(state), dtype=tf.float32)
-        action_probs, _ = self.actor_critic_net(state_tensor)
-        action_probs = action_probs.numpy().flatten()
-        root = Node(state, action_probs)
         for _ in range(self.num_simulations):
-            node = root
-            search_path = [node]
+            node, search_path = root, [root]
+
             while node.expanded():
-                best_score = -np.inf
-                best_action = -1
-                for action, child in node.children.items():
-                    uct_score = child.get_score(self.cpuct)
-                    if np.any(uct_score > best_score):
-                        best_score = uct_score
-                        best_action = action
-
-                if best_action != -1:
-                    action = best_action
-                    node = node.children[action]
-                    search_path.append(node)
-                else:
-                    break
+                action, node = node.select_child(self.cpuct)
+                if action is None:
+                    action = chosen_action
+                search_path.append(node)
+
+            parent, action = (search_path[-2], search_path[-1].action) if len(
+                search_path) > 1 else (search_path[0], None)
+            step_output = self.env.step(action) if action is not None else (
+                parent.state, 0, False, None)
+            state, reward, done, *_ = step_output
+            Logger.verb('mcts:select_action', f"Step Output Reward: {reward}")
+
+            if not done:
+                state_tensor = self.check_tensor(state)
+                action_probs, _ = self.actor_critic_net(state_tensor)
+                node.expand(self.env.action_space.n,
+                            action_probs.numpy().flatten(), False)
+
+            self.backpropagate(search_path, reward, done)
+
+        chosen_action_node = root.children[chosen_action]
 
-            if len(search_path) > 1:
-                parent, action = search_path[-2], search_path[-1].action
-            else:
-                parent, action = search_path[0], None
-            if True not in self.dones:  # Check if the game is not over
-                state_tensor = tf.convert_to_tensor(
-                    self.check_tensor(node.state), dtype=tf.float32)
-                action_probs, value = self.actor_critic_net(state_tensor)
-                action_space = self.env.action_space.n
-                node.expand(action_space, action_probs, False)
-            state_tensor = tf.convert_to_tensor(
-                self.check_tensor(node.state), dtype=tf.float32)
-            _, value = self.actor_critic_net(state_tensor)
-            self.backpropagate(search_path, value.numpy(), node.done)
-        root_state_tensor = tf.convert_to_tensor(
-            self.check_tensor(root.state), dtype=tf.float32)
-        action_probs, _ = self.actor_critic_net(root_state_tensor)
-        action_probs = action_probs.numpy().flatten()  # make sure it is a flat array
-        Logger.verb('mcis:select_action:action_probs', f'{action_probs}')
-        chosen_action = np.random.choice(
-            range(len(action_probs)), p=action_probs)  # choosing from the range of all possible actions
-        return chosen_action
+        self.state = chosen_action_node.state
+        self.action = chosen_action
+        self.reward = chosen_action_node.total_value
+        self.done = self.reward != 0
+
+        self.total_reward += self.reward
+        self.total_value = self.total_reward
+
+        return self.state, self.action, self.reward, self.done
 
     def backpropagate(self, search_path, reward, done):
         """
         Backpropagate the value estimates back to the root node.
 
         :param search_path: The nodes visited during the search.
         :type search_path: list of Node
         :param reward: The reward obtained after the search.
         :type reward: float
         :param done: Whether the episode has ended.
         :type done: bool
         """
         for node in reversed(search_path):
+            # Logger.verb('mcts:backpropagate',
+            #            f"Node Reward({reward}) after Update Stats: {node.total_value}")
             node.update_stats(reward)
-            if not done:
-                if isinstance(node.state, np.ndarray):
-                    state_tensor = tf.convert_to_tensor(
-                        node.state, dtype=tf.float32)
-                elif tf.is_tensor(node.state):
-                    state_tensor = node.state
-                else:
-                    raise ValueError(
-                        "node.state must be a numpy array or tensorflow tensor")
-                _, reward = self.actor_critic_net(state_tensor)
-                reward = reward.numpy()
 
-    def compute_loss(self, state, action, reward, next_state, done):
+    def compute_loss(self, state, action, reward, done):
         '''
-        This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
+        This function computes the actor and critic loss using the provided state, action, reward, and done variables.
         The actor loss is computed based on the policy gradient algorithm,
         and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
 
-        compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
-
-        The state parameter is the current state of the environment.
-        The action parameter is the action taken in the current state.
-        The reward parameter is the reward received for taking the action in the current state.
-        The next_state parameter is the state resulting from taking the action in the current state.
-        The done parameter is a flag indicating whether the episode has ended.
-
         :param state: The current state of the environment.
         :param action: The action taken in the current state.
         :param reward: The reward received for taking the action in the current state.
-        :param next_state: The state resulting from taking the action in the current state.
         :param done: A flag indicating whether the episode has ended.
         :return: The computed actor and critic loss values.
         '''
-
         # Predict action probabilities and values
+        state = self.ensure_float(state)
         action_probs, values = self.actor_critic_net(state)
 
+        # Convert reward to tensor
+        reward = tf.convert_to_tensor(reward, dtype=tf.float32)
         # Compute the value loss
-        actor_output, critic_output = self.actor_critic_net(next_state)
-        target_values = reward + self.gamma * \
-            tf.reduce_mean(critic_output) * (1 - done)
-        target_values = tf.expand_dims(target_values, 1)
-        critic_loss = tf.keras.losses.MSE(
-            values, tf.stop_gradient(target_values))
+        target_values = reward + self.gamma * self.total_value * (1 - done)
+        target_values = tf.expand_dims(target_values, axis=0)
+        critic_loss = tf.keras.losses.MSE(values, target_values)
+
+        # If action is not a list or tuple or its length is zero, initialize it with zeros
+        if not isinstance(action, (list, tuple)) or len(action) == 0:
+            action = tf.zeros_like(action_probs)
 
         # Compute the policy loss
         m = tfp.distributions.Categorical(probs=action_probs)
         logprobs = m.log_prob(self.check_tensor(action))
-        actor_loss = -logprobs * tf.stop_gradient(target_values - values)
+        actor_loss = -logprobs * (target_values - values)
+
+        # Average the actor and critic loss
+        loss = (tf.reduce_mean(actor_loss) + tf.reduce_mean(critic_loss)) / 2
 
-        # Take mean of actor_loss and critic_loss
-        actor_loss = tf.reduce_mean(actor_loss)
-        critic_loss = tf.reduce_mean(critic_loss)
+        return loss
 
-        return actor_loss, critic_loss
+    def ensure_float(self, tensor):
+        if tensor.dtype != tf.float32:
+            return tf.cast(tensor, tf.float32)
+        return tensor
 
     def update(self):
-        """
+        '''
         This function updates the network parameters using the optimizer and computed loss values.
-        """
 
-        if not self.states:  # Check if the states list is empty
-            return
+        update() function updates the network parameters using the optimizer and computed loss values.
+        It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
+
+        This function does not take any parameters and does not return anything.
+
+        :return: None
+        '''
 
-        # Prepare data
-        states_tensor = tf.stack(
-            [self.check_tensor(state) for state in self.states])
-        actions_tensor = tf.convert_to_tensor(self.actions, dtype=tf.float32)
-        rewards_tensor = tf.convert_to_tensor(self.rewards, dtype=tf.float32)
-        next_states_tensor = tf.stack(
-            [self.check_tensor(state) for state in self.next_states])
-        dones_tensor = tf.convert_to_tensor(self.dones, dtype=tf.float32)
+        # Convert state to tensor
+        state_tensor = self.check_tensor(self.state)
 
-        # Compute gradients and update network parameters
+        # Compute loss and update network parameters
         with tf.GradientTape() as tape:
-            # Compute loss
-            actor_loss, critic_loss = self.compute_loss(
-                states_tensor, actions_tensor, rewards_tensor, next_states_tensor, dones_tensor)
-            loss = actor_loss + critic_loss
+            loss = self.compute_loss(
+                state_tensor, self.action, self.reward, self.done)
+            Logger.verb('mcts:update',
+                        f"Loss: {loss.numpy()}, Reward: {self.reward}")
 
         # Calculate gradients
         gradients = tape.gradient(
             loss, self.actor_critic_net.trainable_variables)
 
         # Apply gradients
         self.actor_critic_optimizer.apply_gradients(
             zip(gradients, self.actor_critic_net.trainable_variables))
 
-        # Reset the lists for the next episode
         self.reset()
-        self.update_episode()
+
+    def check_tensor(self, obj):
+        '''
+        This function checks if the provided object is a TensorFlow tensor, and if not, converts it to a tensor.
+
+        check_tensor() function checks if the provided obj parameter is a TensorFlow tensor.
+        If it is not a tensor, it converts it to a tensor using tf.convert_to_tensor().
+        If it is already a tensor, it simply returns the tensor.
+
+        The obj parameter is the object to check/convert to a TensorFlow tensor.
+
+        The function returns the input object as a TensorFlow tensor.
+
+        :param obj: The object to check/convert to a TensorFlow tensor.
+        :return: The input object as a TensorFlow tensor.
+        '''
+
+        if not tf.is_tensor(obj):
+            obj_tensor = tf.convert_to_tensor(obj, dtype=tf.float32)
+        else:
+            obj_tensor = obj
+
+        Logger.verb('mcts:check_tensor', f"Before remapping: {obj_tensor}")
+        obj_tensor = obj_tensor % self.env.action_space.n
+        obj_tensor = tf.where(
+            obj_tensor >= self.env.action_space.n, self.env.action_space.n - 1, obj_tensor)
+        obj_tensor = self._check_state(tf.round(obj_tensor))
+        Logger.verb('mcts:check_tensor', f"After remapping: {obj_tensor}")
+        return obj_tensor
 
     def learn(self):
         """
         Train the agent.
         """
         self.train()
 
@@ -246,48 +247,44 @@
         self.total_reward = 0
         for episode in range(self.max_episodes):
             self.episode = episode
             state = self.learn_reset()
 
             for t in range(self.max_timesteps):
                 state = self._check_state(state)
-                Logger.verb('mcis:train', f'{state.shape}')
                 self.state_tensor = self.check_tensor(state).numpy()
+                self.state_tensor = tf.squeeze(self.state_tensor, axis=0)
+                self.next_state, self.action, self.reward, self.done = self.select_action(
+                    self.state_tensor)
 
-                # Select an action
-                action = self.select_action(self.state_tensor)
+                self.learn_check()
 
-                # Take a step in the environment
-                step_out = self.env.step(action)
-                next_state, reward, done = self.step_unpack(step_out)
-
-                # Update the agent's experience
-                self.update_step(state, action, reward, done, next_state)
-
-                # Update the network parameters at the end of the episode
-                if done:
-                    self.update()
-                    self.learn_check()
+                if self.done:
                     break
 
-                state = next_state
+                self.update()
 
-            self.episode += 1
+                state = self.next_state
 
-    def check_tensor(self, state):
-        '''
-        This function checks if the provided object is a TensorFlow tensor, and if not, converts it to a tensor.
+            self.episode += 1
+            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
 
-        :param state: The object to check/convert to a TensorFlow tensor.
-        :return: The input object as a TensorFlow tensor.
-        '''
-        Logger.verb('_agent:check_tensor', f'state={state}')
-        if not isinstance(state, tf.Tensor):
-            state = tf.convert_to_tensor(state, dtype=tf.float32)
-        return state
+    def update_step(self, state, action, reward, done, next_state):
+        """
+        In MCTS, update_step is not necessary as the agent is updated
+        after every simulation (or a batch of simulations), each of which
+        represents an entire episode. Thus, this method can be left blank or removed.
+        """
+        self.state = state
+        self.action = action
+        self.reward = reward
+        self.done = done
+        self.next_state = next_state
+        self.update_reward(reward)
+        self.update_episode()
 
     def save_model(self, file_name):
         """
         This function saves the model to the specified file.
 
         :param file_name: The name of the file to save the model to.
         :return: None
```

### Comparing `modular_rl-0.4.1/modular_rl/agents/tensorflow/mcts.py` & `modular_rl-0.4.2/modular_rl/agents/tensorflow/ppo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # -*- coding: utf-8 -*-
 """
 ModularRL project
 
 Copyright (c) 2023 horrible-gh
 
-Class AgentMCTS is an implementation of the Monte Carlo Tree Search (MCTS) algorithm.
+Class AgentPPO is an implementation of the Proximal Policy Optimization (PPO) algorithm.
 It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
 and sets various learning parameters.
 It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
 save and load a checkpoint, and reset learning parameters.
 The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
 
 This software includes the following third-party libraries:
@@ -19,301 +19,306 @@
 """
 
 import tensorflow as tf
 import tensorflow_probability as tfp
 import numpy as np
 from LogAssist.log import Logger
 from modular_rl.agents.tensorflow._agent import Agent
-from modular_rl.util.node import Node
 
 
-class TensorFlowAgentMCTS(Agent):
+class TensorFlowAgentPPO(Agent):
     def __init__(self, env, setting):
-        """
-        Initialize the AgentMCIS class with the specified environment and settings.
+        super(TensorFlowAgentPPO, self).__init__(env, setting)
+        super(TensorFlowAgentPPO, self).init_policy_value()
 
-        :param env: The environment to use for training.
-        :type env: gym.Env or None
-        :param setting: The settings for the MCIS algorithm.
-        :type setting: AgentSettings
-        """
-
-        super().__init__(env, setting)
-        super().init_actor_critic()
-
-        # mcis parameters
-        self.num_simulations = setting.get('num_simulations', 800)
-        self.cpuct = setting.get('cpuct', 1.0)
-        self.temperature = setting.get('temperature', 1.0)
-
-        self.device = setting.get('device', None)
-        if self.device == None:
-            # TensorFlow automatically uses the GPU if one is available, otherwise it uses the CPU.
-            # Therefore, there is no need to manually set the device as in PyTorch.
-            pass
+        # Set learning parameters
+        self.ppo_epochs = setting.get('ppo_epochs', 4)
+        self.mini_batch_size = setting.get('mini_batch_size', 64)
+        self.lam = setting.get('lam', 0.95)
+        self.clip_param = setting.get('clip_param', 0.2)
 
-    def reset(self):
+        # Set learn modular parameters
         self.state = None
-        self.action = None
-        self.reward = None
-        self.done = None
-        self.total_reward = 0
+        self.dist = None
 
-    def select_action(self, state):
-        """
-        Select an action using MCTS.
+        # Create optimizers
+        self.value_optimizer = tf.keras.optimizers.Adam()
 
-        :param state: The current state.
-        :type state: numpy.ndarray
-        :return: The selected action.
-        :rtype: int
-        """
-        state = self._check_state(state)
-        state_tensor = self.check_tensor(state)
-        action_probs, _ = self.actor_critic_net(state_tensor)
-        action_probs = tf.stop_gradient(action_probs)
-        m = tfp.distributions.Categorical(probs=action_probs)
-        chosen_action = m.sample().numpy().item()
-
-        # Use uniform prior for root node.
-        root = Node(state, [1 / self.env.action_space.n]
-                    * self.env.action_space.n)
-
-        for _ in range(self.num_simulations):
-            node, search_path = root, [root]
-
-            while node.expanded():
-                action, node = node.select_child(self.cpuct)
-                if action is None:
-                    action = chosen_action
-                search_path.append(node)
-
-            parent, action = (search_path[-2], search_path[-1].action) if len(
-                search_path) > 1 else (search_path[0], None)
-            step_output = self.env.step(action) if action is not None else (
-                parent.state, 0, False, None)
-            state, reward, done, *_ = step_output
-            Logger.verb('mcts:select_action', f"Step Output Reward: {reward}")
-
-            if not done:
-                state_tensor = self.check_tensor(state)
-                action_probs, _ = self.actor_critic_net(state_tensor)
-                node.expand(self.env.action_space.n,
-                            action_probs.numpy().flatten(), False)
-
-            self.backpropagate(search_path, reward, done)
-
-        chosen_action_node = root.children[chosen_action]
-
-        self.state = chosen_action_node.state
-        self.action = chosen_action
-        self.reward = chosen_action_node.total_value
-        self.done = self.reward != 0
-
-        self.total_reward += self.reward
-
-        return self.state, self.action, self.reward, self.done
-
-    def backpropagate(self, search_path, reward, done):
-        """
-        Backpropagate the value estimates back to the root node.
-
-        :param search_path: The nodes visited during the search.
-        :type search_path: list of Node
-        :param reward: The reward obtained after the search.
-        :type reward: float
-        :param done: Whether the episode has ended.
-        :type done: bool
-        """
-        for node in reversed(search_path):
-            # Logger.verb('mcts:backpropagate',
-            #            f"Node Reward({reward}) after Update Stats: {node.total_value}")
-            node.update_stats(reward)
+    def learn_reset(self):
+        return super(TensorFlowAgentPPO, self).learn_reset()
 
-    def compute_loss(self, state, action, reward, done):
-        '''
-        This function computes the actor and critic loss using the provided state, action, reward, and done variables.
-        The actor loss is computed based on the policy gradient algorithm,
-        and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
-
-        :param state: The current state of the environment.
-        :param action: The action taken in the current state.
-        :param reward: The reward received for taking the action in the current state.
-        :param done: A flag indicating whether the episode has ended.
-        :return: The computed actor and critic loss values.
-        '''
-        # Predict action probabilities and values
-        state = self.ensure_float(state)
-        action_probs, values = self.actor_critic_net(state)
-
-        # Convert reward to tensor
-        reward = tf.convert_to_tensor(reward, dtype=tf.float32)
-        # Compute the value loss
-        target_values = reward + self.gamma * self.total_value * (1 - done)
-        target_values = tf.expand_dims(target_values, axis=0)
-        critic_loss = tf.keras.losses.MSE(values, target_values)
-
-        # If action is not a list or tuple or its length is zero, initialize it with zeros
-        if not isinstance(action, (list, tuple)) or len(action) == 0:
-            action = tf.zeros_like(action_probs)
-
-        # Compute the policy loss
-        m = tfp.distributions.Categorical(probs=action_probs)
-        logprobs = m.log_prob(self.check_tensor(action))
-        actor_loss = -logprobs * (target_values - values)
-
-        # Average the actor and critic loss
-        loss = (tf.reduce_mean(actor_loss) + tf.reduce_mean(critic_loss)) / 2
-
-        return loss
-
-    def ensure_float(self, tensor):
-        if tensor.dtype != tf.float32:
-            return tf.cast(tensor, tf.float32)
-        return tensor
+    def reset(self):
+        super(TensorFlowAgentPPO, self).reset()
 
-    def update(self):
+    def check_tensor(self, state):
         '''
-        This function updates the network parameters using the optimizer and computed loss values.
-
-        update() function updates the network parameters using the optimizer and computed loss values.
-        It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
-
-        This function does not take any parameters and does not return anything.
+        This function checks if the provided object is a TensorFlow tensor, and if not, converts it to a tensor.
 
-        :return: None
+        :param state: The object to check/convert to a TensorFlow tensor.
+        :return: The input object as a TensorFlow tensor.
         '''
+        Logger.verb('_agent:check_tensor', f'state={state}')
+        if not isinstance(state[0], tf.Tensor):
+            state = (tf.convert_to_tensor(
+                state[0], dtype=tf.float32), state[1])
+        return state
+
+    def compute_advantages(self, rewards, values, dones, gamma=0.99, lam=0.95):
+        advantages = np.zeros_like(rewards)
+        last_advantage = 0
+        for t in reversed(range(len(rewards))):
+            delta = rewards[t] + gamma * \
+                values[t + 1] * (1 - dones[t]) - values[t]
+            advantages[t] = delta + gamma * lam * \
+                last_advantage * (1 - dones[t])
+            last_advantage = advantages[t]
+        return advantages
 
-        # Convert state to tensor
-        state_tensor = self.check_tensor(self.state)
+    def select_action(self, state):
+        state = self._check_state(self.state)
+        state_tensor = tf.convert_to_tensor(state, dtype=tf.float32)
+        action_probs = self.policy_net(state_tensor)
+        dist = tfp.distributions.Categorical(probs=action_probs)
+        self.dist = dist
+        action = dist.sample()
+        return action, dist
+
+    def learn_step(self, state, timestep):
+        action, dist = self.select_action(state)
+        return self.update_step(state, dist, action, timestep)
+
+    def update_step(self, state, dist, action, timestep, auto_step=True, is_done=False, reward=0, next_state=None):
+        if dist is None and self.dist:
+            dist = self.dist
+        if auto_step:
+            step_output = self.env.step(int(action.numpy()[0]))
+            next_state, reward, is_done = self.step_unpack(step_output)
+        else:
+            if next_state is None:
+                next_state = state
+        self.update_reward(reward)
+        state = self._check_state(state)
+        # Note: we use Python lists here, as TensorFlow has a better support for Pythonic operations
+        self.states.append(state)
+        self.actions.append(action)
+        self.rewards.append(reward)
+        self.next_states.append(next_state)
+        self.dones.append(is_done)
+        self.log_probs.append(dist.log_prob(action))
+        self.state = next_state
+        if timestep > 0:
+            timestep += 1
+        if self.update_timestep > 0 and timestep > 0 and (timestep % self.update_timestep == 0):
+            self.update()
+        return action, reward, is_done, timestep
 
-        # Compute loss and update network parameters
-        with tf.GradientTape() as tape:
-            loss = self.compute_loss(
-                state_tensor, self.action, self.reward, self.done)
-            Logger.verb('mcts:update',
-                        f"Loss: {loss.numpy()}, Reward: {self.reward}")
-
-        # Calculate gradients
-        gradients = tape.gradient(
-            loss, self.actor_critic_net.trainable_variables)
-
-        # Apply gradients
-        self.actor_critic_optimizer.apply_gradients(
-            zip(gradients, self.actor_critic_net.trainable_variables))
+    def update(self):
+        Logger.verb("Shape of self.next_states:",   len(self.next_states))
+        Logger.verb("Shape of self.states:",        len(self.states))
+        Logger.verb("Shape of self.actions:",       len(self.actions))
+        Logger.verb("Shape of self.rewards:",       len(self.rewards))
+        Logger.verb("Shape of self.dones:",         len(self.dones))
+
+        for i, log_prob in enumerate(self.log_probs):
+            Logger.verb(f"Shape of log_probs[{i}]:", tf.shape(log_prob))
+
+        # Ensure all tensors in self.next_states have the same shape
+        self.next_states = [tf.squeeze(state) if len(
+            state.shape) == 2 and state.shape[0] == 1 else state for state in self.next_states]
+
+        # Convert lists to tensors
+        states_tensor = tf.stack(self.states)
+        actions_tensor = tf.stack(self.actions)
+        rewards_tensor = tf.stack(self.rewards)
+        next_states_tensor = tf.stack(self.next_states)
+        done_tensor = tf.stack(self.dones)
+        log_probs_tensor = tf.stack(self.log_probs)
+
+        # Adjusting dtype after stacking
+        states_tensor = tf.cast(states_tensor, dtype=tf.float32)
+        actions_tensor = tf.cast(actions_tensor, dtype=tf.int32)
+        rewards_tensor = tf.cast(rewards_tensor, dtype=tf.float32)
+        next_states_tensor = tf.cast(next_states_tensor, dtype=tf.float32)
+        done_tensor = tf.cast(done_tensor, dtype=tf.float32)
 
-        self.reset()
+        values = self.value_net(states_tensor).numpy().squeeze(1)
+        next_values = self.value_net(next_states_tensor).numpy().squeeze(1)
 
-    def check_tensor(self, obj):
-        '''
-        This function checks if the provided object is a TensorFlow tensor, and if not, converts it to a tensor.
+        if len(next_states_tensor) > 0:
+            last_value = next_values[-1]
+        else:
+            last_value = 0
 
-        check_tensor() function checks if the provided obj parameter is a TensorFlow tensor.
-        If it is not a tensor, it converts it to a tensor using tf.convert_to_tensor().
-        If it is already a tensor, it simply returns the tensor.
+        advantages = self.compute_advantages(rewards_tensor.numpy(), np.append(
+            values, last_value), done_tensor.numpy(), self.gamma, self.lam)
+        advantages = (advantages - advantages.mean()) / \
+            (advantages.std() + 1e-5)
+        advantages_tensor = tf.convert_to_tensor(advantages, dtype=tf.float32)
 
-        The obj parameter is the object to check/convert to a TensorFlow tensor.
+        if len(advantages) > 1:
+            returns = np.add(advantages[:-1], values[:-1])
+        else:
+            returns = np.add(advantages, values)
 
-        The function returns the input object as a TensorFlow tensor.
+        self.ppo_update(self.ppo_epochs, self.mini_batch_size, states_tensor,
+                        actions_tensor, log_probs_tensor, returns, advantages_tensor)
 
-        :param obj: The object to check/convert to a TensorFlow tensor.
-        :return: The input object as a TensorFlow tensor.
-        '''
-
-        if not tf.is_tensor(obj):
-            obj_tensor = tf.convert_to_tensor(obj, dtype=tf.float32)
-        else:
-            obj_tensor = obj
+        self.reset()
+        self.update_episode()
 
-        Logger.verb('mcts:check_tensor', f"Before remapping: {obj_tensor}")
-        obj_tensor = obj_tensor % self.env.action_space.n
-        obj_tensor = tf.where(
-            obj_tensor >= self.env.action_space.n, self.env.action_space.n - 1, obj_tensor)
-        obj_tensor = self._check_state(tf.round(obj_tensor))
-        Logger.verb('mcts:check_tensor', f"After remapping: {obj_tensor}")
-        return obj_tensor
+    def ppo_update(self, ppo_epochs, mini_batch_size, states, actions, log_probs, returns, advantages, clip_param=0.2):
+        batch_size = states.shape[0]
+        returns = tf.convert_to_tensor(returns, dtype=tf.float32)
+        for _ in range(ppo_epochs):
+            for idx in range(batch_size // mini_batch_size):
+                # Extract mini-batch
+                minibatch_indices = tf.range(
+                    idx * mini_batch_size, (idx + 1) * mini_batch_size)
+                states_minibatch = tf.gather(states, minibatch_indices)
+                actions_minibatch = tf.gather(actions, minibatch_indices)
+                old_log_probs_minibatch = tf.gather(
+                    log_probs, minibatch_indices)
+                returns_minibatch = tf.gather(returns, minibatch_indices)
+                advantages_minibatch = tf.gather(advantages, minibatch_indices)
+
+                # Calculate policy loss
+                with tf.GradientTape() as tape:
+                    new_probs = self.policy_net(states_minibatch)
+                    new_dist = tfp.distributions.Categorical(probs=new_probs)
+                    new_log_probs = new_dist.log_prob(actions_minibatch)
+                    ratio = tf.exp(new_log_probs - old_log_probs_minibatch)
+                    surr1 = ratio * advantages_minibatch
+                    surr2 = tf.clip_by_value(
+                        ratio, 1.0 - clip_param, 1.0 + clip_param) * advantages_minibatch
+                    policy_loss = -tf.reduce_mean(tf.minimum(surr1, surr2))
+
+                # Calculate gradients
+                policy_gradients = tape.gradient(
+                    policy_loss, self.policy_net.trainable_variables)
+                # Apply gradients
+                self.policy_optimizer.apply_gradients(
+                    zip(policy_gradients, self.policy_net.trainable_variables))
+
+                # Calculate value loss
+                with tf.GradientTape() as tape:
+                    current_value_estimate = self.value_net(states_minibatch)
+                    value_loss = tf.reduce_mean(
+                        (returns_minibatch - current_value_estimate) ** 2)
+
+                # Calculate gradients
+                value_gradients = tape.gradient(
+                    value_loss, self.value_net.trainable_variables)
+                # Apply gradients
+                self.value_optimizer.apply_gradients(
+                    zip(value_gradients, self.value_net.trainable_variables))
 
-    def learn(self):
+    def train(self):
         """
-        Train the agent.
+        Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
         """
-        self.train()
+        self.learn()
 
-    def train(self):
+    def learn(self):
         """
-        Train the agent.
+        Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
         """
+
+        timestep = 0
+        test = 0
         self.total_reward = 0
-        for episode in range(self.max_episodes):
-            self.episode = episode
-            state = self.learn_reset()
-
-            for t in range(self.max_timesteps):
-                state = self._check_state(state)
-                self.state_tensor = self.check_tensor(state).numpy()
-                self.state_tensor = tf.squeeze(self.state_tensor, axis=0)
-                self.next_state, self.action, self.reward, self.done = self.select_action(
-                    self.state_tensor)
+
+        if self.max_episodes > 0 and self.max_timesteps > 0:
+            is_done = False
+            for episode in range(self.max_episodes):
+                self.episode = episode
+                self.reset()
+                self.learn_reset()
+                self.episode_reward = 0
+                reward = 0
+
+                for t in range(self.max_timesteps):
+                    state_tensor = self.check_tensor(self.state)
+                    action, reward, is_done, timestep = self.learn_step(
+                        state_tensor, timestep)
+                    if is_done:
+                        break
 
                 self.learn_check()
+                avg_reward = self.total_reward / (self.episode + 1)
+
+                if avg_reward >= self.early_stop_threshold > 0:
+                    Logger.info(
+                        f'Early stopping: Average reward has reached the threshold ({self.early_stop_threshold}) at episode {self.episode}')
+                    break
+                if is_done and self.done_loop_end:
+                    break
 
-                if self.done:
+                if self.episode + 1 >= self.max_episodes:
                     break
 
-                self.update()
+            self.env.close()
+        else:
+            self.reset()
 
-                state = self.next_state
+    def learn_next(self):
+        """
+        Perform a single learning step and update the episode and total rewards.
 
-            self.episode += 1
-            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
+        :return: The action taken, the resulting reward, and whether the episode is done or not.
+        :rtype: tuple(torch.Tensor, float, bool)
+        """
 
-    def update_step(self, state, action, reward, done, next_state):
+        action, reward, is_done, timestep = self.learn_step(self.state, -1)
+
+        return action, reward, is_done, timestep
+
+    def learn_close(self):
         """
-        In MCTS, update_step is not necessary as the agent is updated
-        after every simulation (or a batch of simulations), each of which
-        represents an entire episode. Thus, this method can be left blank or removed.
+        Close the environment and reset the agent's total reward, episode count, and episode reward.
         """
-        self.state = state
-        self.action = action
-        self.reward = reward
-        self.done = done
-        self.next_state = next_state
-        self.update_reward(reward)
-        self.update_episode()
+
+        super().learn_close()
+
+    def learn_check(self):
+        """
+        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
+        """
+
+        super().learn_check()
 
     def save_model(self, file_name):
         """
         This function saves the model to the specified file.
 
         :param file_name: The name of the file to save the model to.
         :return: None
         """
         self.save(file_name)
 
     def save(self, file_name):
         """
-        This function saves the actor critic network to the specified file.
+        This function saves the policy and value networks to the specified file.
 
-        :param file_name: The name of the file to save the actor critic network to.
+        :param file_name: The name of the file to save the policy and value networks to.
         :return: None
         """
 
-        self.save_actor_critic(file_name)
+        self.save_policy_value(file_name)
 
     def load_model(self, file_name):
         """
         This function loads the model from the specified file.
 
         :param file_name: The name of the file to load the model from.
         :return: None
         """
         self.load(file_name)
 
     def load(self, file_name):
         """
-        This function loads the actor critic network from the specified file.
+        This function loads the policy and value networks from the specified file.
 
-        :param file_name: The name of the file to load the actor critic network from.
+        :param file_name: The name of the file to load the policy and value networks from.
         :return: None
         """
 
-        self.load_actor_critic(file_name)
+        self.load_policy_value(file_name)
```

### Comparing `modular_rl-0.4.1/modular_rl/envs/mim/card_evaluator.py` & `modular_rl-0.4.2/modular_rl/envs/mim/card_evaluator.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/networks/pytorch/actor_critic.py` & `modular_rl-0.4.2/modular_rl/networks/pytorch/actor_critic.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/networks/pytorch/policy.py` & `modular_rl-0.4.2/modular_rl/networks/pytorch/policy.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/networks/pytorch/value.py` & `modular_rl-0.4.2/modular_rl/networks/pytorch/value.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/networks/tensorflow/actor_critic.py` & `modular_rl-0.4.2/modular_rl/networks/tensorflow/actor_critic.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/networks/tensorflow/policy.py` & `modular_rl-0.4.2/modular_rl/networks/tensorflow/policy.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/networks/tensorflow/value.py` & `modular_rl-0.4.2/modular_rl/networks/tensorflow/value.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/params/mcis.py` & `modular_rl-0.4.2/modular_rl/params/mcis.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/params/mcts.py` & `modular_rl-0.4.2/modular_rl/params/mcts.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/params/ppo.py` & `modular_rl-0.4.2/modular_rl/params/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl/settings.py` & `modular_rl-0.4.2/modular_rl/settings.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-'''
-The AgentSettings class is a configuration class used for setting up various reinforcement learning agents.
-
-It provides default values for various parameters used in the agents, such as the maximum number of episodes,
-maximum number of timesteps per episode, update timestep, network architecture, learning rate,
-discount factor, early stopping threshold, and whether to end training when the environment is done.
-
-The class currently supports PPO and MCTS algorithms, but it can be extended to include other algorithms in the future.
-The default dictionary provides default values for all parameters, while the modular version provides default values
-with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
-key-value pairs to the AgentSettings constructor.
-
-'''
-
-from modular_rl.params.ppo import ParamPPO
-from modular_rl.params.mcts import ParamMCTS
-from modular_rl.params.mcis import ParamMCIS
-from modular_rl.params.mim import ParamMIM
-
-
-class AgentSettings:
-    default_ppo = ParamPPO.default
-    default_ppo_modular = ParamPPO.default_modular
-    default_mcts = ParamMCTS.default
-    default_mcts_modular = ParamMCTS.default_modular
-    default_mcis = ParamMCIS.default
-    default_mcis_modular = ParamMCIS.default_modular
-    default_mim = ParamMIM.default
-    default_mim_modular = ParamMIM.default_modular
+'''
+The AgentSettings class is a configuration class used for setting up various reinforcement learning agents.
+
+It provides default values for various parameters used in the agents, such as the maximum number of episodes,
+maximum number of timesteps per episode, update timestep, network architecture, learning rate,
+discount factor, early stopping threshold, and whether to end training when the environment is done.
+
+The class currently supports PPO and MCTS algorithms, but it can be extended to include other algorithms in the future.
+The default dictionary provides default values for all parameters, while the modular version provides default values
+with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
+key-value pairs to the AgentSettings constructor.
+
+'''
+
+from modular_rl.params.ppo import ParamPPO
+from modular_rl.params.mcts import ParamMCTS
+from modular_rl.params.mcis import ParamMCIS
+from modular_rl.params.mim import ParamMIM
+
+
+class AgentSettings:
+    default_ppo = ParamPPO.default
+    default_ppo_modular = ParamPPO.default_modular
+    default_mcts = ParamMCTS.default
+    default_mcts_modular = ParamMCTS.default_modular
+    default_mcis = ParamMCIS.default
+    default_mcis_modular = ParamMCIS.default_modular
+    default_mim = ParamMIM.default
+    default_mim_modular = ParamMIM.default_modular
```

### Comparing `modular_rl-0.4.1/modular_rl/util/node.py` & `modular_rl-0.4.2/modular_rl/util/node.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/modular_rl.egg-info/SOURCES.txt` & `modular_rl-0.4.2/modular_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modular_rl-0.4.1/pyproject.toml` & `modular_rl-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.4.1/setup.py` & `modular_rl-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.4.1',
+    version='0.4.2',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/ModularRL',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

