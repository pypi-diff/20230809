# Comparing `tmp/swarms-1.1.4.tar.gz` & `tmp/swarms-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-1.1.4.tar", last modified: Thu Aug  3 18:31:46 2023, max compression
+gzip compressed data, was "swarms-1.1.5.tar", last modified: Tue Aug  8 18:12:22 2023, max compression
```

## Comparing `swarms-1.1.4.tar` & `swarms-1.1.5.tar`

### file list

```diff
@@ -1,174 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 18:31:34.000000 swarms-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 18:31:46.296811 swarms-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-08-03 18:31:34.000000 swarms-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-03 18:31:34.000000 swarms-1.1.4/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 18:31:46.296811 swarms-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-03 18:31:34.000000 swarms-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/swarms/agents/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory/ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.280810 swarms-1.1.4/swarms/agents/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/models/petals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.280810 swarms-1.1.4/swarms/agents/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/agent_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/agent_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/agent_prompt_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.280810 swarms-1.1.4/swarms/agents/prompts/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/chains/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/chat_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/prompt_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.280810 swarms-1.1.4/swarms/agents/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/autogpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/code_intepretor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/developer.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/exit_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/file_mangagement.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/tools/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/Calback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/ChatOpenAI.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/ConversationalChatAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/agent_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/agent_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/agents/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/human_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/agents/utils/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/boss/boss_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/orchestrator/orchestrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/swarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/swarms/hivemind.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/utils/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/embeddings/pegasus.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.284811 swarms-1.1.4/swarms/utils/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/utils/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/character_generative.py
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/generative_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.288811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.292811 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.292811 swarms-1.1.4/swarms/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.292811 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/models/segment_anything/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/swarms/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.296811 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/worker_agent_ultra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/worker_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-03 18:31:34.000000 swarms-1.1.4/swarms/workers/worker_ultra_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:31:46.276810 swarms-1.1.4/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 18:31:46.000000 swarms-1.1.4/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.427535 swarms-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 18:12:09.000000 swarms-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-08 18:12:22.427535 swarms-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-08-08 18:12:09.000000 swarms-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.403533 swarms-1.1.5/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-08 18:12:09.000000 swarms-1.1.5/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:12:22.427535 swarms-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-08 18:12:09.000000 swarms-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.403533 swarms-1.1.5/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.403533 swarms-1.1.5/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.403533 swarms-1.1.5/swarms/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory/base_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory/chat_message_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.407534 swarms-1.1.5/swarms/agents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/petals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.407534 swarms-1.1.5/swarms/agents/models/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/agent_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/agent_prompt_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.407534 swarms-1.1.5/swarms/agents/models/prompts/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/chains/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/chat_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/prompt_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/sales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/models/prompts/summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.411534 swarms-1.1.5/swarms/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/autogpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/code_intepretor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/developer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/exit_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/file_mangagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/tools/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.411534 swarms-1.1.5/swarms/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/Calback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/ChatOpenAI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/ConversationalChatAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/agent_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/agent_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.411534 swarms-1.1.5/swarms/agents/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/human_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/agents/utils/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.411534 swarms-1.1.5/swarms/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/boss/boss_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.411534 swarms-1.1.5/swarms/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/orchestrator/orchestrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.411534 swarms-1.1.5/swarms/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/swarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/swarms/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.415534 swarms-1.1.5/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.415534 swarms-1.1.5/swarms/utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/embeddings/pegasus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.415534 swarms-1.1.5/swarms/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/utils/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.415534 swarms-1.1.5/swarms/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/character_generative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/generative_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.415534 swarms-1.1.5/swarms/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.415534 swarms-1.1.5/swarms/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.415534 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.415534 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.419534 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.419534 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.419534 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.419534 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.423534 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.423534 swarms-1.1.5/swarms/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:09.000000 swarms-1.1.5/swarms/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.423534 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.423534 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.427535 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/models/segment_anything/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/multi_modal_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.427535 swarms-1.1.5/swarms/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.427535 swarms-1.1.5/swarms/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/omni_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/worker_agent_ultra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/worker_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-08 18:12:10.000000 swarms-1.1.5/swarms/workers/worker_ultra_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:12:22.403533 swarms-1.1.5/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-08 18:12:22.000000 swarms-1.1.5/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-08-08 18:12:22.000000 swarms-1.1.5/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:12:22.000000 swarms-1.1.5/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-08 18:12:22.000000 swarms-1.1.5/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 18:12:22.000000 swarms-1.1.5/swarms.egg-info/top_level.txt
```

### Comparing `swarms-1.1.4/LICENSE` & `swarms-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/PKG-INFO` & `swarms-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.1.4
+Version: 1.1.5
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.1.4/README.md` & `swarms-1.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,62 @@
-<div align="center">
+<!-- # Swarms 🤖 🤖 🤖 -->
 
+![Swarming banner icon](images/swarmsbanner2.png)
 
-# Swarms of Autonomous AI Agents  🤖 🤖 🤖
 
-<!-- ![Swarming banner icon](images/swarmsbannernew.png) -->
+<div align="center">
 
 Introducing Swarms, automating all digital activities with multi-agent collaboration, get started in 30 seconds in a seamless onboarding experience.
 
-</div>
 
----
-<!-- 
-![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023) -->
 
 
-[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)
-[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)
 
+[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)
 
-<div align="center">
-
-
-
-<p>
+<!-- <p>
 <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/kyegomez/swarms" />
 <img alt="GitHub Last Commit" src="https://img.shields.io/github/last-commit/kyegomez/swarms" />
 <img alt="" src="https://img.shields.io/github/repo-size/kyegomez/swarms" />
 <img alt="GitHub Issues" src="https://img.shields.io/github/issues/kyegomez/swarms" />
 <img alt="GitHub Pull Requests" src="https://img.shields.io/github/issues-pr/kyegomez/swarms" />
 <br />
-</div>
+</div> -->
 
 
 
-<div align="center">
 
 ### Share on Social Media
 
 [![Open Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dopen)](https://console.algora.io/org/kyegomez/bounties?status=open)
 [![Rewarded Bounties](https://img.shields.io/endpoint?url=https%3A%2F%2Fconsole.algora.io%2Fapi%2Fshields%2Fkyegomez%2Fbounties%3Fstatus%3Dcompleted)](https://console.algora.io/org/kyegomez/bounties?status=completed)
 
 [![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
 
 [![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 </div>
 
----
 
-## Purpose
-At Swarms, we're transforming the landscape of AI from siloed AI agents to a unified 'swarm' of intelligence. Through relentless iteration and the power of collective insight from our 1500+ Agora researchers, we're developing a groundbreaking framework for AI collaboration. Our mission is to catalyze a paradigm shift, advancing Humanity with the power of unified autonomous AI agent swarms.
 
 
----
+## Purpose
+At Swarms, we're transforming the landscape of AI from siloed AI agents to a unified 'swarm' of intelligence. Through relentless iteration and the power of collective insight from our 1500+ Agora researchers, we're developing a groundbreaking framework for AI collaboration. Our mission is to catalyze a paradigm shift, advancing Humanity with the power of unified autonomous AI agent swarms.
 
-## Table of Contents
-1. [Introduction](#introduction)
-2. [Vision](#purpose)
-3. [Installation](#installation)
-4. [Share on Social Media](#share-on-social-media)
-5. [Other Platforms](#other-platforms)
-6. [Contribute](#contribute)
-7. [Roadmap](#roadmap)
-8. [Bounty Program](#bounty-program)
-9. [EcoSystem](#ecosystem)
-10. [Demos](#demos)
+-----
+## Hiring
+We're hiring: Engineers, Researchers, Interns And, salesprofessionals to work on democratizing swarms, email me at with your story at `kye@apac.ai`
 
----
+----------
 
 ## Installation
 
 There are 2 methods, one is through `git clone` and the other is by `pip install swarms`. Check out the [DOCUMENTATION](DOCS/DOCUMENTATION.md) for more information on the classes.
 
-# Method1
+# Method 1
 * Pip install `python3 -m pip install swarms`
 
 * Create new python file and unleash superintelligence
 
 ```python
 
 from swarms import swarm
@@ -98,14 +78,23 @@
 * `python3 -m pip install -r requirements.txt`
 
 * `python3 example.py`
 
 * or create a new file:
 
 ```python
+from swarms import OpenAI
+
+chat = OpenAI()
+response = chat("Hello world!")
+
+```
+
+
+```python
 from swarms.swarms import HierarchicalSwarm
 
 # Retrieve your API key from the environment or replace with your actual key
 api_key = "sksdsds"
 
 # Initialize Swarms with your API key
 swarm = HierarchicalSwarm(openai_api_key=api_key)
@@ -138,49 +127,25 @@
 objective = "Please make a web GUI for using HTTP API server..."
 
 # Run the task
 task = node.run(objective)
 
 print(task)
 ```
+---
 
-# Various agents
-
-Here are some agents in the swarm you can use!
-
-| Agent        | Import Statement                                   | Example Usage                                           |
-|--------------|----------------------------------------------------|---------------------------------------------------------|
-| WorkerNode   | `from swarms import worker_node`                   | ```python api_key = "sksdsds" node = worker_node(api_key) objective = "Please make a web GUI for using HTTP API server..." task = node.run(objective) print(task)``` |
-| Swarms       | `from swarms.swarms import Swarms`                 | ```python import os from swarms.swarms import Swarms api_key = os.getenv("OPENAI_API_KEY") swarm = Swarms(openai_api_key=api_key) objective = "Please make a web GUI for using HTTP API server..." task = swarm.run(objective) print(task)``` |
-
-## Hierarhical Swarm
-
-```python
-from swarms import HierarchicalSwarm
-
-swarm = HierarchicalSwarm(
-    openai_api_key="your_openai_api_key", 
-    use_vectorstore=True, 
-    embedding_size=768, 
-    use_async=True, 
-    worker_name="My Custom Worker", 
-    human_in_the_loop=True, 
-    boss_prompt="You are a custom boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n ", 
-    worker_prompt="You are a custom worker in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n ", 
-    temperature=0.5, 
-    max_iterations=5, 
-    logging_enabled=True
-)
-result = swarm.run("your_objective")
+# Documentation
+For documentation, go here, [the docs folder in the root diectory](docs)
 
-```
----
+**NOTE: We need help building the documentation**
 
+-----
 
 # Docker Setup
+The docker file is located in the docker folder in the `infra` folder, [click here and navigate here in your environment](/infra/Docker)
 
 * Build the Docker image
 
 * You can build the Docker image using the provided Dockerfile. Navigate to the infra/Docker directory where the Dockerfiles are located.
 
 * For the CPU version, use:
 
@@ -215,21 +180,29 @@
 
 ```bash
 curl -X POST -H "Content-Type: application/json" -d '{"api_key": "your_openai_api_key", "objective": "your_objective"}' http://localhost:8000/chat
 ```
 Replace your_openai_api_key and your_objective with your actual OpenAI API key and objective.
 
 
-## Share with your Friends
 
-[![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
+# ✨ Features
+* Easy to use Base LLMs, `OpenAI` `Palm` `Anthropic` `HuggingFace`
+* Enterprise Grade, Production Ready with robust Error Handling
+* Multi-Modality Native with Multi-Modal LLMs as tools
+* Infinite Memory Processing: Store infinite sequences of infinite Multi-Modal data, text, images, videos, audio
+* Usability: Extreme emphasis on useability, code is at it's theortical minimum simplicity factor to use
+* Reliability: Outputs that accomplish tasks and activities you wish to execute.
+* Fluidity: A seamless all-around experience to build production grade workflows
+* Speed: Lower the time to automate tasks by 90%. 
+* Simplicity: Swarms is extremely simple to use, if not thee simplest agent framework of all time
+* Powerful: Swarms is capable of building entire software apps, to large scale data analysis, and handling chaotic situations
 
 
-[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
----
+-----
 
 ## Contribute
 We're always looking for contributors to help us improve and expand this project. If you're interested, please check out our [Contributing Guidelines](DOCS/C0NTRIBUTING.md).
 
 Thank you for being a part of our project!
 
 ---
```

### Comparing `swarms-1.1.4/api/app.py` & `swarms-1.1.5/api/app.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/setup.py` & `swarms-1.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 ##
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '1.1.4',
+  version = '1.1.5',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -25,80 +25,69 @@
         'torchvision',
         'torchaudio',
         'asyncio',
         'nest_asyncio',
         'bs4',
         'pegasusx',
         'oceandb',
-        'codeinterpreterapi[all]',
+        'codeinterpreterapi',
         'playwright',
         'duckduckgo_search',
         'faiss-cpu',
         'wget==3.2',
         'accelerate',
-        'sphinx_rtd_theme',
         'addict',
         'albumentations',
         'basicsr',
         'controlnet-aux',
         'diffusers',
         'einops',
-        'gradio',
         'imageio',
+        'simpleaichat',
         'imageio-ffmpeg',
         'kornia',
         'numpy',
         'omegaconf',
         'open_clip_torch',
         'opencv-python',
         'prettytable',
         'safetensors',
         'streamlit',
         'test-tube',
         'timm',
         'torchmetrics',
         'webdataset',
         'yapf',
-        'wolframalpha',
         'wikipedia==1.4.0',
         'httpx',
         'ggl',
         'gradio_tools',
-        'arxiv',
-        'google-api-python-client',
-        'google-auth-httplib2',
         'beautifulsoup4==4.11.2',
-        'O365',
-        'pytube',
-        'pydub',
         'llama-index',
         'fastapi==0.94.1',
         'pydantic==1.10.6',
         'tenacity==8.2.2',
         'python-dotenv',
         'boto3',
         'uvicorn==0.21.1',
         'jinja2==3.1.2',
         'python-multipart==0.0.6',
         'celery==5.3.1',
         'redis==4.6.0',
         'sentencepiece',
-        'bitsandbytes==0.41.0',
         'psycopg2-binary==2.9.5',
         'google-search-results==2.4.2',
         'black==23.7.0',
         'Pillow',
         'selenium',
         'diffusers',
         'controlnet_aux',
         'tiktoken',
         'espnet==202301',
         'espnet_model_zoo==0.1.7',
-        'flask==2.2.3',
-        'flask_cors==3.0.10',
         'waitress==2.1.2',
         'asteroid',
         'speechbrain',
         'timm',
         'typeguard',
         'pytesseract',
         'huggingface_hub',
```

### Comparing `swarms-1.1.4/swarms/agents/__init__.py` & `swarms-1.1.5/swarms/agents/tools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-"""Agent Infrastructure, models, memory, utils, tools"""
-
-
-#models
-
-
-
-#tools
 from swarms.agents.tools.base import BaseTool, Tool, StructuredTool, ToolWrapper, BaseToolSet, ToolCreator, GlobalToolsCreator, SessionToolsCreator, ToolsFactory
 from swarms.agents.tools.autogpt import pushd, process_csv, async_load_playwright, run_async, browse_web_page, WebpageQATool, web_search, query_website_tool
 from swarms.agents.tools.exit_conversation import ExitConversation
 
 from swarms.agents.tools.models import MaskFormer, ImageEditing, InstructPix2Pix, Text2Image, VisualQuestionAnswering, ImageCaptioning
 from swarms.agents.tools.file_mangagement import read_tool, write_tool, list_tool
 from swarms.agents.tools.requests import RequestsGet
```

### Comparing `swarms-1.1.4/swarms/agents/base.py` & `swarms-1.1.5/swarms/agents/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 from langchain.chains.llm import LLMChain
-from langchain.memory import ChatMessageHistory
-from langchain.schema import BaseChatMessageHistory, Document
-from langchain.vectorstores.base import VectorStoreRetriever
 from pydantic import ValidationError
 
+from swarms.agents.memory.base import VectorStoreRetriever
+from swarms.agents.memory.base_memory import BaseChatMessageHistory
+from swarms.agents.memory.chat_message_history import ChatMessageHistory
+from swarms.agents.memory.document import Document
 from swarms.agents.models.base import AbstractModel
-from swarms.agents.prompts.agent_output_parser import AgentOutputParser
-from swarms.agents.prompts.agent_prompt import AIMessage, HumanMessage, SystemMessage
-from swarms.agents.prompts.agent_prompt_auto import MessageFormatter, PromptConstructor
-from swarms.agents.prompts.prompt_generator import FINISH_NAME
+from swarms.agents.models.prompts.agent_output_parser import AgentOutputParser
+from swarms.agents.models.prompts.agent_prompt import (
+    AIMessage,
+    HumanMessage,
+    SystemMessage,
+)
+from swarms.agents.models.prompts.agent_prompt_auto import (
+    MessageFormatter,
+    PromptConstructor,
+)
+from swarms.agents.models.prompts.prompt_generator import FINISH_NAME
 from swarms.agents.tools.base import BaseTool
 from swarms.agents.utils.Agent import AgentOutputParser
 from swarms.agents.utils.human_input import HumanInputRun
 
 
 class Agent:
     """Base Agent class"""
```

### Comparing `swarms-1.1.4/swarms/agents/memory/base.py` & `swarms-1.1.5/swarms/agents/memory/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,20 @@
     TypeVar,
 )
 
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForRetrieverRun,
     CallbackManagerForRetrieverRun,
 )
-from langchain.docstore.document import Document
-from langchain.embeddings.base import Embeddings
+
+from swarms.agents.memory.document import Document
+from swarms.utils.embeddings.base import Embeddings
+
 from langchain.schema import BaseRetriever
+
 from pydantic import Field, root_validator
 
 VST = TypeVar("VST", bound="VectorStore")
 
 
 class VectorStore(ABC):
     """Interface for vector stores."""
```

### Comparing `swarms-1.1.4/swarms/agents/memory/chroma.py` & `swarms-1.1.5/swarms/agents/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/memory/ocean.py` & `swarms-1.1.5/swarms/agents/memory/ocean.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/memory.py` & `swarms-1.1.5/swarms/agents/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Any, Dict, List
 from pydantic import Field
 
-from langchain.memory.chat_memory import BaseChatMemory, get_prompt_input_key
-from langchain.vectorstores.base import VectorStoreRetriever
+from swarms.agents.memory.base_memory import BaseChatMemory, get_prompt_input_key
+from swarms.agents.memory.base import VectorStoreRetriever
 
-
-
-class AutoGPTMemory(BaseChatMemory):
+class AgentMemory(BaseChatMemory):
     retriever: VectorStoreRetriever = Field(exclude=True)
     """VectorStoreRetriever object to connect to."""
 
     @property
     def memory_variables(self) -> List[str]:
         return ["chat_history", "relevant_context"]
```

### Comparing `swarms-1.1.4/swarms/agents/models/anthropic.py` & `swarms-1.1.5/swarms/agents/models/anthropic.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,8 +36,21 @@
         headers = {"Authorization": f"Bearer {self.anthropic_api_key}"}
         data = {
             "prompt": prompt,
             "stop_sequences": stop,
             **params
         }
         response = requests.post(f"{self.anthropic_api_url}/completions", headers=headers, json=data, timeout=self.default_request_timeout)
+        return response.json().get("completion")
+    
+    def __call__(self, prompt, stop=None):
+        """Call out to Anthropic's completion endpoint."""
+        stop = stop or []
+        params = self._default_params()
+        headers = {"Authorization": f"Bearer {self.anthropic_api_key}"}
+        data = {
+            "prompt": prompt,
+            "stop_sequences": stop,
+            **params
+        }
+        response = requests.post(f"{self.anthropic_api_url}/completions", headers=headers, json=data, timeout=self.default_request_timeout)
         return response.json().get("completion")
```

### Comparing `swarms-1.1.4/swarms/agents/models/huggingface.py` & `swarms-1.1.5/swarms/agents/models/huggingface.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,14 +23,27 @@
         try:
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_id)
             self.model = AutoModelForCausalLM.from_pretrained(self.model_id, quantization_config=bnb_config)
             self.model.to(self.device)
         except Exception as e:
             self.logger.error(f"Failed to load the model or the tokenizer: {e}")
             raise
+
+    def __call__(self, prompt_text: str, max_length: int = None):
+        max_length = max_length if max_length else self.max_length
+        try:
+            inputs = self.tokenizer.encode(prompt_text, return_tensors="pt").to(self.device)
+            with torch.no_grad():
+                outputs = self.model.generate(inputs, max_length=max_length, do_sample=True)
+            return self.tokenizer.decode(outputs[0], skip_special_tokens=True)
+        except Exception as e:
+            self.logger.error(f"Failed to generate the text: {e}")
+            raise
+
+
     def generate(self, prompt_text: str, max_length: int = None):
         max_length = max_length if max_length else self.max_length
         try:
             inputs = self.tokenizer.encode(prompt_text, return_tensors="pt").to(self.device)
             with torch.no_grad():
                 outputs = self.model.generate(inputs, max_length=max_length, do_sample=True)
             return self.tokenizer.decode(outputs[0], skip_special_tokens=True)
```

### Comparing `swarms-1.1.4/swarms/agents/models/palm.py` & `swarms-1.1.5/swarms/agents/models/palm.py`

 * *Files 15% similar despite different names*

```diff
@@ -108,14 +108,34 @@
         retry_decorator = _create_retry_decorator()
 
         @retry_decorator
         async def _achat_with_retry(**kwargs: Any) -> Any:
             return await self.client.chat_async(**kwargs)
 
         return await _achat_with_retry(**kwargs)
+    
+    def __call__(
+        self,
+        messages: List[Dict[str, Any]],
+        stop: Optional[List[str]] = None,
+        **kwargs: Any,
+    ) -> Dict[str, Any]:
+        prompt = _messages_to_prompt_dict(messages)
+
+        response: genai.types.ChatResponse = self.chat_with_retry(
+            model=self.model_name,
+            prompt=prompt,
+            temperature=self.temperature,
+            top_p=self.top_p,
+            top_k=self.top_k,
+            candidate_count=self.n,
+            **kwargs,
+        )
+
+        return _response_to_result(response, stop)
 
     def generate(
         self,
         messages: List[Dict[str, Any]],
         stop: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> Dict[str, Any]:
```

### Comparing `swarms-1.1.4/swarms/agents/models/petals.py` & `swarms-1.1.5/swarms/agents/models/petals.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/prompts/agent_output_parser.py` & `swarms-1.1.5/swarms/agents/models/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/prompts/agent_prompt.py` & `swarms-1.1.5/swarms/agents/models/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/prompts/agent_prompt_auto.py` & `swarms-1.1.5/swarms/agents/models/prompts/agent_prompt_auto.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/prompts/chains/llm.py` & `swarms-1.1.5/swarms/agents/models/prompts/chains/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/prompts/chat_prompt.py` & `swarms-1.1.5/swarms/agents/models/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/prompts/prompt_generator.py` & `swarms-1.1.5/swarms/agents/models/prompts/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/prompts/prompts.py` & `swarms-1.1.5/swarms/agents/models/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/tools/__init__.py` & `swarms-1.1.5/swarms/agents/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,21 @@
+"""Agent Infrastructure, models, memory, utils, tools"""
+
+
+#models
+from swarms.agents.models.anthropic import Anthropic
+from swarms.agents.models.huggingface import HuggingFaceLLM
+from swarms.agents.models.palm import GooglePalm
+from swarms.agents.models.petals import Petals
+from swarms.agents.models.openai import OpenAI
+
+###########
+#tools
 from swarms.agents.tools.base import BaseTool, Tool, StructuredTool, ToolWrapper, BaseToolSet, ToolCreator, GlobalToolsCreator, SessionToolsCreator, ToolsFactory
 from swarms.agents.tools.autogpt import pushd, process_csv, async_load_playwright, run_async, browse_web_page, WebpageQATool, web_search, query_website_tool
 from swarms.agents.tools.exit_conversation import ExitConversation
 
 from swarms.agents.tools.models import MaskFormer, ImageEditing, InstructPix2Pix, Text2Image, VisualQuestionAnswering, ImageCaptioning
 from swarms.agents.tools.file_mangagement import read_tool, write_tool, list_tool
 from swarms.agents.tools.requests import RequestsGet
 
-from swarms.agents.tools.developer import Terminal, CodeEditor
+from swarms.agents.tools.developer import Terminal, CodeEditor
```

### Comparing `swarms-1.1.4/swarms/agents/tools/autogpt.py` & `swarms-1.1.5/swarms/agents/tools/autogpt.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/tools/base.py` & `swarms-1.1.5/swarms/agents/tools/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/tools/code_intepretor.py` & `swarms-1.1.5/swarms/agents/tools/code_intepretor.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/tools/developer.py` & `swarms-1.1.5/swarms/agents/tools/developer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/tools/exit_conversation.py` & `swarms-1.1.5/swarms/agents/tools/exit_conversation.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/tools/file_mangagement.py` & `swarms-1.1.5/swarms/agents/tools/file_mangagement.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/tools/models.py` & `swarms-1.1.5/swarms/agents/tools/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     BlipForConditionalGeneration,
     BlipForQuestionAnswering,
     BlipProcessor,
     CLIPSegForImageSegmentation,
     CLIPSegProcessor,
 )
 
-from swarms.agents.prompts.prompts import IMAGE_PROMPT
+from swarms.agents.models.prompts.prompts import IMAGE_PROMPT
 from swarms.agents.tools.base import tool
 from swarms.agents.tools.main import BaseToolSet
 from swarms.utils.logger import logger
 from swarms.utils.main import BaseHandler, get_new_image_name
 
 
 class MaskFormer(BaseToolSet):
```

### Comparing `swarms-1.1.4/swarms/agents/tools/requests.py` & `swarms-1.1.5/swarms/agents/tools/requests.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/utils/Agent.py` & `swarms-1.1.5/swarms/agents/utils/Agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/utils/Calback.py` & `swarms-1.1.5/swarms/agents/utils/Calback.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/utils/ChatOpenAI.py` & `swarms-1.1.5/swarms/agents/utils/ChatOpenAI.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/utils/ConversationalChatAgent.py` & `swarms-1.1.5/swarms/agents/utils/ConversationalChatAgent.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     AIMessage,
     BaseMessage,
     BaseOutputParser,
     HumanMessage,
 )
 from langchain.tools.base import BaseTool
 
-from swarms.agents.prompts.prompts import EVAL_TOOL_RESPONSE
+from swarms.agents.models.prompts.prompts import EVAL_TOOL_RESPONSE
 from swarms.agents.utils.Agent import Agent
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 class ConversationalChatAgent(Agent):
     """An agent designed to hold a conversation in addition to using tools."""
```

### Comparing `swarms-1.1.4/swarms/agents/utils/agent_creator.py` & `swarms-1.1.5/swarms/agents/utils/agent_creator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/utils/agent_setup.py` & `swarms-1.1.5/swarms/agents/utils/agent_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from langchain.callbacks.base import BaseCallbackManager
 
 # from .ChatOpenAI import ChatOpenAI
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import BaseOutputParser
 
-from swarms.agents.prompts.prompts import EVAL_PREFIX, EVAL_SUFFIX
+from swarms.agents.models.prompts.prompts import EVAL_PREFIX, EVAL_SUFFIX
 from swarms.agents.tools.main import BaseToolSet, ToolsFactory
 
 from .ConversationalChatAgent import ConversationalChatAgent
 from .output_parser import EvalOutputParser
 
 
 class AgentSetup:
```

### Comparing `swarms-1.1.4/swarms/agents/utils/human_input.py` & `swarms-1.1.5/swarms/agents/utils/human_input.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/agents/utils/output_parser.py` & `swarms-1.1.5/swarms/agents/utils/output_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import re
 from abc import abstractmethod
 from typing import Dict, NamedTuple
 
 from langchain.schema import BaseOutputParser
 
-from swarms.agents.prompts.prompts import EVAL_FORMAT_INSTRUCTIONS
+from swarms.agents.models.prompts.prompts import EVAL_FORMAT_INSTRUCTIONS
 
 
 class EvalOutputParser(BaseOutputParser):
     @staticmethod
     def parse_all(text: str) -> Dict[str, str]:
         regex = r"Action: (.*?)[\n]Plan:(.*)[\n]What I Did:(.*)[\n]Action Input: (.*)"
         match = re.search(regex, text, re.DOTALL)
```

### Comparing `swarms-1.1.4/swarms/agents/utils/prompts.py` & `swarms-1.1.5/swarms/agents/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/boss/boss_node.py` & `swarms-1.1.5/swarms/boss/boss_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/orchestrator/orchestrate.py` & `swarms-1.1.5/swarms/orchestrator/orchestrate.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/swarms/hivemind.py` & `swarms-1.1.5/swarms/swarms/hivemind.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/swarms/swarms.py` & `swarms-1.1.5/swarms/swarms/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/utils/embeddings/base.py` & `swarms-1.1.5/swarms/utils/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/utils/embeddings/pegasus.py` & `swarms-1.1.5/swarms/utils/embeddings/pegasus.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/utils/main.py` & `swarms-1.1.5/swarms/utils/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
 
 
 
 
 #############===========================>
 
-from swarms.agents.prompts.prompts import DATAFRAME_PROMPT
+from swarms.agents.models.prompts.prompts import DATAFRAME_PROMPT
 
 import pandas as pd
 class CsvToDataframe(BaseHandler):
     def handle(self, filename: str):
         df = pd.read_csv(filename)
         description = (
             f"Dataframe with {len(df)} rows and {len(df.columns)} columns. "
```

### Comparing `swarms-1.1.4/swarms/utils/static.py` & `swarms-1.1.5/swarms/utils/static.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/character_generative.py` & `swarms-1.1.5/swarms/workers/character_generative.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/generative_worker.py` & `swarms-1.1.5/swarms/workers/generative_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/GroundingDINO/setup.py` & `swarms-1.1.5/swarms/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/models/segment_anything/setup.py` & `swarms-1.1.5/swarms/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/multi_modal_worker.py` & `swarms-1.1.5/swarms/workers/multi_modal_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-1.1.5/swarms/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-1.1.5/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-1.1.5/swarms/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-1.1.5/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/omni_worker.py` & `swarms-1.1.5/swarms/workers/omni_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/worker_agent_ultra.py` & `swarms-1.1.5/swarms/workers/worker_agent_ultra.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/worker_node.py` & `swarms-1.1.5/swarms/workers/worker_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms/workers/worker_ultra_node.py` & `swarms-1.1.5/swarms/workers/worker_ultra_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.4/swarms.egg-info/PKG-INFO` & `swarms-1.1.5/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.1.4
+Version: 1.1.5
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.1.4/swarms.egg-info/SOURCES.txt` & `swarms-1.1.5/swarms.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,40 @@
 swarms.egg-info/requires.txt
 swarms.egg-info/top_level.txt
 swarms/agents/__init__.py
 swarms/agents/base.py
 swarms/agents/memory.py
 swarms/agents/memory/__init__.py
 swarms/agents/memory/base.py
+swarms/agents/memory/base_memory.py
+swarms/agents/memory/chat_message_history.py
 swarms/agents/memory/chroma.py
+swarms/agents/memory/document.py
 swarms/agents/memory/ocean.py
+swarms/agents/memory/utils.py
 swarms/agents/models/__init__.py
 swarms/agents/models/anthropic.py
 swarms/agents/models/base.py
 swarms/agents/models/huggingface.py
 swarms/agents/models/openai.py
 swarms/agents/models/palm.py
 swarms/agents/models/petals.py
-swarms/agents/prompts/__init__.py
-swarms/agents/prompts/agent_output_parser.py
-swarms/agents/prompts/agent_prompt.py
-swarms/agents/prompts/agent_prompt_auto.py
-swarms/agents/prompts/chat_prompt.py
-swarms/agents/prompts/prompt_generator.py
-swarms/agents/prompts/prompts.py
-swarms/agents/prompts/chains/__init__.py
-swarms/agents/prompts/chains/llm.py
+swarms/agents/models/prompts/__init__.py
+swarms/agents/models/prompts/agent_output_parser.py
+swarms/agents/models/prompts/agent_prompt.py
+swarms/agents/models/prompts/agent_prompt_auto.py
+swarms/agents/models/prompts/base.py
+swarms/agents/models/prompts/chat_prompt.py
+swarms/agents/models/prompts/project_manager.py
+swarms/agents/models/prompts/prompt_generator.py
+swarms/agents/models/prompts/prompts.py
+swarms/agents/models/prompts/sales.py
+swarms/agents/models/prompts/summaries.py
+swarms/agents/models/prompts/chains/__init__.py
+swarms/agents/models/prompts/chains/llm.py
 swarms/agents/tools/__init__.py
 swarms/agents/tools/autogpt.py
 swarms/agents/tools/base.py
 swarms/agents/tools/code_intepretor.py
 swarms/agents/tools/developer.py
 swarms/agents/tools/exit_conversation.py
 swarms/agents/tools/file_mangagement.py
@@ -58,18 +66,20 @@
 swarms/orchestrator/orchestrate.py
 swarms/swarms/__init__.py
 swarms/swarms/hivemind.py
 swarms/swarms/swarms.py
 swarms/utils/__init__.py
 swarms/utils/logger.py
 swarms/utils/main.py
+swarms/utils/serializable.py
 swarms/utils/static.py
 swarms/utils/task.py
 swarms/utils/embeddings/__init__.py
 swarms/utils/embeddings/base.py
+swarms/utils/embeddings/openai.py
 swarms/utils/embeddings/pegasus.py
 swarms/utils/schema/__init__.py
 swarms/utils/schema/base.py
 swarms/workers/__init__.py
 swarms/workers/character_generative.py
 swarms/workers/generative_worker.py
 swarms/workers/multi_modal_worker.py
```

### Comparing `swarms-1.1.4/swarms.egg-info/requires.txt` & `swarms-1.1.5/swarms.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -5,80 +5,69 @@
 torchvision
 torchaudio
 asyncio
 nest_asyncio
 bs4
 pegasusx
 oceandb
-codeinterpreterapi[all]
+codeinterpreterapi
 playwright
 duckduckgo_search
 faiss-cpu
 wget==3.2
 accelerate
-sphinx_rtd_theme
 addict
 albumentations
 basicsr
 controlnet-aux
 diffusers
 einops
-gradio
 imageio
+simpleaichat
 imageio-ffmpeg
 kornia
 numpy
 omegaconf
 open_clip_torch
 opencv-python
 prettytable
 safetensors
 streamlit
 test-tube
 timm
 torchmetrics
 webdataset
 yapf
-wolframalpha
 wikipedia==1.4.0
 httpx
 ggl
 gradio_tools
-arxiv
-google-api-python-client
-google-auth-httplib2
 beautifulsoup4==4.11.2
-O365
-pytube
-pydub
 llama-index
 fastapi==0.94.1
 pydantic==1.10.6
 tenacity==8.2.2
 python-dotenv
 boto3
 uvicorn==0.21.1
 jinja2==3.1.2
 python-multipart==0.0.6
 celery==5.3.1
 redis==4.6.0
 sentencepiece
-bitsandbytes==0.41.0
 psycopg2-binary==2.9.5
 google-search-results==2.4.2
 black==23.7.0
 Pillow
 selenium
 diffusers
 controlnet_aux
 tiktoken
 espnet==202301
 espnet_model_zoo==0.1.7
-flask==2.2.3
-flask_cors==3.0.10
 waitress==2.1.2
 asteroid
 speechbrain
 timm
 typeguard
 pytesseract
 huggingface_hub
```

