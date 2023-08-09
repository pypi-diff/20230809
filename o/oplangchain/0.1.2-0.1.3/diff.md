# Comparing `tmp/oplangchain-0.1.2.tar.gz` & `tmp/oplangchain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oplangchain-0.1.2.tar", max compression
+gzip compressed data, was "oplangchain-0.1.3.tar", max compression
```

## Comparing `oplangchain-0.1.2.tar` & `oplangchain-0.1.3.tar`

### file list

```diff
@@ -1,972 +1,972 @@
--rw-r--r--   0        0        0     3112 2023-08-08 04:52:52.339954 oplangchain-0.1.2/oplangchain/__init__.py
--rw-r--r--   0        0        0     3430 2023-08-08 04:52:52.736001 oplangchain-0.1.2/oplangchain/agents/__init__.py
--rw-r--r--   0        0        0    41327 2023-08-08 04:52:52.741001 oplangchain-0.1.2/oplangchain/agents/agent.py
--rw-r--r--   0        0        0    18339 2023-08-08 04:52:52.741001 oplangchain-0.1.2/oplangchain/agents/agent_iterator.py
--rw-r--r--   0        0        0     3524 2023-08-08 04:52:52.757592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0      883 2023-08-08 04:52:52.761592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0      925 2023-08-08 04:52:52.757592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0      371 2023-08-08 04:52:52.757592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/base.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.393154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0     3397 2023-08-08 04:52:52.761592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
--rw-r--r--   0        0        0      734 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/conversational_retrieval/tool.py
--rw-r--r--   0        0        0       19 2023-08-07 21:21:40.394154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0     1154 2023-08-08 04:52:52.761592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/csv/base.py
--rw-r--r--   0        0        0      176 2023-08-08 04:52:52.761592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0     2092 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-07 21:21:40.396155 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0     2494 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       21 2023-08-07 21:21:40.398154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0     1583 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2023-08-07 21:21:40.399153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0     1929 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2023-08-07 21:21:40.400153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0     1729 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/json/base.py
--rw-r--r--   0        0        0     1819 2023-08-07 21:21:40.401154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0      561 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0       23 2023-08-07 21:21:40.402153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0      668 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.403154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0     1949 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0     3779 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2023-08-07 21:21:40.405154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0     1187 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2023-08-07 21:21:40.406154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0     2156 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0    11263 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0    10462 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0     1743 2023-08-07 21:21:40.407153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0     3835 2023-08-07 21:21:40.408153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0     2396 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-07 21:21:40.409153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0    11540 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/pandas/base.py
--rw-r--r--   0        0        0     1113 2023-08-07 21:21:40.410153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/pandas/prompt.py
--rw-r--r--   0        0        0      164 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0     3034 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-07 21:21:40.412153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0     2340 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0     2509 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0     2773 2023-08-07 21:21:40.413154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0     3239 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.414153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0     2220 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/python/base.py
--rw-r--r--   0        0        0      513 2023-08-07 21:21:40.415153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/python/prompt.py
--rw-r--r--   0        0        0       20 2023-08-07 21:21:40.416154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0     2748 2023-08-08 04:52:52.760593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark/base.py
--rw-r--r--   0        0        0      295 2023-08-07 21:21:40.416154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark/prompt.py
--rw-r--r--   0        0        0       23 2023-08-07 21:21:40.417153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0     2088 2023-08-08 04:52:52.759593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0     1202 2023-08-07 21:21:40.418154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0     1044 2023-08-08 04:52:52.757592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2023-08-07 21:21:40.419153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0     3458 2023-08-08 04:52:52.759593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0     1428 2023-08-07 21:21:40.420153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0     2826 2023-08-08 04:52:52.759593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       56 2023-08-07 21:21:40.421153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/vectorstore/__init__.py
--rw-r--r--   0        0        0     2422 2023-08-08 04:52:52.759593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/vectorstore/base.py
--rw-r--r--   0        0        0      834 2023-08-07 21:21:40.422154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/vectorstore/prompt.py
--rw-r--r--   0        0        0     2973 2023-08-08 04:52:52.759593 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/vectorstore/toolkit.py
--rw-r--r--   0        0        0       23 2023-08-07 21:21:40.423153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0     3119 2023-08-08 04:52:52.757592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/xorbits/base.py
--rw-r--r--   0        0        0     1070 2023-08-07 21:21:40.424153 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/xorbits/prompt.py
--rw-r--r--   0        0        0       22 2023-08-07 21:21:40.425154 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0     1617 2023-08-08 04:52:52.757592 oplangchain-0.1.2/oplangchain/agents/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0      688 2023-08-07 21:21:40.426153 oplangchain-0.1.2/oplangchain/agents/agent_types.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.426153 oplangchain-0.1.2/oplangchain/agents/chat/__init__.py
--rw-r--r--   0        0        0     4928 2023-08-08 04:52:52.752596 oplangchain-0.1.2/oplangchain/agents/chat/base.py
--rw-r--r--   0        0        0     1712 2023-08-08 04:52:52.752596 oplangchain-0.1.2/oplangchain/agents/chat/output_parser.py
--rw-r--r--   0        0        0     1158 2023-08-07 21:21:40.427153 oplangchain-0.1.2/oplangchain/agents/chat/prompt.py
--rw-r--r--   0        0        0       75 2023-08-07 21:21:40.428154 oplangchain-0.1.2/oplangchain/agents/conversational/__init__.py
--rw-r--r--   0        0        0     4840 2023-08-08 04:52:52.754593 oplangchain-0.1.2/oplangchain/agents/conversational/base.py
--rw-r--r--   0        0        0     1156 2023-08-08 04:52:52.754593 oplangchain-0.1.2/oplangchain/agents/conversational/output_parser.py
--rw-r--r--   0        0        0     1859 2023-08-07 21:21:40.429153 oplangchain-0.1.2/oplangchain/agents/conversational/prompt.py
--rw-r--r--   0        0        0       75 2023-08-07 21:21:40.430153 oplangchain-0.1.2/oplangchain/agents/conversational_chat/__init__.py
--rw-r--r--   0        0        0     4999 2023-08-08 04:52:52.752002 oplangchain-0.1.2/oplangchain/agents/conversational_chat/base.py
--rw-r--r--   0        0        0     2264 2023-08-08 04:52:52.752596 oplangchain-0.1.2/oplangchain/agents/conversational_chat/output_parser.py
--rw-r--r--   0        0        0     2757 2023-08-07 21:21:40.431155 oplangchain-0.1.2/oplangchain/agents/conversational_chat/prompt.py
--rw-r--r--   0        0        0     3007 2023-08-08 04:52:52.741001 oplangchain-0.1.2/oplangchain/agents/initialize.py
--rw-r--r--   0        0        0    17413 2023-08-08 04:52:52.740001 oplangchain-0.1.2/oplangchain/agents/load_tools.py
--rw-r--r--   0        0        0     4385 2023-08-08 04:52:52.741001 oplangchain-0.1.2/oplangchain/agents/loading.py
--rw-r--r--   0        0        0       86 2023-08-07 21:21:40.433153 oplangchain-0.1.2/oplangchain/agents/mrkl/__init__.py
--rw-r--r--   0        0        0     7127 2023-08-08 04:52:52.752002 oplangchain-0.1.2/oplangchain/agents/mrkl/base.py
--rw-r--r--   0        0        0     2712 2023-08-08 04:52:52.752596 oplangchain-0.1.2/oplangchain/agents/mrkl/output_parser.py
--rw-r--r--   0        0        0      641 2023-08-07 21:21:40.435153 oplangchain-0.1.2/oplangchain/agents/mrkl/prompt.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.435153 oplangchain-0.1.2/oplangchain/agents/openai_functions_agent/__init__.py
--rw-r--r--   0        0        0     2535 2023-08-08 04:52:52.752002 oplangchain-0.1.2/oplangchain/agents/openai_functions_agent/agent_token_buffer_memory.py
--rw-r--r--   0        0        0    11916 2023-08-08 04:52:52.752002 oplangchain-0.1.2/oplangchain/agents/openai_functions_agent/base.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.437154 oplangchain-0.1.2/oplangchain/agents/openai_functions_multi_agent/__init__.py
--rw-r--r--   0        0        0    13355 2023-08-08 04:52:52.752002 oplangchain-0.1.2/oplangchain/agents/openai_functions_multi_agent/base.py
--rw-r--r--   0        0        0       76 2023-08-07 21:21:40.438153 oplangchain-0.1.2/oplangchain/agents/react/__init__.py
--rw-r--r--   0        0        0     5690 2023-08-08 04:52:52.752002 oplangchain-0.1.2/oplangchain/agents/react/base.py
--rw-r--r--   0        0        0     1192 2023-08-08 04:52:52.751004 oplangchain-0.1.2/oplangchain/agents/react/output_parser.py
--rw-r--r--   0        0        0     1903 2023-08-08 04:52:52.751004 oplangchain-0.1.2/oplangchain/agents/react/textworld_prompt.py
--rw-r--r--   0        0        0     6124 2023-08-08 04:52:52.751004 oplangchain-0.1.2/oplangchain/agents/react/wiki_prompt.py
--rw-r--r--   0        0        0     1089 2023-08-08 04:52:52.740001 oplangchain-0.1.2/oplangchain/agents/schema.py
--rw-r--r--   0        0        0      106 2023-08-07 21:21:40.441153 oplangchain-0.1.2/oplangchain/agents/self_ask_with_search/__init__.py
--rw-r--r--   0        0        0     3118 2023-08-08 04:52:52.746003 oplangchain-0.1.2/oplangchain/agents/self_ask_with_search/base.py
--rw-r--r--   0        0        0      966 2023-08-08 04:52:52.745003 oplangchain-0.1.2/oplangchain/agents/self_ask_with_search/output_parser.py
--rw-r--r--   0        0        0     1923 2023-08-08 04:52:52.745003 oplangchain-0.1.2/oplangchain/agents/self_ask_with_search/prompt.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.443153 oplangchain-0.1.2/oplangchain/agents/structured_chat/__init__.py
--rw-r--r--   0        0        0     5162 2023-08-08 04:52:52.749002 oplangchain-0.1.2/oplangchain/agents/structured_chat/base.py
--rw-r--r--   0        0        0     3462 2023-08-08 04:52:52.749002 oplangchain-0.1.2/oplangchain/agents/structured_chat/output_parser.py
--rw-r--r--   0        0        0      992 2023-08-07 21:21:40.444153 oplangchain-0.1.2/oplangchain/agents/structured_chat/prompt.py
--rw-r--r--   0        0        0     1406 2023-08-08 04:52:52.740001 oplangchain-0.1.2/oplangchain/agents/tools.py
--rw-r--r--   0        0        0     1497 2023-08-08 04:52:52.740001 oplangchain-0.1.2/oplangchain/agents/types.py
--rw-r--r--   0        0        0      386 2023-08-08 04:52:52.737004 oplangchain-0.1.2/oplangchain/agents/utils.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.446153 oplangchain-0.1.2/oplangchain/agents/xml/__init__.py
--rw-r--r--   0        0        0     3905 2023-08-08 04:52:52.741001 oplangchain-0.1.2/oplangchain/agents/xml/base.py
--rw-r--r--   0        0        0      749 2023-08-07 21:21:40.447154 oplangchain-0.1.2/oplangchain/agents/xml/prompt.py
--rw-r--r--   0        0        0      220 2023-08-08 04:52:52.346953 oplangchain-0.1.2/oplangchain/base_language.py
--rw-r--r--   0        0        0    24775 2023-08-08 05:01:50.900148 oplangchain-0.1.2/oplangchain/cache.py
--rw-r--r--   0        0        0     2887 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/callbacks/__init__.py
--rw-r--r--   0        0        0    14488 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/aim_callback.py
--rw-r--r--   0        0        0    13727 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/argilla_callback.py
--rw-r--r--   0        0        0     7509 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/arize_callback.py
--rw-r--r--   0        0        0    11347 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/callbacks/arthur_callback.py
--rw-r--r--   0        0        0    15188 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/base.py
--rw-r--r--   0        0        0    18502 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/clearml_callback.py
--rw-r--r--   0        0        0    23246 2023-08-08 05:01:50.902666 oplangchain-0.1.2/oplangchain/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0     6438 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/context_callback.py
--rw-r--r--   0        0        0     2567 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/file.py
--rw-r--r--   0        0        0    13163 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/callbacks/flyte_callback.py
--rw-r--r--   0        0        0     1412 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/human.py
--rw-r--r--   0        0        0     5574 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/infino_callback.py
--rw-r--r--   0        0        0    53799 2023-08-08 05:06:24.195893 oplangchain-0.1.2/oplangchain/callbacks/manager.py
--rw-r--r--   0        0        0    24171 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0     5352 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/openai_info.py
--rw-r--r--   0        0        0     5529 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0     8829 2023-08-08 04:52:52.612956 oplangchain-0.1.2/oplangchain/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0     3209 2023-08-08 04:52:52.612956 oplangchain-0.1.2/oplangchain/callbacks/stdout.py
--rw-r--r--   0        0        0     2440 2023-08-08 04:52:52.612956 oplangchain-0.1.2/oplangchain/callbacks/streaming_aiter.py
--rw-r--r--   0        0        0     3368 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/callbacks/streaming_aiter_final_only.py
--rw-r--r--   0        0        0     2174 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     3370 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/callbacks/streaming_stdout_final_only.py
--rw-r--r--   0        0        0     3196 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0     5435 2023-08-07 21:21:40.460153 oplangchain-0.1.2/oplangchain/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0    15677 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0      510 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0    17028 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/callbacks/tracers/base.py
--rw-r--r--   0        0        0     4866 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0     8065 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0     7370 2023-08-08 04:52:52.618953 oplangchain-0.1.2/oplangchain/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0     1541 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0     3458 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0     6033 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0    18987 2023-08-08 04:52:52.617952 oplangchain-0.1.2/oplangchain/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0     8505 2023-08-07 21:21:40.465154 oplangchain-0.1.2/oplangchain/callbacks/utils.py
--rw-r--r--   0        0        0    20665 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/callbacks/wandb_callback.py
--rw-r--r--   0        0        0     8066 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0     5378 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/__init__.py
--rw-r--r--   0        0        0       84 2023-08-07 21:21:40.468155 oplangchain-0.1.2/oplangchain/chains/api/__init__.py
--rw-r--r--   0        0        0     5348 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/api/base.py
--rw-r--r--   0        0        0     2452 2023-08-07 21:21:40.469154 oplangchain-0.1.2/oplangchain/chains/api/news_docs.py
--rw-r--r--   0        0        0     3399 2023-08-07 21:21:40.469154 oplangchain-0.1.2/oplangchain/chains/api/open_meteo_docs.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.470153 oplangchain-0.1.2/oplangchain/chains/api/openapi/__init__.py
--rw-r--r--   0        0        0     8766 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/api/openapi/chain.py
--rw-r--r--   0        0        0     1791 2023-08-07 21:21:40.471154 oplangchain-0.1.2/oplangchain/chains/api/openapi/prompts.py
--rw-r--r--   0        0        0     1887 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/api/openapi/requests_chain.py
--rw-r--r--   0        0        0     1759 2023-08-08 04:52:52.725542 oplangchain-0.1.2/oplangchain/chains/api/openapi/response_chain.py
--rw-r--r--   0        0        0     1920 2023-08-07 21:21:40.472154 oplangchain-0.1.2/oplangchain/chains/api/podcast_docs.py
--rw-r--r--   0        0        0     1028 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/api/prompt.py
--rw-r--r--   0        0        0     1537 2023-08-07 21:21:40.473154 oplangchain-0.1.2/oplangchain/chains/api/tmdb_docs.py
--rw-r--r--   0        0        0    24830 2023-08-08 05:06:24.195893 oplangchain-0.1.2/oplangchain/chains/base.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.474154 oplangchain-0.1.2/oplangchain/chains/chat_vector_db/__init__.py
--rw-r--r--   0        0        0      691 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/chat_vector_db/prompts.py
--rw-r--r--   0        0        0       43 2023-08-07 21:21:40.475154 oplangchain-0.1.2/oplangchain/chains/combine_documents/__init__.py
--rw-r--r--   0        0        0     6398 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/combine_documents/base.py
--rw-r--r--   0        0        0    11165 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/combine_documents/map_reduce.py
--rw-r--r--   0        0        0     8386 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/combine_documents/map_rerank.py
--rw-r--r--   0        0        0    11016 2023-08-08 04:52:52.723542 oplangchain-0.1.2/oplangchain/chains/combine_documents/reduce.py
--rw-r--r--   0        0        0     9093 2023-08-08 04:52:52.721990 oplangchain-0.1.2/oplangchain/chains/combine_documents/refine.py
--rw-r--r--   0        0        0     7676 2023-08-08 04:52:52.720989 oplangchain-0.1.2/oplangchain/chains/combine_documents/stuff.py
--rw-r--r--   0        0        0      107 2023-08-07 21:21:40.479154 oplangchain-0.1.2/oplangchain/chains/constitutional_ai/__init__.py
--rw-r--r--   0        0        0     6350 2023-08-08 04:52:52.720989 oplangchain-0.1.2/oplangchain/chains/constitutional_ai/base.py
--rw-r--r--   0        0        0      265 2023-08-07 21:21:40.480154 oplangchain-0.1.2/oplangchain/chains/constitutional_ai/models.py
--rw-r--r--   0        0        0    21740 2023-08-08 04:52:52.720989 oplangchain-0.1.2/oplangchain/chains/constitutional_ai/principles.py
--rw-r--r--   0        0        0     8660 2023-08-08 04:52:52.718988 oplangchain-0.1.2/oplangchain/chains/constitutional_ai/prompts.py
--rw-r--r--   0        0        0       71 2023-08-07 21:21:40.482154 oplangchain-0.1.2/oplangchain/chains/conversation/__init__.py
--rw-r--r--   0        0        0     2184 2023-08-08 04:52:52.718988 oplangchain-0.1.2/oplangchain/chains/conversation/base.py
--rw-r--r--   0        0        0      870 2023-08-08 04:52:52.717989 oplangchain-0.1.2/oplangchain/chains/conversation/memory.py
--rw-r--r--   0        0        0      912 2023-08-08 04:52:52.717989 oplangchain-0.1.2/oplangchain/chains/conversation/prompt.py
--rw-r--r--   0        0        0       49 2023-08-07 21:21:40.484154 oplangchain-0.1.2/oplangchain/chains/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0    16735 2023-08-08 04:52:52.709600 oplangchain-0.1.2/oplangchain/chains/conversational_retrieval/base.py
--rw-r--r--   0        0        0      717 2023-08-08 04:52:52.709600 oplangchain-0.1.2/oplangchain/chains/conversational_retrieval/prompts.py
--rw-r--r--   0        0        0      128 2023-08-08 04:52:52.716988 oplangchain-0.1.2/oplangchain/chains/elasticsearch_database/__init__.py
--rw-r--r--   0        0        0     8182 2023-08-08 04:52:52.717989 oplangchain-0.1.2/oplangchain/chains/elasticsearch_database/base.py
--rw-r--r--   0        0        0     1422 2023-08-08 04:52:52.717989 oplangchain-0.1.2/oplangchain/chains/elasticsearch_database/prompts.py
--rw-r--r--   0        0        0      739 2023-08-08 04:52:52.667997 oplangchain-0.1.2/oplangchain/chains/example_generator.py
--rw-r--r--   0        0        0       51 2023-08-07 21:21:40.487153 oplangchain-0.1.2/oplangchain/chains/flare/__init__.py
--rw-r--r--   0        0        0     8779 2023-08-08 04:52:52.715988 oplangchain-0.1.2/oplangchain/chains/flare/base.py
--rw-r--r--   0        0        0     1457 2023-08-08 04:52:52.715988 oplangchain-0.1.2/oplangchain/chains/flare/prompts.py
--rw-r--r--   0        0        0       49 2023-08-07 21:21:40.489153 oplangchain-0.1.2/oplangchain/chains/graph_qa/__init__.py
--rw-r--r--   0        0        0     7690 2023-08-08 04:52:52.715988 oplangchain-0.1.2/oplangchain/chains/graph_qa/arangodb.py
--rw-r--r--   0        0        0     2984 2023-08-08 04:52:52.715988 oplangchain-0.1.2/oplangchain/chains/graph_qa/base.py
--rw-r--r--   0        0        0     4600 2023-08-08 04:52:52.714991 oplangchain-0.1.2/oplangchain/chains/graph_qa/cypher.py
--rw-r--r--   0        0        0     3033 2023-08-08 04:52:52.714991 oplangchain-0.1.2/oplangchain/chains/graph_qa/hugegraph.py
--rw-r--r--   0        0        0     3033 2023-08-08 04:52:52.714991 oplangchain-0.1.2/oplangchain/chains/graph_qa/kuzu.py
--rw-r--r--   0        0        0     3008 2023-08-08 04:52:52.714991 oplangchain-0.1.2/oplangchain/chains/graph_qa/nebulagraph.py
--rw-r--r--   0        0        0     4493 2023-08-08 04:52:52.714991 oplangchain-0.1.2/oplangchain/chains/graph_qa/neptune_cypher.py
--rw-r--r--   0        0        0    13730 2023-08-08 04:52:52.714991 oplangchain-0.1.2/oplangchain/chains/graph_qa/prompts.py
--rw-r--r--   0        0        0     4785 2023-08-08 04:52:52.714991 oplangchain-0.1.2/oplangchain/chains/graph_qa/sparql.py
--rw-r--r--   0        0        0       75 2023-08-07 21:21:40.493153 oplangchain-0.1.2/oplangchain/chains/hyde/__init__.py
--rw-r--r--   0        0        0     2843 2023-08-08 04:52:52.712601 oplangchain-0.1.2/oplangchain/chains/hyde/base.py
--rw-r--r--   0        0        0     1910 2023-08-08 04:52:52.712601 oplangchain-0.1.2/oplangchain/chains/hyde/prompts.py
--rw-r--r--   0        0        0    12157 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/llm.py
--rw-r--r--   0        0        0       88 2023-08-07 21:21:40.495154 oplangchain-0.1.2/oplangchain/chains/llm_bash/__init__.py
--rw-r--r--   0        0        0     4181 2023-08-08 04:52:52.712601 oplangchain-0.1.2/oplangchain/chains/llm_bash/base.py
--rw-r--r--   0        0        0     1941 2023-08-08 04:52:52.712601 oplangchain-0.1.2/oplangchain/chains/llm_bash/prompt.py
--rw-r--r--   0        0        0      139 2023-08-07 21:21:40.497153 oplangchain-0.1.2/oplangchain/chains/llm_checker/__init__.py
--rw-r--r--   0        0        0     6106 2023-08-08 04:52:52.706600 oplangchain-0.1.2/oplangchain/chains/llm_checker/base.py
--rw-r--r--   0        0        0     1122 2023-08-08 04:52:52.706600 oplangchain-0.1.2/oplangchain/chains/llm_checker/prompt.py
--rw-r--r--   0        0        0      143 2023-08-07 21:21:40.499153 oplangchain-0.1.2/oplangchain/chains/llm_math/__init__.py
--rw-r--r--   0        0        0     6386 2023-08-08 04:52:52.709600 oplangchain-0.1.2/oplangchain/chains/llm_math/base.py
--rw-r--r--   0        0        0      865 2023-08-08 04:52:52.709600 oplangchain-0.1.2/oplangchain/chains/llm_math/prompt.py
--rw-r--r--   0        0        0     2885 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/llm_requests.py
--rw-r--r--   0        0        0      352 2023-08-07 21:21:40.500154 oplangchain-0.1.2/oplangchain/chains/llm_summarization_checker/__init__.py
--rw-r--r--   0        0        0     6620 2023-08-08 04:52:52.706600 oplangchain-0.1.2/oplangchain/chains/llm_summarization_checker/base.py
--rw-r--r--   0        0        0      654 2023-08-07 21:21:40.502153 oplangchain-0.1.2/oplangchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
--rw-r--r--   0        0        0      377 2023-08-07 21:21:40.502153 oplangchain-0.1.2/oplangchain/chains/llm_summarization_checker/prompts/check_facts.txt
--rw-r--r--   0        0        0      128 2023-08-07 21:21:40.503153 oplangchain-0.1.2/oplangchain/chains/llm_summarization_checker/prompts/create_facts.txt
--rw-r--r--   0        0        0      416 2023-08-07 21:21:40.503153 oplangchain-0.1.2/oplangchain/chains/llm_summarization_checker/prompts/revise_summary.txt
--rw-r--r--   0        0        0      126 2023-08-07 21:21:40.504153 oplangchain-0.1.2/oplangchain/chains/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0     5569 2023-08-08 04:52:52.706600 oplangchain-0.1.2/oplangchain/chains/llm_symbolic_math/base.py
--rw-r--r--   0        0        0     1089 2023-08-08 04:52:52.706600 oplangchain-0.1.2/oplangchain/chains/llm_symbolic_math/prompt.py
--rw-r--r--   0        0        0    23991 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/loading.py
--rw-r--r--   0        0        0     3737 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/mapreduce.py
--rw-r--r--   0        0        0     3058 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/moderation.py
--rw-r--r--   0        0        0       96 2023-08-07 21:21:40.507154 oplangchain-0.1.2/oplangchain/chains/natbot/__init__.py
--rw-r--r--   0        0        0     4193 2023-08-08 04:52:52.701599 oplangchain-0.1.2/oplangchain/chains/natbot/base.py
--rw-r--r--   0        0        0    15466 2023-08-07 21:21:40.508154 oplangchain-0.1.2/oplangchain/chains/natbot/crawler.py
--rw-r--r--   0        0        0     4986 2023-08-08 04:52:52.701599 oplangchain-0.1.2/oplangchain/chains/natbot/prompt.py
--rw-r--r--   0        0        0      958 2023-08-08 04:52:52.698599 oplangchain-0.1.2/oplangchain/chains/openai_functions/__init__.py
--rw-r--r--   0        0        0    14630 2023-08-08 04:52:52.701599 oplangchain-0.1.2/oplangchain/chains/openai_functions/base.py
--rw-r--r--   0        0        0     3518 2023-08-08 04:52:52.701599 oplangchain-0.1.2/oplangchain/chains/openai_functions/citation_fuzzy_match.py
--rw-r--r--   0        0        0     3350 2023-08-08 04:52:52.701599 oplangchain-0.1.2/oplangchain/chains/openai_functions/extraction.py
--rw-r--r--   0        0        0    11226 2023-08-08 05:04:13.464638 oplangchain-0.1.2/oplangchain/chains/openai_functions/openapi.py
--rw-r--r--   0        0        0     3725 2023-08-08 04:52:52.701599 oplangchain-0.1.2/oplangchain/chains/openai_functions/qa_with_structure.py
--rw-r--r--   0        0        0     2665 2023-08-08 04:52:52.698599 oplangchain-0.1.2/oplangchain/chains/openai_functions/tagging.py
--rw-r--r--   0        0        0     1257 2023-08-07 21:21:40.512154 oplangchain-0.1.2/oplangchain/chains/openai_functions/utils.py
--rw-r--r--   0        0        0     1969 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/prompt_selector.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.513154 oplangchain-0.1.2/oplangchain/chains/qa_generation/__init__.py
--rw-r--r--   0        0        0     2458 2023-08-08 04:52:52.698599 oplangchain-0.1.2/oplangchain/chains/qa_generation/base.py
--rw-r--r--   0        0        0     1871 2023-08-08 04:52:52.698599 oplangchain-0.1.2/oplangchain/chains/qa_generation/prompt.py
--rw-r--r--   0        0        0      175 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/qa_with_sources/__init__.py
--rw-r--r--   0        0        0     7741 2023-08-08 04:52:52.698599 oplangchain-0.1.2/oplangchain/chains/qa_with_sources/base.py
--rw-r--r--   0        0        0     6825 2023-08-08 04:52:52.698599 oplangchain-0.1.2/oplangchain/chains/qa_with_sources/loading.py
--rw-r--r--   0        0        0     6968 2023-08-08 04:52:52.698599 oplangchain-0.1.2/oplangchain/chains/qa_with_sources/map_reduce_prompt.py
--rw-r--r--   0        0        0     1315 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/qa_with_sources/refine_prompts.py
--rw-r--r--   0        0        0     2354 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/qa_with_sources/retrieval.py
--rw-r--r--   0        0        0     6578 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/qa_with_sources/stuff_prompt.py
--rw-r--r--   0        0        0     2811 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/qa_with_sources/vector_db.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.519154 oplangchain-0.1.2/oplangchain/chains/query_constructor/__init__.py
--rw-r--r--   0        0        0     5824 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/query_constructor/base.py
--rw-r--r--   0        0        0     3129 2023-08-07 21:21:40.520154 oplangchain-0.1.2/oplangchain/chains/query_constructor/ir.py
--rw-r--r--   0        0        0     4756 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/query_constructor/parser.py
--rw-r--r--   0        0        0     6448 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/query_constructor/prompt.py
--rw-r--r--   0        0        0      303 2023-08-07 21:21:40.521153 oplangchain-0.1.2/oplangchain/chains/query_constructor/schema.py
--rw-r--r--   0        0        0     8578 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/question_answering/__init__.py
--rw-r--r--   0        0        0     8009 2023-08-08 04:52:52.696616 oplangchain-0.1.2/oplangchain/chains/question_answering/map_reduce_prompt.py
--rw-r--r--   0        0        0     1621 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/question_answering/map_rerank_prompt.py
--rw-r--r--   0        0        0     2732 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/question_answering/refine_prompts.py
--rw-r--r--   0        0        0     1141 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/question_answering/stuff_prompt.py
--rw-r--r--   0        0        0       62 2023-08-07 21:21:40.524154 oplangchain-0.1.2/oplangchain/chains/retrieval_qa/__init__.py
--rw-r--r--   0        0        0     9794 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/retrieval_qa/base.py
--rw-r--r--   0        0        0      396 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/retrieval_qa/prompt.py
--rw-r--r--   0        0        0      415 2023-08-08 04:52:52.667997 oplangchain-0.1.2/oplangchain/chains/router/__init__.py
--rw-r--r--   0        0        0     4560 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/router/base.py
--rw-r--r--   0        0        0     1980 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/router/embedding_router.py
--rw-r--r--   0        0        0     4197 2023-08-08 04:52:52.695606 oplangchain-0.1.2/oplangchain/chains/router/llm_router.py
--rw-r--r--   0        0        0     2576 2023-08-08 04:52:52.694599 oplangchain-0.1.2/oplangchain/chains/router/multi_prompt.py
--rw-r--r--   0        0        0     1123 2023-08-07 21:21:40.528154 oplangchain-0.1.2/oplangchain/chains/router/multi_prompt_prompt.py
--rw-r--r--   0        0        0     1079 2023-08-07 21:21:40.528154 oplangchain-0.1.2/oplangchain/chains/router/multi_retrieval_prompt.py
--rw-r--r--   0        0        0     3657 2023-08-08 04:52:52.667997 oplangchain-0.1.2/oplangchain/chains/router/multi_retrieval_qa.py
--rw-r--r--   0        0        0     7487 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/sequential.py
--rw-r--r--   0        0        0       47 2023-08-07 21:21:40.530154 oplangchain-0.1.2/oplangchain/chains/sql_database/__init__.py
--rw-r--r--   0        0        0    14206 2023-08-08 04:52:52.667997 oplangchain-0.1.2/oplangchain/chains/sql_database/prompt.py
--rw-r--r--   0        0        0     2078 2023-08-08 04:52:52.667997 oplangchain-0.1.2/oplangchain/chains/sql_database/query.py
--rw-r--r--   0        0        0     5715 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/summarize/__init__.py
--rw-r--r--   0        0        0      235 2023-08-08 04:52:52.667997 oplangchain-0.1.2/oplangchain/chains/summarize/map_reduce_prompt.py
--rw-r--r--   0        0        0      807 2023-08-08 04:52:52.667997 oplangchain-0.1.2/oplangchain/chains/summarize/refine_prompts.py
--rw-r--r--   0        0        0      235 2023-08-08 04:52:52.667997 oplangchain-0.1.2/oplangchain/chains/summarize/stuff_prompt.py
--rw-r--r--   0        0        0     2239 2023-08-08 04:52:52.666996 oplangchain-0.1.2/oplangchain/chains/transform.py
--rw-r--r--   0        0        0     1374 2023-08-08 04:52:52.725542 oplangchain-0.1.2/oplangchain/chat_models/__init__.py
--rw-r--r--   0        0        0     7002 2023-08-08 04:52:52.729543 oplangchain-0.1.2/oplangchain/chat_models/anthropic.py
--rw-r--r--   0        0        0     4713 2023-08-08 04:52:52.729543 oplangchain-0.1.2/oplangchain/chat_models/azure_openai.py
--rw-r--r--   0        0        0     5406 2023-08-08 04:52:52.729543 oplangchain-0.1.2/oplangchain/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0    23298 2023-08-08 05:09:17.586726 oplangchain-0.1.2/oplangchain/chat_models/base.py
--rw-r--r--   0        0        0     1046 2023-08-08 04:52:52.728543 oplangchain-0.1.2/oplangchain/chat_models/fake.py
--rw-r--r--   0        0        0    11139 2023-08-08 04:52:52.727543 oplangchain-0.1.2/oplangchain/chat_models/google_palm.py
--rw-r--r--   0        0        0     4027 2023-08-08 04:52:52.726542 oplangchain-0.1.2/oplangchain/chat_models/human.py
--rw-r--r--   0        0        0    15237 2023-08-08 04:52:52.726542 oplangchain-0.1.2/oplangchain/chat_models/jinachat.py
--rw-r--r--   0        0        0     6865 2023-08-08 04:52:52.726542 oplangchain-0.1.2/oplangchain/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0    22380 2023-08-08 04:52:52.726542 oplangchain-0.1.2/oplangchain/chat_models/openai.py
--rw-r--r--   0        0        0     5174 2023-08-08 04:52:52.726542 oplangchain-0.1.2/oplangchain/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0     6018 2023-08-08 04:52:52.725542 oplangchain-0.1.2/oplangchain/chat_models/vertexai.py
--rw-r--r--   0        0        0      685 2023-08-07 21:21:40.540154 oplangchain-0.1.2/oplangchain/docker-compose.yaml
--rw-r--r--   0        0        0      525 2023-08-08 04:52:52.729543 oplangchain-0.1.2/oplangchain/docstore/__init__.py
--rw-r--r--   0        0        0     1075 2023-08-08 04:52:52.736001 oplangchain-0.1.2/oplangchain/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      838 2023-08-08 04:52:52.732543 oplangchain-0.1.2/oplangchain/docstore/base.py
--rw-r--r--   0        0        0       64 2023-08-08 04:52:52.732543 oplangchain-0.1.2/oplangchain/docstore/document.py
--rw-r--r--   0        0        0     1606 2023-08-08 04:52:52.730543 oplangchain-0.1.2/oplangchain/docstore/in_memory.py
--rw-r--r--   0        0        0     1483 2023-08-08 04:52:52.729543 oplangchain-0.1.2/oplangchain/docstore/wikipedia.py
--rw-r--r--   0        0        0    13128 2023-08-08 04:52:52.566956 oplangchain-0.1.2/oplangchain/document_loaders/__init__.py
--rw-r--r--   0        0        0     2851 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/acreom.py
--rw-r--r--   0        0        0      845 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0     1277 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/airtable.py
--rw-r--r--   0        0        0     2724 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0     1144 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/arxiv.py
--rw-r--r--   0        0        0     4865 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/async_html.py
--rw-r--r--   0        0        0      580 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/azlyrics.py
--rw-r--r--   0        0        0     1618 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0     1637 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0     3047 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/base.py
--rw-r--r--   0        0        0     3934 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/bibtex.py
--rw-r--r--   0        0        0     3151 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/bigquery.py
--rw-r--r--   0        0        0     2726 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/bilibili.py
--rw-r--r--   0        0        0    10099 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/blackboard.py
--rw-r--r--   0        0        0      332 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0     4283 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0     5765 2023-08-07 21:21:40.551154 oplangchain-0.1.2/oplangchain/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0     1510 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0     5732 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/blockchain.py
--rw-r--r--   0        0        0     1074 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/brave_search.py
--rw-r--r--   0        0        0     2136 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/browserless.py
--rw-r--r--   0        0        0     2030 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/chatgpt.py
--rw-r--r--   0        0        0      556 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/college_confidential.py
--rw-r--r--   0        0        0     2153 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/concurrent.py
--rw-r--r--   0        0        0    25403 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/confluence.py
--rw-r--r--   0        0        0     1072 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/conllu.py
--rw-r--r--   0        0        0     4203 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/csv_loader.py
--rw-r--r--   0        0        0     5905 2023-08-08 04:52:52.609953 oplangchain-0.1.2/oplangchain/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0     4997 2023-08-08 04:52:52.608952 oplangchain-0.1.2/oplangchain/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0     1329 2023-08-08 04:52:52.608952 oplangchain-0.1.2/oplangchain/document_loaders/dataframe.py
--rw-r--r--   0        0        0     2114 2023-08-08 04:52:52.607953 oplangchain-0.1.2/oplangchain/document_loaders/diffbot.py
--rw-r--r--   0        0        0     5104 2023-08-08 04:52:52.607953 oplangchain-0.1.2/oplangchain/document_loaders/directory.py
--rw-r--r--   0        0        0     1265 2023-08-08 04:52:52.607953 oplangchain-0.1.2/oplangchain/document_loaders/discord.py
--rw-r--r--   0        0        0    13220 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/docugami.py
--rw-r--r--   0        0        0     6095 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/dropbox.py
--rw-r--r--   0        0        0     3185 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0     3792 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/email.py
--rw-r--r--   0        0        0     8951 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/embaas.py
--rw-r--r--   0        0        0     1514 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/epub.py
--rw-r--r--   0        0        0     7812 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/etherscan.py
--rw-r--r--   0        0        0     5748 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/evernote.py
--rw-r--r--   0        0        0     1668 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/excel.py
--rw-r--r--   0        0        0     1302 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0     2245 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/fauna.py
--rw-r--r--   0        0        0     1575 2023-08-08 04:52:52.606954 oplangchain-0.1.2/oplangchain/document_loaders/figma.py
--rw-r--r--   0        0        0     1579 2023-08-08 04:52:52.605952 oplangchain-0.1.2/oplangchain/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0     1737 2023-08-08 04:52:52.605952 oplangchain-0.1.2/oplangchain/document_loaders/gcs_file.py
--rw-r--r--   0        0        0     4543 2023-08-08 04:52:52.605952 oplangchain-0.1.2/oplangchain/document_loaders/generic.py
--rw-r--r--   0        0        0     1686 2023-08-08 04:52:52.605952 oplangchain-0.1.2/oplangchain/document_loaders/geodataframe.py
--rw-r--r--   0        0        0     4142 2023-08-08 04:52:52.605952 oplangchain-0.1.2/oplangchain/document_loaders/git.py
--rw-r--r--   0        0        0     3110 2023-08-08 04:52:52.605540 oplangchain-0.1.2/oplangchain/document_loaders/gitbook.py
--rw-r--r--   0        0        0     6874 2023-08-08 04:52:52.604954 oplangchain-0.1.2/oplangchain/document_loaders/github.py
--rw-r--r--   0        0        0    13930 2023-08-08 04:52:52.604954 oplangchain-0.1.2/oplangchain/document_loaders/googledrive.py
--rw-r--r--   0        0        0      973 2023-08-08 04:52:52.603954 oplangchain-0.1.2/oplangchain/document_loaders/gutenberg.py
--rw-r--r--   0        0        0     1559 2023-08-07 21:21:40.568154 oplangchain-0.1.2/oplangchain/document_loaders/helpers.py
--rw-r--r--   0        0        0     2065 2023-08-08 04:52:52.603954 oplangchain-0.1.2/oplangchain/document_loaders/hn.py
--rw-r--r--   0        0        0     1208 2023-08-08 04:52:52.602952 oplangchain-0.1.2/oplangchain/document_loaders/html.py
--rw-r--r--   0        0        0     2122 2023-08-08 04:52:52.600954 oplangchain-0.1.2/oplangchain/document_loaders/html_bs.py
--rw-r--r--   0        0        0     3029 2023-08-08 04:52:52.599953 oplangchain-0.1.2/oplangchain/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0     7654 2023-08-08 04:52:52.599953 oplangchain-0.1.2/oplangchain/document_loaders/ifixit.py
--rw-r--r--   0        0        0     1190 2023-08-08 04:52:52.599953 oplangchain-0.1.2/oplangchain/document_loaders/image.py
--rw-r--r--   0        0        0     3103 2023-08-08 04:52:52.599953 oplangchain-0.1.2/oplangchain/document_loaders/image_captions.py
--rw-r--r--   0        0        0      491 2023-08-08 04:52:52.599953 oplangchain-0.1.2/oplangchain/document_loaders/imsdb.py
--rw-r--r--   0        0        0     1740 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/iugu.py
--rw-r--r--   0        0        0     3705 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/joplin.py
--rw-r--r--   0        0        0     5491 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/json_loader.py
--rw-r--r--   0        0        0     2056 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/larksuite.py
--rw-r--r--   0        0        0     1832 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/markdown.py
--rw-r--r--   0        0        0     3134 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/mastodon.py
--rw-r--r--   0        0        0     3299 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/max_compute.py
--rw-r--r--   0        0        0     3487 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      842 2023-08-08 04:52:52.598953 oplangchain-0.1.2/oplangchain/document_loaders/merge.py
--rw-r--r--   0        0        0     2604 2023-08-08 04:52:52.597955 oplangchain-0.1.2/oplangchain/document_loaders/mhtml.py
--rw-r--r--   0        0        0     3137 2023-08-08 04:52:52.596954 oplangchain-0.1.2/oplangchain/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0     4293 2023-08-08 04:52:52.595955 oplangchain-0.1.2/oplangchain/document_loaders/news.py
--rw-r--r--   0        0        0     4285 2023-08-08 04:52:52.595955 oplangchain-0.1.2/oplangchain/document_loaders/notebook.py
--rw-r--r--   0        0        0      745 2023-08-08 04:52:52.593953 oplangchain-0.1.2/oplangchain/document_loaders/notion.py
--rw-r--r--   0        0        0     5896 2023-08-08 04:52:52.593953 oplangchain-0.1.2/oplangchain/document_loaders/notiondb.py
--rw-r--r--   0        0        0     1090 2023-08-08 04:52:52.590953 oplangchain-0.1.2/oplangchain/document_loaders/nuclia.py
--rw-r--r--   0        0        0     3600 2023-08-08 04:52:52.590953 oplangchain-0.1.2/oplangchain/document_loaders/obs_directory.py
--rw-r--r--   0        0        0     4751 2023-08-08 04:52:52.590953 oplangchain-0.1.2/oplangchain/document_loaders/obs_file.py
--rw-r--r--   0        0        0     2541 2023-08-08 04:52:52.590953 oplangchain-0.1.2/oplangchain/document_loaders/obsidian.py
--rw-r--r--   0        0        0     1797 2023-08-08 04:52:52.590953 oplangchain-0.1.2/oplangchain/document_loaders/odt.py
--rw-r--r--   0        0        0     8641 2023-08-08 04:52:52.589954 oplangchain-0.1.2/oplangchain/document_loaders/onedrive.py
--rw-r--r--   0        0        0     1114 2023-08-08 04:52:52.589954 oplangchain-0.1.2/oplangchain/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0     1326 2023-08-08 04:52:52.588955 oplangchain-0.1.2/oplangchain/document_loaders/open_city_data.py
--rw-r--r--   0        0        0     1769 2023-08-08 04:52:52.587955 oplangchain-0.1.2/oplangchain/document_loaders/org_mode.py
--rw-r--r--   0        0        0      655 2023-08-08 04:52:52.610953 oplangchain-0.1.2/oplangchain/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0     6089 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0     2474 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0     5765 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0      101 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0     1608 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      119 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0      499 2023-08-07 21:21:40.586154 oplangchain-0.1.2/oplangchain/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0     2090 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0     4690 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0     1664 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0     8807 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0      920 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0      482 2023-08-08 04:52:52.611952 oplangchain-0.1.2/oplangchain/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0    20559 2023-08-08 04:52:52.586953 oplangchain-0.1.2/oplangchain/document_loaders/pdf.py
--rw-r--r--   0        0        0     2521 2023-08-08 04:52:52.586953 oplangchain-0.1.2/oplangchain/document_loaders/powerpoint.py
--rw-r--r--   0        0        0     1416 2023-08-08 04:52:52.585954 oplangchain-0.1.2/oplangchain/document_loaders/psychic.py
--rw-r--r--   0        0        0     3422 2023-08-08 04:52:52.585954 oplangchain-0.1.2/oplangchain/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0      527 2023-08-08 04:52:52.585954 oplangchain-0.1.2/oplangchain/document_loaders/python.py
--rw-r--r--   0        0        0     3530 2023-08-08 04:52:52.585954 oplangchain-0.1.2/oplangchain/document_loaders/readthedocs.py
--rw-r--r--   0        0        0    12432 2023-08-08 04:52:52.585954 oplangchain-0.1.2/oplangchain/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0     4609 2023-08-08 04:52:52.584953 oplangchain-0.1.2/oplangchain/document_loaders/reddit.py
--rw-r--r--   0        0        0      726 2023-08-08 04:52:52.584953 oplangchain-0.1.2/oplangchain/document_loaders/roam.py
--rw-r--r--   0        0        0     4441 2023-08-08 04:52:52.584953 oplangchain-0.1.2/oplangchain/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0     4938 2023-08-08 04:52:52.584953 oplangchain-0.1.2/oplangchain/document_loaders/rss.py
--rw-r--r--   0        0        0     1825 2023-08-08 04:52:52.584953 oplangchain-0.1.2/oplangchain/document_loaders/rst.py
--rw-r--r--   0        0        0     2054 2023-08-08 04:52:52.583955 oplangchain-0.1.2/oplangchain/document_loaders/rtf.py
--rw-r--r--   0        0        0     1231 2023-08-08 04:52:52.583955 oplangchain-0.1.2/oplangchain/document_loaders/s3_directory.py
--rw-r--r--   0        0        0     1322 2023-08-08 04:52:52.582954 oplangchain-0.1.2/oplangchain/document_loaders/s3_file.py
--rw-r--r--   0        0        0     5012 2023-08-08 04:52:52.582954 oplangchain-0.1.2/oplangchain/document_loaders/sitemap.py
--rw-r--r--   0        0        0     4184 2023-08-08 04:52:52.582954 oplangchain-0.1.2/oplangchain/document_loaders/slack_directory.py
--rw-r--r--   0        0        0     4830 2023-08-08 04:52:52.582954 oplangchain-0.1.2/oplangchain/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0     2065 2023-08-08 04:52:52.581954 oplangchain-0.1.2/oplangchain/document_loaders/spreedly.py
--rw-r--r--   0        0        0      891 2023-08-08 04:52:52.581954 oplangchain-0.1.2/oplangchain/document_loaders/srt.py
--rw-r--r--   0        0        0     1861 2023-08-08 04:52:52.580954 oplangchain-0.1.2/oplangchain/document_loaders/stripe.py
--rw-r--r--   0        0        0     9047 2023-08-08 04:52:52.580954 oplangchain-0.1.2/oplangchain/document_loaders/telegram.py
--rw-r--r--   0        0        0     1846 2023-08-08 04:52:52.579957 oplangchain-0.1.2/oplangchain/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0     1758 2023-08-08 04:52:52.579957 oplangchain-0.1.2/oplangchain/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0     1999 2023-08-08 04:52:52.580954 oplangchain-0.1.2/oplangchain/document_loaders/text.py
--rw-r--r--   0        0        0      998 2023-08-08 04:52:52.579957 oplangchain-0.1.2/oplangchain/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0     1653 2023-08-08 04:52:52.579957 oplangchain-0.1.2/oplangchain/document_loaders/toml.py
--rw-r--r--   0        0        0     6602 2023-08-08 04:52:52.579957 oplangchain-0.1.2/oplangchain/document_loaders/trello.py
--rw-r--r--   0        0        0     1282 2023-08-08 04:52:52.576954 oplangchain-0.1.2/oplangchain/document_loaders/tsv.py
--rw-r--r--   0        0        0     3458 2023-08-08 04:52:52.576954 oplangchain-0.1.2/oplangchain/document_loaders/twitter.py
--rw-r--r--   0        0        0    13889 2023-08-08 04:52:52.576954 oplangchain-0.1.2/oplangchain/document_loaders/unstructured.py
--rw-r--r--   0        0        0     6017 2023-08-08 04:52:52.574953 oplangchain-0.1.2/oplangchain/document_loaders/url.py
--rw-r--r--   0        0        0     4951 2023-08-08 04:52:52.574953 oplangchain-0.1.2/oplangchain/document_loaders/url_playwright.py
--rw-r--r--   0        0        0     5225 2023-08-08 04:52:52.574953 oplangchain-0.1.2/oplangchain/document_loaders/url_selenium.py
--rw-r--r--   0        0        0     1639 2023-08-08 04:52:52.570954 oplangchain-0.1.2/oplangchain/document_loaders/weather.py
--rw-r--r--   0        0        0     8015 2023-08-08 04:52:52.570954 oplangchain-0.1.2/oplangchain/document_loaders/web_base.py
--rw-r--r--   0        0        0     1765 2023-08-08 04:52:52.569953 oplangchain-0.1.2/oplangchain/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0     2188 2023-08-08 04:52:52.569953 oplangchain-0.1.2/oplangchain/document_loaders/wikipedia.py
--rw-r--r--   0        0        0     4561 2023-08-08 04:52:52.568953 oplangchain-0.1.2/oplangchain/document_loaders/word_document.py
--rw-r--r--   0        0        0     1483 2023-08-08 04:52:52.567953 oplangchain-0.1.2/oplangchain/document_loaders/xml.py
--rw-r--r--   0        0        0     1627 2023-08-08 04:52:52.567953 oplangchain-0.1.2/oplangchain/document_loaders/xorbits.py
--rw-r--r--   0        0        0    14680 2023-08-08 04:52:52.566956 oplangchain-0.1.2/oplangchain/document_loaders/youtube.py
--rw-r--r--   0        0        0     1452 2023-08-08 04:52:52.561953 oplangchain-0.1.2/oplangchain/document_transformers/__init__.py
--rw-r--r--   0        0        0     3452 2023-08-08 04:52:52.566956 oplangchain-0.1.2/oplangchain/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0     2176 2023-08-08 04:52:52.565955 oplangchain-0.1.2/oplangchain/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0     2320 2023-08-08 04:52:52.565955 oplangchain-0.1.2/oplangchain/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0     8084 2023-08-08 04:52:52.564953 oplangchain-0.1.2/oplangchain/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0     1297 2023-08-08 04:52:52.564953 oplangchain-0.1.2/oplangchain/document_transformers/html2text.py
--rw-r--r--   0        0        0     1376 2023-08-08 04:52:52.563954 oplangchain-0.1.2/oplangchain/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0     1473 2023-08-08 04:52:52.562953 oplangchain-0.1.2/oplangchain/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0     6220 2023-08-08 04:52:52.561953 oplangchain-0.1.2/oplangchain/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     4678 2023-08-08 04:52:52.547953 oplangchain-0.1.2/oplangchain/embeddings/__init__.py
--rw-r--r--   0        0        0     9596 2023-08-08 04:52:52.561953 oplangchain-0.1.2/oplangchain/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0     1633 2023-08-08 04:52:52.560954 oplangchain-0.1.2/oplangchain/embeddings/awa.py
--rw-r--r--   0        0        0      655 2023-08-07 21:21:40.614153 oplangchain-0.1.2/oplangchain/embeddings/base.py
--rw-r--r--   0        0        0     5484 2023-08-08 04:52:52.560954 oplangchain-0.1.2/oplangchain/embeddings/bedrock.py
--rw-r--r--   0        0        0     6553 2023-08-08 04:52:52.560954 oplangchain-0.1.2/oplangchain/embeddings/clarifai.py
--rw-r--r--   0        0        0     3383 2023-08-08 04:52:52.560954 oplangchain-0.1.2/oplangchain/embeddings/cohere.py
--rw-r--r--   0        0        0     4890 2023-08-08 04:52:52.560954 oplangchain-0.1.2/oplangchain/embeddings/dashscope.py
--rw-r--r--   0        0        0     4400 2023-08-08 04:52:52.557952 oplangchain-0.1.2/oplangchain/embeddings/deepinfra.py
--rw-r--r--   0        0        0     2798 2023-08-08 04:52:52.556953 oplangchain-0.1.2/oplangchain/embeddings/edenai.py
--rw-r--r--   0        0        0     8384 2023-08-08 04:52:52.555960 oplangchain-0.1.2/oplangchain/embeddings/elasticsearch.py
--rw-r--r--   0        0        0     4794 2023-08-08 04:52:52.554955 oplangchain-0.1.2/oplangchain/embeddings/embaas.py
--rw-r--r--   0        0        0     1497 2023-08-08 04:52:52.551953 oplangchain-0.1.2/oplangchain/embeddings/fake.py
--rw-r--r--   0        0        0     2686 2023-08-08 04:52:52.551953 oplangchain-0.1.2/oplangchain/embeddings/google_palm.py
--rw-r--r--   0        0        0     1641 2023-08-08 04:52:52.533954 oplangchain-0.1.2/oplangchain/embeddings/gpt4all.py
--rw-r--r--   0        0        0     6040 2023-08-08 04:52:52.537954 oplangchain-0.1.2/oplangchain/embeddings/huggingface.py
--rw-r--r--   0        0        0     3686 2023-08-08 04:52:52.550953 oplangchain-0.1.2/oplangchain/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0     3449 2023-08-08 04:52:52.538954 oplangchain-0.1.2/oplangchain/embeddings/jina.py
--rw-r--r--   0        0        0     4025 2023-08-08 04:52:52.542952 oplangchain-0.1.2/oplangchain/embeddings/llamacpp.py
--rw-r--r--   0        0        0    12079 2023-08-08 04:52:52.550953 oplangchain-0.1.2/oplangchain/embeddings/localai.py
--rw-r--r--   0        0        0     4690 2023-08-08 04:52:52.543952 oplangchain-0.1.2/oplangchain/embeddings/minimax.py
--rw-r--r--   0        0        0     2244 2023-08-08 04:52:52.543952 oplangchain-0.1.2/oplangchain/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0     2361 2023-08-08 04:52:52.550953 oplangchain-0.1.2/oplangchain/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0     5883 2023-08-08 04:52:52.545953 oplangchain-0.1.2/oplangchain/embeddings/mosaicml.py
--rw-r--r--   0        0        0     2176 2023-08-08 04:52:52.546953 oplangchain-0.1.2/oplangchain/embeddings/nlpcloud.py
--rw-r--r--   0        0        0     3402 2023-08-08 04:52:52.549953 oplangchain-0.1.2/oplangchain/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0    19945 2023-08-08 04:52:52.546953 oplangchain-0.1.2/oplangchain/embeddings/openai.py
--rw-r--r--   0        0        0     7110 2023-08-08 04:52:52.547953 oplangchain-0.1.2/oplangchain/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0     3755 2023-08-08 04:52:52.549953 oplangchain-0.1.2/oplangchain/embeddings/self_hosted.py
--rw-r--r--   0        0        0     6552 2023-08-08 04:52:52.547953 oplangchain-0.1.2/oplangchain/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      181 2023-08-08 04:52:52.547953 oplangchain-0.1.2/oplangchain/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0     3728 2023-08-08 04:52:52.547953 oplangchain-0.1.2/oplangchain/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0     2390 2023-08-08 04:52:52.547953 oplangchain-0.1.2/oplangchain/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0     1881 2023-08-08 04:52:52.547953 oplangchain-0.1.2/oplangchain/embeddings/vertexai.py
--rw-r--r--   0        0        0     3309 2023-08-08 04:52:52.547953 oplangchain-0.1.2/oplangchain/embeddings/xinference.py
--rw-r--r--   0        0        0      478 2023-08-08 04:52:52.346953 oplangchain-0.1.2/oplangchain/env.py
--rw-r--r--   0        0        0     5062 2023-08-08 04:52:52.517955 oplangchain-0.1.2/oplangchain/evaluation/__init__.py
--rw-r--r--   0        0        0      167 2023-08-08 04:52:52.526953 oplangchain-0.1.2/oplangchain/evaluation/agents/__init__.py
--rw-r--r--   0        0        0    13177 2023-08-08 04:52:52.530953 oplangchain-0.1.2/oplangchain/evaluation/agents/trajectory_eval_chain.py
--rw-r--r--   0        0        0     5939 2023-08-08 04:52:52.529956 oplangchain-0.1.2/oplangchain/evaluation/agents/trajectory_eval_prompt.py
--rw-r--r--   0        0        0     1404 2023-08-08 04:52:52.525951 oplangchain-0.1.2/oplangchain/evaluation/comparison/__init__.py
--rw-r--r--   0        0        0    15065 2023-08-08 04:52:52.526953 oplangchain-0.1.2/oplangchain/evaluation/comparison/eval_chain.py
--rw-r--r--   0        0        0     2177 2023-08-08 04:52:52.525951 oplangchain-0.1.2/oplangchain/evaluation/comparison/prompt.py
--rw-r--r--   0        0        0     1638 2023-08-08 04:52:52.525951 oplangchain-0.1.2/oplangchain/evaluation/criteria/__init__.py
--rw-r--r--   0        0        0    20332 2023-08-08 04:52:52.525951 oplangchain-0.1.2/oplangchain/evaluation/criteria/eval_chain.py
--rw-r--r--   0        0        0     1753 2023-08-08 04:52:52.525951 oplangchain-0.1.2/oplangchain/evaluation/criteria/prompt.py
--rw-r--r--   0        0        0      325 2023-08-08 04:52:52.522952 oplangchain-0.1.2/oplangchain/evaluation/embedding_distance/__init__.py
--rw-r--r--   0        0        0    15489 2023-08-08 04:52:52.524954 oplangchain-0.1.2/oplangchain/evaluation/embedding_distance/base.py
--rw-r--r--   0        0        0     5220 2023-08-08 04:52:52.518955 oplangchain-0.1.2/oplangchain/evaluation/loading.py
--rw-r--r--   0        0        0      348 2023-08-08 04:52:52.519953 oplangchain-0.1.2/oplangchain/evaluation/qa/__init__.py
--rw-r--r--   0        0        0    10001 2023-08-08 04:52:52.521954 oplangchain-0.1.2/oplangchain/evaluation/qa/eval_chain.py
--rw-r--r--   0        0        0     3908 2023-08-08 04:52:52.521954 oplangchain-0.1.2/oplangchain/evaluation/qa/eval_prompt.py
--rw-r--r--   0        0        0      966 2023-08-08 04:52:52.520955 oplangchain-0.1.2/oplangchain/evaluation/qa/generate_chain.py
--rw-r--r--   0        0        0      605 2023-08-08 04:52:52.520955 oplangchain-0.1.2/oplangchain/evaluation/qa/generate_prompt.py
--rw-r--r--   0        0        0    16806 2023-08-08 04:52:52.517955 oplangchain-0.1.2/oplangchain/evaluation/schema.py
--rw-r--r--   0        0        0      287 2023-08-08 04:52:52.518955 oplangchain-0.1.2/oplangchain/evaluation/string_distance/__init__.py
--rw-r--r--   0        0        0    14008 2023-08-08 04:52:52.518955 oplangchain-0.1.2/oplangchain/evaluation/string_distance/base.py
--rw-r--r--   0        0        0      143 2023-08-08 04:52:52.346953 oplangchain-0.1.2/oplangchain/example_generator.py
--rw-r--r--   0        0        0      164 2023-08-08 04:52:52.346953 oplangchain-0.1.2/oplangchain/formatting.py
--rw-r--r--   0        0        0      769 2023-08-08 04:52:52.530953 oplangchain-0.1.2/oplangchain/graphs/__init__.py
--rw-r--r--   0        0        0     6198 2023-08-07 21:21:40.642153 oplangchain-0.1.2/oplangchain/graphs/arangodb_graph.py
--rw-r--r--   0        0        0     1841 2023-08-07 21:21:40.643153 oplangchain-0.1.2/oplangchain/graphs/hugegraph.py
--rw-r--r--   0        0        0     3559 2023-08-07 21:21:40.643153 oplangchain-0.1.2/oplangchain/graphs/kuzu_graph.py
--rw-r--r--   0        0        0      715 2023-08-08 04:52:52.532953 oplangchain-0.1.2/oplangchain/graphs/memgraph_graph.py
--rw-r--r--   0        0        0     7362 2023-08-07 21:21:40.644153 oplangchain-0.1.2/oplangchain/graphs/nebula_graph.py
--rw-r--r--   0        0        0     3625 2023-08-07 21:21:40.645154 oplangchain-0.1.2/oplangchain/graphs/neo4j_graph.py
--rw-r--r--   0        0        0     6553 2023-08-07 21:21:40.645154 oplangchain-0.1.2/oplangchain/graphs/neptune_graph.py
--rw-r--r--   0        0        0     5877 2023-08-07 21:21:40.646154 oplangchain-0.1.2/oplangchain/graphs/networkx_graph.py
--rw-r--r--   0        0        0     9461 2023-08-07 21:21:40.646154 oplangchain-0.1.2/oplangchain/graphs/rdf_graph.py
--rw-r--r--   0        0        0      211 2023-08-08 04:52:52.496954 oplangchain-0.1.2/oplangchain/indexes/__init__.py
--rw-r--r--   0        0        0     1722 2023-08-08 04:52:52.496954 oplangchain-0.1.2/oplangchain/indexes/graph.py
--rw-r--r--   0        0        0       49 2023-08-07 21:21:40.648155 oplangchain-0.1.2/oplangchain/indexes/prompts/__init__.py
--rw-r--r--   0        0        0     1949 2023-08-08 04:52:52.499953 oplangchain-0.1.2/oplangchain/indexes/prompts/entity_extraction.py
--rw-r--r--   0        0        0     1154 2023-08-08 04:52:52.497954 oplangchain-0.1.2/oplangchain/indexes/prompts/entity_summarization.py
--rw-r--r--   0        0        0     1588 2023-08-08 04:52:52.498952 oplangchain-0.1.2/oplangchain/indexes/prompts/knowledge_triplet_extraction.py
--rw-r--r--   0        0        0     3070 2023-08-08 04:52:52.496954 oplangchain-0.1.2/oplangchain/indexes/vectorstore.py
--rw-r--r--   0        0        0      279 2023-08-08 04:52:52.346953 oplangchain-0.1.2/oplangchain/input.py
--rw-r--r--   0        0        0     6508 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/__init__.py
--rw-r--r--   0        0        0     5004 2023-08-08 04:52:52.517955 oplangchain-0.1.2/oplangchain/llms/ai21.py
--rw-r--r--   0        0        0    11362 2023-08-08 04:52:52.517955 oplangchain-0.1.2/oplangchain/llms/aleph_alpha.py
--rw-r--r--   0        0        0     3029 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0    11178 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/anthropic.py
--rw-r--r--   0        0        0     4667 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/anyscale.py
--rw-r--r--   0        0        0     5375 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/aviary.py
--rw-r--r--   0        0        0    10224 2023-08-08 04:52:52.505530 oplangchain-0.1.2/oplangchain/llms/azureml_endpoint.py
--rw-r--r--   0        0        0     4319 2023-08-08 04:52:52.505952 oplangchain-0.1.2/oplangchain/llms/bananadev.py
--rw-r--r--   0        0        0    34755 2023-08-08 05:09:17.579726 oplangchain-0.1.2/oplangchain/llms/base.py
--rw-r--r--   0        0        0     2365 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/baseten.py
--rw-r--r--   0        0        0     9070 2023-08-08 04:52:52.507954 oplangchain-0.1.2/oplangchain/llms/beam.py
--rw-r--r--   0        0        0     6698 2023-08-08 04:52:52.508955 oplangchain-0.1.2/oplangchain/llms/bedrock.py
--rw-r--r--   0        0        0     3783 2023-08-08 04:52:52.508955 oplangchain-0.1.2/oplangchain/llms/cerebriumai.py
--rw-r--r--   0        0        0     3945 2023-08-08 04:52:52.508955 oplangchain-0.1.2/oplangchain/llms/chatglm.py
--rw-r--r--   0        0        0     5812 2023-08-08 04:52:52.508955 oplangchain-0.1.2/oplangchain/llms/clarifai.py
--rw-r--r--   0        0        0     7313 2023-08-08 04:52:52.508955 oplangchain-0.1.2/oplangchain/llms/cohere.py
--rw-r--r--   0        0        0     4193 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/ctransformers.py
--rw-r--r--   0        0        0    12072 2023-08-08 04:52:52.508955 oplangchain-0.1.2/oplangchain/llms/databricks.py
--rw-r--r--   0        0        0     3765 2023-08-08 04:52:52.508955 oplangchain-0.1.2/oplangchain/llms/deepinfra.py
--rw-r--r--   0        0        0     7455 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/edenai.py
--rw-r--r--   0        0        0     1339 2023-08-08 04:52:52.509954 oplangchain-0.1.2/oplangchain/llms/fake.py
--rw-r--r--   0        0        0    13047 2023-08-08 04:52:52.510953 oplangchain-0.1.2/oplangchain/llms/fireworks.py
--rw-r--r--   0        0        0     3661 2023-08-08 04:52:52.510953 oplangchain-0.1.2/oplangchain/llms/forefrontai.py
--rw-r--r--   0        0        0     5741 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/google_palm.py
--rw-r--r--   0        0        0     5130 2023-08-08 04:52:52.511953 oplangchain-0.1.2/oplangchain/llms/gooseai.py
--rw-r--r--   0        0        0     6320 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/gpt4all.py
--rw-r--r--   0        0        0     5462 2023-08-08 04:52:52.511953 oplangchain-0.1.2/oplangchain/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0     4613 2023-08-08 04:52:52.511953 oplangchain-0.1.2/oplangchain/llms/huggingface_hub.py
--rw-r--r--   0        0        0     6576 2023-08-08 04:52:52.512955 oplangchain-0.1.2/oplangchain/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0     9723 2023-08-08 04:52:52.512955 oplangchain-0.1.2/oplangchain/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0     2547 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/human.py
--rw-r--r--   0        0        0     5071 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/koboldai.py
--rw-r--r--   0        0        0    10905 2023-08-08 04:52:52.512955 oplangchain-0.1.2/oplangchain/llms/llamacpp.py
--rw-r--r--   0        0        0     1253 2023-08-08 04:52:52.512955 oplangchain-0.1.2/oplangchain/llms/loading.py
--rw-r--r--   0        0        0     1878 2023-08-08 04:52:52.512955 oplangchain-0.1.2/oplangchain/llms/manifest.py
--rw-r--r--   0        0        0     5162 2023-08-08 04:52:52.512955 oplangchain-0.1.2/oplangchain/llms/minimax.py
--rw-r--r--   0        0        0     2925 2023-08-08 04:52:52.516955 oplangchain-0.1.2/oplangchain/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0     3247 2023-08-08 04:52:52.512955 oplangchain-0.1.2/oplangchain/llms/modal.py
--rw-r--r--   0        0        0     6752 2023-08-08 04:52:52.512955 oplangchain-0.1.2/oplangchain/llms/mosaicml.py
--rw-r--r--   0        0        0     5450 2023-08-08 04:52:52.513954 oplangchain-0.1.2/oplangchain/llms/nlpcloud.py
--rw-r--r--   0        0        0     3814 2023-08-08 04:52:52.513954 oplangchain-0.1.2/oplangchain/llms/octoai_endpoint.py
--rw-r--r--   0        0        0    34744 2023-08-08 04:52:52.513954 oplangchain-0.1.2/oplangchain/llms/openai.py
--rw-r--r--   0        0        0     9930 2023-08-08 04:52:52.514953 oplangchain-0.1.2/oplangchain/llms/openllm.py
--rw-r--r--   0        0        0      796 2023-08-08 04:52:52.514953 oplangchain-0.1.2/oplangchain/llms/openlm.py
--rw-r--r--   0        0        0     5273 2023-08-08 04:52:52.514953 oplangchain-0.1.2/oplangchain/llms/petals.py
--rw-r--r--   0        0        0     4023 2023-08-08 04:52:52.514953 oplangchain-0.1.2/oplangchain/llms/pipelineai.py
--rw-r--r--   0        0        0     1531 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/predibase.py
--rw-r--r--   0        0        0     4372 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/predictionguard.py
--rw-r--r--   0        0        0     8692 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/promptlayer_openai.py
--rw-r--r--   0        0        0     5168 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/replicate.py
--rw-r--r--   0        0        0     7343 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/rwkv.py
--rw-r--r--   0        0        0     8821 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0     7685 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/self_hosted.py
--rw-r--r--   0        0        0     7699 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0     4573 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/stochasticai.py
--rw-r--r--   0        0        0     7587 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/textgen.py
--rw-r--r--   0        0        0     7882 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/tongyi.py
--rw-r--r--   0        0        0      246 2023-08-07 21:21:40.678154 oplangchain-0.1.2/oplangchain/llms/utils.py
--rw-r--r--   0        0        0     7717 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/vertexai.py
--rw-r--r--   0        0        0     3984 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/vllm.py
--rw-r--r--   0        0        0     4919 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/writer.py
--rw-r--r--   0        0        0     6017 2023-08-08 04:52:52.515962 oplangchain-0.1.2/oplangchain/llms/xinference.py
--rw-r--r--   0        0        0       41 2023-08-07 21:21:40.680153 oplangchain-0.1.2/oplangchain/load/__init__.py
--rw-r--r--   0        0        0      755 2023-08-08 04:52:52.496954 oplangchain-0.1.2/oplangchain/load/dump.py
--rw-r--r--   0        0        0     4039 2023-08-08 04:52:52.496954 oplangchain-0.1.2/oplangchain/load/load.py
--rw-r--r--   0        0        0     4618 2023-08-07 21:21:40.681154 oplangchain-0.1.2/oplangchain/load/serializable.py
--rw-r--r--   0        0        0     2872 2023-08-08 04:52:52.479955 oplangchain-0.1.2/oplangchain/memory/__init__.py
--rw-r--r--   0        0        0     3074 2023-08-08 04:52:52.490953 oplangchain-0.1.2/oplangchain/memory/buffer.py
--rw-r--r--   0        0        0     1232 2023-08-08 04:52:52.485953 oplangchain-0.1.2/oplangchain/memory/buffer_window.py
--rw-r--r--   0        0        0     1618 2023-08-08 04:52:52.485953 oplangchain-0.1.2/oplangchain/memory/chat_memory.py
--rw-r--r--   0        0        0     1592 2023-08-08 04:52:52.490953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/__init__.py
--rw-r--r--   0        0        0     2371 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0     6497 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0     2885 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0     1366 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/file.py
--rw-r--r--   0        0        0     3336 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      588 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0     6835 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/momento.py
--rw-r--r--   0        0        0     2723 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0     2648 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/postgres.py
--rw-r--r--   0        0        0     1951 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/redis.py
--rw-r--r--   0        0        0     2901 2023-08-08 04:52:52.492952 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/sql.py
--rw-r--r--   0        0        0     1180 2023-08-08 04:52:52.492952 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0     6406 2023-08-08 04:52:52.492952 oplangchain-0.1.2/oplangchain/memory/chat_message_histories/zep.py
--rw-r--r--   0        0        0     2893 2023-08-08 04:52:52.483955 oplangchain-0.1.2/oplangchain/memory/combined.py
--rw-r--r--   0        0        0    12998 2023-08-08 04:52:52.482954 oplangchain-0.1.2/oplangchain/memory/entity.py
--rw-r--r--   0        0        0     5035 2023-08-08 04:52:52.475954 oplangchain-0.1.2/oplangchain/memory/kg.py
--rw-r--r--   0        0        0     3102 2023-08-08 04:52:52.475954 oplangchain-0.1.2/oplangchain/memory/motorhead_memory.py
--rw-r--r--   0        0        0     8178 2023-08-08 04:52:52.482954 oplangchain-0.1.2/oplangchain/memory/prompt.py
--rw-r--r--   0        0        0      791 2023-08-08 04:52:52.476953 oplangchain-0.1.2/oplangchain/memory/readonly.py
--rw-r--r--   0        0        0      758 2023-08-08 04:52:52.482954 oplangchain-0.1.2/oplangchain/memory/simple.py
--rw-r--r--   0        0        0     3354 2023-08-08 04:52:52.482954 oplangchain-0.1.2/oplangchain/memory/summary.py
--rw-r--r--   0        0        0     2939 2023-08-08 04:52:52.478954 oplangchain-0.1.2/oplangchain/memory/summary_buffer.py
--rw-r--r--   0        0        0     1921 2023-08-08 04:52:52.481955 oplangchain-0.1.2/oplangchain/memory/token_buffer.py
--rw-r--r--   0        0        0      689 2023-08-08 04:52:52.481955 oplangchain-0.1.2/oplangchain/memory/utils.py
--rw-r--r--   0        0        0     2984 2023-08-08 04:52:52.480955 oplangchain-0.1.2/oplangchain/memory/vectorstore.py
--rw-r--r--   0        0        0     5071 2023-08-08 04:52:52.479955 oplangchain-0.1.2/oplangchain/memory/zep_memory.py
--rw-r--r--   0        0        0     3246 2023-08-08 04:52:52.346953 oplangchain-0.1.2/oplangchain/model_laboratory.py
--rw-r--r--   0        0        0     1612 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     1073 2023-08-08 04:52:52.496954 oplangchain-0.1.2/oplangchain/output_parsers/boolean.py
--rw-r--r--   0        0        0     1765 2023-08-08 04:52:52.496954 oplangchain-0.1.2/oplangchain/output_parsers/combining.py
--rw-r--r--   0        0        0     1821 2023-08-08 04:52:52.496954 oplangchain-0.1.2/oplangchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1140 2023-08-08 04:52:52.495954 oplangchain-0.1.2/oplangchain/output_parsers/enum.py
--rw-r--r--   0        0        0     1813 2023-08-08 04:52:52.495954 oplangchain-0.1.2/oplangchain/output_parsers/fix.py
--rw-r--r--   0        0        0      810 2023-08-07 21:21:40.702154 oplangchain-0.1.2/oplangchain/output_parsers/format_instructions.py
--rw-r--r--   0        0        0     2211 2023-08-08 04:52:52.494953 oplangchain-0.1.2/oplangchain/output_parsers/json.py
--rw-r--r--   0        0        0      941 2023-08-08 04:52:52.494953 oplangchain-0.1.2/oplangchain/output_parsers/list.py
--rw-r--r--   0        0        0      704 2023-08-08 04:52:52.494953 oplangchain-0.1.2/oplangchain/output_parsers/loading.py
--rw-r--r--   0        0        0     3354 2023-08-08 04:52:52.494953 oplangchain-0.1.2/oplangchain/output_parsers/openai_functions.py
--rw-r--r--   0        0        0      505 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/output_parsers/prompts.py
--rw-r--r--   0        0        0     1735 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/output_parsers/pydantic.py
--rw-r--r--   0        0        0     3167 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/output_parsers/rail_parser.py
--rw-r--r--   0        0        0     1198 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/output_parsers/regex.py
--rw-r--r--   0        0        0     1698 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/output_parsers/regex_dict.py
--rw-r--r--   0        0        0     4717 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/output_parsers/retry.py
--rw-r--r--   0        0        0     3078 2023-08-08 04:52:52.493953 oplangchain-0.1.2/oplangchain/output_parsers/structured.py
--rw-r--r--   0        0        0     2762 2023-08-08 04:52:52.467952 oplangchain-0.1.2/oplangchain/prompts/__init__.py
--rw-r--r--   0        0        0     3679 2023-08-08 04:52:52.474953 oplangchain-0.1.2/oplangchain/prompts/base.py
--rw-r--r--   0        0        0    21577 2023-08-08 04:52:52.474953 oplangchain-0.1.2/oplangchain/prompts/chat.py
--rw-r--r--   0        0        0      559 2023-08-08 04:52:52.474953 oplangchain-0.1.2/oplangchain/prompts/example_selector/__init__.py
--rw-r--r--   0        0        0      526 2023-08-07 21:21:40.709154 oplangchain-0.1.2/oplangchain/prompts/example_selector/base.py
--rw-r--r--   0        0        0     2437 2023-08-08 04:52:52.474953 oplangchain-0.1.2/oplangchain/prompts/example_selector/length_based.py
--rw-r--r--   0        0        0     3802 2023-08-08 04:52:52.474953 oplangchain-0.1.2/oplangchain/prompts/example_selector/ngram_overlap.py
--rw-r--r--   0        0        0     6854 2023-08-08 04:52:52.474953 oplangchain-0.1.2/oplangchain/prompts/example_selector/semantic_similarity.py
--rw-r--r--   0        0        0    11763 2023-08-08 04:52:52.472955 oplangchain-0.1.2/oplangchain/prompts/few_shot.py
--rw-r--r--   0        0        0     5429 2023-08-08 04:52:52.472955 oplangchain-0.1.2/oplangchain/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0     5519 2023-08-08 04:52:52.467952 oplangchain-0.1.2/oplangchain/prompts/loading.py
--rw-r--r--   0        0        0     2258 2023-08-08 04:52:52.468953 oplangchain-0.1.2/oplangchain/prompts/pipeline.py
--rw-r--r--   0        0        0     8140 2023-08-08 04:52:52.465953 oplangchain-0.1.2/oplangchain/prompts/prompt.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.713154 oplangchain-0.1.2/oplangchain/py.typed
--rw-r--r--   0        0        0      113 2023-08-08 04:52:52.345954 oplangchain-0.1.2/oplangchain/python.py
--rw-r--r--   0        0        0      214 2023-08-08 04:52:52.342954 oplangchain-0.1.2/oplangchain/requests.py
--rw-r--r--   0        0        0     3676 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/__init__.py
--rw-r--r--   0        0        0      588 2023-08-08 04:52:52.452954 oplangchain-0.1.2/oplangchain/retrievers/arxiv.py
--rw-r--r--   0        0        0     4048 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/azure_cognitive_search.py
--rw-r--r--   0        0        0     3657 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/bm25.py
--rw-r--r--   0        0        0     2653 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/chaindesk.py
--rw-r--r--   0        0        0     3002 2023-08-08 04:52:52.456954 oplangchain-0.1.2/oplangchain/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0     2261 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/contextual_compression.py
--rw-r--r--   0        0        0     2307 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/databerry.py
--rw-r--r--   0        0        0     6738 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/docarray.py
--rw-r--r--   0        0        0      601 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/document_compressors/__init__.py
--rw-r--r--   0        0        0     3662 2023-08-08 04:52:52.458953 oplangchain-0.1.2/oplangchain/retrievers/document_compressors/base.py
--rw-r--r--   0        0        0     3825 2023-08-08 04:52:52.458953 oplangchain-0.1.2/oplangchain/retrievers/document_compressors/chain_extract.py
--rw-r--r--   0        0        0      366 2023-08-07 21:21:40.721154 oplangchain-0.1.2/oplangchain/retrievers/document_compressors/chain_extract_prompt.py
--rw-r--r--   0        0        0     2979 2023-08-08 04:52:52.457954 oplangchain-0.1.2/oplangchain/retrievers/document_compressors/chain_filter.py
--rw-r--r--   0        0        0      231 2023-08-07 21:21:40.722154 oplangchain-0.1.2/oplangchain/retrievers/document_compressors/chain_filter_prompt.py
--rw-r--r--   0        0        0     2969 2023-08-08 04:52:52.457954 oplangchain-0.1.2/oplangchain/retrievers/document_compressors/cohere_rerank.py
--rw-r--r--   0        0        0     3151 2023-08-08 04:52:52.457954 oplangchain-0.1.2/oplangchain/retrievers/document_compressors/embeddings_filter.py
--rw-r--r--   0        0        0     4664 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0     5797 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/ensemble.py
--rw-r--r--   0        0        0     7436 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/google_cloud_enterprise_search.py
--rw-r--r--   0        0        0    12607 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/kendra.py
--rw-r--r--   0        0        0     2533 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/knn.py
--rw-r--r--   0        0        0     3026 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/llama_index.py
--rw-r--r--   0        0        0     3377 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/merger_retriever.py
--rw-r--r--   0        0        0     1443 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/metal.py
--rw-r--r--   0        0        0     2385 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/milvus.py
--rw-r--r--   0        0        0     4846 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/multi_query.py
--rw-r--r--   0        0        0     5442 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0      598 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/pubmed.py
--rw-r--r--   0        0        0       96 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/pupmed.py
--rw-r--r--   0        0        0     2611 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/re_phraser.py
--rw-r--r--   0        0        0     1907 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/remote_retriever.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.731154 oplangchain-0.1.2/oplangchain/retrievers/self_query/__init__.py
--rw-r--r--   0        0        0     5973 2023-08-08 04:52:52.465953 oplangchain-0.1.2/oplangchain/retrievers/self_query/base.py
--rw-r--r--   0        0        0     1444 2023-08-08 04:52:52.464953 oplangchain-0.1.2/oplangchain/retrievers/self_query/chroma.py
--rw-r--r--   0        0        0     2594 2023-08-08 04:52:52.462957 oplangchain-0.1.2/oplangchain/retrievers/self_query/deeplake.py
--rw-r--r--   0        0        0     3597 2023-08-08 04:52:52.462957 oplangchain-0.1.2/oplangchain/retrievers/self_query/myscale.py
--rw-r--r--   0        0        0     1450 2023-08-08 04:52:52.462957 oplangchain-0.1.2/oplangchain/retrievers/self_query/pinecone.py
--rw-r--r--   0        0        0     2813 2023-08-08 04:52:52.462957 oplangchain-0.1.2/oplangchain/retrievers/self_query/qdrant.py
--rw-r--r--   0        0        0     1503 2023-08-08 04:52:52.459954 oplangchain-0.1.2/oplangchain/retrievers/self_query/weaviate.py
--rw-r--r--   0        0        0     3663 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/svm.py
--rw-r--r--   0        0        0     4039 2023-08-08 04:52:52.454955 oplangchain-0.1.2/oplangchain/retrievers/tfidf.py
--rw-r--r--   0        0        0     5818 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/time_weighted_retriever.py
--rw-r--r--   0        0        0     4601 2023-08-08 04:52:52.455957 oplangchain-0.1.2/oplangchain/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0     4059 2023-08-08 04:52:52.454955 oplangchain-0.1.2/oplangchain/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0     8302 2023-08-08 04:52:52.454955 oplangchain-0.1.2/oplangchain/retrievers/web_research.py
--rw-r--r--   0        0        0      611 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/wikipedia.py
--rw-r--r--   0        0        0     3075 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/zep.py
--rw-r--r--   0        0        0     2679 2023-08-08 04:52:52.453954 oplangchain-0.1.2/oplangchain/retrievers/zilliz.py
--rw-r--r--   0        0        0     1736 2023-08-08 04:52:52.443954 oplangchain-0.1.2/oplangchain/schema/__init__.py
--rw-r--r--   0        0        0      643 2023-08-07 21:21:40.739154 oplangchain-0.1.2/oplangchain/schema/agent.py
--rw-r--r--   0        0        0     2658 2023-08-08 04:52:52.452954 oplangchain-0.1.2/oplangchain/schema/document.py
--rw-r--r--   0        0        0    10183 2023-08-08 04:52:52.452954 oplangchain-0.1.2/oplangchain/schema/language_model.py
--rw-r--r--   0        0        0     4099 2023-08-08 04:52:52.451953 oplangchain-0.1.2/oplangchain/schema/memory.py
--rw-r--r--   0        0        0     7490 2023-08-08 04:52:52.451953 oplangchain-0.1.2/oplangchain/schema/messages.py
--rw-r--r--   0        0        0     5451 2023-08-08 04:52:52.451953 oplangchain-0.1.2/oplangchain/schema/output.py
--rw-r--r--   0        0        0     7792 2023-08-08 04:52:52.451953 oplangchain-0.1.2/oplangchain/schema/output_parser.py
--rw-r--r--   0        0        0      638 2023-08-08 04:52:52.451953 oplangchain-0.1.2/oplangchain/schema/prompt.py
--rw-r--r--   0        0        0     6879 2023-08-08 04:52:52.451953 oplangchain-0.1.2/oplangchain/schema/prompt_template.py
--rw-r--r--   0        0        0    10059 2023-08-08 04:52:52.450953 oplangchain-0.1.2/oplangchain/schema/retriever.py
--rw-r--r--   0        0        0    40398 2023-08-08 04:52:52.448953 oplangchain-0.1.2/oplangchain/schema/runnable.py
--rw-r--r--   0        0        0      122 2023-08-08 04:52:52.341954 oplangchain-0.1.2/oplangchain/serpapi.py
--rw-r--r--   0        0        0      533 2023-08-07 21:21:40.745154 oplangchain-0.1.2/oplangchain/server.py
--rw-r--r--   0        0        0     3571 2023-08-08 04:52:52.439954 oplangchain-0.1.2/oplangchain/smith/__init__.py
--rw-r--r--   0        0        0     2201 2023-08-08 04:52:52.439954 oplangchain-0.1.2/oplangchain/smith/evaluation/__init__.py
--rw-r--r--   0        0        0     8581 2023-08-08 04:52:52.443954 oplangchain-0.1.2/oplangchain/smith/evaluation/config.py
--rw-r--r--   0        0        0    51540 2023-08-08 04:52:52.440954 oplangchain-0.1.2/oplangchain/smith/evaluation/runner_utils.py
--rw-r--r--   0        0        0    15823 2023-08-08 04:52:52.439954 oplangchain-0.1.2/oplangchain/smith/evaluation/string_run_evaluator.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.748154 oplangchain-0.1.2/oplangchain/smith/evaluation/utils.py
--rw-r--r--   0        0        0      131 2023-08-08 04:52:52.339954 oplangchain-0.1.2/oplangchain/sql_database.py
--rw-r--r--   0        0        0    38443 2023-08-08 04:52:52.339954 oplangchain-0.1.2/oplangchain/text_splitter.py
--rw-r--r--   0        0        0     6686 2023-08-08 04:52:52.386955 oplangchain-0.1.2/oplangchain/tools/__init__.py
--rw-r--r--   0        0        0      241 2023-08-08 04:52:52.438954 oplangchain-0.1.2/oplangchain/tools/amadeus/__init__.py
--rw-r--r--   0        0        0      411 2023-08-08 04:52:52.439954 oplangchain-0.1.2/oplangchain/tools/amadeus/base.py
--rw-r--r--   0        0        0     1982 2023-08-08 04:52:52.439954 oplangchain-0.1.2/oplangchain/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0     5561 2023-08-08 04:52:52.439954 oplangchain-0.1.2/oplangchain/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0     1123 2023-08-07 21:21:40.753154 oplangchain-0.1.2/oplangchain/tools/amadeus/utils.py
--rw-r--r--   0        0        0       25 2023-08-07 21:21:40.753154 oplangchain-0.1.2/oplangchain/tools/arxiv/__init__.py
--rw-r--r--   0        0        0     1006 2023-08-08 04:52:52.438954 oplangchain-0.1.2/oplangchain/tools/arxiv/tool.py
--rw-r--r--   0        0        0      603 2023-08-08 04:52:52.436954 oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0     5334 2023-08-08 04:52:52.438954 oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0     5263 2023-08-08 04:52:52.438954 oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0     4304 2023-08-08 04:52:52.438954 oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0     3652 2023-08-08 04:52:52.436954 oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0      776 2023-08-07 21:21:40.757154 oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/utils.py
--rw-r--r--   0        0        0    26849 2023-08-08 04:52:52.392956 oplangchain-0.1.2/oplangchain/tools/base.py
--rw-r--r--   0        0        0      162 2023-08-08 04:52:52.436954 oplangchain-0.1.2/oplangchain/tools/bing_search/__init__.py
--rw-r--r--   0        0        0     1441 2023-08-08 04:52:52.436954 oplangchain-0.1.2/oplangchain/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.759154 oplangchain-0.1.2/oplangchain/tools/brave_search/__init__.py
--rw-r--r--   0        0        0     1342 2023-08-08 04:52:52.436954 oplangchain-0.1.2/oplangchain/tools/brave_search/tool.py
--rw-r--r--   0        0        0     1738 2023-08-08 04:52:52.390954 oplangchain-0.1.2/oplangchain/tools/convert_to_openai.py
--rw-r--r--   0        0        0      260 2023-08-08 04:52:52.435953 oplangchain-0.1.2/oplangchain/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0     2182 2023-08-08 04:52:52.435953 oplangchain-0.1.2/oplangchain/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      139 2023-08-08 04:52:52.436954 oplangchain-0.1.2/oplangchain/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0     2321 2023-08-08 04:52:52.436954 oplangchain-0.1.2/oplangchain/tools/ddg_search/tool.py
--rw-r--r--   0        0        0      667 2023-08-08 04:52:52.428954 oplangchain-0.1.2/oplangchain/tools/file_management/__init__.py
--rw-r--r--   0        0        0     1730 2023-08-08 04:52:52.433955 oplangchain-0.1.2/oplangchain/tools/file_management/copy.py
--rw-r--r--   0        0        0     1326 2023-08-08 04:52:52.433955 oplangchain-0.1.2/oplangchain/tools/file_management/delete.py
--rw-r--r--   0        0        0     1946 2023-08-08 04:52:52.432954 oplangchain-0.1.2/oplangchain/tools/file_management/file_search.py
--rw-r--r--   0        0        0     1413 2023-08-08 04:52:52.431953 oplangchain-0.1.2/oplangchain/tools/file_management/list_dir.py
--rw-r--r--   0        0        0     1870 2023-08-08 04:52:52.428954 oplangchain-0.1.2/oplangchain/tools/file_management/move.py
--rw-r--r--   0        0        0     1321 2023-08-08 04:52:52.428954 oplangchain-0.1.2/oplangchain/tools/file_management/read.py
--rw-r--r--   0        0        0     1708 2023-08-07 21:21:40.767154 oplangchain-0.1.2/oplangchain/tools/file_management/utils.py
--rw-r--r--   0        0        0     1595 2023-08-08 04:52:52.422954 oplangchain-0.1.2/oplangchain/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2023-08-07 21:21:40.768154 oplangchain-0.1.2/oplangchain/tools/github/__init__.py
--rw-r--r--   0        0        0     3438 2023-08-07 21:21:40.769155 oplangchain-0.1.2/oplangchain/tools/github/prompt.py
--rw-r--r--   0        0        0      927 2023-08-08 04:52:52.422954 oplangchain-0.1.2/oplangchain/tools/github/tool.py
--rw-r--r--   0        0        0      553 2023-08-08 04:52:52.418954 oplangchain-0.1.2/oplangchain/tools/gmail/__init__.py
--rw-r--r--   0        0        0      980 2023-08-08 04:52:52.422954 oplangchain-0.1.2/oplangchain/tools/gmail/base.py
--rw-r--r--   0        0        0     2543 2023-08-08 04:52:52.420954 oplangchain-0.1.2/oplangchain/tools/gmail/create_draft.py
--rw-r--r--   0        0        0     1733 2023-08-08 04:52:52.416952 oplangchain-0.1.2/oplangchain/tools/gmail/get_message.py
--rw-r--r--   0        0        0     1539 2023-08-08 04:52:52.420954 oplangchain-0.1.2/oplangchain/tools/gmail/get_thread.py
--rw-r--r--   0        0        0     4369 2023-08-08 04:52:52.416952 oplangchain-0.1.2/oplangchain/tools/gmail/search.py
--rw-r--r--   0        0        0     2851 2023-08-08 04:52:52.417953 oplangchain-0.1.2/oplangchain/tools/gmail/send_message.py
--rw-r--r--   0        0        0     4528 2023-08-07 21:21:40.773153 oplangchain-0.1.2/oplangchain/tools/gmail/utils.py
--rw-r--r--   0        0        0      128 2023-08-08 04:52:52.416952 oplangchain-0.1.2/oplangchain/tools/golden_query/__init__.py
--rw-r--r--   0        0        0     1096 2023-08-08 04:52:52.416952 oplangchain-0.1.2/oplangchain/tools/golden_query/tool.py
--rw-r--r--   0        0        0      132 2023-08-08 04:52:52.415952 oplangchain-0.1.2/oplangchain/tools/google_places/__init__.py
--rw-r--r--   0        0        0     1112 2023-08-08 04:52:52.416952 oplangchain-0.1.2/oplangchain/tools/google_places/tool.py
--rw-r--r--   0        0        0      174 2023-08-08 04:52:52.415952 oplangchain-0.1.2/oplangchain/tools/google_search/__init__.py
--rw-r--r--   0        0        0     1467 2023-08-08 04:52:52.415952 oplangchain-0.1.2/oplangchain/tools/google_search/tool.py
--rw-r--r--   0        0        0      222 2023-08-08 04:52:52.415952 oplangchain-0.1.2/oplangchain/tools/google_serper/__init__.py
--rw-r--r--   0        0        0     2082 2023-08-08 04:52:52.415952 oplangchain-0.1.2/oplangchain/tools/google_serper/tool.py
--rw-r--r--   0        0        0       47 2023-08-07 21:21:40.778154 oplangchain-0.1.2/oplangchain/tools/graphql/__init__.py
--rw-r--r--   0        0        0     1192 2023-08-08 04:52:52.415952 oplangchain-0.1.2/oplangchain/tools/graphql/tool.py
--rw-r--r--   0        0        0      124 2023-08-08 04:52:52.415952 oplangchain-0.1.2/oplangchain/tools/human/__init__.py
--rw-r--r--   0        0        0      963 2023-08-08 04:52:52.415952 oplangchain-0.1.2/oplangchain/tools/human/tool.py
--rw-r--r--   0        0        0     2294 2023-08-08 04:52:52.389957 oplangchain-0.1.2/oplangchain/tools/ifttt.py
--rw-r--r--   0        0        0       43 2023-08-07 21:21:40.781153 oplangchain-0.1.2/oplangchain/tools/interaction/__init__.py
--rw-r--r--   0        0        0      456 2023-08-08 04:52:52.415933 oplangchain-0.1.2/oplangchain/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2023-08-07 21:21:40.782154 oplangchain-0.1.2/oplangchain/tools/jira/__init__.py
--rw-r--r--   0        0        0     3170 2023-08-07 21:21:40.783154 oplangchain-0.1.2/oplangchain/tools/jira/prompt.py
--rw-r--r--   0        0        0     1585 2023-08-08 04:52:52.414953 oplangchain-0.1.2/oplangchain/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2023-08-07 21:21:40.784153 oplangchain-0.1.2/oplangchain/tools/json/__init__.py
--rw-r--r--   0        0        0     4091 2023-08-08 04:52:52.414953 oplangchain-0.1.2/oplangchain/tools/json/tool.py
--rw-r--r--   0        0        0      146 2023-08-08 04:52:52.414953 oplangchain-0.1.2/oplangchain/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0     2678 2023-08-08 04:52:52.414953 oplangchain-0.1.2/oplangchain/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0      241 2023-08-08 04:52:52.414953 oplangchain-0.1.2/oplangchain/tools/multion/__init__.py
--rw-r--r--   0        0        0     1581 2023-08-08 04:52:52.414953 oplangchain-0.1.2/oplangchain/tools/multion/create_session.py
--rw-r--r--   0        0        0     2120 2023-08-08 04:52:52.414953 oplangchain-0.1.2/oplangchain/tools/multion/update_session.py
--rw-r--r--   0        0        0      103 2023-08-08 04:52:52.413953 oplangchain-0.1.2/oplangchain/tools/nuclia/__init__.py
--rw-r--r--   0        0        0     7579 2023-08-08 04:52:52.414953 oplangchain-0.1.2/oplangchain/tools/nuclia/tool.py
--rw-r--r--   0        0        0      597 2023-08-08 04:52:52.405953 oplangchain-0.1.2/oplangchain/tools/office365/__init__.py
--rw-r--r--   0        0        0      484 2023-08-08 04:52:52.412953 oplangchain-0.1.2/oplangchain/tools/office365/base.py
--rw-r--r--   0        0        0     1836 2023-08-08 04:52:52.409952 oplangchain-0.1.2/oplangchain/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0     4852 2023-08-08 04:52:52.406955 oplangchain-0.1.2/oplangchain/tools/office365/events_search.py
--rw-r--r--   0        0        0     4166 2023-08-08 04:52:52.408952 oplangchain-0.1.2/oplangchain/tools/office365/messages_search.py
--rw-r--r--   0        0        0     2834 2023-08-08 04:52:52.406955 oplangchain-0.1.2/oplangchain/tools/office365/send_event.py
--rw-r--r--   0        0        0     1767 2023-08-08 04:52:52.406955 oplangchain-0.1.2/oplangchain/tools/office365/send_message.py
--rw-r--r--   0        0        0     2136 2023-08-07 21:21:40.792153 oplangchain-0.1.2/oplangchain/tools/office365/utils.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.793153 oplangchain-0.1.2/oplangchain/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.793153 oplangchain-0.1.2/oplangchain/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0    20555 2023-08-08 04:52:52.413953 oplangchain-0.1.2/oplangchain/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      158 2023-08-08 04:52:52.413953 oplangchain-0.1.2/oplangchain/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      154 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      922 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/openweathermap/tool.py
--rw-r--r--   0        0        0      698 2023-08-08 04:52:52.405953 oplangchain-0.1.2/oplangchain/tools/playwright/__init__.py
--rw-r--r--   0        0        0     2120 2023-08-08 04:52:52.405953 oplangchain-0.1.2/oplangchain/tools/playwright/base.py
--rw-r--r--   0        0        0     3054 2023-08-08 04:52:52.405953 oplangchain-0.1.2/oplangchain/tools/playwright/click.py
--rw-r--r--   0        0        0     1298 2023-08-08 04:52:52.405953 oplangchain-0.1.2/oplangchain/tools/playwright/current_page.py
--rw-r--r--   0        0        0     3009 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0     2341 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/playwright/extract_text.py
--rw-r--r--   0        0        0     3701 2023-08-08 04:52:52.405953 oplangchain-0.1.2/oplangchain/tools/playwright/get_elements.py
--rw-r--r--   0        0        0     1762 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/playwright/navigate.py
--rw-r--r--   0        0        0     1897 2023-08-08 04:52:52.405953 oplangchain-0.1.2/oplangchain/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0     2813 2023-08-07 21:21:40.800154 oplangchain-0.1.2/oplangchain/tools/playwright/utils.py
--rw-r--r--   0        0        0     2892 2023-08-08 04:52:52.388957 oplangchain-0.1.2/oplangchain/tools/plugin.py
--rw-r--r--   0        0        0       52 2023-08-07 21:21:40.801153 oplangchain-0.1.2/oplangchain/tools/powerbi/__init__.py
--rw-r--r--   0        0        0     7339 2023-08-07 21:21:40.802153 oplangchain-0.1.2/oplangchain/tools/powerbi/prompt.py
--rw-r--r--   0        0        0    11069 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2023-08-07 21:21:40.803153 oplangchain-0.1.2/oplangchain/tools/pubmed/__init__.py
--rw-r--r--   0        0        0     1016 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/pubmed/tool.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.804154 oplangchain-0.1.2/oplangchain/tools/python/__init__.py
--rw-r--r--   0        0        0     4319 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/python/tool.py
--rw-r--r--   0        0        0       52 2023-08-07 21:21:40.805154 oplangchain-0.1.2/oplangchain/tools/requests/__init__.py
--rw-r--r--   0        0        0     6254 2023-08-08 04:52:52.404955 oplangchain-0.1.2/oplangchain/tools/requests/tool.py
--rw-r--r--   0        0        0       31 2023-08-07 21:21:40.806153 oplangchain-0.1.2/oplangchain/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0     1071 2023-08-08 04:52:52.395953 oplangchain-0.1.2/oplangchain/tools/scenexplain/tool.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.807153 oplangchain-0.1.2/oplangchain/tools/searx_search/__init__.py
--rw-r--r--   0        0        0     2222 2023-08-08 04:52:52.396955 oplangchain-0.1.2/oplangchain/tools/searx_search/tool.py
--rw-r--r--   0        0        0       95 2023-08-08 04:52:52.394953 oplangchain-0.1.2/oplangchain/tools/shell/__init__.py
--rw-r--r--   0        0        0     2390 2023-08-08 04:52:52.394953 oplangchain-0.1.2/oplangchain/tools/shell/tool.py
--rw-r--r--   0        0        0       18 2023-08-07 21:21:40.809153 oplangchain-0.1.2/oplangchain/tools/sleep/__init__.py
--rw-r--r--   0        0        0     1209 2023-08-08 04:52:52.394953 oplangchain-0.1.2/oplangchain/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2023-08-07 21:21:40.811153 oplangchain-0.1.2/oplangchain/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0      550 2023-08-07 21:21:40.811153 oplangchain-0.1.2/oplangchain/tools/spark_sql/prompt.py
--rw-r--r--   0        0        0     4526 2023-08-08 04:52:52.394953 oplangchain-0.1.2/oplangchain/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2023-08-07 21:21:40.812153 oplangchain-0.1.2/oplangchain/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      597 2023-08-07 21:21:40.813154 oplangchain-0.1.2/oplangchain/tools/sql_database/prompt.py
--rw-r--r--   0        0        0     4588 2023-08-08 04:52:52.394953 oplangchain-0.1.2/oplangchain/tools/sql_database/tool.py
--rw-r--r--   0        0        0      169 2023-08-08 04:52:52.393954 oplangchain-0.1.2/oplangchain/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0     3335 2023-08-08 04:52:52.394953 oplangchain-0.1.2/oplangchain/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0     1395 2023-08-07 21:21:40.815153 oplangchain-0.1.2/oplangchain/tools/steamship_image_generation/utils.py
--rw-r--r--   0        0        0       51 2023-08-07 21:21:40.815153 oplangchain-0.1.2/oplangchain/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0     3255 2023-08-08 04:52:52.394953 oplangchain-0.1.2/oplangchain/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       29 2023-08-07 21:21:40.817153 oplangchain-0.1.2/oplangchain/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      855 2023-08-08 04:52:52.393954 oplangchain-0.1.2/oplangchain/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      148 2023-08-08 04:52:52.393954 oplangchain-0.1.2/oplangchain/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      875 2023-08-08 04:52:52.393954 oplangchain-0.1.2/oplangchain/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.819153 oplangchain-0.1.2/oplangchain/tools/youtube/__init__.py
--rw-r--r--   0        0        0     1665 2023-08-08 04:52:52.393954 oplangchain-0.1.2/oplangchain/tools/youtube/search.py
--rw-r--r--   0        0        0      172 2023-08-08 04:52:52.392956 oplangchain-0.1.2/oplangchain/tools/zapier/__init__.py
--rw-r--r--   0        0        0     1182 2023-08-07 21:21:40.820154 oplangchain-0.1.2/oplangchain/tools/zapier/prompt.py
--rw-r--r--   0        0        0     7081 2023-08-08 04:52:52.393954 oplangchain-0.1.2/oplangchain/tools/zapier/tool.py
--rw-r--r--   0        0        0     2928 2023-08-08 04:52:52.374954 oplangchain-0.1.2/oplangchain/utilities/__init__.py
--rw-r--r--   0        0        0     6390 2023-08-08 04:52:52.386955 oplangchain-0.1.2/oplangchain/utilities/arxiv.py
--rw-r--r--   0        0        0      274 2023-08-07 21:21:40.822153 oplangchain-0.1.2/oplangchain/utilities/asyncio.py
--rw-r--r--   0        0        0     2419 2023-08-07 21:21:40.823154 oplangchain-0.1.2/oplangchain/utilities/awslambda.py
--rw-r--r--   0        0        0     5705 2023-08-08 04:52:52.386955 oplangchain-0.1.2/oplangchain/utilities/bash.py
--rw-r--r--   0        0        0     2481 2023-08-07 21:21:40.824154 oplangchain-0.1.2/oplangchain/utilities/bibtex.py
--rw-r--r--   0        0        0     3335 2023-08-08 04:52:52.386955 oplangchain-0.1.2/oplangchain/utilities/bing_search.py
--rw-r--r--   0        0        0     2328 2023-08-08 04:52:52.385954 oplangchain-0.1.2/oplangchain/utilities/brave_search.py
--rw-r--r--   0        0        0     7834 2023-08-08 04:52:52.385954 oplangchain-0.1.2/oplangchain/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0     3764 2023-08-07 21:21:40.825153 oplangchain-0.1.2/oplangchain/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0    11596 2023-08-08 04:52:52.385517 oplangchain-0.1.2/oplangchain/utilities/github.py
--rw-r--r--   0        0        0     1838 2023-08-08 04:52:52.384954 oplangchain-0.1.2/oplangchain/utilities/golden_query.py
--rw-r--r--   0        0        0     4069 2023-08-08 04:52:52.384954 oplangchain-0.1.2/oplangchain/utilities/google_places_api.py
--rw-r--r--   0        0        0     5096 2023-08-08 04:52:52.383953 oplangchain-0.1.2/oplangchain/utilities/google_search.py
--rw-r--r--   0        0        0     6507 2023-08-08 04:52:52.383953 oplangchain-0.1.2/oplangchain/utilities/google_serper.py
--rw-r--r--   0        0        0     1885 2023-08-07 21:21:40.828153 oplangchain-0.1.2/oplangchain/utilities/graphql.py
--rw-r--r--   0        0        0     6175 2023-08-08 04:52:52.379954 oplangchain-0.1.2/oplangchain/utilities/jira.py
--rw-r--r--   0        0        0     1974 2023-08-08 04:52:52.378954 oplangchain-0.1.2/oplangchain/utilities/loading.py
--rw-r--r--   0        0        0     2644 2023-08-08 04:52:52.377955 oplangchain-0.1.2/oplangchain/utilities/max_compute.py
--rw-r--r--   0        0        0     6707 2023-08-08 04:52:52.376953 oplangchain-0.1.2/oplangchain/utilities/metaphor_search.py
--rw-r--r--   0        0        0    10299 2023-08-07 21:21:40.830153 oplangchain-0.1.2/oplangchain/utilities/openapi.py
--rw-r--r--   0        0        0     2442 2023-08-08 04:52:52.376953 oplangchain-0.1.2/oplangchain/utilities/openweathermap.py
--rw-r--r--   0        0        0     2198 2023-08-07 21:21:40.831154 oplangchain-0.1.2/oplangchain/utilities/portkey.py
--rw-r--r--   0        0        0    11237 2023-08-07 21:21:40.832154 oplangchain-0.1.2/oplangchain/utilities/powerbi.py
--rw-r--r--   0        0        0     5629 2023-08-08 04:52:52.376953 oplangchain-0.1.2/oplangchain/utilities/pupmed.py
--rw-r--r--   0        0        0     2141 2023-08-07 21:21:40.833154 oplangchain-0.1.2/oplangchain/utilities/python.py
--rw-r--r--   0        0        0     5439 2023-08-08 04:52:52.376953 oplangchain-0.1.2/oplangchain/utilities/redis.py
--rw-r--r--   0        0        0     7120 2023-08-07 21:21:40.834153 oplangchain-0.1.2/oplangchain/utilities/requests.py
--rw-r--r--   0        0        0     2200 2023-08-08 04:52:52.376953 oplangchain-0.1.2/oplangchain/utilities/scenexplain.py
--rw-r--r--   0        0        0    16539 2023-08-08 04:52:52.376953 oplangchain-0.1.2/oplangchain/utilities/searx_search.py
--rw-r--r--   0        0        0     6029 2023-08-08 04:52:52.375952 oplangchain-0.1.2/oplangchain/utilities/serpapi.py
--rw-r--r--   0        0        0     6964 2023-08-07 21:21:40.836153 oplangchain-0.1.2/oplangchain/utilities/spark_sql.py
--rw-r--r--   0        0        0    18265 2023-08-08 04:52:52.375952 oplangchain-0.1.2/oplangchain/utilities/sql_database.py
--rw-r--r--   0        0        0     3413 2023-08-08 04:52:52.374954 oplangchain-0.1.2/oplangchain/utilities/twilio.py
--rw-r--r--   0        0        0     1457 2023-08-07 21:21:40.837154 oplangchain-0.1.2/oplangchain/utilities/vertexai.py
--rw-r--r--   0        0        0     3922 2023-08-08 04:52:52.374954 oplangchain-0.1.2/oplangchain/utilities/wikipedia.py
--rw-r--r--   0        0        0     1991 2023-08-08 04:52:52.374954 oplangchain-0.1.2/oplangchain/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0    11562 2023-08-08 04:52:52.374954 oplangchain-0.1.2/oplangchain/utilities/zapier.py
--rw-r--r--   0        0        0     1161 2023-08-08 04:52:52.374954 oplangchain-0.1.2/oplangchain/utils/__init__.py
--rw-r--r--   0        0        0      873 2023-08-07 21:21:40.840155 oplangchain-0.1.2/oplangchain/utils/env.py
--rw-r--r--   0        0        0     1237 2023-08-07 21:21:40.840155 oplangchain-0.1.2/oplangchain/utils/formatting.py
--rw-r--r--   0        0        0     1289 2023-08-07 21:21:40.841153 oplangchain-0.1.2/oplangchain/utils/input.py
--rw-r--r--   0        0        0     2016 2023-08-07 21:21:40.841153 oplangchain-0.1.2/oplangchain/utils/math.py
--rw-r--r--   0        0        0      908 2023-08-07 21:21:40.842153 oplangchain-0.1.2/oplangchain/utils/strings.py
--rw-r--r--   0        0        0     5606 2023-08-07 21:21:40.842153 oplangchain-0.1.2/oplangchain/utils/utils.py
--rw-r--r--   0        0        0     4085 2023-08-08 04:52:52.346953 oplangchain-0.1.2/oplangchain/vectorstores/__init__.py
--rw-r--r--   0        0        0     2027 2023-08-08 04:52:52.347954 oplangchain-0.1.2/oplangchain/vectorstores/_pgvector_data_models.py
--rw-r--r--   0        0        0    13541 2023-08-08 04:52:52.372952 oplangchain-0.1.2/oplangchain/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0    15800 2023-08-08 04:52:52.370954 oplangchain-0.1.2/oplangchain/vectorstores/analyticdb.py
--rw-r--r--   0        0        0    16597 2023-08-08 04:52:52.370954 oplangchain-0.1.2/oplangchain/vectorstores/annoy.py
--rw-r--r--   0        0        0    12143 2023-08-08 04:52:52.369953 oplangchain-0.1.2/oplangchain/vectorstores/atlas.py
--rw-r--r--   0        0        0    21228 2023-08-08 04:52:52.369953 oplangchain-0.1.2/oplangchain/vectorstores/awadb.py
--rw-r--r--   0        0        0    20726 2023-08-08 04:52:52.369953 oplangchain-0.1.2/oplangchain/vectorstores/azuresearch.py
--rw-r--r--   0        0        0    22441 2023-08-08 04:52:52.369953 oplangchain-0.1.2/oplangchain/vectorstores/base.py
--rw-r--r--   0        0        0    13404 2023-08-08 04:52:52.366955 oplangchain-0.1.2/oplangchain/vectorstores/cassandra.py
--rw-r--r--   0        0        0    23822 2023-08-08 04:52:52.366955 oplangchain-0.1.2/oplangchain/vectorstores/chroma.py
--rw-r--r--   0        0        0    12739 2023-08-08 04:52:52.365954 oplangchain-0.1.2/oplangchain/vectorstores/clarifai.py
--rw-r--r--   0        0        0    17817 2023-08-08 04:52:52.365954 oplangchain-0.1.2/oplangchain/vectorstores/clickhouse.py
--rw-r--r--   0        0        0    34980 2023-08-08 04:52:52.364955 oplangchain-0.1.2/oplangchain/vectorstores/deeplake.py
--rw-r--r--   0        0        0      220 2023-08-08 04:52:52.373955 oplangchain-0.1.2/oplangchain/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0     6879 2023-08-08 04:52:52.374954 oplangchain-0.1.2/oplangchain/vectorstores/docarray/base.py
--rw-r--r--   0        0        0     4061 2023-08-08 04:52:52.374954 oplangchain-0.1.2/oplangchain/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0     2415 2023-08-08 04:52:52.373955 oplangchain-0.1.2/oplangchain/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0    27795 2023-08-08 04:52:52.364955 oplangchain-0.1.2/oplangchain/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0    29137 2023-08-08 04:52:52.364955 oplangchain-0.1.2/oplangchain/vectorstores/faiss.py
--rw-r--r--   0        0        0    16411 2023-08-08 04:52:52.364955 oplangchain-0.1.2/oplangchain/vectorstores/hologres.py
--rw-r--r--   0        0        0     4242 2023-08-08 04:52:52.364955 oplangchain-0.1.2/oplangchain/vectorstores/lancedb.py
--rw-r--r--   0        0        0    17162 2023-08-08 04:52:52.364955 oplangchain-0.1.2/oplangchain/vectorstores/marqo.py
--rw-r--r--   0        0        0    15184 2023-08-08 04:52:52.364955 oplangchain-0.1.2/oplangchain/vectorstores/matching_engine.py
--rw-r--r--   0        0        0    10437 2023-08-08 04:52:52.360956 oplangchain-0.1.2/oplangchain/vectorstores/meilisearch.py
--rw-r--r--   0        0        0    31480 2023-08-08 04:52:52.360956 oplangchain-0.1.2/oplangchain/vectorstores/milvus.py
--rw-r--r--   0        0        0    12361 2023-08-08 04:52:52.359955 oplangchain-0.1.2/oplangchain/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0    16545 2023-08-08 04:52:52.358954 oplangchain-0.1.2/oplangchain/vectorstores/myscale.py
--rw-r--r--   0        0        0    27702 2023-08-08 04:52:52.358954 oplangchain-0.1.2/oplangchain/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0    17352 2023-08-08 04:52:52.358954 oplangchain-0.1.2/oplangchain/vectorstores/pgembedding.py
--rw-r--r--   0        0        0    21271 2023-08-08 04:52:52.358954 oplangchain-0.1.2/oplangchain/vectorstores/pgvector.py
--rw-r--r--   0        0        0    14921 2023-08-08 04:52:52.358954 oplangchain-0.1.2/oplangchain/vectorstores/pinecone.py
--rw-r--r--   0        0        0    68545 2023-08-08 04:52:52.357953 oplangchain-0.1.2/oplangchain/vectorstores/qdrant.py
--rw-r--r--   0        0        0    23162 2023-08-08 04:52:52.357953 oplangchain-0.1.2/oplangchain/vectorstores/redis.py
--rw-r--r--   0        0        0    12196 2023-08-08 04:52:52.357953 oplangchain-0.1.2/oplangchain/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0    19535 2023-08-08 04:52:52.357953 oplangchain-0.1.2/oplangchain/vectorstores/scann.py
--rw-r--r--   0        0        0    18282 2023-08-08 04:52:52.357953 oplangchain-0.1.2/oplangchain/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0    12395 2023-08-08 04:52:52.356954 oplangchain-0.1.2/oplangchain/vectorstores/sklearn.py
--rw-r--r--   0        0        0    17225 2023-08-08 04:52:52.355953 oplangchain-0.1.2/oplangchain/vectorstores/starrocks.py
--rw-r--r--   0        0        0    14251 2023-08-08 04:52:52.352954 oplangchain-0.1.2/oplangchain/vectorstores/supabase.py
--rw-r--r--   0        0        0     8886 2023-08-08 04:52:52.352954 oplangchain-0.1.2/oplangchain/vectorstores/tair.py
--rw-r--r--   0        0        0     4884 2023-08-08 04:52:52.352954 oplangchain-0.1.2/oplangchain/vectorstores/tigris.py
--rw-r--r--   0        0        0     9744 2023-08-08 04:52:52.352954 oplangchain-0.1.2/oplangchain/vectorstores/typesense.py
--rw-r--r--   0        0        0     1792 2023-08-08 04:52:52.351954 oplangchain-0.1.2/oplangchain/vectorstores/utils.py
--rw-r--r--   0        0        0    15869 2023-08-08 04:52:52.351954 oplangchain-0.1.2/oplangchain/vectorstores/vectara.py
--rw-r--r--   0        0        0    16891 2023-08-08 04:52:52.351954 oplangchain-0.1.2/oplangchain/vectorstores/weaviate.py
--rw-r--r--   0        0        0     7567 2023-08-08 04:52:52.350953 oplangchain-0.1.2/oplangchain/vectorstores/zilliz.py
--rw-r--r--   0        0        0    13300 2023-08-08 14:25:37.255488 oplangchain-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6801 2023-08-08 05:21:38.027643 oplangchain-0.1.2/README.md
--rw-r--r--   0        0        0    16025 1970-01-01 00:00:00.000000 oplangchain-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3112 2023-08-08 04:52:52.339954 oplangchain-0.1.3/oplangchain/__init__.py
+-rw-r--r--   0        0        0     3439 2023-08-08 20:14:00.983604 oplangchain-0.1.3/oplangchain/agents/__init__.py
+-rw-r--r--   0        0        0    41327 2023-08-08 04:52:52.741001 oplangchain-0.1.3/oplangchain/agents/agent.py
+-rw-r--r--   0        0        0    18339 2023-08-08 04:52:52.741001 oplangchain-0.1.3/oplangchain/agents/agent_iterator.py
+-rw-r--r--   0        0        0     3533 2023-08-08 20:14:01.016598 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0      883 2023-08-08 04:52:52.761592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0      925 2023-08-08 04:52:52.757592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0      371 2023-08-08 04:52:52.757592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.393154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0     3397 2023-08-08 04:52:52.761592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
+-rw-r--r--   0        0        0      734 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/conversational_retrieval/tool.py
+-rw-r--r--   0        0        0       19 2023-08-07 21:21:40.394154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0     1154 2023-08-08 04:52:52.761592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/csv/base.py
+-rw-r--r--   0        0        0      176 2023-08-08 04:52:52.761592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0     2092 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-07 21:21:40.396155 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0     2494 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       21 2023-08-07 21:21:40.398154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0     1583 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2023-08-07 21:21:40.399153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0     1929 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2023-08-07 21:21:40.400153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0     1729 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0     1819 2023-08-07 21:21:40.401154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0      561 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0       23 2023-08-07 21:21:40.402153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0      668 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.403154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0     1949 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0     3779 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2023-08-07 21:21:40.405154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0     1187 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2023-08-07 21:21:40.406154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0     2156 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0    11263 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0    10462 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0     1743 2023-08-07 21:21:40.407153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0     3835 2023-08-07 21:21:40.408153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0     2396 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-07 21:21:40.409153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0    11540 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/pandas/base.py
+-rw-r--r--   0        0        0     1113 2023-08-07 21:21:40.410153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/pandas/prompt.py
+-rw-r--r--   0        0        0      173 2023-08-08 20:14:01.128597 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0     3034 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-07 21:21:40.412153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0     2340 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0     2509 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0     2773 2023-08-07 21:21:40.413154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0     3239 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.414153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0     2220 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/python/base.py
+-rw-r--r--   0        0        0      513 2023-08-07 21:21:40.415153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/python/prompt.py
+-rw-r--r--   0        0        0       20 2023-08-07 21:21:40.416154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0     2748 2023-08-08 04:52:52.760593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark/base.py
+-rw-r--r--   0        0        0      295 2023-08-07 21:21:40.416154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark/prompt.py
+-rw-r--r--   0        0        0       23 2023-08-07 21:21:40.417153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0     2088 2023-08-08 04:52:52.759593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0     1202 2023-08-07 21:21:40.418154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0     1044 2023-08-08 04:52:52.757592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2023-08-07 21:21:40.419153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0     3458 2023-08-08 04:52:52.759593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0     1428 2023-08-07 21:21:40.420153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0     2826 2023-08-08 04:52:52.759593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       56 2023-08-07 21:21:40.421153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/vectorstore/__init__.py
+-rw-r--r--   0        0        0     2422 2023-08-08 04:52:52.759593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/vectorstore/base.py
+-rw-r--r--   0        0        0      834 2023-08-07 21:21:40.422154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/vectorstore/prompt.py
+-rw-r--r--   0        0        0     2973 2023-08-08 04:52:52.759593 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/vectorstore/toolkit.py
+-rw-r--r--   0        0        0       23 2023-08-07 21:21:40.423153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0     3119 2023-08-08 04:52:52.757592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/xorbits/base.py
+-rw-r--r--   0        0        0     1070 2023-08-07 21:21:40.424153 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/xorbits/prompt.py
+-rw-r--r--   0        0        0       22 2023-08-07 21:21:40.425154 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0     1617 2023-08-08 04:52:52.757592 oplangchain-0.1.3/oplangchain/agents/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0      688 2023-08-07 21:21:40.426153 oplangchain-0.1.3/oplangchain/agents/agent_types.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.426153 oplangchain-0.1.3/oplangchain/agents/chat/__init__.py
+-rw-r--r--   0        0        0     4928 2023-08-08 04:52:52.752596 oplangchain-0.1.3/oplangchain/agents/chat/base.py
+-rw-r--r--   0        0        0     1712 2023-08-08 04:52:52.752596 oplangchain-0.1.3/oplangchain/agents/chat/output_parser.py
+-rw-r--r--   0        0        0     1158 2023-08-07 21:21:40.427153 oplangchain-0.1.3/oplangchain/agents/chat/prompt.py
+-rw-r--r--   0        0        0       75 2023-08-07 21:21:40.428154 oplangchain-0.1.3/oplangchain/agents/conversational/__init__.py
+-rw-r--r--   0        0        0     4840 2023-08-08 04:52:52.754593 oplangchain-0.1.3/oplangchain/agents/conversational/base.py
+-rw-r--r--   0        0        0     1156 2023-08-08 04:52:52.754593 oplangchain-0.1.3/oplangchain/agents/conversational/output_parser.py
+-rw-r--r--   0        0        0     1859 2023-08-07 21:21:40.429153 oplangchain-0.1.3/oplangchain/agents/conversational/prompt.py
+-rw-r--r--   0        0        0       75 2023-08-07 21:21:40.430153 oplangchain-0.1.3/oplangchain/agents/conversational_chat/__init__.py
+-rw-r--r--   0        0        0     4999 2023-08-08 04:52:52.752002 oplangchain-0.1.3/oplangchain/agents/conversational_chat/base.py
+-rw-r--r--   0        0        0     2264 2023-08-08 04:52:52.752596 oplangchain-0.1.3/oplangchain/agents/conversational_chat/output_parser.py
+-rw-r--r--   0        0        0     2757 2023-08-07 21:21:40.431155 oplangchain-0.1.3/oplangchain/agents/conversational_chat/prompt.py
+-rw-r--r--   0        0        0     3007 2023-08-08 04:52:52.741001 oplangchain-0.1.3/oplangchain/agents/initialize.py
+-rw-r--r--   0        0        0    17413 2023-08-08 04:52:52.740001 oplangchain-0.1.3/oplangchain/agents/load_tools.py
+-rw-r--r--   0        0        0     4385 2023-08-08 04:52:52.741001 oplangchain-0.1.3/oplangchain/agents/loading.py
+-rw-r--r--   0        0        0       86 2023-08-07 21:21:40.433153 oplangchain-0.1.3/oplangchain/agents/mrkl/__init__.py
+-rw-r--r--   0        0        0     7127 2023-08-08 04:52:52.752002 oplangchain-0.1.3/oplangchain/agents/mrkl/base.py
+-rw-r--r--   0        0        0     2712 2023-08-08 04:52:52.752596 oplangchain-0.1.3/oplangchain/agents/mrkl/output_parser.py
+-rw-r--r--   0        0        0      641 2023-08-07 21:21:40.435153 oplangchain-0.1.3/oplangchain/agents/mrkl/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.435153 oplangchain-0.1.3/oplangchain/agents/openai_functions_agent/__init__.py
+-rw-r--r--   0        0        0     2535 2023-08-08 04:52:52.752002 oplangchain-0.1.3/oplangchain/agents/openai_functions_agent/agent_token_buffer_memory.py
+-rw-r--r--   0        0        0    11916 2023-08-08 04:52:52.752002 oplangchain-0.1.3/oplangchain/agents/openai_functions_agent/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.437154 oplangchain-0.1.3/oplangchain/agents/openai_functions_multi_agent/__init__.py
+-rw-r--r--   0        0        0    13355 2023-08-08 04:52:52.752002 oplangchain-0.1.3/oplangchain/agents/openai_functions_multi_agent/base.py
+-rw-r--r--   0        0        0       76 2023-08-07 21:21:40.438153 oplangchain-0.1.3/oplangchain/agents/react/__init__.py
+-rw-r--r--   0        0        0     5690 2023-08-08 04:52:52.752002 oplangchain-0.1.3/oplangchain/agents/react/base.py
+-rw-r--r--   0        0        0     1192 2023-08-08 04:52:52.751004 oplangchain-0.1.3/oplangchain/agents/react/output_parser.py
+-rw-r--r--   0        0        0     1903 2023-08-08 04:52:52.751004 oplangchain-0.1.3/oplangchain/agents/react/textworld_prompt.py
+-rw-r--r--   0        0        0     6124 2023-08-08 04:52:52.751004 oplangchain-0.1.3/oplangchain/agents/react/wiki_prompt.py
+-rw-r--r--   0        0        0     1089 2023-08-08 04:52:52.740001 oplangchain-0.1.3/oplangchain/agents/schema.py
+-rw-r--r--   0        0        0      106 2023-08-07 21:21:40.441153 oplangchain-0.1.3/oplangchain/agents/self_ask_with_search/__init__.py
+-rw-r--r--   0        0        0     3118 2023-08-08 04:52:52.746003 oplangchain-0.1.3/oplangchain/agents/self_ask_with_search/base.py
+-rw-r--r--   0        0        0      966 2023-08-08 04:52:52.745003 oplangchain-0.1.3/oplangchain/agents/self_ask_with_search/output_parser.py
+-rw-r--r--   0        0        0     1923 2023-08-08 04:52:52.745003 oplangchain-0.1.3/oplangchain/agents/self_ask_with_search/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.443153 oplangchain-0.1.3/oplangchain/agents/structured_chat/__init__.py
+-rw-r--r--   0        0        0     5179 2023-08-08 20:14:01.349597 oplangchain-0.1.3/oplangchain/agents/structured_chat/base.py
+-rw-r--r--   0        0        0     3462 2023-08-08 04:52:52.749002 oplangchain-0.1.3/oplangchain/agents/structured_chat/output_parser.py
+-rw-r--r--   0        0        0      992 2023-08-07 21:21:40.444153 oplangchain-0.1.3/oplangchain/agents/structured_chat/prompt.py
+-rw-r--r--   0        0        0     1406 2023-08-08 04:52:52.740001 oplangchain-0.1.3/oplangchain/agents/tools.py
+-rw-r--r--   0        0        0     1506 2023-08-08 20:14:01.288597 oplangchain-0.1.3/oplangchain/agents/types.py
+-rw-r--r--   0        0        0      386 2023-08-08 04:52:52.737004 oplangchain-0.1.3/oplangchain/agents/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.446153 oplangchain-0.1.3/oplangchain/agents/xml/__init__.py
+-rw-r--r--   0        0        0     3905 2023-08-08 04:52:52.741001 oplangchain-0.1.3/oplangchain/agents/xml/base.py
+-rw-r--r--   0        0        0      749 2023-08-07 21:21:40.447154 oplangchain-0.1.3/oplangchain/agents/xml/prompt.py
+-rw-r--r--   0        0        0      220 2023-08-08 04:52:52.346953 oplangchain-0.1.3/oplangchain/base_language.py
+-rw-r--r--   0        0        0    24879 2023-08-08 20:14:01.641598 oplangchain-0.1.3/oplangchain/cache.py
+-rw-r--r--   0        0        0     2887 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/callbacks/__init__.py
+-rw-r--r--   0        0        0    14488 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/aim_callback.py
+-rw-r--r--   0        0        0    13727 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0     7509 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/arize_callback.py
+-rw-r--r--   0        0        0    11347 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0    15188 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/base.py
+-rw-r--r--   0        0        0    18502 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0    23246 2023-08-08 05:01:50.902666 oplangchain-0.1.3/oplangchain/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0     6438 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/context_callback.py
+-rw-r--r--   0        0        0     2567 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/file.py
+-rw-r--r--   0        0        0    13163 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0     1412 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/human.py
+-rw-r--r--   0        0        0     5574 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/infino_callback.py
+-rw-r--r--   0        0        0    53812 2023-08-08 20:14:02.389597 oplangchain-0.1.3/oplangchain/callbacks/manager.py
+-rw-r--r--   0        0        0    24171 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0     5352 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/openai_info.py
+-rw-r--r--   0        0        0     5529 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0     8829 2023-08-08 04:52:52.612956 oplangchain-0.1.3/oplangchain/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0     3209 2023-08-08 04:52:52.612956 oplangchain-0.1.3/oplangchain/callbacks/stdout.py
+-rw-r--r--   0        0        0     2440 2023-08-08 04:52:52.612956 oplangchain-0.1.3/oplangchain/callbacks/streaming_aiter.py
+-rw-r--r--   0        0        0     3368 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/callbacks/streaming_aiter_final_only.py
+-rw-r--r--   0        0        0     2174 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     3370 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/callbacks/streaming_stdout_final_only.py
+-rw-r--r--   0        0        0     3196 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0     5435 2023-08-07 21:21:40.460153 oplangchain-0.1.3/oplangchain/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0    15677 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0      510 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0    17028 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/callbacks/tracers/base.py
+-rw-r--r--   0        0        0     4866 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0     8065 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0     7370 2023-08-08 04:52:52.618953 oplangchain-0.1.3/oplangchain/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0     1541 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0     3458 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0     6033 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0    18987 2023-08-08 04:52:52.617952 oplangchain-0.1.3/oplangchain/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0     8505 2023-08-07 21:21:40.465154 oplangchain-0.1.3/oplangchain/callbacks/utils.py
+-rw-r--r--   0        0        0    20665 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0     8066 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0     5387 2023-08-08 20:14:01.668597 oplangchain-0.1.3/oplangchain/chains/__init__.py
+-rw-r--r--   0        0        0       84 2023-08-07 21:21:40.468155 oplangchain-0.1.3/oplangchain/chains/api/__init__.py
+-rw-r--r--   0        0        0     5348 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/api/base.py
+-rw-r--r--   0        0        0     2452 2023-08-07 21:21:40.469154 oplangchain-0.1.3/oplangchain/chains/api/news_docs.py
+-rw-r--r--   0        0        0     3399 2023-08-07 21:21:40.469154 oplangchain-0.1.3/oplangchain/chains/api/open_meteo_docs.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.470153 oplangchain-0.1.3/oplangchain/chains/api/openapi/__init__.py
+-rw-r--r--   0        0        0     8766 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/api/openapi/chain.py
+-rw-r--r--   0        0        0     1791 2023-08-07 21:21:40.471154 oplangchain-0.1.3/oplangchain/chains/api/openapi/prompts.py
+-rw-r--r--   0        0        0     1887 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/api/openapi/requests_chain.py
+-rw-r--r--   0        0        0     1759 2023-08-08 04:52:52.725542 oplangchain-0.1.3/oplangchain/chains/api/openapi/response_chain.py
+-rw-r--r--   0        0        0     1920 2023-08-07 21:21:40.472154 oplangchain-0.1.3/oplangchain/chains/api/podcast_docs.py
+-rw-r--r--   0        0        0     1028 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/api/prompt.py
+-rw-r--r--   0        0        0     1537 2023-08-07 21:21:40.473154 oplangchain-0.1.3/oplangchain/chains/api/tmdb_docs.py
+-rw-r--r--   0        0        0    24830 2023-08-08 05:06:24.195893 oplangchain-0.1.3/oplangchain/chains/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.474154 oplangchain-0.1.3/oplangchain/chains/chat_vector_db/__init__.py
+-rw-r--r--   0        0        0      691 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/chat_vector_db/prompts.py
+-rw-r--r--   0        0        0       43 2023-08-07 21:21:40.475154 oplangchain-0.1.3/oplangchain/chains/combine_documents/__init__.py
+-rw-r--r--   0        0        0     6398 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/combine_documents/base.py
+-rw-r--r--   0        0        0    11165 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/combine_documents/map_reduce.py
+-rw-r--r--   0        0        0     8386 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/combine_documents/map_rerank.py
+-rw-r--r--   0        0        0    11016 2023-08-08 04:52:52.723542 oplangchain-0.1.3/oplangchain/chains/combine_documents/reduce.py
+-rw-r--r--   0        0        0     9093 2023-08-08 04:52:52.721990 oplangchain-0.1.3/oplangchain/chains/combine_documents/refine.py
+-rw-r--r--   0        0        0     7676 2023-08-08 04:52:52.720989 oplangchain-0.1.3/oplangchain/chains/combine_documents/stuff.py
+-rw-r--r--   0        0        0      107 2023-08-07 21:21:40.479154 oplangchain-0.1.3/oplangchain/chains/constitutional_ai/__init__.py
+-rw-r--r--   0        0        0     6363 2023-08-08 20:14:01.754597 oplangchain-0.1.3/oplangchain/chains/constitutional_ai/base.py
+-rw-r--r--   0        0        0      265 2023-08-07 21:21:40.480154 oplangchain-0.1.3/oplangchain/chains/constitutional_ai/models.py
+-rw-r--r--   0        0        0    21740 2023-08-08 04:52:52.720989 oplangchain-0.1.3/oplangchain/chains/constitutional_ai/principles.py
+-rw-r--r--   0        0        0     8660 2023-08-08 04:52:52.718988 oplangchain-0.1.3/oplangchain/chains/constitutional_ai/prompts.py
+-rw-r--r--   0        0        0       71 2023-08-07 21:21:40.482154 oplangchain-0.1.3/oplangchain/chains/conversation/__init__.py
+-rw-r--r--   0        0        0     2184 2023-08-08 04:52:52.718988 oplangchain-0.1.3/oplangchain/chains/conversation/base.py
+-rw-r--r--   0        0        0      870 2023-08-08 04:52:52.717989 oplangchain-0.1.3/oplangchain/chains/conversation/memory.py
+-rw-r--r--   0        0        0      912 2023-08-08 04:52:52.717989 oplangchain-0.1.3/oplangchain/chains/conversation/prompt.py
+-rw-r--r--   0        0        0       49 2023-08-07 21:21:40.484154 oplangchain-0.1.3/oplangchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0    16735 2023-08-08 04:52:52.709600 oplangchain-0.1.3/oplangchain/chains/conversational_retrieval/base.py
+-rw-r--r--   0        0        0      717 2023-08-08 04:52:52.709600 oplangchain-0.1.3/oplangchain/chains/conversational_retrieval/prompts.py
+-rw-r--r--   0        0        0      128 2023-08-08 04:52:52.716988 oplangchain-0.1.3/oplangchain/chains/elasticsearch_database/__init__.py
+-rw-r--r--   0        0        0     8182 2023-08-08 04:52:52.717989 oplangchain-0.1.3/oplangchain/chains/elasticsearch_database/base.py
+-rw-r--r--   0        0        0     1422 2023-08-08 04:52:52.717989 oplangchain-0.1.3/oplangchain/chains/elasticsearch_database/prompts.py
+-rw-r--r--   0        0        0      739 2023-08-08 04:52:52.667997 oplangchain-0.1.3/oplangchain/chains/example_generator.py
+-rw-r--r--   0        0        0       51 2023-08-07 21:21:40.487153 oplangchain-0.1.3/oplangchain/chains/flare/__init__.py
+-rw-r--r--   0        0        0     8779 2023-08-08 04:52:52.715988 oplangchain-0.1.3/oplangchain/chains/flare/base.py
+-rw-r--r--   0        0        0     1457 2023-08-08 04:52:52.715988 oplangchain-0.1.3/oplangchain/chains/flare/prompts.py
+-rw-r--r--   0        0        0       49 2023-08-07 21:21:40.489153 oplangchain-0.1.3/oplangchain/chains/graph_qa/__init__.py
+-rw-r--r--   0        0        0     7690 2023-08-08 04:52:52.715988 oplangchain-0.1.3/oplangchain/chains/graph_qa/arangodb.py
+-rw-r--r--   0        0        0     2997 2023-08-08 20:14:01.793598 oplangchain-0.1.3/oplangchain/chains/graph_qa/base.py
+-rw-r--r--   0        0        0     4613 2023-08-08 20:14:01.827601 oplangchain-0.1.3/oplangchain/chains/graph_qa/cypher.py
+-rw-r--r--   0        0        0     3033 2023-08-08 04:52:52.714991 oplangchain-0.1.3/oplangchain/chains/graph_qa/hugegraph.py
+-rw-r--r--   0        0        0     3033 2023-08-08 04:52:52.714991 oplangchain-0.1.3/oplangchain/chains/graph_qa/kuzu.py
+-rw-r--r--   0        0        0     3008 2023-08-08 04:52:52.714991 oplangchain-0.1.3/oplangchain/chains/graph_qa/nebulagraph.py
+-rw-r--r--   0        0        0     4493 2023-08-08 04:52:52.714991 oplangchain-0.1.3/oplangchain/chains/graph_qa/neptune_cypher.py
+-rw-r--r--   0        0        0    13730 2023-08-08 04:52:52.714991 oplangchain-0.1.3/oplangchain/chains/graph_qa/prompts.py
+-rw-r--r--   0        0        0     4785 2023-08-08 04:52:52.714991 oplangchain-0.1.3/oplangchain/chains/graph_qa/sparql.py
+-rw-r--r--   0        0        0       75 2023-08-07 21:21:40.493153 oplangchain-0.1.3/oplangchain/chains/hyde/__init__.py
+-rw-r--r--   0        0        0     2843 2023-08-08 04:52:52.712601 oplangchain-0.1.3/oplangchain/chains/hyde/base.py
+-rw-r--r--   0        0        0     1910 2023-08-08 04:52:52.712601 oplangchain-0.1.3/oplangchain/chains/hyde/prompts.py
+-rw-r--r--   0        0        0    12157 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/llm.py
+-rw-r--r--   0        0        0       88 2023-08-07 21:21:40.495154 oplangchain-0.1.3/oplangchain/chains/llm_bash/__init__.py
+-rw-r--r--   0        0        0     4181 2023-08-08 04:52:52.712601 oplangchain-0.1.3/oplangchain/chains/llm_bash/base.py
+-rw-r--r--   0        0        0     1941 2023-08-08 04:52:52.712601 oplangchain-0.1.3/oplangchain/chains/llm_bash/prompt.py
+-rw-r--r--   0        0        0      139 2023-08-07 21:21:40.497153 oplangchain-0.1.3/oplangchain/chains/llm_checker/__init__.py
+-rw-r--r--   0        0        0     6106 2023-08-08 04:52:52.706600 oplangchain-0.1.3/oplangchain/chains/llm_checker/base.py
+-rw-r--r--   0        0        0     1122 2023-08-08 04:52:52.706600 oplangchain-0.1.3/oplangchain/chains/llm_checker/prompt.py
+-rw-r--r--   0        0        0      143 2023-08-07 21:21:40.499153 oplangchain-0.1.3/oplangchain/chains/llm_math/__init__.py
+-rw-r--r--   0        0        0     6386 2023-08-08 04:52:52.709600 oplangchain-0.1.3/oplangchain/chains/llm_math/base.py
+-rw-r--r--   0        0        0      865 2023-08-08 04:52:52.709600 oplangchain-0.1.3/oplangchain/chains/llm_math/prompt.py
+-rw-r--r--   0        0        0     2885 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/llm_requests.py
+-rw-r--r--   0        0        0      352 2023-08-07 21:21:40.500154 oplangchain-0.1.3/oplangchain/chains/llm_summarization_checker/__init__.py
+-rw-r--r--   0        0        0     6620 2023-08-08 04:52:52.706600 oplangchain-0.1.3/oplangchain/chains/llm_summarization_checker/base.py
+-rw-r--r--   0        0        0      654 2023-08-07 21:21:40.502153 oplangchain-0.1.3/oplangchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
+-rw-r--r--   0        0        0      377 2023-08-07 21:21:40.502153 oplangchain-0.1.3/oplangchain/chains/llm_summarization_checker/prompts/check_facts.txt
+-rw-r--r--   0        0        0      128 2023-08-07 21:21:40.503153 oplangchain-0.1.3/oplangchain/chains/llm_summarization_checker/prompts/create_facts.txt
+-rw-r--r--   0        0        0      416 2023-08-07 21:21:40.503153 oplangchain-0.1.3/oplangchain/chains/llm_summarization_checker/prompts/revise_summary.txt
+-rw-r--r--   0        0        0      126 2023-08-07 21:21:40.504153 oplangchain-0.1.3/oplangchain/chains/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0     5569 2023-08-08 04:52:52.706600 oplangchain-0.1.3/oplangchain/chains/llm_symbolic_math/base.py
+-rw-r--r--   0        0        0     1089 2023-08-08 04:52:52.706600 oplangchain-0.1.3/oplangchain/chains/llm_symbolic_math/prompt.py
+-rw-r--r--   0        0        0    23991 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/loading.py
+-rw-r--r--   0        0        0     3737 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/mapreduce.py
+-rw-r--r--   0        0        0     3058 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/moderation.py
+-rw-r--r--   0        0        0       96 2023-08-07 21:21:40.507154 oplangchain-0.1.3/oplangchain/chains/natbot/__init__.py
+-rw-r--r--   0        0        0     4193 2023-08-08 04:52:52.701599 oplangchain-0.1.3/oplangchain/chains/natbot/base.py
+-rw-r--r--   0        0        0    15466 2023-08-07 21:21:40.508154 oplangchain-0.1.3/oplangchain/chains/natbot/crawler.py
+-rw-r--r--   0        0        0     4986 2023-08-08 04:52:52.701599 oplangchain-0.1.3/oplangchain/chains/natbot/prompt.py
+-rw-r--r--   0        0        0      958 2023-08-08 04:52:52.698599 oplangchain-0.1.3/oplangchain/chains/openai_functions/__init__.py
+-rw-r--r--   0        0        0    14630 2023-08-08 04:52:52.701599 oplangchain-0.1.3/oplangchain/chains/openai_functions/base.py
+-rw-r--r--   0        0        0     3518 2023-08-08 04:52:52.701599 oplangchain-0.1.3/oplangchain/chains/openai_functions/citation_fuzzy_match.py
+-rw-r--r--   0        0        0     3350 2023-08-08 04:52:52.701599 oplangchain-0.1.3/oplangchain/chains/openai_functions/extraction.py
+-rw-r--r--   0        0        0    11915 2023-08-09 04:12:38.570020 oplangchain-0.1.3/oplangchain/chains/openai_functions/openapi.py
+-rw-r--r--   0        0        0     3725 2023-08-08 04:52:52.701599 oplangchain-0.1.3/oplangchain/chains/openai_functions/qa_with_structure.py
+-rw-r--r--   0        0        0     2665 2023-08-08 04:52:52.698599 oplangchain-0.1.3/oplangchain/chains/openai_functions/tagging.py
+-rw-r--r--   0        0        0     1257 2023-08-07 21:21:40.512154 oplangchain-0.1.3/oplangchain/chains/openai_functions/utils.py
+-rw-r--r--   0        0        0     1969 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/prompt_selector.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.513154 oplangchain-0.1.3/oplangchain/chains/qa_generation/__init__.py
+-rw-r--r--   0        0        0     2458 2023-08-08 04:52:52.698599 oplangchain-0.1.3/oplangchain/chains/qa_generation/base.py
+-rw-r--r--   0        0        0     1871 2023-08-08 04:52:52.698599 oplangchain-0.1.3/oplangchain/chains/qa_generation/prompt.py
+-rw-r--r--   0        0        0      175 2023-08-08 04:52:52.696616 oplangchain-0.1.3/oplangchain/chains/qa_with_sources/__init__.py
+-rw-r--r--   0        0        0     7741 2023-08-08 04:52:52.698599 oplangchain-0.1.3/oplangchain/chains/qa_with_sources/base.py
+-rw-r--r--   0        0        0     6825 2023-08-08 04:52:52.698599 oplangchain-0.1.3/oplangchain/chains/qa_with_sources/loading.py
+-rw-r--r--   0        0        0     6968 2023-08-08 04:52:52.698599 oplangchain-0.1.3/oplangchain/chains/qa_with_sources/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1315 2023-08-08 04:52:52.696616 oplangchain-0.1.3/oplangchain/chains/qa_with_sources/refine_prompts.py
+-rw-r--r--   0        0        0     2354 2023-08-08 04:52:52.696616 oplangchain-0.1.3/oplangchain/chains/qa_with_sources/retrieval.py
+-rw-r--r--   0        0        0     6578 2023-08-08 04:52:52.696616 oplangchain-0.1.3/oplangchain/chains/qa_with_sources/stuff_prompt.py
+-rw-r--r--   0        0        0     2811 2023-08-08 04:52:52.696616 oplangchain-0.1.3/oplangchain/chains/qa_with_sources/vector_db.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.519154 oplangchain-0.1.3/oplangchain/chains/query_constructor/__init__.py
+-rw-r--r--   0        0        0     5841 2023-08-08 20:14:02.075598 oplangchain-0.1.3/oplangchain/chains/query_constructor/base.py
+-rw-r--r--   0        0        0     3129 2023-08-07 21:21:40.520154 oplangchain-0.1.3/oplangchain/chains/query_constructor/ir.py
+-rw-r--r--   0        0        0     4756 2023-08-08 04:52:52.696616 oplangchain-0.1.3/oplangchain/chains/query_constructor/parser.py
+-rw-r--r--   0        0        0     6448 2023-08-08 04:52:52.696616 oplangchain-0.1.3/oplangchain/chains/query_constructor/prompt.py
+-rw-r--r--   0        0        0      303 2023-08-07 21:21:40.521153 oplangchain-0.1.3/oplangchain/chains/query_constructor/schema.py
+-rw-r--r--   0        0        0     8578 2023-08-08 04:52:52.695606 oplangchain-0.1.3/oplangchain/chains/question_answering/__init__.py
+-rw-r--r--   0        0        0     8009 2023-08-08 04:52:52.696616 oplangchain-0.1.3/oplangchain/chains/question_answering/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1621 2023-08-08 04:52:52.695606 oplangchain-0.1.3/oplangchain/chains/question_answering/map_rerank_prompt.py
+-rw-r--r--   0        0        0     2732 2023-08-08 04:52:52.695606 oplangchain-0.1.3/oplangchain/chains/question_answering/refine_prompts.py
+-rw-r--r--   0        0        0     1141 2023-08-08 04:52:52.695606 oplangchain-0.1.3/oplangchain/chains/question_answering/stuff_prompt.py
+-rw-r--r--   0        0        0       62 2023-08-07 21:21:40.524154 oplangchain-0.1.3/oplangchain/chains/retrieval_qa/__init__.py
+-rw-r--r--   0        0        0     9794 2023-08-08 04:52:52.695606 oplangchain-0.1.3/oplangchain/chains/retrieval_qa/base.py
+-rw-r--r--   0        0        0      396 2023-08-08 04:52:52.695606 oplangchain-0.1.3/oplangchain/chains/retrieval_qa/prompt.py
+-rw-r--r--   0        0        0      415 2023-08-08 04:52:52.667997 oplangchain-0.1.3/oplangchain/chains/router/__init__.py
+-rw-r--r--   0        0        0     4560 2023-08-08 04:52:52.695606 oplangchain-0.1.3/oplangchain/chains/router/base.py
+-rw-r--r--   0        0        0     1980 2023-08-08 04:52:52.695606 oplangchain-0.1.3/oplangchain/chains/router/embedding_router.py
+-rw-r--r--   0        0        0     4214 2023-08-08 20:14:02.138597 oplangchain-0.1.3/oplangchain/chains/router/llm_router.py
+-rw-r--r--   0        0        0     2576 2023-08-08 04:52:52.694599 oplangchain-0.1.3/oplangchain/chains/router/multi_prompt.py
+-rw-r--r--   0        0        0     1123 2023-08-07 21:21:40.528154 oplangchain-0.1.3/oplangchain/chains/router/multi_prompt_prompt.py
+-rw-r--r--   0        0        0     1079 2023-08-07 21:21:40.528154 oplangchain-0.1.3/oplangchain/chains/router/multi_retrieval_prompt.py
+-rw-r--r--   0        0        0     3657 2023-08-08 04:52:52.667997 oplangchain-0.1.3/oplangchain/chains/router/multi_retrieval_qa.py
+-rw-r--r--   0        0        0     7487 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/sequential.py
+-rw-r--r--   0        0        0       47 2023-08-07 21:21:40.530154 oplangchain-0.1.3/oplangchain/chains/sql_database/__init__.py
+-rw-r--r--   0        0        0    14206 2023-08-08 04:52:52.667997 oplangchain-0.1.3/oplangchain/chains/sql_database/prompt.py
+-rw-r--r--   0        0        0     2078 2023-08-08 04:52:52.667997 oplangchain-0.1.3/oplangchain/chains/sql_database/query.py
+-rw-r--r--   0        0        0     5715 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/summarize/__init__.py
+-rw-r--r--   0        0        0      235 2023-08-08 04:52:52.667997 oplangchain-0.1.3/oplangchain/chains/summarize/map_reduce_prompt.py
+-rw-r--r--   0        0        0      807 2023-08-08 04:52:52.667997 oplangchain-0.1.3/oplangchain/chains/summarize/refine_prompts.py
+-rw-r--r--   0        0        0      235 2023-08-08 04:52:52.667997 oplangchain-0.1.3/oplangchain/chains/summarize/stuff_prompt.py
+-rw-r--r--   0        0        0     2239 2023-08-08 04:52:52.666996 oplangchain-0.1.3/oplangchain/chains/transform.py
+-rw-r--r--   0        0        0     1374 2023-08-08 04:52:52.725542 oplangchain-0.1.3/oplangchain/chat_models/__init__.py
+-rw-r--r--   0        0        0     7002 2023-08-08 04:52:52.729543 oplangchain-0.1.3/oplangchain/chat_models/anthropic.py
+-rw-r--r--   0        0        0     4713 2023-08-08 04:52:52.729543 oplangchain-0.1.3/oplangchain/chat_models/azure_openai.py
+-rw-r--r--   0        0        0     5419 2023-08-08 20:14:02.185599 oplangchain-0.1.3/oplangchain/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0    23298 2023-08-08 05:09:17.586726 oplangchain-0.1.3/oplangchain/chat_models/base.py
+-rw-r--r--   0        0        0     1046 2023-08-08 04:52:52.728543 oplangchain-0.1.3/oplangchain/chat_models/fake.py
+-rw-r--r--   0        0        0    11139 2023-08-08 04:52:52.727543 oplangchain-0.1.3/oplangchain/chat_models/google_palm.py
+-rw-r--r--   0        0        0     4027 2023-08-08 04:52:52.726542 oplangchain-0.1.3/oplangchain/chat_models/human.py
+-rw-r--r--   0        0        0    15237 2023-08-08 04:52:52.726542 oplangchain-0.1.3/oplangchain/chat_models/jinachat.py
+-rw-r--r--   0        0        0     6865 2023-08-08 04:52:52.726542 oplangchain-0.1.3/oplangchain/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0    22380 2023-08-08 04:52:52.726542 oplangchain-0.1.3/oplangchain/chat_models/openai.py
+-rw-r--r--   0        0        0     5174 2023-08-08 04:52:52.726542 oplangchain-0.1.3/oplangchain/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0     6018 2023-08-08 04:52:52.725542 oplangchain-0.1.3/oplangchain/chat_models/vertexai.py
+-rw-r--r--   0        0        0      685 2023-08-07 21:21:40.540154 oplangchain-0.1.3/oplangchain/docker-compose.yaml
+-rw-r--r--   0        0        0      525 2023-08-08 04:52:52.729543 oplangchain-0.1.3/oplangchain/docstore/__init__.py
+-rw-r--r--   0        0        0     1075 2023-08-08 04:52:52.736001 oplangchain-0.1.3/oplangchain/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      838 2023-08-08 04:52:52.732543 oplangchain-0.1.3/oplangchain/docstore/base.py
+-rw-r--r--   0        0        0       64 2023-08-08 04:52:52.732543 oplangchain-0.1.3/oplangchain/docstore/document.py
+-rw-r--r--   0        0        0     1606 2023-08-08 04:52:52.730543 oplangchain-0.1.3/oplangchain/docstore/in_memory.py
+-rw-r--r--   0        0        0     1483 2023-08-08 04:52:52.729543 oplangchain-0.1.3/oplangchain/docstore/wikipedia.py
+-rw-r--r--   0        0        0    13128 2023-08-08 04:52:52.566956 oplangchain-0.1.3/oplangchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2851 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/acreom.py
+-rw-r--r--   0        0        0      845 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0     1277 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/airtable.py
+-rw-r--r--   0        0        0     2724 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0     1144 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/arxiv.py
+-rw-r--r--   0        0        0     4865 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/async_html.py
+-rw-r--r--   0        0        0      580 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0     1618 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0     1637 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0     3047 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/base.py
+-rw-r--r--   0        0        0     3934 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/bibtex.py
+-rw-r--r--   0        0        0     3151 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/bigquery.py
+-rw-r--r--   0        0        0     2726 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/bilibili.py
+-rw-r--r--   0        0        0    10099 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/blackboard.py
+-rw-r--r--   0        0        0      332 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0     4283 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0     5765 2023-08-07 21:21:40.551154 oplangchain-0.1.3/oplangchain/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0     1510 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0     5732 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/blockchain.py
+-rw-r--r--   0        0        0     1074 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/brave_search.py
+-rw-r--r--   0        0        0     2136 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/browserless.py
+-rw-r--r--   0        0        0     2030 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0      556 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0     2153 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/concurrent.py
+-rw-r--r--   0        0        0    25403 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/confluence.py
+-rw-r--r--   0        0        0     1072 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/conllu.py
+-rw-r--r--   0        0        0     4203 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0     5905 2023-08-08 04:52:52.609953 oplangchain-0.1.3/oplangchain/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0     4997 2023-08-08 04:52:52.608952 oplangchain-0.1.3/oplangchain/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0     1329 2023-08-08 04:52:52.608952 oplangchain-0.1.3/oplangchain/document_loaders/dataframe.py
+-rw-r--r--   0        0        0     2114 2023-08-08 04:52:52.607953 oplangchain-0.1.3/oplangchain/document_loaders/diffbot.py
+-rw-r--r--   0        0        0     5104 2023-08-08 04:52:52.607953 oplangchain-0.1.3/oplangchain/document_loaders/directory.py
+-rw-r--r--   0        0        0     1265 2023-08-08 04:52:52.607953 oplangchain-0.1.3/oplangchain/document_loaders/discord.py
+-rw-r--r--   0        0        0    13220 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0     6095 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/dropbox.py
+-rw-r--r--   0        0        0     3185 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0     3792 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/email.py
+-rw-r--r--   0        0        0     8951 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/embaas.py
+-rw-r--r--   0        0        0     1514 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/epub.py
+-rw-r--r--   0        0        0     7812 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/etherscan.py
+-rw-r--r--   0        0        0     5748 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/evernote.py
+-rw-r--r--   0        0        0     1668 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/excel.py
+-rw-r--r--   0        0        0     1302 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0     2245 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/fauna.py
+-rw-r--r--   0        0        0     1575 2023-08-08 04:52:52.606954 oplangchain-0.1.3/oplangchain/document_loaders/figma.py
+-rw-r--r--   0        0        0     1579 2023-08-08 04:52:52.605952 oplangchain-0.1.3/oplangchain/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0     1737 2023-08-08 04:52:52.605952 oplangchain-0.1.3/oplangchain/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0     4543 2023-08-08 04:52:52.605952 oplangchain-0.1.3/oplangchain/document_loaders/generic.py
+-rw-r--r--   0        0        0     1686 2023-08-08 04:52:52.605952 oplangchain-0.1.3/oplangchain/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0     4142 2023-08-08 04:52:52.605952 oplangchain-0.1.3/oplangchain/document_loaders/git.py
+-rw-r--r--   0        0        0     3110 2023-08-08 04:52:52.605540 oplangchain-0.1.3/oplangchain/document_loaders/gitbook.py
+-rw-r--r--   0        0        0     6874 2023-08-08 04:52:52.604954 oplangchain-0.1.3/oplangchain/document_loaders/github.py
+-rw-r--r--   0        0        0    13930 2023-08-08 04:52:52.604954 oplangchain-0.1.3/oplangchain/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      973 2023-08-08 04:52:52.603954 oplangchain-0.1.3/oplangchain/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0     1559 2023-08-07 21:21:40.568154 oplangchain-0.1.3/oplangchain/document_loaders/helpers.py
+-rw-r--r--   0        0        0     2065 2023-08-08 04:52:52.603954 oplangchain-0.1.3/oplangchain/document_loaders/hn.py
+-rw-r--r--   0        0        0     1208 2023-08-08 04:52:52.602952 oplangchain-0.1.3/oplangchain/document_loaders/html.py
+-rw-r--r--   0        0        0     2122 2023-08-08 04:52:52.600954 oplangchain-0.1.3/oplangchain/document_loaders/html_bs.py
+-rw-r--r--   0        0        0     3029 2023-08-08 04:52:52.599953 oplangchain-0.1.3/oplangchain/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0     7654 2023-08-08 04:52:52.599953 oplangchain-0.1.3/oplangchain/document_loaders/ifixit.py
+-rw-r--r--   0        0        0     1190 2023-08-08 04:52:52.599953 oplangchain-0.1.3/oplangchain/document_loaders/image.py
+-rw-r--r--   0        0        0     3103 2023-08-08 04:52:52.599953 oplangchain-0.1.3/oplangchain/document_loaders/image_captions.py
+-rw-r--r--   0        0        0      491 2023-08-08 04:52:52.599953 oplangchain-0.1.3/oplangchain/document_loaders/imsdb.py
+-rw-r--r--   0        0        0     1740 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/iugu.py
+-rw-r--r--   0        0        0     3705 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/joplin.py
+-rw-r--r--   0        0        0     5491 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/json_loader.py
+-rw-r--r--   0        0        0     2056 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/larksuite.py
+-rw-r--r--   0        0        0     1832 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/markdown.py
+-rw-r--r--   0        0        0     3134 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/mastodon.py
+-rw-r--r--   0        0        0     3299 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/max_compute.py
+-rw-r--r--   0        0        0     3487 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      842 2023-08-08 04:52:52.598953 oplangchain-0.1.3/oplangchain/document_loaders/merge.py
+-rw-r--r--   0        0        0     2604 2023-08-08 04:52:52.597955 oplangchain-0.1.3/oplangchain/document_loaders/mhtml.py
+-rw-r--r--   0        0        0     3137 2023-08-08 04:52:52.596954 oplangchain-0.1.3/oplangchain/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0     4293 2023-08-08 04:52:52.595955 oplangchain-0.1.3/oplangchain/document_loaders/news.py
+-rw-r--r--   0        0        0     4285 2023-08-08 04:52:52.595955 oplangchain-0.1.3/oplangchain/document_loaders/notebook.py
+-rw-r--r--   0        0        0      745 2023-08-08 04:52:52.593953 oplangchain-0.1.3/oplangchain/document_loaders/notion.py
+-rw-r--r--   0        0        0     5896 2023-08-08 04:52:52.593953 oplangchain-0.1.3/oplangchain/document_loaders/notiondb.py
+-rw-r--r--   0        0        0     1090 2023-08-08 04:52:52.590953 oplangchain-0.1.3/oplangchain/document_loaders/nuclia.py
+-rw-r--r--   0        0        0     3600 2023-08-08 04:52:52.590953 oplangchain-0.1.3/oplangchain/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0     4751 2023-08-08 04:52:52.590953 oplangchain-0.1.3/oplangchain/document_loaders/obs_file.py
+-rw-r--r--   0        0        0     2541 2023-08-08 04:52:52.590953 oplangchain-0.1.3/oplangchain/document_loaders/obsidian.py
+-rw-r--r--   0        0        0     1797 2023-08-08 04:52:52.590953 oplangchain-0.1.3/oplangchain/document_loaders/odt.py
+-rw-r--r--   0        0        0     8641 2023-08-08 04:52:52.589954 oplangchain-0.1.3/oplangchain/document_loaders/onedrive.py
+-rw-r--r--   0        0        0     1114 2023-08-08 04:52:52.589954 oplangchain-0.1.3/oplangchain/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0     1326 2023-08-08 04:52:52.588955 oplangchain-0.1.3/oplangchain/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0     1769 2023-08-08 04:52:52.587955 oplangchain-0.1.3/oplangchain/document_loaders/org_mode.py
+-rw-r--r--   0        0        0      655 2023-08-08 04:52:52.610953 oplangchain-0.1.3/oplangchain/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0     6089 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0     2474 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0     5765 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0      101 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0     1608 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      119 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0      499 2023-08-07 21:21:40.586154 oplangchain-0.1.3/oplangchain/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0     2090 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0     4690 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0     1664 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0     8807 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0      920 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0      482 2023-08-08 04:52:52.611952 oplangchain-0.1.3/oplangchain/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0    20559 2023-08-08 04:52:52.586953 oplangchain-0.1.3/oplangchain/document_loaders/pdf.py
+-rw-r--r--   0        0        0     2521 2023-08-08 04:52:52.586953 oplangchain-0.1.3/oplangchain/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0     1416 2023-08-08 04:52:52.585954 oplangchain-0.1.3/oplangchain/document_loaders/psychic.py
+-rw-r--r--   0        0        0     3422 2023-08-08 04:52:52.585954 oplangchain-0.1.3/oplangchain/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0      527 2023-08-08 04:52:52.585954 oplangchain-0.1.3/oplangchain/document_loaders/python.py
+-rw-r--r--   0        0        0     3530 2023-08-08 04:52:52.585954 oplangchain-0.1.3/oplangchain/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0    12432 2023-08-08 04:52:52.585954 oplangchain-0.1.3/oplangchain/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0     4609 2023-08-08 04:52:52.584953 oplangchain-0.1.3/oplangchain/document_loaders/reddit.py
+-rw-r--r--   0        0        0      726 2023-08-08 04:52:52.584953 oplangchain-0.1.3/oplangchain/document_loaders/roam.py
+-rw-r--r--   0        0        0     4441 2023-08-08 04:52:52.584953 oplangchain-0.1.3/oplangchain/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0     4938 2023-08-08 04:52:52.584953 oplangchain-0.1.3/oplangchain/document_loaders/rss.py
+-rw-r--r--   0        0        0     1825 2023-08-08 04:52:52.584953 oplangchain-0.1.3/oplangchain/document_loaders/rst.py
+-rw-r--r--   0        0        0     2054 2023-08-08 04:52:52.583955 oplangchain-0.1.3/oplangchain/document_loaders/rtf.py
+-rw-r--r--   0        0        0     1231 2023-08-08 04:52:52.583955 oplangchain-0.1.3/oplangchain/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0     1322 2023-08-08 04:52:52.582954 oplangchain-0.1.3/oplangchain/document_loaders/s3_file.py
+-rw-r--r--   0        0        0     5012 2023-08-08 04:52:52.582954 oplangchain-0.1.3/oplangchain/document_loaders/sitemap.py
+-rw-r--r--   0        0        0     4184 2023-08-08 04:52:52.582954 oplangchain-0.1.3/oplangchain/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0     4830 2023-08-08 04:52:52.582954 oplangchain-0.1.3/oplangchain/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0     2065 2023-08-08 04:52:52.581954 oplangchain-0.1.3/oplangchain/document_loaders/spreedly.py
+-rw-r--r--   0        0        0      891 2023-08-08 04:52:52.581954 oplangchain-0.1.3/oplangchain/document_loaders/srt.py
+-rw-r--r--   0        0        0     1861 2023-08-08 04:52:52.580954 oplangchain-0.1.3/oplangchain/document_loaders/stripe.py
+-rw-r--r--   0        0        0     9047 2023-08-08 04:52:52.580954 oplangchain-0.1.3/oplangchain/document_loaders/telegram.py
+-rw-r--r--   0        0        0     1846 2023-08-08 04:52:52.579957 oplangchain-0.1.3/oplangchain/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0     1758 2023-08-08 04:52:52.579957 oplangchain-0.1.3/oplangchain/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0     1999 2023-08-08 04:52:52.580954 oplangchain-0.1.3/oplangchain/document_loaders/text.py
+-rw-r--r--   0        0        0      998 2023-08-08 04:52:52.579957 oplangchain-0.1.3/oplangchain/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0     1653 2023-08-08 04:52:52.579957 oplangchain-0.1.3/oplangchain/document_loaders/toml.py
+-rw-r--r--   0        0        0     6602 2023-08-08 04:52:52.579957 oplangchain-0.1.3/oplangchain/document_loaders/trello.py
+-rw-r--r--   0        0        0     1282 2023-08-08 04:52:52.576954 oplangchain-0.1.3/oplangchain/document_loaders/tsv.py
+-rw-r--r--   0        0        0     3458 2023-08-08 04:52:52.576954 oplangchain-0.1.3/oplangchain/document_loaders/twitter.py
+-rw-r--r--   0        0        0    13889 2023-08-08 04:52:52.576954 oplangchain-0.1.3/oplangchain/document_loaders/unstructured.py
+-rw-r--r--   0        0        0     6017 2023-08-08 04:52:52.574953 oplangchain-0.1.3/oplangchain/document_loaders/url.py
+-rw-r--r--   0        0        0     4951 2023-08-08 04:52:52.574953 oplangchain-0.1.3/oplangchain/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0     5225 2023-08-08 04:52:52.574953 oplangchain-0.1.3/oplangchain/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0     1639 2023-08-08 04:52:52.570954 oplangchain-0.1.3/oplangchain/document_loaders/weather.py
+-rw-r--r--   0        0        0     8015 2023-08-08 04:52:52.570954 oplangchain-0.1.3/oplangchain/document_loaders/web_base.py
+-rw-r--r--   0        0        0     1765 2023-08-08 04:52:52.569953 oplangchain-0.1.3/oplangchain/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0     2188 2023-08-08 04:52:52.569953 oplangchain-0.1.3/oplangchain/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0     4561 2023-08-08 04:52:52.568953 oplangchain-0.1.3/oplangchain/document_loaders/word_document.py
+-rw-r--r--   0        0        0     1483 2023-08-08 04:52:52.567953 oplangchain-0.1.3/oplangchain/document_loaders/xml.py
+-rw-r--r--   0        0        0     1627 2023-08-08 04:52:52.567953 oplangchain-0.1.3/oplangchain/document_loaders/xorbits.py
+-rw-r--r--   0        0        0    14680 2023-08-08 04:52:52.566956 oplangchain-0.1.3/oplangchain/document_loaders/youtube.py
+-rw-r--r--   0        0        0     1470 2023-08-08 20:14:02.707598 oplangchain-0.1.3/oplangchain/document_transformers/__init__.py
+-rw-r--r--   0        0        0     3452 2023-08-08 04:52:52.566956 oplangchain-0.1.3/oplangchain/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0     2176 2023-08-08 04:52:52.565955 oplangchain-0.1.3/oplangchain/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0     2320 2023-08-08 04:52:52.565955 oplangchain-0.1.3/oplangchain/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0     8084 2023-08-08 04:52:52.564953 oplangchain-0.1.3/oplangchain/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0     1297 2023-08-08 04:52:52.564953 oplangchain-0.1.3/oplangchain/document_transformers/html2text.py
+-rw-r--r--   0        0        0     1376 2023-08-08 04:52:52.563954 oplangchain-0.1.3/oplangchain/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0     1473 2023-08-08 04:52:52.562953 oplangchain-0.1.3/oplangchain/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0     6220 2023-08-08 04:52:52.561953 oplangchain-0.1.3/oplangchain/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     4678 2023-08-08 04:52:52.547953 oplangchain-0.1.3/oplangchain/embeddings/__init__.py
+-rw-r--r--   0        0        0     9596 2023-08-08 04:52:52.561953 oplangchain-0.1.3/oplangchain/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0     1633 2023-08-08 04:52:52.560954 oplangchain-0.1.3/oplangchain/embeddings/awa.py
+-rw-r--r--   0        0        0      655 2023-08-07 21:21:40.614153 oplangchain-0.1.3/oplangchain/embeddings/base.py
+-rw-r--r--   0        0        0     5484 2023-08-08 04:52:52.560954 oplangchain-0.1.3/oplangchain/embeddings/bedrock.py
+-rw-r--r--   0        0        0     6553 2023-08-08 04:52:52.560954 oplangchain-0.1.3/oplangchain/embeddings/clarifai.py
+-rw-r--r--   0        0        0     3383 2023-08-08 04:52:52.560954 oplangchain-0.1.3/oplangchain/embeddings/cohere.py
+-rw-r--r--   0        0        0     4890 2023-08-08 04:52:52.560954 oplangchain-0.1.3/oplangchain/embeddings/dashscope.py
+-rw-r--r--   0        0        0     4400 2023-08-08 04:52:52.557952 oplangchain-0.1.3/oplangchain/embeddings/deepinfra.py
+-rw-r--r--   0        0        0     2798 2023-08-08 04:52:52.556953 oplangchain-0.1.3/oplangchain/embeddings/edenai.py
+-rw-r--r--   0        0        0     8384 2023-08-08 04:52:52.555960 oplangchain-0.1.3/oplangchain/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0     4794 2023-08-08 04:52:52.554955 oplangchain-0.1.3/oplangchain/embeddings/embaas.py
+-rw-r--r--   0        0        0     1497 2023-08-08 04:52:52.551953 oplangchain-0.1.3/oplangchain/embeddings/fake.py
+-rw-r--r--   0        0        0     2686 2023-08-08 04:52:52.551953 oplangchain-0.1.3/oplangchain/embeddings/google_palm.py
+-rw-r--r--   0        0        0     1641 2023-08-08 04:52:52.533954 oplangchain-0.1.3/oplangchain/embeddings/gpt4all.py
+-rw-r--r--   0        0        0     6040 2023-08-08 04:52:52.537954 oplangchain-0.1.3/oplangchain/embeddings/huggingface.py
+-rw-r--r--   0        0        0     3686 2023-08-08 04:52:52.550953 oplangchain-0.1.3/oplangchain/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0     3449 2023-08-08 04:52:52.538954 oplangchain-0.1.3/oplangchain/embeddings/jina.py
+-rw-r--r--   0        0        0     4025 2023-08-08 04:52:52.542952 oplangchain-0.1.3/oplangchain/embeddings/llamacpp.py
+-rw-r--r--   0        0        0    12079 2023-08-08 04:52:52.550953 oplangchain-0.1.3/oplangchain/embeddings/localai.py
+-rw-r--r--   0        0        0     4690 2023-08-08 04:52:52.543952 oplangchain-0.1.3/oplangchain/embeddings/minimax.py
+-rw-r--r--   0        0        0     2244 2023-08-08 04:52:52.543952 oplangchain-0.1.3/oplangchain/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0     2361 2023-08-08 04:52:52.550953 oplangchain-0.1.3/oplangchain/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0     5883 2023-08-08 04:52:52.545953 oplangchain-0.1.3/oplangchain/embeddings/mosaicml.py
+-rw-r--r--   0        0        0     2176 2023-08-08 04:52:52.546953 oplangchain-0.1.3/oplangchain/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0     3402 2023-08-08 04:52:52.549953 oplangchain-0.1.3/oplangchain/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0    19945 2023-08-08 04:52:52.546953 oplangchain-0.1.3/oplangchain/embeddings/openai.py
+-rw-r--r--   0        0        0     7110 2023-08-08 04:52:52.547953 oplangchain-0.1.3/oplangchain/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     3755 2023-08-08 04:52:52.549953 oplangchain-0.1.3/oplangchain/embeddings/self_hosted.py
+-rw-r--r--   0        0        0     6552 2023-08-08 04:52:52.547953 oplangchain-0.1.3/oplangchain/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      181 2023-08-08 04:52:52.547953 oplangchain-0.1.3/oplangchain/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0     3728 2023-08-08 04:52:52.547953 oplangchain-0.1.3/oplangchain/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0     2390 2023-08-08 04:52:52.547953 oplangchain-0.1.3/oplangchain/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0     1881 2023-08-08 04:52:52.547953 oplangchain-0.1.3/oplangchain/embeddings/vertexai.py
+-rw-r--r--   0        0        0     3309 2023-08-08 04:52:52.547953 oplangchain-0.1.3/oplangchain/embeddings/xinference.py
+-rw-r--r--   0        0        0      478 2023-08-08 04:52:52.346953 oplangchain-0.1.3/oplangchain/env.py
+-rw-r--r--   0        0        0     5062 2023-08-08 04:52:52.517955 oplangchain-0.1.3/oplangchain/evaluation/__init__.py
+-rw-r--r--   0        0        0      167 2023-08-08 04:52:52.526953 oplangchain-0.1.3/oplangchain/evaluation/agents/__init__.py
+-rw-r--r--   0        0        0    13177 2023-08-08 04:52:52.530953 oplangchain-0.1.3/oplangchain/evaluation/agents/trajectory_eval_chain.py
+-rw-r--r--   0        0        0     5939 2023-08-08 04:52:52.529956 oplangchain-0.1.3/oplangchain/evaluation/agents/trajectory_eval_prompt.py
+-rw-r--r--   0        0        0     1404 2023-08-08 04:52:52.525951 oplangchain-0.1.3/oplangchain/evaluation/comparison/__init__.py
+-rw-r--r--   0        0        0    15065 2023-08-08 04:52:52.526953 oplangchain-0.1.3/oplangchain/evaluation/comparison/eval_chain.py
+-rw-r--r--   0        0        0     2177 2023-08-08 04:52:52.525951 oplangchain-0.1.3/oplangchain/evaluation/comparison/prompt.py
+-rw-r--r--   0        0        0     1638 2023-08-08 04:52:52.525951 oplangchain-0.1.3/oplangchain/evaluation/criteria/__init__.py
+-rw-r--r--   0        0        0    20332 2023-08-08 04:52:52.525951 oplangchain-0.1.3/oplangchain/evaluation/criteria/eval_chain.py
+-rw-r--r--   0        0        0     1753 2023-08-08 04:52:52.525951 oplangchain-0.1.3/oplangchain/evaluation/criteria/prompt.py
+-rw-r--r--   0        0        0      325 2023-08-08 04:52:52.522952 oplangchain-0.1.3/oplangchain/evaluation/embedding_distance/__init__.py
+-rw-r--r--   0        0        0    15489 2023-08-08 04:52:52.524954 oplangchain-0.1.3/oplangchain/evaluation/embedding_distance/base.py
+-rw-r--r--   0        0        0     5220 2023-08-08 04:52:52.518955 oplangchain-0.1.3/oplangchain/evaluation/loading.py
+-rw-r--r--   0        0        0      348 2023-08-08 04:52:52.519953 oplangchain-0.1.3/oplangchain/evaluation/qa/__init__.py
+-rw-r--r--   0        0        0    10001 2023-08-08 04:52:52.521954 oplangchain-0.1.3/oplangchain/evaluation/qa/eval_chain.py
+-rw-r--r--   0        0        0     3908 2023-08-08 04:52:52.521954 oplangchain-0.1.3/oplangchain/evaluation/qa/eval_prompt.py
+-rw-r--r--   0        0        0      966 2023-08-08 04:52:52.520955 oplangchain-0.1.3/oplangchain/evaluation/qa/generate_chain.py
+-rw-r--r--   0        0        0      605 2023-08-08 04:52:52.520955 oplangchain-0.1.3/oplangchain/evaluation/qa/generate_prompt.py
+-rw-r--r--   0        0        0    16806 2023-08-08 04:52:52.517955 oplangchain-0.1.3/oplangchain/evaluation/schema.py
+-rw-r--r--   0        0        0      287 2023-08-08 04:52:52.518955 oplangchain-0.1.3/oplangchain/evaluation/string_distance/__init__.py
+-rw-r--r--   0        0        0    14008 2023-08-08 04:52:52.518955 oplangchain-0.1.3/oplangchain/evaluation/string_distance/base.py
+-rw-r--r--   0        0        0      143 2023-08-08 04:52:52.346953 oplangchain-0.1.3/oplangchain/example_generator.py
+-rw-r--r--   0        0        0      164 2023-08-08 04:52:52.346953 oplangchain-0.1.3/oplangchain/formatting.py
+-rw-r--r--   0        0        0      769 2023-08-08 04:52:52.530953 oplangchain-0.1.3/oplangchain/graphs/__init__.py
+-rw-r--r--   0        0        0     6198 2023-08-07 21:21:40.642153 oplangchain-0.1.3/oplangchain/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0     1841 2023-08-07 21:21:40.643153 oplangchain-0.1.3/oplangchain/graphs/hugegraph.py
+-rw-r--r--   0        0        0     3559 2023-08-07 21:21:40.643153 oplangchain-0.1.3/oplangchain/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0      715 2023-08-08 04:52:52.532953 oplangchain-0.1.3/oplangchain/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0     7362 2023-08-07 21:21:40.644153 oplangchain-0.1.3/oplangchain/graphs/nebula_graph.py
+-rw-r--r--   0        0        0     3625 2023-08-07 21:21:40.645154 oplangchain-0.1.3/oplangchain/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0     6553 2023-08-07 21:21:40.645154 oplangchain-0.1.3/oplangchain/graphs/neptune_graph.py
+-rw-r--r--   0        0        0     5877 2023-08-07 21:21:40.646154 oplangchain-0.1.3/oplangchain/graphs/networkx_graph.py
+-rw-r--r--   0        0        0     9461 2023-08-07 21:21:40.646154 oplangchain-0.1.3/oplangchain/graphs/rdf_graph.py
+-rw-r--r--   0        0        0      211 2023-08-08 04:52:52.496954 oplangchain-0.1.3/oplangchain/indexes/__init__.py
+-rw-r--r--   0        0        0     1722 2023-08-08 04:52:52.496954 oplangchain-0.1.3/oplangchain/indexes/graph.py
+-rw-r--r--   0        0        0       49 2023-08-07 21:21:40.648155 oplangchain-0.1.3/oplangchain/indexes/prompts/__init__.py
+-rw-r--r--   0        0        0     1949 2023-08-08 04:52:52.499953 oplangchain-0.1.3/oplangchain/indexes/prompts/entity_extraction.py
+-rw-r--r--   0        0        0     1154 2023-08-08 04:52:52.497954 oplangchain-0.1.3/oplangchain/indexes/prompts/entity_summarization.py
+-rw-r--r--   0        0        0     1588 2023-08-08 04:52:52.498952 oplangchain-0.1.3/oplangchain/indexes/prompts/knowledge_triplet_extraction.py
+-rw-r--r--   0        0        0     3070 2023-08-08 04:52:52.496954 oplangchain-0.1.3/oplangchain/indexes/vectorstore.py
+-rw-r--r--   0        0        0      279 2023-08-08 04:52:52.346953 oplangchain-0.1.3/oplangchain/input.py
+-rw-r--r--   0        0        0     6508 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/__init__.py
+-rw-r--r--   0        0        0     5004 2023-08-08 04:52:52.517955 oplangchain-0.1.3/oplangchain/llms/ai21.py
+-rw-r--r--   0        0        0    11362 2023-08-08 04:52:52.517955 oplangchain-0.1.3/oplangchain/llms/aleph_alpha.py
+-rw-r--r--   0        0        0     3029 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0    11178 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/anthropic.py
+-rw-r--r--   0        0        0     4667 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/anyscale.py
+-rw-r--r--   0        0        0     5375 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/aviary.py
+-rw-r--r--   0        0        0    10224 2023-08-08 04:52:52.505530 oplangchain-0.1.3/oplangchain/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0     4319 2023-08-08 04:52:52.505952 oplangchain-0.1.3/oplangchain/llms/bananadev.py
+-rw-r--r--   0        0        0    34755 2023-08-08 05:09:17.579726 oplangchain-0.1.3/oplangchain/llms/base.py
+-rw-r--r--   0        0        0     2365 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/baseten.py
+-rw-r--r--   0        0        0     9070 2023-08-08 04:52:52.507954 oplangchain-0.1.3/oplangchain/llms/beam.py
+-rw-r--r--   0        0        0     6698 2023-08-08 04:52:52.508955 oplangchain-0.1.3/oplangchain/llms/bedrock.py
+-rw-r--r--   0        0        0     3783 2023-08-08 04:52:52.508955 oplangchain-0.1.3/oplangchain/llms/cerebriumai.py
+-rw-r--r--   0        0        0     3945 2023-08-08 04:52:52.508955 oplangchain-0.1.3/oplangchain/llms/chatglm.py
+-rw-r--r--   0        0        0     5812 2023-08-08 04:52:52.508955 oplangchain-0.1.3/oplangchain/llms/clarifai.py
+-rw-r--r--   0        0        0     7313 2023-08-08 04:52:52.508955 oplangchain-0.1.3/oplangchain/llms/cohere.py
+-rw-r--r--   0        0        0     4193 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/ctransformers.py
+-rw-r--r--   0        0        0    12072 2023-08-08 04:52:52.508955 oplangchain-0.1.3/oplangchain/llms/databricks.py
+-rw-r--r--   0        0        0     3765 2023-08-08 04:52:52.508955 oplangchain-0.1.3/oplangchain/llms/deepinfra.py
+-rw-r--r--   0        0        0     7455 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/edenai.py
+-rw-r--r--   0        0        0     1339 2023-08-08 04:52:52.509954 oplangchain-0.1.3/oplangchain/llms/fake.py
+-rw-r--r--   0        0        0    13047 2023-08-08 04:52:52.510953 oplangchain-0.1.3/oplangchain/llms/fireworks.py
+-rw-r--r--   0        0        0     3661 2023-08-08 04:52:52.510953 oplangchain-0.1.3/oplangchain/llms/forefrontai.py
+-rw-r--r--   0        0        0     5741 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/google_palm.py
+-rw-r--r--   0        0        0     5130 2023-08-08 04:52:52.511953 oplangchain-0.1.3/oplangchain/llms/gooseai.py
+-rw-r--r--   0        0        0     6320 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/gpt4all.py
+-rw-r--r--   0        0        0     5462 2023-08-08 04:52:52.511953 oplangchain-0.1.3/oplangchain/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0     4613 2023-08-08 04:52:52.511953 oplangchain-0.1.3/oplangchain/llms/huggingface_hub.py
+-rw-r--r--   0        0        0     6576 2023-08-08 04:52:52.512955 oplangchain-0.1.3/oplangchain/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0     9723 2023-08-08 04:52:52.512955 oplangchain-0.1.3/oplangchain/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0     2547 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/human.py
+-rw-r--r--   0        0        0     5071 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/koboldai.py
+-rw-r--r--   0        0        0    10905 2023-08-08 04:52:52.512955 oplangchain-0.1.3/oplangchain/llms/llamacpp.py
+-rw-r--r--   0        0        0     1253 2023-08-08 04:52:52.512955 oplangchain-0.1.3/oplangchain/llms/loading.py
+-rw-r--r--   0        0        0     1878 2023-08-08 04:52:52.512955 oplangchain-0.1.3/oplangchain/llms/manifest.py
+-rw-r--r--   0        0        0     5162 2023-08-08 04:52:52.512955 oplangchain-0.1.3/oplangchain/llms/minimax.py
+-rw-r--r--   0        0        0     2925 2023-08-08 04:52:52.516955 oplangchain-0.1.3/oplangchain/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0     3247 2023-08-08 04:52:52.512955 oplangchain-0.1.3/oplangchain/llms/modal.py
+-rw-r--r--   0        0        0     6752 2023-08-08 04:52:52.512955 oplangchain-0.1.3/oplangchain/llms/mosaicml.py
+-rw-r--r--   0        0        0     5450 2023-08-08 04:52:52.513954 oplangchain-0.1.3/oplangchain/llms/nlpcloud.py
+-rw-r--r--   0        0        0     3814 2023-08-08 04:52:52.513954 oplangchain-0.1.3/oplangchain/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0    34744 2023-08-08 04:52:52.513954 oplangchain-0.1.3/oplangchain/llms/openai.py
+-rw-r--r--   0        0        0     9930 2023-08-08 04:52:52.514953 oplangchain-0.1.3/oplangchain/llms/openllm.py
+-rw-r--r--   0        0        0      796 2023-08-08 04:52:52.514953 oplangchain-0.1.3/oplangchain/llms/openlm.py
+-rw-r--r--   0        0        0     5273 2023-08-08 04:52:52.514953 oplangchain-0.1.3/oplangchain/llms/petals.py
+-rw-r--r--   0        0        0     4023 2023-08-08 04:52:52.514953 oplangchain-0.1.3/oplangchain/llms/pipelineai.py
+-rw-r--r--   0        0        0     1531 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/predibase.py
+-rw-r--r--   0        0        0     4372 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/predictionguard.py
+-rw-r--r--   0        0        0     8692 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0     5168 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/replicate.py
+-rw-r--r--   0        0        0     7343 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/rwkv.py
+-rw-r--r--   0        0        0     8821 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     7685 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/self_hosted.py
+-rw-r--r--   0        0        0     7699 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0     4573 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/stochasticai.py
+-rw-r--r--   0        0        0     7587 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/textgen.py
+-rw-r--r--   0        0        0     7882 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/tongyi.py
+-rw-r--r--   0        0        0      246 2023-08-07 21:21:40.678154 oplangchain-0.1.3/oplangchain/llms/utils.py
+-rw-r--r--   0        0        0     7717 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/vertexai.py
+-rw-r--r--   0        0        0     3984 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/vllm.py
+-rw-r--r--   0        0        0     4919 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/writer.py
+-rw-r--r--   0        0        0     6017 2023-08-08 04:52:52.515962 oplangchain-0.1.3/oplangchain/llms/xinference.py
+-rw-r--r--   0        0        0       41 2023-08-07 21:21:40.680153 oplangchain-0.1.3/oplangchain/load/__init__.py
+-rw-r--r--   0        0        0      755 2023-08-08 04:52:52.496954 oplangchain-0.1.3/oplangchain/load/dump.py
+-rw-r--r--   0        0        0     4039 2023-08-08 04:52:52.496954 oplangchain-0.1.3/oplangchain/load/load.py
+-rw-r--r--   0        0        0     4618 2023-08-07 21:21:40.681154 oplangchain-0.1.3/oplangchain/load/serializable.py
+-rw-r--r--   0        0        0     2872 2023-08-08 04:52:52.479955 oplangchain-0.1.3/oplangchain/memory/__init__.py
+-rw-r--r--   0        0        0     3074 2023-08-08 04:52:52.490953 oplangchain-0.1.3/oplangchain/memory/buffer.py
+-rw-r--r--   0        0        0     1232 2023-08-08 04:52:52.485953 oplangchain-0.1.3/oplangchain/memory/buffer_window.py
+-rw-r--r--   0        0        0     1618 2023-08-08 04:52:52.485953 oplangchain-0.1.3/oplangchain/memory/chat_memory.py
+-rw-r--r--   0        0        0     1619 2023-08-08 20:14:03.318597 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0     2388 2023-08-08 20:14:03.330600 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0     6514 2023-08-08 20:14:03.393600 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0     2885 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0     1383 2023-08-08 20:14:03.323597 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/file.py
+-rw-r--r--   0        0        0     3353 2023-08-08 20:14:03.446597 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      588 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0     6852 2023-08-08 20:14:03.393600 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/momento.py
+-rw-r--r--   0        0        0     2740 2023-08-08 20:14:03.442598 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0     2665 2023-08-08 20:14:03.363598 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0     1968 2023-08-08 20:14:03.394597 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/redis.py
+-rw-r--r--   0        0        0     2918 2023-08-08 20:14:03.508597 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/sql.py
+-rw-r--r--   0        0        0     1180 2023-08-08 04:52:52.492952 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0     6406 2023-08-08 04:52:52.492952 oplangchain-0.1.3/oplangchain/memory/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     2893 2023-08-08 04:52:52.483955 oplangchain-0.1.3/oplangchain/memory/combined.py
+-rw-r--r--   0        0        0    12998 2023-08-08 04:52:52.482954 oplangchain-0.1.3/oplangchain/memory/entity.py
+-rw-r--r--   0        0        0     5052 2023-08-08 20:14:03.560596 oplangchain-0.1.3/oplangchain/memory/kg.py
+-rw-r--r--   0        0        0     3102 2023-08-08 04:52:52.475954 oplangchain-0.1.3/oplangchain/memory/motorhead_memory.py
+-rw-r--r--   0        0        0     8178 2023-08-08 04:52:52.482954 oplangchain-0.1.3/oplangchain/memory/prompt.py
+-rw-r--r--   0        0        0      791 2023-08-08 04:52:52.476953 oplangchain-0.1.3/oplangchain/memory/readonly.py
+-rw-r--r--   0        0        0      758 2023-08-08 04:52:52.482954 oplangchain-0.1.3/oplangchain/memory/simple.py
+-rw-r--r--   0        0        0     3354 2023-08-08 04:52:52.482954 oplangchain-0.1.3/oplangchain/memory/summary.py
+-rw-r--r--   0        0        0     2939 2023-08-08 04:52:52.478954 oplangchain-0.1.3/oplangchain/memory/summary_buffer.py
+-rw-r--r--   0        0        0     1921 2023-08-08 04:52:52.481955 oplangchain-0.1.3/oplangchain/memory/token_buffer.py
+-rw-r--r--   0        0        0      689 2023-08-08 04:52:52.481955 oplangchain-0.1.3/oplangchain/memory/utils.py
+-rw-r--r--   0        0        0     2984 2023-08-08 04:52:52.480955 oplangchain-0.1.3/oplangchain/memory/vectorstore.py
+-rw-r--r--   0        0        0     5071 2023-08-08 04:52:52.479955 oplangchain-0.1.3/oplangchain/memory/zep_memory.py
+-rw-r--r--   0        0        0     3246 2023-08-08 04:52:52.346953 oplangchain-0.1.3/oplangchain/model_laboratory.py
+-rw-r--r--   0        0        0     1625 2023-08-08 20:14:03.465599 oplangchain-0.1.3/oplangchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1073 2023-08-08 04:52:52.496954 oplangchain-0.1.3/oplangchain/output_parsers/boolean.py
+-rw-r--r--   0        0        0     1765 2023-08-08 04:52:52.496954 oplangchain-0.1.3/oplangchain/output_parsers/combining.py
+-rw-r--r--   0        0        0     1821 2023-08-08 04:52:52.496954 oplangchain-0.1.3/oplangchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1140 2023-08-08 04:52:52.495954 oplangchain-0.1.3/oplangchain/output_parsers/enum.py
+-rw-r--r--   0        0        0     1830 2023-08-08 20:14:03.520600 oplangchain-0.1.3/oplangchain/output_parsers/fix.py
+-rw-r--r--   0        0        0      810 2023-08-07 21:21:40.702154 oplangchain-0.1.3/oplangchain/output_parsers/format_instructions.py
+-rw-r--r--   0        0        0     2211 2023-08-08 04:52:52.494953 oplangchain-0.1.3/oplangchain/output_parsers/json.py
+-rw-r--r--   0        0        0      941 2023-08-08 04:52:52.494953 oplangchain-0.1.3/oplangchain/output_parsers/list.py
+-rw-r--r--   0        0        0      704 2023-08-08 04:52:52.494953 oplangchain-0.1.3/oplangchain/output_parsers/loading.py
+-rw-r--r--   0        0        0     3354 2023-08-08 04:52:52.494953 oplangchain-0.1.3/oplangchain/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0      505 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/output_parsers/prompts.py
+-rw-r--r--   0        0        0     1735 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/output_parsers/pydantic.py
+-rw-r--r--   0        0        0     3167 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/output_parsers/rail_parser.py
+-rw-r--r--   0        0        0     1198 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/output_parsers/regex.py
+-rw-r--r--   0        0        0     1698 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/output_parsers/regex_dict.py
+-rw-r--r--   0        0        0     4717 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/output_parsers/retry.py
+-rw-r--r--   0        0        0     3078 2023-08-08 04:52:52.493953 oplangchain-0.1.3/oplangchain/output_parsers/structured.py
+-rw-r--r--   0        0        0     2762 2023-08-08 04:52:52.467952 oplangchain-0.1.3/oplangchain/prompts/__init__.py
+-rw-r--r--   0        0        0     3679 2023-08-08 04:52:52.474953 oplangchain-0.1.3/oplangchain/prompts/base.py
+-rw-r--r--   0        0        0    21577 2023-08-08 04:52:52.474953 oplangchain-0.1.3/oplangchain/prompts/chat.py
+-rw-r--r--   0        0        0      568 2023-08-08 20:14:03.567596 oplangchain-0.1.3/oplangchain/prompts/example_selector/__init__.py
+-rw-r--r--   0        0        0      526 2023-08-07 21:21:40.709154 oplangchain-0.1.3/oplangchain/prompts/example_selector/base.py
+-rw-r--r--   0        0        0     2437 2023-08-08 04:52:52.474953 oplangchain-0.1.3/oplangchain/prompts/example_selector/length_based.py
+-rw-r--r--   0        0        0     3802 2023-08-08 04:52:52.474953 oplangchain-0.1.3/oplangchain/prompts/example_selector/ngram_overlap.py
+-rw-r--r--   0        0        0     6854 2023-08-08 04:52:52.474953 oplangchain-0.1.3/oplangchain/prompts/example_selector/semantic_similarity.py
+-rw-r--r--   0        0        0    11763 2023-08-08 04:52:52.472955 oplangchain-0.1.3/oplangchain/prompts/few_shot.py
+-rw-r--r--   0        0        0     5429 2023-08-08 04:52:52.472955 oplangchain-0.1.3/oplangchain/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0     5519 2023-08-08 04:52:52.467952 oplangchain-0.1.3/oplangchain/prompts/loading.py
+-rw-r--r--   0        0        0     2258 2023-08-08 04:52:52.468953 oplangchain-0.1.3/oplangchain/prompts/pipeline.py
+-rw-r--r--   0        0        0     8140 2023-08-08 04:52:52.465953 oplangchain-0.1.3/oplangchain/prompts/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.713154 oplangchain-0.1.3/oplangchain/py.typed
+-rw-r--r--   0        0        0      113 2023-08-08 04:52:52.345954 oplangchain-0.1.3/oplangchain/python.py
+-rw-r--r--   0        0        0      214 2023-08-08 04:52:52.342954 oplangchain-0.1.3/oplangchain/requests.py
+-rw-r--r--   0        0        0     3676 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/__init__.py
+-rw-r--r--   0        0        0      588 2023-08-08 04:52:52.452954 oplangchain-0.1.3/oplangchain/retrievers/arxiv.py
+-rw-r--r--   0        0        0     4048 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/azure_cognitive_search.py
+-rw-r--r--   0        0        0     3657 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/bm25.py
+-rw-r--r--   0        0        0     2653 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/chaindesk.py
+-rw-r--r--   0        0        0     3002 2023-08-08 04:52:52.456954 oplangchain-0.1.3/oplangchain/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0     2261 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/contextual_compression.py
+-rw-r--r--   0        0        0     2307 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/databerry.py
+-rw-r--r--   0        0        0     6738 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/docarray.py
+-rw-r--r--   0        0        0      601 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/document_compressors/__init__.py
+-rw-r--r--   0        0        0     3662 2023-08-08 04:52:52.458953 oplangchain-0.1.3/oplangchain/retrievers/document_compressors/base.py
+-rw-r--r--   0        0        0     3825 2023-08-08 04:52:52.458953 oplangchain-0.1.3/oplangchain/retrievers/document_compressors/chain_extract.py
+-rw-r--r--   0        0        0      366 2023-08-07 21:21:40.721154 oplangchain-0.1.3/oplangchain/retrievers/document_compressors/chain_extract_prompt.py
+-rw-r--r--   0        0        0     2979 2023-08-08 04:52:52.457954 oplangchain-0.1.3/oplangchain/retrievers/document_compressors/chain_filter.py
+-rw-r--r--   0        0        0      231 2023-08-07 21:21:40.722154 oplangchain-0.1.3/oplangchain/retrievers/document_compressors/chain_filter_prompt.py
+-rw-r--r--   0        0        0     2969 2023-08-08 04:52:52.457954 oplangchain-0.1.3/oplangchain/retrievers/document_compressors/cohere_rerank.py
+-rw-r--r--   0        0        0     3151 2023-08-08 04:52:52.457954 oplangchain-0.1.3/oplangchain/retrievers/document_compressors/embeddings_filter.py
+-rw-r--r--   0        0        0     4664 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0     5797 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/ensemble.py
+-rw-r--r--   0        0        0     7436 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/google_cloud_enterprise_search.py
+-rw-r--r--   0        0        0    12607 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/kendra.py
+-rw-r--r--   0        0        0     2533 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/knn.py
+-rw-r--r--   0        0        0     3026 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/llama_index.py
+-rw-r--r--   0        0        0     3377 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/merger_retriever.py
+-rw-r--r--   0        0        0     1443 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/metal.py
+-rw-r--r--   0        0        0     2385 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/milvus.py
+-rw-r--r--   0        0        0     4846 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/multi_query.py
+-rw-r--r--   0        0        0     5442 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0      598 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/pubmed.py
+-rw-r--r--   0        0        0       96 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/pupmed.py
+-rw-r--r--   0        0        0     2611 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/re_phraser.py
+-rw-r--r--   0        0        0     1907 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.731154 oplangchain-0.1.3/oplangchain/retrievers/self_query/__init__.py
+-rw-r--r--   0        0        0     5973 2023-08-08 04:52:52.465953 oplangchain-0.1.3/oplangchain/retrievers/self_query/base.py
+-rw-r--r--   0        0        0     1444 2023-08-08 04:52:52.464953 oplangchain-0.1.3/oplangchain/retrievers/self_query/chroma.py
+-rw-r--r--   0        0        0     2594 2023-08-08 04:52:52.462957 oplangchain-0.1.3/oplangchain/retrievers/self_query/deeplake.py
+-rw-r--r--   0        0        0     3597 2023-08-08 04:52:52.462957 oplangchain-0.1.3/oplangchain/retrievers/self_query/myscale.py
+-rw-r--r--   0        0        0     1450 2023-08-08 04:52:52.462957 oplangchain-0.1.3/oplangchain/retrievers/self_query/pinecone.py
+-rw-r--r--   0        0        0     2813 2023-08-08 04:52:52.462957 oplangchain-0.1.3/oplangchain/retrievers/self_query/qdrant.py
+-rw-r--r--   0        0        0     1503 2023-08-08 04:52:52.459954 oplangchain-0.1.3/oplangchain/retrievers/self_query/weaviate.py
+-rw-r--r--   0        0        0     3663 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/svm.py
+-rw-r--r--   0        0        0     4039 2023-08-08 04:52:52.454955 oplangchain-0.1.3/oplangchain/retrievers/tfidf.py
+-rw-r--r--   0        0        0     5818 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/time_weighted_retriever.py
+-rw-r--r--   0        0        0     4601 2023-08-08 04:52:52.455957 oplangchain-0.1.3/oplangchain/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0     4059 2023-08-08 04:52:52.454955 oplangchain-0.1.3/oplangchain/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0     8302 2023-08-08 04:52:52.454955 oplangchain-0.1.3/oplangchain/retrievers/web_research.py
+-rw-r--r--   0        0        0      611 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/wikipedia.py
+-rw-r--r--   0        0        0     3075 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/zep.py
+-rw-r--r--   0        0        0     2679 2023-08-08 04:52:52.453954 oplangchain-0.1.3/oplangchain/retrievers/zilliz.py
+-rw-r--r--   0        0        0     1736 2023-08-08 04:52:52.443954 oplangchain-0.1.3/oplangchain/schema/__init__.py
+-rw-r--r--   0        0        0      643 2023-08-07 21:21:40.739154 oplangchain-0.1.3/oplangchain/schema/agent.py
+-rw-r--r--   0        0        0     2658 2023-08-08 04:52:52.452954 oplangchain-0.1.3/oplangchain/schema/document.py
+-rw-r--r--   0        0        0    10183 2023-08-08 04:52:52.452954 oplangchain-0.1.3/oplangchain/schema/language_model.py
+-rw-r--r--   0        0        0     4099 2023-08-08 04:52:52.451953 oplangchain-0.1.3/oplangchain/schema/memory.py
+-rw-r--r--   0        0        0     7490 2023-08-08 04:52:52.451953 oplangchain-0.1.3/oplangchain/schema/messages.py
+-rw-r--r--   0        0        0     5451 2023-08-08 04:52:52.451953 oplangchain-0.1.3/oplangchain/schema/output.py
+-rw-r--r--   0        0        0     7792 2023-08-08 04:52:52.451953 oplangchain-0.1.3/oplangchain/schema/output_parser.py
+-rw-r--r--   0        0        0      638 2023-08-08 04:52:52.451953 oplangchain-0.1.3/oplangchain/schema/prompt.py
+-rw-r--r--   0        0        0     6879 2023-08-08 04:52:52.451953 oplangchain-0.1.3/oplangchain/schema/prompt_template.py
+-rw-r--r--   0        0        0    10059 2023-08-08 04:52:52.450953 oplangchain-0.1.3/oplangchain/schema/retriever.py
+-rw-r--r--   0        0        0    40398 2023-08-08 04:52:52.448953 oplangchain-0.1.3/oplangchain/schema/runnable.py
+-rw-r--r--   0        0        0      122 2023-08-08 04:52:52.341954 oplangchain-0.1.3/oplangchain/serpapi.py
+-rw-r--r--   0        0        0      533 2023-08-07 21:21:40.745154 oplangchain-0.1.3/oplangchain/server.py
+-rw-r--r--   0        0        0     3571 2023-08-08 04:52:52.439954 oplangchain-0.1.3/oplangchain/smith/__init__.py
+-rw-r--r--   0        0        0     2201 2023-08-08 04:52:52.439954 oplangchain-0.1.3/oplangchain/smith/evaluation/__init__.py
+-rw-r--r--   0        0        0     8581 2023-08-08 04:52:52.443954 oplangchain-0.1.3/oplangchain/smith/evaluation/config.py
+-rw-r--r--   0        0        0    51540 2023-08-08 04:52:52.440954 oplangchain-0.1.3/oplangchain/smith/evaluation/runner_utils.py
+-rw-r--r--   0        0        0    15823 2023-08-08 04:52:52.439954 oplangchain-0.1.3/oplangchain/smith/evaluation/string_run_evaluator.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.748154 oplangchain-0.1.3/oplangchain/smith/evaluation/utils.py
+-rw-r--r--   0        0        0      131 2023-08-08 04:52:52.339954 oplangchain-0.1.3/oplangchain/sql_database.py
+-rw-r--r--   0        0        0    38443 2023-08-08 04:52:52.339954 oplangchain-0.1.3/oplangchain/text_splitter.py
+-rw-r--r--   0        0        0     6699 2023-08-08 20:14:03.876599 oplangchain-0.1.3/oplangchain/tools/__init__.py
+-rw-r--r--   0        0        0      241 2023-08-08 04:52:52.438954 oplangchain-0.1.3/oplangchain/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0      411 2023-08-08 04:52:52.439954 oplangchain-0.1.3/oplangchain/tools/amadeus/base.py
+-rw-r--r--   0        0        0     1982 2023-08-08 04:52:52.439954 oplangchain-0.1.3/oplangchain/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0     5561 2023-08-08 04:52:52.439954 oplangchain-0.1.3/oplangchain/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0     1123 2023-08-07 21:21:40.753154 oplangchain-0.1.3/oplangchain/tools/amadeus/utils.py
+-rw-r--r--   0        0        0       25 2023-08-07 21:21:40.753154 oplangchain-0.1.3/oplangchain/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0     1006 2023-08-08 04:52:52.438954 oplangchain-0.1.3/oplangchain/tools/arxiv/tool.py
+-rw-r--r--   0        0        0      603 2023-08-08 04:52:52.436954 oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0     5334 2023-08-08 04:52:52.438954 oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0     5263 2023-08-08 04:52:52.438954 oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0     4304 2023-08-08 04:52:52.438954 oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0     3652 2023-08-08 04:52:52.436954 oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0      776 2023-08-07 21:21:40.757154 oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/utils.py
+-rw-r--r--   0        0        0    26849 2023-08-08 04:52:52.392956 oplangchain-0.1.3/oplangchain/tools/base.py
+-rw-r--r--   0        0        0      162 2023-08-08 04:52:52.436954 oplangchain-0.1.3/oplangchain/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0     1441 2023-08-08 04:52:52.436954 oplangchain-0.1.3/oplangchain/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.759154 oplangchain-0.1.3/oplangchain/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0     1342 2023-08-08 04:52:52.436954 oplangchain-0.1.3/oplangchain/tools/brave_search/tool.py
+-rw-r--r--   0        0        0     1738 2023-08-08 04:52:52.390954 oplangchain-0.1.3/oplangchain/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      260 2023-08-08 04:52:52.435953 oplangchain-0.1.3/oplangchain/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0     2182 2023-08-08 04:52:52.435953 oplangchain-0.1.3/oplangchain/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      139 2023-08-08 04:52:52.436954 oplangchain-0.1.3/oplangchain/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0     2321 2023-08-08 04:52:52.436954 oplangchain-0.1.3/oplangchain/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0      667 2023-08-08 04:52:52.428954 oplangchain-0.1.3/oplangchain/tools/file_management/__init__.py
+-rw-r--r--   0        0        0     1730 2023-08-08 04:52:52.433955 oplangchain-0.1.3/oplangchain/tools/file_management/copy.py
+-rw-r--r--   0        0        0     1326 2023-08-08 04:52:52.433955 oplangchain-0.1.3/oplangchain/tools/file_management/delete.py
+-rw-r--r--   0        0        0     1946 2023-08-08 04:52:52.432954 oplangchain-0.1.3/oplangchain/tools/file_management/file_search.py
+-rw-r--r--   0        0        0     1413 2023-08-08 04:52:52.431953 oplangchain-0.1.3/oplangchain/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0     1870 2023-08-08 04:52:52.428954 oplangchain-0.1.3/oplangchain/tools/file_management/move.py
+-rw-r--r--   0        0        0     1321 2023-08-08 04:52:52.428954 oplangchain-0.1.3/oplangchain/tools/file_management/read.py
+-rw-r--r--   0        0        0     1708 2023-08-07 21:21:40.767154 oplangchain-0.1.3/oplangchain/tools/file_management/utils.py
+-rw-r--r--   0        0        0     1595 2023-08-08 04:52:52.422954 oplangchain-0.1.3/oplangchain/tools/file_management/write.py
+-rw-r--r--   0        0        0       20 2023-08-07 21:21:40.768154 oplangchain-0.1.3/oplangchain/tools/github/__init__.py
+-rw-r--r--   0        0        0     3438 2023-08-07 21:21:40.769155 oplangchain-0.1.3/oplangchain/tools/github/prompt.py
+-rw-r--r--   0        0        0      927 2023-08-08 04:52:52.422954 oplangchain-0.1.3/oplangchain/tools/github/tool.py
+-rw-r--r--   0        0        0      553 2023-08-08 04:52:52.418954 oplangchain-0.1.3/oplangchain/tools/gmail/__init__.py
+-rw-r--r--   0        0        0      980 2023-08-08 04:52:52.422954 oplangchain-0.1.3/oplangchain/tools/gmail/base.py
+-rw-r--r--   0        0        0     2543 2023-08-08 04:52:52.420954 oplangchain-0.1.3/oplangchain/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0     1733 2023-08-08 04:52:52.416952 oplangchain-0.1.3/oplangchain/tools/gmail/get_message.py
+-rw-r--r--   0        0        0     1539 2023-08-08 04:52:52.420954 oplangchain-0.1.3/oplangchain/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0     4369 2023-08-08 04:52:52.416952 oplangchain-0.1.3/oplangchain/tools/gmail/search.py
+-rw-r--r--   0        0        0     2851 2023-08-08 04:52:52.417953 oplangchain-0.1.3/oplangchain/tools/gmail/send_message.py
+-rw-r--r--   0        0        0     4528 2023-08-07 21:21:40.773153 oplangchain-0.1.3/oplangchain/tools/gmail/utils.py
+-rw-r--r--   0        0        0      128 2023-08-08 04:52:52.416952 oplangchain-0.1.3/oplangchain/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0     1096 2023-08-08 04:52:52.416952 oplangchain-0.1.3/oplangchain/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      132 2023-08-08 04:52:52.415952 oplangchain-0.1.3/oplangchain/tools/google_places/__init__.py
+-rw-r--r--   0        0        0     1112 2023-08-08 04:52:52.416952 oplangchain-0.1.3/oplangchain/tools/google_places/tool.py
+-rw-r--r--   0        0        0      174 2023-08-08 04:52:52.415952 oplangchain-0.1.3/oplangchain/tools/google_search/__init__.py
+-rw-r--r--   0        0        0     1467 2023-08-08 04:52:52.415952 oplangchain-0.1.3/oplangchain/tools/google_search/tool.py
+-rw-r--r--   0        0        0      222 2023-08-08 04:52:52.415952 oplangchain-0.1.3/oplangchain/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0     2082 2023-08-08 04:52:52.415952 oplangchain-0.1.3/oplangchain/tools/google_serper/tool.py
+-rw-r--r--   0        0        0       47 2023-08-07 21:21:40.778154 oplangchain-0.1.3/oplangchain/tools/graphql/__init__.py
+-rw-r--r--   0        0        0     1192 2023-08-08 04:52:52.415952 oplangchain-0.1.3/oplangchain/tools/graphql/tool.py
+-rw-r--r--   0        0        0      124 2023-08-08 04:52:52.415952 oplangchain-0.1.3/oplangchain/tools/human/__init__.py
+-rw-r--r--   0        0        0      963 2023-08-08 04:52:52.415952 oplangchain-0.1.3/oplangchain/tools/human/tool.py
+-rw-r--r--   0        0        0     2294 2023-08-08 04:52:52.389957 oplangchain-0.1.3/oplangchain/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2023-08-07 21:21:40.781153 oplangchain-0.1.3/oplangchain/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      456 2023-08-08 04:52:52.415933 oplangchain-0.1.3/oplangchain/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2023-08-07 21:21:40.782154 oplangchain-0.1.3/oplangchain/tools/jira/__init__.py
+-rw-r--r--   0        0        0     3170 2023-08-07 21:21:40.783154 oplangchain-0.1.3/oplangchain/tools/jira/prompt.py
+-rw-r--r--   0        0        0     1585 2023-08-08 04:52:52.414953 oplangchain-0.1.3/oplangchain/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2023-08-07 21:21:40.784153 oplangchain-0.1.3/oplangchain/tools/json/__init__.py
+-rw-r--r--   0        0        0     4091 2023-08-08 04:52:52.414953 oplangchain-0.1.3/oplangchain/tools/json/tool.py
+-rw-r--r--   0        0        0      146 2023-08-08 04:52:52.414953 oplangchain-0.1.3/oplangchain/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0     2678 2023-08-08 04:52:52.414953 oplangchain-0.1.3/oplangchain/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0      241 2023-08-08 04:52:52.414953 oplangchain-0.1.3/oplangchain/tools/multion/__init__.py
+-rw-r--r--   0        0        0     1581 2023-08-08 04:52:52.414953 oplangchain-0.1.3/oplangchain/tools/multion/create_session.py
+-rw-r--r--   0        0        0     2120 2023-08-08 04:52:52.414953 oplangchain-0.1.3/oplangchain/tools/multion/update_session.py
+-rw-r--r--   0        0        0      103 2023-08-08 04:52:52.413953 oplangchain-0.1.3/oplangchain/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0     7579 2023-08-08 04:52:52.414953 oplangchain-0.1.3/oplangchain/tools/nuclia/tool.py
+-rw-r--r--   0        0        0      597 2023-08-08 04:52:52.405953 oplangchain-0.1.3/oplangchain/tools/office365/__init__.py
+-rw-r--r--   0        0        0      484 2023-08-08 04:52:52.412953 oplangchain-0.1.3/oplangchain/tools/office365/base.py
+-rw-r--r--   0        0        0     1836 2023-08-08 04:52:52.409952 oplangchain-0.1.3/oplangchain/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0     4852 2023-08-08 04:52:52.406955 oplangchain-0.1.3/oplangchain/tools/office365/events_search.py
+-rw-r--r--   0        0        0     4166 2023-08-08 04:52:52.408952 oplangchain-0.1.3/oplangchain/tools/office365/messages_search.py
+-rw-r--r--   0        0        0     2834 2023-08-08 04:52:52.406955 oplangchain-0.1.3/oplangchain/tools/office365/send_event.py
+-rw-r--r--   0        0        0     1767 2023-08-08 04:52:52.406955 oplangchain-0.1.3/oplangchain/tools/office365/send_message.py
+-rw-r--r--   0        0        0     2136 2023-08-07 21:21:40.792153 oplangchain-0.1.3/oplangchain/tools/office365/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.793153 oplangchain-0.1.3/oplangchain/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.793153 oplangchain-0.1.3/oplangchain/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0    20555 2023-08-08 04:52:52.413953 oplangchain-0.1.3/oplangchain/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      158 2023-08-08 04:52:52.413953 oplangchain-0.1.3/oplangchain/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      154 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      922 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0      698 2023-08-08 04:52:52.405953 oplangchain-0.1.3/oplangchain/tools/playwright/__init__.py
+-rw-r--r--   0        0        0     2120 2023-08-08 04:52:52.405953 oplangchain-0.1.3/oplangchain/tools/playwright/base.py
+-rw-r--r--   0        0        0     3054 2023-08-08 04:52:52.405953 oplangchain-0.1.3/oplangchain/tools/playwright/click.py
+-rw-r--r--   0        0        0     1298 2023-08-08 04:52:52.405953 oplangchain-0.1.3/oplangchain/tools/playwright/current_page.py
+-rw-r--r--   0        0        0     3009 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0     2341 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0     3701 2023-08-08 04:52:52.405953 oplangchain-0.1.3/oplangchain/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0     1762 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/playwright/navigate.py
+-rw-r--r--   0        0        0     1897 2023-08-08 04:52:52.405953 oplangchain-0.1.3/oplangchain/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0     2813 2023-08-07 21:21:40.800154 oplangchain-0.1.3/oplangchain/tools/playwright/utils.py
+-rw-r--r--   0        0        0     2892 2023-08-08 04:52:52.388957 oplangchain-0.1.3/oplangchain/tools/plugin.py
+-rw-r--r--   0        0        0       52 2023-08-07 21:21:40.801153 oplangchain-0.1.3/oplangchain/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0     7339 2023-08-07 21:21:40.802153 oplangchain-0.1.3/oplangchain/tools/powerbi/prompt.py
+-rw-r--r--   0        0        0    11069 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2023-08-07 21:21:40.803153 oplangchain-0.1.3/oplangchain/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0     1016 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/pubmed/tool.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.804154 oplangchain-0.1.3/oplangchain/tools/python/__init__.py
+-rw-r--r--   0        0        0     4319 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/python/tool.py
+-rw-r--r--   0        0        0       52 2023-08-07 21:21:40.805154 oplangchain-0.1.3/oplangchain/tools/requests/__init__.py
+-rw-r--r--   0        0        0     6254 2023-08-08 04:52:52.404955 oplangchain-0.1.3/oplangchain/tools/requests/tool.py
+-rw-r--r--   0        0        0       31 2023-08-07 21:21:40.806153 oplangchain-0.1.3/oplangchain/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0     1071 2023-08-08 04:52:52.395953 oplangchain-0.1.3/oplangchain/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.807153 oplangchain-0.1.3/oplangchain/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0     2222 2023-08-08 04:52:52.396955 oplangchain-0.1.3/oplangchain/tools/searx_search/tool.py
+-rw-r--r--   0        0        0       95 2023-08-08 04:52:52.394953 oplangchain-0.1.3/oplangchain/tools/shell/__init__.py
+-rw-r--r--   0        0        0     2390 2023-08-08 04:52:52.394953 oplangchain-0.1.3/oplangchain/tools/shell/tool.py
+-rw-r--r--   0        0        0       18 2023-08-07 21:21:40.809153 oplangchain-0.1.3/oplangchain/tools/sleep/__init__.py
+-rw-r--r--   0        0        0     1209 2023-08-08 04:52:52.394953 oplangchain-0.1.3/oplangchain/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2023-08-07 21:21:40.811153 oplangchain-0.1.3/oplangchain/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0      550 2023-08-07 21:21:40.811153 oplangchain-0.1.3/oplangchain/tools/spark_sql/prompt.py
+-rw-r--r--   0        0        0     4526 2023-08-08 04:52:52.394953 oplangchain-0.1.3/oplangchain/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2023-08-07 21:21:40.812153 oplangchain-0.1.3/oplangchain/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      597 2023-08-07 21:21:40.813154 oplangchain-0.1.3/oplangchain/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0     4588 2023-08-08 04:52:52.394953 oplangchain-0.1.3/oplangchain/tools/sql_database/tool.py
+-rw-r--r--   0        0        0      178 2023-08-08 20:14:04.138598 oplangchain-0.1.3/oplangchain/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0     3335 2023-08-08 04:52:52.394953 oplangchain-0.1.3/oplangchain/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0     1395 2023-08-07 21:21:40.815153 oplangchain-0.1.3/oplangchain/tools/steamship_image_generation/utils.py
+-rw-r--r--   0        0        0       51 2023-08-07 21:21:40.815153 oplangchain-0.1.3/oplangchain/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0     3255 2023-08-08 04:52:52.394953 oplangchain-0.1.3/oplangchain/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       29 2023-08-07 21:21:40.817153 oplangchain-0.1.3/oplangchain/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      855 2023-08-08 04:52:52.393954 oplangchain-0.1.3/oplangchain/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      148 2023-08-08 04:52:52.393954 oplangchain-0.1.3/oplangchain/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      875 2023-08-08 04:52:52.393954 oplangchain-0.1.3/oplangchain/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:21:40.819153 oplangchain-0.1.3/oplangchain/tools/youtube/__init__.py
+-rw-r--r--   0        0        0     1665 2023-08-08 04:52:52.393954 oplangchain-0.1.3/oplangchain/tools/youtube/search.py
+-rw-r--r--   0        0        0      172 2023-08-08 04:52:52.392956 oplangchain-0.1.3/oplangchain/tools/zapier/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-07 21:21:40.820154 oplangchain-0.1.3/oplangchain/tools/zapier/prompt.py
+-rw-r--r--   0        0        0     7081 2023-08-08 04:52:52.393954 oplangchain-0.1.3/oplangchain/tools/zapier/tool.py
+-rw-r--r--   0        0        0     2945 2023-08-08 20:14:04.205599 oplangchain-0.1.3/oplangchain/utilities/__init__.py
+-rw-r--r--   0        0        0     6390 2023-08-08 04:52:52.386955 oplangchain-0.1.3/oplangchain/utilities/arxiv.py
+-rw-r--r--   0        0        0      274 2023-08-07 21:21:40.822153 oplangchain-0.1.3/oplangchain/utilities/asyncio.py
+-rw-r--r--   0        0        0     2419 2023-08-07 21:21:40.823154 oplangchain-0.1.3/oplangchain/utilities/awslambda.py
+-rw-r--r--   0        0        0     5705 2023-08-08 04:52:52.386955 oplangchain-0.1.3/oplangchain/utilities/bash.py
+-rw-r--r--   0        0        0     2481 2023-08-07 21:21:40.824154 oplangchain-0.1.3/oplangchain/utilities/bibtex.py
+-rw-r--r--   0        0        0     3335 2023-08-08 04:52:52.386955 oplangchain-0.1.3/oplangchain/utilities/bing_search.py
+-rw-r--r--   0        0        0     2328 2023-08-08 04:52:52.385954 oplangchain-0.1.3/oplangchain/utilities/brave_search.py
+-rw-r--r--   0        0        0     7834 2023-08-08 04:52:52.385954 oplangchain-0.1.3/oplangchain/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0     3764 2023-08-07 21:21:40.825153 oplangchain-0.1.3/oplangchain/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0    11596 2023-08-08 04:52:52.385517 oplangchain-0.1.3/oplangchain/utilities/github.py
+-rw-r--r--   0        0        0     1838 2023-08-08 04:52:52.384954 oplangchain-0.1.3/oplangchain/utilities/golden_query.py
+-rw-r--r--   0        0        0     4069 2023-08-08 04:52:52.384954 oplangchain-0.1.3/oplangchain/utilities/google_places_api.py
+-rw-r--r--   0        0        0     5096 2023-08-08 04:52:52.383953 oplangchain-0.1.3/oplangchain/utilities/google_search.py
+-rw-r--r--   0        0        0     6507 2023-08-08 04:52:52.383953 oplangchain-0.1.3/oplangchain/utilities/google_serper.py
+-rw-r--r--   0        0        0     1885 2023-08-07 21:21:40.828153 oplangchain-0.1.3/oplangchain/utilities/graphql.py
+-rw-r--r--   0        0        0     6175 2023-08-08 04:52:52.379954 oplangchain-0.1.3/oplangchain/utilities/jira.py
+-rw-r--r--   0        0        0     1974 2023-08-08 04:52:52.378954 oplangchain-0.1.3/oplangchain/utilities/loading.py
+-rw-r--r--   0        0        0     2644 2023-08-08 04:52:52.377955 oplangchain-0.1.3/oplangchain/utilities/max_compute.py
+-rw-r--r--   0        0        0     6707 2023-08-08 04:52:52.376953 oplangchain-0.1.3/oplangchain/utilities/metaphor_search.py
+-rw-r--r--   0        0        0    10588 2023-08-09 04:12:38.548022 oplangchain-0.1.3/oplangchain/utilities/openapi.py
+-rw-r--r--   0        0        0     2442 2023-08-08 04:52:52.376953 oplangchain-0.1.3/oplangchain/utilities/openweathermap.py
+-rw-r--r--   0        0        0     2198 2023-08-07 21:21:40.831154 oplangchain-0.1.3/oplangchain/utilities/portkey.py
+-rw-r--r--   0        0        0    11237 2023-08-07 21:21:40.832154 oplangchain-0.1.3/oplangchain/utilities/powerbi.py
+-rw-r--r--   0        0        0     5629 2023-08-08 04:52:52.376953 oplangchain-0.1.3/oplangchain/utilities/pupmed.py
+-rw-r--r--   0        0        0     2141 2023-08-07 21:21:40.833154 oplangchain-0.1.3/oplangchain/utilities/python.py
+-rw-r--r--   0        0        0     5439 2023-08-08 04:52:52.376953 oplangchain-0.1.3/oplangchain/utilities/redis.py
+-rw-r--r--   0        0        0     7120 2023-08-07 21:21:40.834153 oplangchain-0.1.3/oplangchain/utilities/requests.py
+-rw-r--r--   0        0        0     2200 2023-08-08 04:52:52.376953 oplangchain-0.1.3/oplangchain/utilities/scenexplain.py
+-rw-r--r--   0        0        0    16539 2023-08-08 04:52:52.376953 oplangchain-0.1.3/oplangchain/utilities/searx_search.py
+-rw-r--r--   0        0        0     6029 2023-08-08 04:52:52.375952 oplangchain-0.1.3/oplangchain/utilities/serpapi.py
+-rw-r--r--   0        0        0     6964 2023-08-07 21:21:40.836153 oplangchain-0.1.3/oplangchain/utilities/spark_sql.py
+-rw-r--r--   0        0        0    18265 2023-08-08 04:52:52.375952 oplangchain-0.1.3/oplangchain/utilities/sql_database.py
+-rw-r--r--   0        0        0     3413 2023-08-08 04:52:52.374954 oplangchain-0.1.3/oplangchain/utilities/twilio.py
+-rw-r--r--   0        0        0     1457 2023-08-07 21:21:40.837154 oplangchain-0.1.3/oplangchain/utilities/vertexai.py
+-rw-r--r--   0        0        0     3922 2023-08-08 04:52:52.374954 oplangchain-0.1.3/oplangchain/utilities/wikipedia.py
+-rw-r--r--   0        0        0     1991 2023-08-08 04:52:52.374954 oplangchain-0.1.3/oplangchain/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0    11562 2023-08-08 04:52:52.374954 oplangchain-0.1.3/oplangchain/utilities/zapier.py
+-rw-r--r--   0        0        0     1161 2023-08-08 04:52:52.374954 oplangchain-0.1.3/oplangchain/utils/__init__.py
+-rw-r--r--   0        0        0      873 2023-08-07 21:21:40.840155 oplangchain-0.1.3/oplangchain/utils/env.py
+-rw-r--r--   0        0        0     1237 2023-08-07 21:21:40.840155 oplangchain-0.1.3/oplangchain/utils/formatting.py
+-rw-r--r--   0        0        0     1289 2023-08-07 21:21:40.841153 oplangchain-0.1.3/oplangchain/utils/input.py
+-rw-r--r--   0        0        0     2016 2023-08-07 21:21:40.841153 oplangchain-0.1.3/oplangchain/utils/math.py
+-rw-r--r--   0        0        0      908 2023-08-07 21:21:40.842153 oplangchain-0.1.3/oplangchain/utils/strings.py
+-rw-r--r--   0        0        0     5606 2023-08-07 21:21:40.842153 oplangchain-0.1.3/oplangchain/utils/utils.py
+-rw-r--r--   0        0        0     4085 2023-08-08 04:52:52.346953 oplangchain-0.1.3/oplangchain/vectorstores/__init__.py
+-rw-r--r--   0        0        0     2027 2023-08-08 04:52:52.347954 oplangchain-0.1.3/oplangchain/vectorstores/_pgvector_data_models.py
+-rw-r--r--   0        0        0    13541 2023-08-08 04:52:52.372952 oplangchain-0.1.3/oplangchain/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0    15800 2023-08-08 04:52:52.370954 oplangchain-0.1.3/oplangchain/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0    16597 2023-08-08 04:52:52.370954 oplangchain-0.1.3/oplangchain/vectorstores/annoy.py
+-rw-r--r--   0        0        0    12143 2023-08-08 04:52:52.369953 oplangchain-0.1.3/oplangchain/vectorstores/atlas.py
+-rw-r--r--   0        0        0    21228 2023-08-08 04:52:52.369953 oplangchain-0.1.3/oplangchain/vectorstores/awadb.py
+-rw-r--r--   0        0        0    20726 2023-08-08 04:52:52.369953 oplangchain-0.1.3/oplangchain/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0    22441 2023-08-08 04:52:52.369953 oplangchain-0.1.3/oplangchain/vectorstores/base.py
+-rw-r--r--   0        0        0    13404 2023-08-08 04:52:52.366955 oplangchain-0.1.3/oplangchain/vectorstores/cassandra.py
+-rw-r--r--   0        0        0    23822 2023-08-08 04:52:52.366955 oplangchain-0.1.3/oplangchain/vectorstores/chroma.py
+-rw-r--r--   0        0        0    12739 2023-08-08 04:52:52.365954 oplangchain-0.1.3/oplangchain/vectorstores/clarifai.py
+-rw-r--r--   0        0        0    17817 2023-08-08 04:52:52.365954 oplangchain-0.1.3/oplangchain/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0    34980 2023-08-08 04:52:52.364955 oplangchain-0.1.3/oplangchain/vectorstores/deeplake.py
+-rw-r--r--   0        0        0      220 2023-08-08 04:52:52.373955 oplangchain-0.1.3/oplangchain/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0     6879 2023-08-08 04:52:52.374954 oplangchain-0.1.3/oplangchain/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0     4061 2023-08-08 04:52:52.374954 oplangchain-0.1.3/oplangchain/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0     2415 2023-08-08 04:52:52.373955 oplangchain-0.1.3/oplangchain/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0    27795 2023-08-08 04:52:52.364955 oplangchain-0.1.3/oplangchain/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0    29137 2023-08-08 04:52:52.364955 oplangchain-0.1.3/oplangchain/vectorstores/faiss.py
+-rw-r--r--   0        0        0    16411 2023-08-08 04:52:52.364955 oplangchain-0.1.3/oplangchain/vectorstores/hologres.py
+-rw-r--r--   0        0        0     4242 2023-08-08 04:52:52.364955 oplangchain-0.1.3/oplangchain/vectorstores/lancedb.py
+-rw-r--r--   0        0        0    17162 2023-08-08 04:52:52.364955 oplangchain-0.1.3/oplangchain/vectorstores/marqo.py
+-rw-r--r--   0        0        0    15184 2023-08-08 04:52:52.364955 oplangchain-0.1.3/oplangchain/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0    10437 2023-08-08 04:52:52.360956 oplangchain-0.1.3/oplangchain/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0    31480 2023-08-08 04:52:52.360956 oplangchain-0.1.3/oplangchain/vectorstores/milvus.py
+-rw-r--r--   0        0        0    12361 2023-08-08 04:52:52.359955 oplangchain-0.1.3/oplangchain/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0    16545 2023-08-08 04:52:52.358954 oplangchain-0.1.3/oplangchain/vectorstores/myscale.py
+-rw-r--r--   0        0        0    27702 2023-08-08 04:52:52.358954 oplangchain-0.1.3/oplangchain/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0    17352 2023-08-08 04:52:52.358954 oplangchain-0.1.3/oplangchain/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0    21271 2023-08-08 04:52:52.358954 oplangchain-0.1.3/oplangchain/vectorstores/pgvector.py
+-rw-r--r--   0        0        0    14921 2023-08-08 04:52:52.358954 oplangchain-0.1.3/oplangchain/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    68545 2023-08-08 04:52:52.357953 oplangchain-0.1.3/oplangchain/vectorstores/qdrant.py
+-rw-r--r--   0        0        0    23162 2023-08-08 04:52:52.357953 oplangchain-0.1.3/oplangchain/vectorstores/redis.py
+-rw-r--r--   0        0        0    12196 2023-08-08 04:52:52.357953 oplangchain-0.1.3/oplangchain/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0    19535 2023-08-08 04:52:52.357953 oplangchain-0.1.3/oplangchain/vectorstores/scann.py
+-rw-r--r--   0        0        0    18282 2023-08-08 04:52:52.357953 oplangchain-0.1.3/oplangchain/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0    12395 2023-08-08 04:52:52.356954 oplangchain-0.1.3/oplangchain/vectorstores/sklearn.py
+-rw-r--r--   0        0        0    17225 2023-08-08 04:52:52.355953 oplangchain-0.1.3/oplangchain/vectorstores/starrocks.py
+-rw-r--r--   0        0        0    14251 2023-08-08 04:52:52.352954 oplangchain-0.1.3/oplangchain/vectorstores/supabase.py
+-rw-r--r--   0        0        0     8886 2023-08-08 04:52:52.352954 oplangchain-0.1.3/oplangchain/vectorstores/tair.py
+-rw-r--r--   0        0        0     4884 2023-08-08 04:52:52.352954 oplangchain-0.1.3/oplangchain/vectorstores/tigris.py
+-rw-r--r--   0        0        0     9744 2023-08-08 04:52:52.352954 oplangchain-0.1.3/oplangchain/vectorstores/typesense.py
+-rw-r--r--   0        0        0     1792 2023-08-08 04:52:52.351954 oplangchain-0.1.3/oplangchain/vectorstores/utils.py
+-rw-r--r--   0        0        0    15869 2023-08-08 04:52:52.351954 oplangchain-0.1.3/oplangchain/vectorstores/vectara.py
+-rw-r--r--   0        0        0    16891 2023-08-08 04:52:52.351954 oplangchain-0.1.3/oplangchain/vectorstores/weaviate.py
+-rw-r--r--   0        0        0     7567 2023-08-08 04:52:52.350953 oplangchain-0.1.3/oplangchain/vectorstores/zilliz.py
+-rw-r--r--   0        0        0    13300 2023-08-09 04:13:43.726861 oplangchain-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6801 2023-08-08 05:21:38.027643 oplangchain-0.1.3/README.md
+-rw-r--r--   0        0        0    16025 1970-01-01 00:00:00.000000 oplangchain-0.1.3/PKG-INFO
```

### Comparing `oplangchain-0.1.2/oplangchain/__init__.py` & `oplangchain-0.1.3/oplangchain/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/__init__.py` & `oplangchain-0.1.3/oplangchain/agents/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     get_all_tool_names,
     load_huggingface_tool,
     load_tools,
 )
 from oplangchain.agents.loading import load_agent
 from oplangchain.agents.mrkl.base import MRKLChain, ZeroShotAgent
 from oplangchain.agents.openai_functions_agent.base import OpenAIFunctionsAgent
-from oplangchain.agents.openai_functions_multi_agent.base import OpenAIMultiFunctionsAgent
+from oplangchain.agents.openai_functions_multi_agent.base import (
+    OpenAIMultiFunctionsAgent,
+)
 from oplangchain.agents.react.base import ReActChain, ReActTextWorldAgent
 from oplangchain.agents.self_ask_with_search.base import SelfAskWithSearchChain
 from oplangchain.agents.structured_chat.base import StructuredChatAgent
 from oplangchain.agents.tools import Tool, tool
 from oplangchain.agents.xml.base import XMLAgent
 
 __all__ = [
```

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent.py` & `oplangchain-0.1.3/oplangchain/agents/agent.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_iterator.py` & `oplangchain-0.1.3/oplangchain/agents/agent_iterator.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/__init__.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from oplangchain.agents.agent_toolkits.json.toolkit import JsonToolkit
 from oplangchain.agents.agent_toolkits.multion.toolkit import MultionToolkit
 from oplangchain.agents.agent_toolkits.nla.toolkit import NLAToolkit
 from oplangchain.agents.agent_toolkits.office365.toolkit import O365Toolkit
 from oplangchain.agents.agent_toolkits.openapi.base import create_openapi_agent
 from oplangchain.agents.agent_toolkits.openapi.toolkit import OpenAPIToolkit
 from oplangchain.agents.agent_toolkits.pandas.base import create_pandas_dataframe_agent
-from oplangchain.agents.agent_toolkits.playwright.toolkit import PlayWrightBrowserToolkit
+from oplangchain.agents.agent_toolkits.playwright.toolkit import (
+    PlayWrightBrowserToolkit,
+)
 from oplangchain.agents.agent_toolkits.powerbi.base import create_pbi_agent
 from oplangchain.agents.agent_toolkits.powerbi.chat_base import create_pbi_chat_agent
 from oplangchain.agents.agent_toolkits.powerbi.toolkit import PowerBIToolkit
 from oplangchain.agents.agent_toolkits.python.base import create_python_agent
 from oplangchain.agents.agent_toolkits.spark.base import create_spark_dataframe_agent
 from oplangchain.agents.agent_toolkits.spark_sql.base import create_spark_sql_agent
 from oplangchain.agents.agent_toolkits.spark_sql.toolkit import SparkSQLToolkit
```

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/amadeus/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/amadeus/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/azure_cognitive_services.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/azure_cognitive_services.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/conversational_retrieval/tool.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/conversational_retrieval/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/csv/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/csv/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/file_management/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/file_management/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/github/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/github/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/gmail/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/gmail/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/jira/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/jira/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/json/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/json/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/json/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/json/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/json/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/json/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/multion/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/multion/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/nla/tool.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/nla/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/nla/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/nla/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/office365/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/office365/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/planner.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/planner.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/planner_prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/planner_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/spec.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/openapi/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/openapi/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/pandas/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/pandas/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/pandas/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/pandas/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/playwright/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/playwright/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/chat_base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/chat_base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/powerbi/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/powerbi/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/python/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/python/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/python/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/python/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark_sql/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark_sql/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark_sql/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/spark_sql/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/spark_sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/sql/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/sql/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/sql/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/sql/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/vectorstore/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/vectorstore/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/vectorstore/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/vectorstore/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/vectorstore/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/vectorstore/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/xorbits/base.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/xorbits/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/xorbits/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/xorbits/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_toolkits/zapier/toolkit.py` & `oplangchain-0.1.3/oplangchain/agents/agent_toolkits/zapier/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/agent_types.py` & `oplangchain-0.1.3/oplangchain/agents/agent_types.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/chat/base.py` & `oplangchain-0.1.3/oplangchain/agents/chat/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/chat/output_parser.py` & `oplangchain-0.1.3/oplangchain/agents/chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/chat/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/chat/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/conversational/base.py` & `oplangchain-0.1.3/oplangchain/agents/conversational/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/conversational/output_parser.py` & `oplangchain-0.1.3/oplangchain/agents/conversational/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/conversational/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/conversational/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/conversational_chat/base.py` & `oplangchain-0.1.3/oplangchain/agents/conversational_chat/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/conversational_chat/output_parser.py` & `oplangchain-0.1.3/oplangchain/agents/conversational_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/conversational_chat/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/conversational_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/initialize.py` & `oplangchain-0.1.3/oplangchain/agents/initialize.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/load_tools.py` & `oplangchain-0.1.3/oplangchain/agents/load_tools.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/loading.py` & `oplangchain-0.1.3/oplangchain/agents/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/mrkl/base.py` & `oplangchain-0.1.3/oplangchain/agents/mrkl/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/mrkl/output_parser.py` & `oplangchain-0.1.3/oplangchain/agents/mrkl/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/mrkl/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/mrkl/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/openai_functions_agent/agent_token_buffer_memory.py` & `oplangchain-0.1.3/oplangchain/agents/openai_functions_agent/agent_token_buffer_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/openai_functions_agent/base.py` & `oplangchain-0.1.3/oplangchain/agents/openai_functions_agent/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/openai_functions_multi_agent/base.py` & `oplangchain-0.1.3/oplangchain/agents/openai_functions_multi_agent/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/react/base.py` & `oplangchain-0.1.3/oplangchain/agents/react/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/react/output_parser.py` & `oplangchain-0.1.3/oplangchain/agents/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/react/textworld_prompt.py` & `oplangchain-0.1.3/oplangchain/agents/react/textworld_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/react/wiki_prompt.py` & `oplangchain-0.1.3/oplangchain/agents/react/wiki_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/schema.py` & `oplangchain-0.1.3/oplangchain/agents/schema.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/self_ask_with_search/base.py` & `oplangchain-0.1.3/oplangchain/agents/self_ask_with_search/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/self_ask_with_search/output_parser.py` & `oplangchain-0.1.3/oplangchain/agents/self_ask_with_search/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/self_ask_with_search/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/self_ask_with_search/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/structured_chat/base.py` & `oplangchain-0.1.3/oplangchain/agents/structured_chat/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 from pydantic import Field
 
 from oplangchain.agents.agent import Agent, AgentOutputParser
 from oplangchain.agents.structured_chat.output_parser import (
     StructuredChatOutputParserWithRetries,
 )
-from oplangchain.agents.structured_chat.prompt import FORMAT_INSTRUCTIONS, PREFIX, SUFFIX
+from oplangchain.agents.structured_chat.prompt import (
+    FORMAT_INSTRUCTIONS,
+    PREFIX,
+    SUFFIX,
+)
 from oplangchain.callbacks.base import BaseCallbackManager
 from oplangchain.chains.llm import LLMChain
 from oplangchain.prompts.chat import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     SystemMessagePromptTemplate,
 )
```

### Comparing `oplangchain-0.1.2/oplangchain/agents/structured_chat/output_parser.py` & `oplangchain-0.1.3/oplangchain/agents/structured_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/structured_chat/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/structured_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/tools.py` & `oplangchain-0.1.3/oplangchain/agents/tools.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/types.py` & `oplangchain-0.1.3/oplangchain/agents/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from oplangchain.agents.agent import BaseSingleActionAgent
 from oplangchain.agents.agent_types import AgentType
 from oplangchain.agents.chat.base import ChatAgent
 from oplangchain.agents.conversational.base import ConversationalAgent
 from oplangchain.agents.conversational_chat.base import ConversationalChatAgent
 from oplangchain.agents.mrkl.base import ZeroShotAgent
 from oplangchain.agents.openai_functions_agent.base import OpenAIFunctionsAgent
-from oplangchain.agents.openai_functions_multi_agent.base import OpenAIMultiFunctionsAgent
+from oplangchain.agents.openai_functions_multi_agent.base import (
+    OpenAIMultiFunctionsAgent,
+)
 from oplangchain.agents.react.base import ReActDocstoreAgent
 from oplangchain.agents.self_ask_with_search.base import SelfAskWithSearchAgent
 from oplangchain.agents.structured_chat.base import StructuredChatAgent
 
 AGENT_TYPE = Union[Type[BaseSingleActionAgent], Type[OpenAIMultiFunctionsAgent]]
 
 AGENT_TO_CLASS: Dict[AgentType, AGENT_TYPE] = {
```

### Comparing `oplangchain-0.1.2/oplangchain/agents/xml/base.py` & `oplangchain-0.1.3/oplangchain/agents/xml/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/agents/xml/prompt.py` & `oplangchain-0.1.3/oplangchain/agents/xml/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/cache.py` & `oplangchain-0.1.3/oplangchain/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,32 +280,32 @@
     # TODO - implement a TTL policy in Redis
 
     def __init__(
         self, redis_url: str, embedding: Embeddings, score_threshold: float = 0.2
     ):
         """Initialize by passing in the `init` GPTCache func
 
-        Args:
-            redis_url (str): URL to connect to Redis.
-            embedding (Embedding): Embedding provider for semantic encoding and search.
-            score_threshold (float, 0.2):
+                Args:
+                    redis_url (str): URL to connect to Redis.
+                    embedding (Embedding): Embedding provider for semantic encoding and search.
+                    score_threshold (float, 0.2):
 
-        Example:
+                Example:
 
-        .. code-block:: python
+                .. code-block:: python
 
-import oplangchain
+        import oplangchain
 
-            from oplangchain.cache import RedisSemanticCache
-            from oplangchain.embeddings import OpenAIEmbeddings
+                    from oplangchain.cache import RedisSemanticCache
+                    from oplangchain.embeddings import OpenAIEmbeddings
 
-            langchain.llm_cache = RedisSemanticCache(
-                redis_url="redis://localhost:6379",
-                embedding=OpenAIEmbeddings()
-            )
+                    langchain.llm_cache = RedisSemanticCache(
+                        redis_url="redis://localhost:6379",
+                        embedding=OpenAIEmbeddings()
+                    )
 
         """
         self._cache_dict: Dict[str, RedisVectorstore] = {}
         self.redis_url = redis_url
         self.embedding = embedding
         self.score_threshold = score_threshold
```

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/__init__.py` & `oplangchain-0.1.3/oplangchain/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/aim_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/aim_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/argilla_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/argilla_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/arize_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/arize_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/arthur_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/arthur_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/base.py` & `oplangchain-0.1.3/oplangchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/clearml_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/clearml_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/comet_ml_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/comet_ml_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/context_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/context_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/file.py` & `oplangchain-0.1.3/oplangchain/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/flyte_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/flyte_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/human.py` & `oplangchain-0.1.3/oplangchain/callbacks/human.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/infino_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/infino_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/manager.py` & `oplangchain-0.1.3/oplangchain/callbacks/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,18 @@
     RetrieverManagerMixin,
     RunManagerMixin,
     ToolManagerMixin,
 )
 from oplangchain.callbacks.openai_info import OpenAICallbackHandler
 from oplangchain.callbacks.stdout import StdOutCallbackHandler
 from oplangchain.callbacks.tracers.langchain import LangChainTracer
-from oplangchain.callbacks.tracers.langchain_v1 import LangChainTracerV1, TracerSessionV1
+from oplangchain.callbacks.tracers.langchain_v1 import (
+    LangChainTracerV1,
+    TracerSessionV1,
+)
 from oplangchain.callbacks.tracers.stdout import ConsoleCallbackHandler
 from oplangchain.callbacks.tracers.wandb import WandbTracer
 from oplangchain.schema import (
     AgentAction,
     AgentFinish,
     Document,
     LLMResult,
```

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/mlflow_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/mlflow_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/openai_info.py` & `oplangchain-0.1.3/oplangchain/callbacks/openai_info.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/promptlayer_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/promptlayer_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/sagemaker_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/sagemaker_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/stdout.py` & `oplangchain-0.1.3/oplangchain/callbacks/stdout.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/streaming_aiter.py` & `oplangchain-0.1.3/oplangchain/callbacks/streaming_aiter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/streaming_aiter_final_only.py` & `oplangchain-0.1.3/oplangchain/callbacks/streaming_aiter_final_only.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/streaming_stdout.py` & `oplangchain-0.1.3/oplangchain/callbacks/streaming_stdout.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/streaming_stdout_final_only.py` & `oplangchain-0.1.3/oplangchain/callbacks/streaming_stdout_final_only.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/streamlit/__init__.py` & `oplangchain-0.1.3/oplangchain/callbacks/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/streamlit/mutable_expander.py` & `oplangchain-0.1.3/oplangchain/callbacks/streamlit/mutable_expander.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/streamlit/streamlit_callback_handler.py` & `oplangchain-0.1.3/oplangchain/callbacks/streamlit/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/tracers/base.py` & `oplangchain-0.1.3/oplangchain/callbacks/tracers/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/tracers/evaluation.py` & `oplangchain-0.1.3/oplangchain/callbacks/tracers/evaluation.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/tracers/langchain.py` & `oplangchain-0.1.3/oplangchain/callbacks/tracers/langchain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/tracers/langchain_v1.py` & `oplangchain-0.1.3/oplangchain/callbacks/tracers/langchain_v1.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/tracers/run_collector.py` & `oplangchain-0.1.3/oplangchain/callbacks/tracers/run_collector.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/tracers/schemas.py` & `oplangchain-0.1.3/oplangchain/callbacks/tracers/schemas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/tracers/stdout.py` & `oplangchain-0.1.3/oplangchain/callbacks/tracers/stdout.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/tracers/wandb.py` & `oplangchain-0.1.3/oplangchain/callbacks/tracers/wandb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/utils.py` & `oplangchain-0.1.3/oplangchain/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/wandb_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/callbacks/whylabs_callback.py` & `oplangchain-0.1.3/oplangchain/callbacks/whylabs_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/__init__.py` & `oplangchain-0.1.3/oplangchain/chains/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,17 @@
 from oplangchain.chains.graph_qa.sparql import GraphSparqlQAChain
 from oplangchain.chains.hyde.base import HypotheticalDocumentEmbedder
 from oplangchain.chains.llm import LLMChain
 from oplangchain.chains.llm_bash.base import LLMBashChain
 from oplangchain.chains.llm_checker.base import LLMCheckerChain
 from oplangchain.chains.llm_math.base import LLMMathChain
 from oplangchain.chains.llm_requests import LLMRequestsChain
-from oplangchain.chains.llm_summarization_checker.base import LLMSummarizationCheckerChain
+from oplangchain.chains.llm_summarization_checker.base import (
+    LLMSummarizationCheckerChain,
+)
 from oplangchain.chains.loading import load_chain
 from oplangchain.chains.mapreduce import MapReduceChain
 from oplangchain.chains.moderation import OpenAIModerationChain
 from oplangchain.chains.natbot.base import NatBotChain
 from oplangchain.chains.openai_functions import (
     create_citation_fuzzy_match_chain,
     create_extraction_chain,
```

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/base.py` & `oplangchain-0.1.3/oplangchain/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/news_docs.py` & `oplangchain-0.1.3/oplangchain/chains/api/news_docs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/open_meteo_docs.py` & `oplangchain-0.1.3/oplangchain/chains/api/open_meteo_docs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/openapi/chain.py` & `oplangchain-0.1.3/oplangchain/chains/api/openapi/chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/openapi/prompts.py` & `oplangchain-0.1.3/oplangchain/chains/api/openapi/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/openapi/requests_chain.py` & `oplangchain-0.1.3/oplangchain/chains/api/openapi/requests_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/openapi/response_chain.py` & `oplangchain-0.1.3/oplangchain/chains/api/openapi/response_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/podcast_docs.py` & `oplangchain-0.1.3/oplangchain/chains/api/podcast_docs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/api/tmdb_docs.py` & `oplangchain-0.1.3/oplangchain/chains/api/tmdb_docs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/base.py` & `oplangchain-0.1.3/oplangchain/chains/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/chat_vector_db/prompts.py` & `oplangchain-0.1.3/oplangchain/chains/chat_vector_db/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/combine_documents/base.py` & `oplangchain-0.1.3/oplangchain/chains/combine_documents/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/combine_documents/map_reduce.py` & `oplangchain-0.1.3/oplangchain/chains/combine_documents/map_reduce.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/combine_documents/map_rerank.py` & `oplangchain-0.1.3/oplangchain/chains/combine_documents/map_rerank.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/combine_documents/reduce.py` & `oplangchain-0.1.3/oplangchain/chains/combine_documents/reduce.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/combine_documents/refine.py` & `oplangchain-0.1.3/oplangchain/chains/combine_documents/refine.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/combine_documents/stuff.py` & `oplangchain-0.1.3/oplangchain/chains/combine_documents/stuff.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/constitutional_ai/base.py` & `oplangchain-0.1.3/oplangchain/chains/constitutional_ai/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Chain for applying constitutional principles to the outputs of another chain."""
 from typing import Any, Dict, List, Optional
 
 from oplangchain.callbacks.manager import CallbackManagerForChainRun
 from oplangchain.chains.base import Chain
 from oplangchain.chains.constitutional_ai.models import ConstitutionalPrinciple
 from oplangchain.chains.constitutional_ai.principles import PRINCIPLES
-from oplangchain.chains.constitutional_ai.prompts import CRITIQUE_PROMPT, REVISION_PROMPT
+from oplangchain.chains.constitutional_ai.prompts import (
+    CRITIQUE_PROMPT,
+    REVISION_PROMPT,
+)
 from oplangchain.chains.llm import LLMChain
 from oplangchain.schema import BasePromptTemplate
 from oplangchain.schema.language_model import BaseLanguageModel
 
 
 class ConstitutionalChain(Chain):
     """Chain for applying constitutional principles.
```

### Comparing `oplangchain-0.1.2/oplangchain/chains/constitutional_ai/principles.py` & `oplangchain-0.1.3/oplangchain/chains/constitutional_ai/principles.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/constitutional_ai/prompts.py` & `oplangchain-0.1.3/oplangchain/chains/constitutional_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/conversation/base.py` & `oplangchain-0.1.3/oplangchain/chains/conversation/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/conversation/memory.py` & `oplangchain-0.1.3/oplangchain/chains/conversation/memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/conversation/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/conversation/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/conversational_retrieval/base.py` & `oplangchain-0.1.3/oplangchain/chains/conversational_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/conversational_retrieval/prompts.py` & `oplangchain-0.1.3/oplangchain/chains/conversational_retrieval/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/elasticsearch_database/base.py` & `oplangchain-0.1.3/oplangchain/chains/elasticsearch_database/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/elasticsearch_database/prompts.py` & `oplangchain-0.1.3/oplangchain/chains/elasticsearch_database/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/example_generator.py` & `oplangchain-0.1.3/oplangchain/chains/example_generator.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/flare/base.py` & `oplangchain-0.1.3/oplangchain/chains/flare/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/flare/prompts.py` & `oplangchain-0.1.3/oplangchain/chains/flare/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/arangodb.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/arangodb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/base.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 
 from typing import Any, Dict, List, Optional
 
 from pydantic import Field
 
 from oplangchain.callbacks.manager import CallbackManagerForChainRun
 from oplangchain.chains.base import Chain
-from oplangchain.chains.graph_qa.prompts import ENTITY_EXTRACTION_PROMPT, GRAPH_QA_PROMPT
+from oplangchain.chains.graph_qa.prompts import (
+    ENTITY_EXTRACTION_PROMPT,
+    GRAPH_QA_PROMPT,
+)
 from oplangchain.chains.llm import LLMChain
 from oplangchain.graphs.networkx_graph import NetworkxEntityGraph, get_entities
 from oplangchain.schema import BasePromptTemplate
 from oplangchain.schema.language_model import BaseLanguageModel
 
 
 class GraphQAChain(Chain):
```

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/cypher.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/cypher.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 import re
 from typing import Any, Dict, List, Optional
 
 from pydantic import Field
 
 from oplangchain.callbacks.manager import CallbackManagerForChainRun
 from oplangchain.chains.base import Chain
-from oplangchain.chains.graph_qa.prompts import CYPHER_GENERATION_PROMPT, CYPHER_QA_PROMPT
+from oplangchain.chains.graph_qa.prompts import (
+    CYPHER_GENERATION_PROMPT,
+    CYPHER_QA_PROMPT,
+)
 from oplangchain.chains.llm import LLMChain
 from oplangchain.graphs.neo4j_graph import Neo4jGraph
 from oplangchain.schema import BasePromptTemplate
 from oplangchain.schema.language_model import BaseLanguageModel
 
 INTERMEDIATE_STEPS_KEY = "intermediate_steps"
```

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/hugegraph.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/hugegraph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/kuzu.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/kuzu.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/nebulagraph.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/neptune_cypher.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/neptune_cypher.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/prompts.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/graph_qa/sparql.py` & `oplangchain-0.1.3/oplangchain/chains/graph_qa/sparql.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/hyde/base.py` & `oplangchain-0.1.3/oplangchain/chains/hyde/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/hyde/prompts.py` & `oplangchain-0.1.3/oplangchain/chains/hyde/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm.py` & `oplangchain-0.1.3/oplangchain/chains/llm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_bash/base.py` & `oplangchain-0.1.3/oplangchain/chains/llm_bash/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_bash/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/llm_bash/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_checker/base.py` & `oplangchain-0.1.3/oplangchain/chains/llm_checker/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_checker/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/llm_checker/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_math/base.py` & `oplangchain-0.1.3/oplangchain/chains/llm_math/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_math/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/llm_math/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_requests.py` & `oplangchain-0.1.3/oplangchain/chains/llm_requests.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_summarization_checker/base.py` & `oplangchain-0.1.3/oplangchain/chains/llm_summarization_checker/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt` & `oplangchain-0.1.3/oplangchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_symbolic_math/base.py` & `oplangchain-0.1.3/oplangchain/chains/llm_symbolic_math/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/llm_symbolic_math/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/llm_symbolic_math/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/loading.py` & `oplangchain-0.1.3/oplangchain/chains/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/mapreduce.py` & `oplangchain-0.1.3/oplangchain/chains/mapreduce.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/moderation.py` & `oplangchain-0.1.3/oplangchain/chains/moderation.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/natbot/base.py` & `oplangchain-0.1.3/oplangchain/chains/natbot/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/natbot/crawler.py` & `oplangchain-0.1.3/oplangchain/chains/natbot/crawler.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/natbot/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/natbot/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/openai_functions/__init__.py` & `oplangchain-0.1.3/oplangchain/chains/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/openai_functions/base.py` & `oplangchain-0.1.3/oplangchain/chains/openai_functions/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/openai_functions/citation_fuzzy_match.py` & `oplangchain-0.1.3/oplangchain/chains/openai_functions/citation_fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/openai_functions/extraction.py` & `oplangchain-0.1.3/oplangchain/chains/openai_functions/extraction.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/openai_functions/openapi.py` & `oplangchain-0.1.3/oplangchain/chains/openai_functions/openapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,14 +149,21 @@
                 "description": api_op.description,
                 "parameters": {
                     "type": "object",
                     "properties": request_args,
                 },
             }
             functions.append(fn)
+            print(
+                f"Assigning \"{fn['name']}\"",
+                {
+                    "method": method,
+                    "url": api_op.base_url + api_op.path,
+                },
+            )
             _name_to_call_map[fn["name"]] = {
                 "method": method,
                 "url": api_op.base_url + api_op.path,
             }
 
     def default_call_api(
         name: str,
@@ -164,18 +171,29 @@
         headers: Optional[dict] = None,
         params: Optional[dict] = None,
         **kwargs: Any,
     ) -> Any:
         method = _name_to_call_map[name]["method"]
         url = _name_to_call_map[name]["url"]
         path_params = fn_args.pop("path_params", {})
+        path_params = {
+            "url": "https://eforms.com/download/2018/01/Non-Disclosure-Agreement-Template.pdf"
+        }
         url = _format_url(url, path_params)
+        if False:  # testing purposes
+            print("Name: ", name)
+            print(f"Making request to {url} with method {method}")
+            print(f"Headers: {headers}")
+            print(f"Params: {params}")
+            print(f"fn_args: {fn_args}")
         if "data" in fn_args and isinstance(fn_args["data"], dict):
             fn_args["data"] = json.dumps(fn_args["data"])
         _kwargs = {**fn_args, **kwargs}
+        if False:  # testing purposes
+            print(f"Other arguments: {_kwargs}")
         if headers is not None:
             if "headers" in _kwargs:
                 _kwargs["headers"].update(headers)
             else:
                 _kwargs["headers"] = headers
         if params is not None:
             if "params" in _kwargs:
```

### Comparing `oplangchain-0.1.2/oplangchain/chains/openai_functions/qa_with_structure.py` & `oplangchain-0.1.3/oplangchain/chains/openai_functions/qa_with_structure.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/openai_functions/tagging.py` & `oplangchain-0.1.3/oplangchain/chains/openai_functions/tagging.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/openai_functions/utils.py` & `oplangchain-0.1.3/oplangchain/chains/openai_functions/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/prompt_selector.py` & `oplangchain-0.1.3/oplangchain/chains/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_generation/base.py` & `oplangchain-0.1.3/oplangchain/chains/qa_generation/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_generation/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/qa_generation/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_with_sources/base.py` & `oplangchain-0.1.3/oplangchain/chains/qa_with_sources/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_with_sources/loading.py` & `oplangchain-0.1.3/oplangchain/chains/qa_with_sources/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_with_sources/map_reduce_prompt.py` & `oplangchain-0.1.3/oplangchain/chains/qa_with_sources/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_with_sources/refine_prompts.py` & `oplangchain-0.1.3/oplangchain/chains/qa_with_sources/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_with_sources/retrieval.py` & `oplangchain-0.1.3/oplangchain/chains/qa_with_sources/retrieval.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_with_sources/stuff_prompt.py` & `oplangchain-0.1.3/oplangchain/chains/qa_with_sources/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/qa_with_sources/vector_db.py` & `oplangchain-0.1.3/oplangchain/chains/qa_with_sources/vector_db.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/query_constructor/base.py` & `oplangchain-0.1.3/oplangchain/chains/query_constructor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,19 @@
     DEFAULT_SUFFIX,
     EXAMPLE_PROMPT,
     EXAMPLES_WITH_LIMIT,
     SCHEMA_WITH_LIMIT,
 )
 from oplangchain.chains.query_constructor.schema import AttributeInfo
 from oplangchain.output_parsers.json import parse_and_check_json_markdown
-from oplangchain.schema import BaseOutputParser, BasePromptTemplate, OutputParserException
+from oplangchain.schema import (
+    BaseOutputParser,
+    BasePromptTemplate,
+    OutputParserException,
+)
 from oplangchain.schema.language_model import BaseLanguageModel
 
 
 class StructuredQueryOutputParser(BaseOutputParser[StructuredQuery]):
     """Output parser that parses a structured query."""
 
     ast_parse: Callable
```

### Comparing `oplangchain-0.1.2/oplangchain/chains/query_constructor/ir.py` & `oplangchain-0.1.3/oplangchain/chains/query_constructor/ir.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/query_constructor/parser.py` & `oplangchain-0.1.3/oplangchain/chains/query_constructor/parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/query_constructor/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/query_constructor/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/question_answering/__init__.py` & `oplangchain-0.1.3/oplangchain/chains/question_answering/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/question_answering/map_reduce_prompt.py` & `oplangchain-0.1.3/oplangchain/chains/question_answering/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/question_answering/map_rerank_prompt.py` & `oplangchain-0.1.3/oplangchain/chains/question_answering/map_rerank_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/question_answering/refine_prompts.py` & `oplangchain-0.1.3/oplangchain/chains/question_answering/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/question_answering/stuff_prompt.py` & `oplangchain-0.1.3/oplangchain/chains/question_answering/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/retrieval_qa/base.py` & `oplangchain-0.1.3/oplangchain/chains/retrieval_qa/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/router/base.py` & `oplangchain-0.1.3/oplangchain/chains/router/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/router/embedding_router.py` & `oplangchain-0.1.3/oplangchain/chains/router/embedding_router.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/router/llm_router.py` & `oplangchain-0.1.3/oplangchain/chains/router/llm_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 from oplangchain.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from oplangchain.chains import LLMChain
 from oplangchain.chains.router.base import RouterChain
 from oplangchain.output_parsers.json import parse_and_check_json_markdown
-from oplangchain.schema import BaseOutputParser, BasePromptTemplate, OutputParserException
+from oplangchain.schema import (
+    BaseOutputParser,
+    BasePromptTemplate,
+    OutputParserException,
+)
 from oplangchain.schema.language_model import BaseLanguageModel
 
 
 class LLMRouterChain(RouterChain):
     """A router chain that uses an LLM chain to perform routing."""
 
     llm_chain: LLMChain
```

### Comparing `oplangchain-0.1.2/oplangchain/chains/router/multi_prompt.py` & `oplangchain-0.1.3/oplangchain/chains/router/multi_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/router/multi_prompt_prompt.py` & `oplangchain-0.1.3/oplangchain/chains/router/multi_prompt_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/router/multi_retrieval_prompt.py` & `oplangchain-0.1.3/oplangchain/chains/router/multi_retrieval_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/router/multi_retrieval_qa.py` & `oplangchain-0.1.3/oplangchain/chains/router/multi_retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/sequential.py` & `oplangchain-0.1.3/oplangchain/chains/sequential.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/sql_database/prompt.py` & `oplangchain-0.1.3/oplangchain/chains/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/sql_database/query.py` & `oplangchain-0.1.3/oplangchain/chains/sql_database/query.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/summarize/__init__.py` & `oplangchain-0.1.3/oplangchain/chains/summarize/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/summarize/refine_prompts.py` & `oplangchain-0.1.3/oplangchain/chains/summarize/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chains/transform.py` & `oplangchain-0.1.3/oplangchain/chains/transform.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/__init__.py` & `oplangchain-0.1.3/oplangchain/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/anthropic.py` & `oplangchain-0.1.3/oplangchain/chat_models/anthropic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/azure_openai.py` & `oplangchain-0.1.3/oplangchain/chat_models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/azureml_endpoint.py` & `oplangchain-0.1.3/oplangchain/chat_models/azureml_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 from typing import Any, Dict, List, Optional
 
 from pydantic import validator
 
 from oplangchain.callbacks.manager import CallbackManagerForLLMRun
 from oplangchain.chat_models.base import SimpleChatModel
-from oplangchain.llms.azureml_endpoint import AzureMLEndpointClient, ContentFormatterBase
+from oplangchain.llms.azureml_endpoint import (
+    AzureMLEndpointClient,
+    ContentFormatterBase,
+)
 from oplangchain.schema.messages import (
     AIMessage,
     BaseMessage,
     ChatMessage,
     HumanMessage,
     SystemMessage,
 )
```

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/base.py` & `oplangchain-0.1.3/oplangchain/chat_models/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/fake.py` & `oplangchain-0.1.3/oplangchain/chat_models/fake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/google_palm.py` & `oplangchain-0.1.3/oplangchain/chat_models/google_palm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/human.py` & `oplangchain-0.1.3/oplangchain/chat_models/human.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/jinachat.py` & `oplangchain-0.1.3/oplangchain/chat_models/jinachat.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/mlflow_ai_gateway.py` & `oplangchain-0.1.3/oplangchain/chat_models/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/openai.py` & `oplangchain-0.1.3/oplangchain/chat_models/openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/promptlayer_openai.py` & `oplangchain-0.1.3/oplangchain/chat_models/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/chat_models/vertexai.py` & `oplangchain-0.1.3/oplangchain/chat_models/vertexai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/docker-compose.yaml` & `oplangchain-0.1.3/oplangchain/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/docstore/__init__.py` & `oplangchain-0.1.3/oplangchain/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/docstore/arbitrary_fn.py` & `oplangchain-0.1.3/oplangchain/docstore/arbitrary_fn.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/docstore/base.py` & `oplangchain-0.1.3/oplangchain/docstore/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/docstore/in_memory.py` & `oplangchain-0.1.3/oplangchain/docstore/in_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/docstore/wikipedia.py` & `oplangchain-0.1.3/oplangchain/docstore/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/__init__.py` & `oplangchain-0.1.3/oplangchain/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/acreom.py` & `oplangchain-0.1.3/oplangchain/document_loaders/acreom.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/airbyte_json.py` & `oplangchain-0.1.3/oplangchain/document_loaders/airbyte_json.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/airtable.py` & `oplangchain-0.1.3/oplangchain/document_loaders/airtable.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/apify_dataset.py` & `oplangchain-0.1.3/oplangchain/document_loaders/apify_dataset.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/arxiv.py` & `oplangchain-0.1.3/oplangchain/document_loaders/arxiv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/async_html.py` & `oplangchain-0.1.3/oplangchain/document_loaders/async_html.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/azlyrics.py` & `oplangchain-0.1.3/oplangchain/document_loaders/azlyrics.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/azure_blob_storage_container.py` & `oplangchain-0.1.3/oplangchain/document_loaders/azure_blob_storage_container.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/azure_blob_storage_file.py` & `oplangchain-0.1.3/oplangchain/document_loaders/azure_blob_storage_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/base.py` & `oplangchain-0.1.3/oplangchain/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/bibtex.py` & `oplangchain-0.1.3/oplangchain/document_loaders/bibtex.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/bigquery.py` & `oplangchain-0.1.3/oplangchain/document_loaders/bigquery.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/bilibili.py` & `oplangchain-0.1.3/oplangchain/document_loaders/bilibili.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/blackboard.py` & `oplangchain-0.1.3/oplangchain/document_loaders/blackboard.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/blob_loaders/file_system.py` & `oplangchain-0.1.3/oplangchain/document_loaders/blob_loaders/file_system.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/blob_loaders/schema.py` & `oplangchain-0.1.3/oplangchain/document_loaders/blob_loaders/schema.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/blob_loaders/youtube_audio.py` & `oplangchain-0.1.3/oplangchain/document_loaders/blob_loaders/youtube_audio.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/blockchain.py` & `oplangchain-0.1.3/oplangchain/document_loaders/blockchain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/brave_search.py` & `oplangchain-0.1.3/oplangchain/document_loaders/brave_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/browserless.py` & `oplangchain-0.1.3/oplangchain/document_loaders/browserless.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/chatgpt.py` & `oplangchain-0.1.3/oplangchain/document_loaders/chatgpt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/college_confidential.py` & `oplangchain-0.1.3/oplangchain/document_loaders/college_confidential.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/concurrent.py` & `oplangchain-0.1.3/oplangchain/document_loaders/concurrent.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/confluence.py` & `oplangchain-0.1.3/oplangchain/document_loaders/confluence.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/conllu.py` & `oplangchain-0.1.3/oplangchain/document_loaders/conllu.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/csv_loader.py` & `oplangchain-0.1.3/oplangchain/document_loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/cube_semantic.py` & `oplangchain-0.1.3/oplangchain/document_loaders/cube_semantic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/datadog_logs.py` & `oplangchain-0.1.3/oplangchain/document_loaders/datadog_logs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/dataframe.py` & `oplangchain-0.1.3/oplangchain/document_loaders/dataframe.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/diffbot.py` & `oplangchain-0.1.3/oplangchain/document_loaders/diffbot.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/directory.py` & `oplangchain-0.1.3/oplangchain/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/discord.py` & `oplangchain-0.1.3/oplangchain/document_loaders/discord.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/docugami.py` & `oplangchain-0.1.3/oplangchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/dropbox.py` & `oplangchain-0.1.3/oplangchain/document_loaders/dropbox.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/duckdb_loader.py` & `oplangchain-0.1.3/oplangchain/document_loaders/duckdb_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/email.py` & `oplangchain-0.1.3/oplangchain/document_loaders/email.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/embaas.py` & `oplangchain-0.1.3/oplangchain/document_loaders/embaas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/epub.py` & `oplangchain-0.1.3/oplangchain/document_loaders/epub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/etherscan.py` & `oplangchain-0.1.3/oplangchain/document_loaders/etherscan.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/evernote.py` & `oplangchain-0.1.3/oplangchain/document_loaders/evernote.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/excel.py` & `oplangchain-0.1.3/oplangchain/document_loaders/excel.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/facebook_chat.py` & `oplangchain-0.1.3/oplangchain/document_loaders/facebook_chat.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/fauna.py` & `oplangchain-0.1.3/oplangchain/document_loaders/fauna.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/figma.py` & `oplangchain-0.1.3/oplangchain/document_loaders/figma.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/gcs_directory.py` & `oplangchain-0.1.3/oplangchain/document_loaders/gcs_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/gcs_file.py` & `oplangchain-0.1.3/oplangchain/document_loaders/gcs_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/generic.py` & `oplangchain-0.1.3/oplangchain/document_loaders/generic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/geodataframe.py` & `oplangchain-0.1.3/oplangchain/document_loaders/geodataframe.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/git.py` & `oplangchain-0.1.3/oplangchain/document_loaders/git.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/gitbook.py` & `oplangchain-0.1.3/oplangchain/document_loaders/gitbook.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/github.py` & `oplangchain-0.1.3/oplangchain/document_loaders/github.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/googledrive.py` & `oplangchain-0.1.3/oplangchain/document_loaders/googledrive.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/gutenberg.py` & `oplangchain-0.1.3/oplangchain/document_loaders/gutenberg.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/helpers.py` & `oplangchain-0.1.3/oplangchain/document_loaders/helpers.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/hn.py` & `oplangchain-0.1.3/oplangchain/document_loaders/hn.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/html.py` & `oplangchain-0.1.3/oplangchain/document_loaders/html.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/html_bs.py` & `oplangchain-0.1.3/oplangchain/document_loaders/html_bs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/hugging_face_dataset.py` & `oplangchain-0.1.3/oplangchain/document_loaders/hugging_face_dataset.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/ifixit.py` & `oplangchain-0.1.3/oplangchain/document_loaders/ifixit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/image.py` & `oplangchain-0.1.3/oplangchain/document_loaders/image.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/image_captions.py` & `oplangchain-0.1.3/oplangchain/document_loaders/image_captions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/iugu.py` & `oplangchain-0.1.3/oplangchain/document_loaders/iugu.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/joplin.py` & `oplangchain-0.1.3/oplangchain/document_loaders/joplin.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/json_loader.py` & `oplangchain-0.1.3/oplangchain/document_loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/larksuite.py` & `oplangchain-0.1.3/oplangchain/document_loaders/larksuite.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/markdown.py` & `oplangchain-0.1.3/oplangchain/document_loaders/markdown.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/mastodon.py` & `oplangchain-0.1.3/oplangchain/document_loaders/mastodon.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/max_compute.py` & `oplangchain-0.1.3/oplangchain/document_loaders/max_compute.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/mediawikidump.py` & `oplangchain-0.1.3/oplangchain/document_loaders/mediawikidump.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/merge.py` & `oplangchain-0.1.3/oplangchain/document_loaders/merge.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/mhtml.py` & `oplangchain-0.1.3/oplangchain/document_loaders/mhtml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/modern_treasury.py` & `oplangchain-0.1.3/oplangchain/document_loaders/modern_treasury.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/news.py` & `oplangchain-0.1.3/oplangchain/document_loaders/news.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/notebook.py` & `oplangchain-0.1.3/oplangchain/document_loaders/notebook.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/notion.py` & `oplangchain-0.1.3/oplangchain/document_loaders/notion.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/notiondb.py` & `oplangchain-0.1.3/oplangchain/document_loaders/notiondb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/nuclia.py` & `oplangchain-0.1.3/oplangchain/document_loaders/nuclia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/obs_directory.py` & `oplangchain-0.1.3/oplangchain/document_loaders/obs_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/obs_file.py` & `oplangchain-0.1.3/oplangchain/document_loaders/obs_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/obsidian.py` & `oplangchain-0.1.3/oplangchain/document_loaders/obsidian.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/odt.py` & `oplangchain-0.1.3/oplangchain/document_loaders/odt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/onedrive.py` & `oplangchain-0.1.3/oplangchain/document_loaders/onedrive.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/onedrive_file.py` & `oplangchain-0.1.3/oplangchain/document_loaders/onedrive_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/open_city_data.py` & `oplangchain-0.1.3/oplangchain/document_loaders/open_city_data.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/org_mode.py` & `oplangchain-0.1.3/oplangchain/document_loaders/org_mode.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/__init__.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/audio.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/generic.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/grobid.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/grobid.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/html/bs4.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/html/bs4.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/language/javascript.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/language/javascript.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/language/language_parser.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/language/language_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/language/python.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/language/python.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/pdf.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/pdf.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/parsers/registry.py` & `oplangchain-0.1.3/oplangchain/document_loaders/parsers/registry.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/pdf.py` & `oplangchain-0.1.3/oplangchain/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/powerpoint.py` & `oplangchain-0.1.3/oplangchain/document_loaders/powerpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/psychic.py` & `oplangchain-0.1.3/oplangchain/document_loaders/psychic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/pyspark_dataframe.py` & `oplangchain-0.1.3/oplangchain/document_loaders/pyspark_dataframe.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/python.py` & `oplangchain-0.1.3/oplangchain/document_loaders/python.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/readthedocs.py` & `oplangchain-0.1.3/oplangchain/document_loaders/readthedocs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/recursive_url_loader.py` & `oplangchain-0.1.3/oplangchain/document_loaders/recursive_url_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/reddit.py` & `oplangchain-0.1.3/oplangchain/document_loaders/reddit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/roam.py` & `oplangchain-0.1.3/oplangchain/document_loaders/roam.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/rocksetdb.py` & `oplangchain-0.1.3/oplangchain/document_loaders/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/rss.py` & `oplangchain-0.1.3/oplangchain/document_loaders/rss.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/rst.py` & `oplangchain-0.1.3/oplangchain/document_loaders/rst.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/rtf.py` & `oplangchain-0.1.3/oplangchain/document_loaders/rtf.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/s3_directory.py` & `oplangchain-0.1.3/oplangchain/document_loaders/s3_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/s3_file.py` & `oplangchain-0.1.3/oplangchain/document_loaders/s3_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/sitemap.py` & `oplangchain-0.1.3/oplangchain/document_loaders/sitemap.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/slack_directory.py` & `oplangchain-0.1.3/oplangchain/document_loaders/slack_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/snowflake_loader.py` & `oplangchain-0.1.3/oplangchain/document_loaders/snowflake_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/spreedly.py` & `oplangchain-0.1.3/oplangchain/document_loaders/spreedly.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/srt.py` & `oplangchain-0.1.3/oplangchain/document_loaders/srt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/stripe.py` & `oplangchain-0.1.3/oplangchain/document_loaders/stripe.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/telegram.py` & `oplangchain-0.1.3/oplangchain/document_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/tencent_cos_directory.py` & `oplangchain-0.1.3/oplangchain/document_loaders/tencent_cos_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/tencent_cos_file.py` & `oplangchain-0.1.3/oplangchain/document_loaders/tencent_cos_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/text.py` & `oplangchain-0.1.3/oplangchain/document_loaders/text.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/tomarkdown.py` & `oplangchain-0.1.3/oplangchain/document_loaders/tomarkdown.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/toml.py` & `oplangchain-0.1.3/oplangchain/document_loaders/toml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/trello.py` & `oplangchain-0.1.3/oplangchain/document_loaders/trello.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/tsv.py` & `oplangchain-0.1.3/oplangchain/document_loaders/tsv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/twitter.py` & `oplangchain-0.1.3/oplangchain/document_loaders/twitter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/unstructured.py` & `oplangchain-0.1.3/oplangchain/document_loaders/unstructured.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/url.py` & `oplangchain-0.1.3/oplangchain/document_loaders/url.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/url_playwright.py` & `oplangchain-0.1.3/oplangchain/document_loaders/url_playwright.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/url_selenium.py` & `oplangchain-0.1.3/oplangchain/document_loaders/url_selenium.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/weather.py` & `oplangchain-0.1.3/oplangchain/document_loaders/weather.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/web_base.py` & `oplangchain-0.1.3/oplangchain/document_loaders/web_base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/whatsapp_chat.py` & `oplangchain-0.1.3/oplangchain/document_loaders/whatsapp_chat.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/wikipedia.py` & `oplangchain-0.1.3/oplangchain/document_loaders/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/word_document.py` & `oplangchain-0.1.3/oplangchain/document_loaders/word_document.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/xml.py` & `oplangchain-0.1.3/oplangchain/document_loaders/xml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/xorbits.py` & `oplangchain-0.1.3/oplangchain/document_loaders/xorbits.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_loaders/youtube.py` & `oplangchain-0.1.3/oplangchain/document_loaders/youtube.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/__init__.py` & `oplangchain-0.1.3/oplangchain/document_transformers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,27 @@
     Document
 """  # noqa: E501
 
 from oplangchain.document_transformers.doctran_text_extract import (
     DoctranPropertyExtractor,
 )
 from oplangchain.document_transformers.doctran_text_qa import DoctranQATransformer
-from oplangchain.document_transformers.doctran_text_translate import DoctranTextTranslator
+from oplangchain.document_transformers.doctran_text_translate import (
+    DoctranTextTranslator,
+)
 from oplangchain.document_transformers.embeddings_redundant_filter import (
     EmbeddingsClusteringFilter,
     EmbeddingsRedundantFilter,
     get_stateful_documents,
 )
 from oplangchain.document_transformers.html2text import Html2TextTransformer
 from oplangchain.document_transformers.long_context_reorder import LongContextReorder
-from oplangchain.document_transformers.nuclia_text_transform import NucliaTextTransformer
+from oplangchain.document_transformers.nuclia_text_transform import (
+    NucliaTextTransformer,
+)
 from oplangchain.document_transformers.openai_functions import OpenAIMetadataTagger
 
 __all__ = [
     "DoctranQATransformer",
     "DoctranTextTranslator",
     "DoctranPropertyExtractor",
     "EmbeddingsClusteringFilter",
```

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/doctran_text_extract.py` & `oplangchain-0.1.3/oplangchain/document_transformers/doctran_text_extract.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/doctran_text_qa.py` & `oplangchain-0.1.3/oplangchain/document_transformers/doctran_text_qa.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/doctran_text_translate.py` & `oplangchain-0.1.3/oplangchain/document_transformers/doctran_text_translate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/embeddings_redundant_filter.py` & `oplangchain-0.1.3/oplangchain/document_transformers/embeddings_redundant_filter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/html2text.py` & `oplangchain-0.1.3/oplangchain/document_transformers/html2text.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/long_context_reorder.py` & `oplangchain-0.1.3/oplangchain/document_transformers/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/nuclia_text_transform.py` & `oplangchain-0.1.3/oplangchain/document_transformers/nuclia_text_transform.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/document_transformers/openai_functions.py` & `oplangchain-0.1.3/oplangchain/document_transformers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/__init__.py` & `oplangchain-0.1.3/oplangchain/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/aleph_alpha.py` & `oplangchain-0.1.3/oplangchain/embeddings/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/awa.py` & `oplangchain-0.1.3/oplangchain/embeddings/awa.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/base.py` & `oplangchain-0.1.3/oplangchain/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/bedrock.py` & `oplangchain-0.1.3/oplangchain/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/clarifai.py` & `oplangchain-0.1.3/oplangchain/embeddings/clarifai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/cohere.py` & `oplangchain-0.1.3/oplangchain/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/dashscope.py` & `oplangchain-0.1.3/oplangchain/embeddings/dashscope.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/deepinfra.py` & `oplangchain-0.1.3/oplangchain/embeddings/deepinfra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/edenai.py` & `oplangchain-0.1.3/oplangchain/embeddings/edenai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/elasticsearch.py` & `oplangchain-0.1.3/oplangchain/embeddings/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/embaas.py` & `oplangchain-0.1.3/oplangchain/embeddings/embaas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/fake.py` & `oplangchain-0.1.3/oplangchain/embeddings/fake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/google_palm.py` & `oplangchain-0.1.3/oplangchain/embeddings/google_palm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/gpt4all.py` & `oplangchain-0.1.3/oplangchain/embeddings/gpt4all.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/huggingface.py` & `oplangchain-0.1.3/oplangchain/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/huggingface_hub.py` & `oplangchain-0.1.3/oplangchain/embeddings/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/jina.py` & `oplangchain-0.1.3/oplangchain/embeddings/jina.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/llamacpp.py` & `oplangchain-0.1.3/oplangchain/embeddings/llamacpp.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/localai.py` & `oplangchain-0.1.3/oplangchain/embeddings/localai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/minimax.py` & `oplangchain-0.1.3/oplangchain/embeddings/minimax.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/mlflow_gateway.py` & `oplangchain-0.1.3/oplangchain/embeddings/mlflow_gateway.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/modelscope_hub.py` & `oplangchain-0.1.3/oplangchain/embeddings/modelscope_hub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/mosaicml.py` & `oplangchain-0.1.3/oplangchain/embeddings/mosaicml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/nlpcloud.py` & `oplangchain-0.1.3/oplangchain/embeddings/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/octoai_embeddings.py` & `oplangchain-0.1.3/oplangchain/embeddings/octoai_embeddings.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/openai.py` & `oplangchain-0.1.3/oplangchain/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/sagemaker_endpoint.py` & `oplangchain-0.1.3/oplangchain/embeddings/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/self_hosted.py` & `oplangchain-0.1.3/oplangchain/embeddings/self_hosted.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/self_hosted_hugging_face.py` & `oplangchain-0.1.3/oplangchain/embeddings/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/spacy_embeddings.py` & `oplangchain-0.1.3/oplangchain/embeddings/spacy_embeddings.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/tensorflow_hub.py` & `oplangchain-0.1.3/oplangchain/embeddings/tensorflow_hub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/vertexai.py` & `oplangchain-0.1.3/oplangchain/embeddings/vertexai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/embeddings/xinference.py` & `oplangchain-0.1.3/oplangchain/embeddings/xinference.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/__init__.py` & `oplangchain-0.1.3/oplangchain/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/agents/trajectory_eval_chain.py` & `oplangchain-0.1.3/oplangchain/evaluation/agents/trajectory_eval_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/agents/trajectory_eval_prompt.py` & `oplangchain-0.1.3/oplangchain/evaluation/agents/trajectory_eval_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/comparison/__init__.py` & `oplangchain-0.1.3/oplangchain/evaluation/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/comparison/eval_chain.py` & `oplangchain-0.1.3/oplangchain/evaluation/comparison/eval_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/comparison/prompt.py` & `oplangchain-0.1.3/oplangchain/evaluation/comparison/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/criteria/__init__.py` & `oplangchain-0.1.3/oplangchain/evaluation/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/criteria/eval_chain.py` & `oplangchain-0.1.3/oplangchain/evaluation/criteria/eval_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/criteria/prompt.py` & `oplangchain-0.1.3/oplangchain/evaluation/criteria/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/embedding_distance/base.py` & `oplangchain-0.1.3/oplangchain/evaluation/embedding_distance/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/loading.py` & `oplangchain-0.1.3/oplangchain/evaluation/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/qa/eval_chain.py` & `oplangchain-0.1.3/oplangchain/evaluation/qa/eval_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/qa/eval_prompt.py` & `oplangchain-0.1.3/oplangchain/evaluation/qa/eval_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/qa/generate_chain.py` & `oplangchain-0.1.3/oplangchain/evaluation/qa/generate_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/qa/generate_prompt.py` & `oplangchain-0.1.3/oplangchain/evaluation/qa/generate_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/schema.py` & `oplangchain-0.1.3/oplangchain/evaluation/schema.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/evaluation/string_distance/base.py` & `oplangchain-0.1.3/oplangchain/evaluation/string_distance/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/__init__.py` & `oplangchain-0.1.3/oplangchain/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/arangodb_graph.py` & `oplangchain-0.1.3/oplangchain/graphs/arangodb_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/hugegraph.py` & `oplangchain-0.1.3/oplangchain/graphs/hugegraph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/kuzu_graph.py` & `oplangchain-0.1.3/oplangchain/graphs/kuzu_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/memgraph_graph.py` & `oplangchain-0.1.3/oplangchain/graphs/memgraph_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/nebula_graph.py` & `oplangchain-0.1.3/oplangchain/graphs/nebula_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/neo4j_graph.py` & `oplangchain-0.1.3/oplangchain/graphs/neo4j_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/neptune_graph.py` & `oplangchain-0.1.3/oplangchain/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/networkx_graph.py` & `oplangchain-0.1.3/oplangchain/graphs/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/graphs/rdf_graph.py` & `oplangchain-0.1.3/oplangchain/graphs/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/indexes/graph.py` & `oplangchain-0.1.3/oplangchain/indexes/graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/indexes/prompts/entity_extraction.py` & `oplangchain-0.1.3/oplangchain/indexes/prompts/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/indexes/prompts/entity_summarization.py` & `oplangchain-0.1.3/oplangchain/indexes/prompts/entity_summarization.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/indexes/prompts/knowledge_triplet_extraction.py` & `oplangchain-0.1.3/oplangchain/indexes/prompts/knowledge_triplet_extraction.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/indexes/vectorstore.py` & `oplangchain-0.1.3/oplangchain/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/__init__.py` & `oplangchain-0.1.3/oplangchain/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/ai21.py` & `oplangchain-0.1.3/oplangchain/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/aleph_alpha.py` & `oplangchain-0.1.3/oplangchain/llms/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/amazon_api_gateway.py` & `oplangchain-0.1.3/oplangchain/llms/amazon_api_gateway.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/anthropic.py` & `oplangchain-0.1.3/oplangchain/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/anyscale.py` & `oplangchain-0.1.3/oplangchain/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/aviary.py` & `oplangchain-0.1.3/oplangchain/llms/aviary.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/azureml_endpoint.py` & `oplangchain-0.1.3/oplangchain/llms/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/bananadev.py` & `oplangchain-0.1.3/oplangchain/llms/bananadev.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/base.py` & `oplangchain-0.1.3/oplangchain/llms/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/baseten.py` & `oplangchain-0.1.3/oplangchain/llms/baseten.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/beam.py` & `oplangchain-0.1.3/oplangchain/llms/beam.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/bedrock.py` & `oplangchain-0.1.3/oplangchain/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/cerebriumai.py` & `oplangchain-0.1.3/oplangchain/llms/cerebriumai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/chatglm.py` & `oplangchain-0.1.3/oplangchain/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/clarifai.py` & `oplangchain-0.1.3/oplangchain/llms/clarifai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/cohere.py` & `oplangchain-0.1.3/oplangchain/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/ctransformers.py` & `oplangchain-0.1.3/oplangchain/llms/ctransformers.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/databricks.py` & `oplangchain-0.1.3/oplangchain/llms/databricks.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/deepinfra.py` & `oplangchain-0.1.3/oplangchain/llms/deepinfra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/edenai.py` & `oplangchain-0.1.3/oplangchain/llms/edenai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/fake.py` & `oplangchain-0.1.3/oplangchain/llms/fake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/fireworks.py` & `oplangchain-0.1.3/oplangchain/llms/fireworks.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/forefrontai.py` & `oplangchain-0.1.3/oplangchain/llms/forefrontai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/google_palm.py` & `oplangchain-0.1.3/oplangchain/llms/google_palm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/gooseai.py` & `oplangchain-0.1.3/oplangchain/llms/gooseai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/gpt4all.py` & `oplangchain-0.1.3/oplangchain/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/huggingface_endpoint.py` & `oplangchain-0.1.3/oplangchain/llms/huggingface_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/huggingface_hub.py` & `oplangchain-0.1.3/oplangchain/llms/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/huggingface_pipeline.py` & `oplangchain-0.1.3/oplangchain/llms/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/huggingface_text_gen_inference.py` & `oplangchain-0.1.3/oplangchain/llms/huggingface_text_gen_inference.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/human.py` & `oplangchain-0.1.3/oplangchain/llms/human.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/koboldai.py` & `oplangchain-0.1.3/oplangchain/llms/koboldai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/llamacpp.py` & `oplangchain-0.1.3/oplangchain/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/loading.py` & `oplangchain-0.1.3/oplangchain/llms/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/manifest.py` & `oplangchain-0.1.3/oplangchain/llms/manifest.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/minimax.py` & `oplangchain-0.1.3/oplangchain/llms/minimax.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/mlflow_ai_gateway.py` & `oplangchain-0.1.3/oplangchain/llms/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/modal.py` & `oplangchain-0.1.3/oplangchain/llms/modal.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/mosaicml.py` & `oplangchain-0.1.3/oplangchain/llms/mosaicml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/nlpcloud.py` & `oplangchain-0.1.3/oplangchain/llms/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/octoai_endpoint.py` & `oplangchain-0.1.3/oplangchain/llms/octoai_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/openai.py` & `oplangchain-0.1.3/oplangchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/openllm.py` & `oplangchain-0.1.3/oplangchain/llms/openllm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/openlm.py` & `oplangchain-0.1.3/oplangchain/llms/openlm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/petals.py` & `oplangchain-0.1.3/oplangchain/llms/petals.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/pipelineai.py` & `oplangchain-0.1.3/oplangchain/llms/pipelineai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/predibase.py` & `oplangchain-0.1.3/oplangchain/llms/predibase.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/predictionguard.py` & `oplangchain-0.1.3/oplangchain/llms/predictionguard.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/promptlayer_openai.py` & `oplangchain-0.1.3/oplangchain/llms/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/replicate.py` & `oplangchain-0.1.3/oplangchain/llms/replicate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/rwkv.py` & `oplangchain-0.1.3/oplangchain/llms/rwkv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/sagemaker_endpoint.py` & `oplangchain-0.1.3/oplangchain/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/self_hosted.py` & `oplangchain-0.1.3/oplangchain/llms/self_hosted.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/self_hosted_hugging_face.py` & `oplangchain-0.1.3/oplangchain/llms/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/stochasticai.py` & `oplangchain-0.1.3/oplangchain/llms/stochasticai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/textgen.py` & `oplangchain-0.1.3/oplangchain/llms/textgen.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/tongyi.py` & `oplangchain-0.1.3/oplangchain/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/vertexai.py` & `oplangchain-0.1.3/oplangchain/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/vllm.py` & `oplangchain-0.1.3/oplangchain/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/writer.py` & `oplangchain-0.1.3/oplangchain/llms/writer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/llms/xinference.py` & `oplangchain-0.1.3/oplangchain/llms/xinference.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/load/dump.py` & `oplangchain-0.1.3/oplangchain/load/dump.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/load/load.py` & `oplangchain-0.1.3/oplangchain/load/load.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/load/serializable.py` & `oplangchain-0.1.3/oplangchain/load/serializable.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/__init__.py` & `oplangchain-0.1.3/oplangchain/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/buffer.py` & `oplangchain-0.1.3/oplangchain/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/buffer_window.py` & `oplangchain-0.1.3/oplangchain/memory/buffer_window.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_memory.py` & `oplangchain-0.1.3/oplangchain/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/__init__.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from oplangchain.memory.chat_message_histories.cassandra import (
     CassandraChatMessageHistory,
 )
-from oplangchain.memory.chat_message_histories.cosmos_db import CosmosDBChatMessageHistory
-from oplangchain.memory.chat_message_histories.dynamodb import DynamoDBChatMessageHistory
+from oplangchain.memory.chat_message_histories.cosmos_db import (
+    CosmosDBChatMessageHistory,
+)
+from oplangchain.memory.chat_message_histories.dynamodb import (
+    DynamoDBChatMessageHistory,
+)
 from oplangchain.memory.chat_message_histories.file import FileChatMessageHistory
 from oplangchain.memory.chat_message_histories.firestore import (
     FirestoreChatMessageHistory,
 )
 from oplangchain.memory.chat_message_histories.in_memory import ChatMessageHistory
 from oplangchain.memory.chat_message_histories.momento import MomentoChatMessageHistory
 from oplangchain.memory.chat_message_histories.mongodb import MongoDBChatMessageHistory
-from oplangchain.memory.chat_message_histories.postgres import PostgresChatMessageHistory
+from oplangchain.memory.chat_message_histories.postgres import (
+    PostgresChatMessageHistory,
+)
 from oplangchain.memory.chat_message_histories.redis import RedisChatMessageHistory
 from oplangchain.memory.chat_message_histories.sql import SQLChatMessageHistory
 from oplangchain.memory.chat_message_histories.streamlit import (
     StreamlitChatMessageHistory,
 )
 from oplangchain.memory.chat_message_histories.zep import ZepChatMessageHistory
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/cassandra.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/cassandra.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 if typing.TYPE_CHECKING:
     from cassandra.cluster import Session
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, _message_to_dict, messages_from_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    _message_to_dict,
+    messages_from_dict,
+)
 
 DEFAULT_TABLE_NAME = "message_store"
 DEFAULT_TTL_SECONDS = None
 
 
 class CassandraChatMessageHistory(BaseChatMessageHistory):
     """Chat message history that stores history in Cassandra.
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/cosmos_db.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/cosmos_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import logging
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, List, Optional, Type
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, messages_from_dict, messages_to_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    messages_from_dict,
+    messages_to_dict,
+)
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from azure.cosmos import ContainerProxy
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/dynamodb.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/dynamodb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/file.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 import logging
 from pathlib import Path
 from typing import List
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, messages_from_dict, messages_to_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    messages_from_dict,
+    messages_to_dict,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class FileChatMessageHistory(BaseChatMessageHistory):
     """
     Chat message history that stores history in a local file.
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/firestore.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/firestore.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 import logging
 from typing import TYPE_CHECKING, List, Optional
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, messages_from_dict, messages_to_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    messages_from_dict,
+    messages_to_dict,
+)
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from google.cloud.firestore import Client, DocumentReference
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/in_memory.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/in_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/momento.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/momento.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import json
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, Optional
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, _message_to_dict, messages_from_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    _message_to_dict,
+    messages_from_dict,
+)
 from oplangchain.utils import get_from_env
 
 if TYPE_CHECKING:
     import momento
 
 
 def _ensure_cache_exists(cache_client: momento.CacheClient, cache_name: str) -> None:
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/mongodb.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/mongodb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import json
 import logging
 from typing import List
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, _message_to_dict, messages_from_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    _message_to_dict,
+    messages_from_dict,
+)
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_DBNAME = "chat_history"
 DEFAULT_COLLECTION_NAME = "message_store"
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/postgres.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import json
 import logging
 from typing import List
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, _message_to_dict, messages_from_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    _message_to_dict,
+    messages_from_dict,
+)
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_CONNECTION_STRING = "postgresql://postgres:mypassword@localhost/chat_history"
 
 
 class PostgresChatMessageHistory(BaseChatMessageHistory):
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/redis.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/redis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import json
 import logging
 from typing import List, Optional
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, _message_to_dict, messages_from_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    _message_to_dict,
+    messages_from_dict,
+)
 from oplangchain.utilities.redis import get_client
 
 logger = logging.getLogger(__name__)
 
 
 class RedisChatMessageHistory(BaseChatMessageHistory):
     """Chat message history stored in a Redis database."""
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/sql.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 except ImportError:
     from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
 from oplangchain.schema import (
     BaseChatMessageHistory,
 )
-from oplangchain.schema.messages import BaseMessage, _message_to_dict, messages_from_dict
+from oplangchain.schema.messages import (
+    BaseMessage,
+    _message_to_dict,
+    messages_from_dict,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def create_message_model(table_name, DynamicBase):  # type: ignore
     """
     Create a message model for a given table name.
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/streamlit.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/streamlit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/chat_message_histories/zep.py` & `oplangchain-0.1.3/oplangchain/memory/chat_message_histories/zep.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/combined.py` & `oplangchain-0.1.3/oplangchain/memory/combined.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/entity.py` & `oplangchain-0.1.3/oplangchain/memory/entity.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/kg.py` & `oplangchain-0.1.3/oplangchain/memory/kg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import Any, Dict, List, Type, Union
 
 from pydantic import Field
 
 from oplangchain.chains.llm import LLMChain
 from oplangchain.graphs import NetworkxEntityGraph
-from oplangchain.graphs.networkx_graph import KnowledgeTriple, get_entities, parse_triples
+from oplangchain.graphs.networkx_graph import (
+    KnowledgeTriple,
+    get_entities,
+    parse_triples,
+)
 from oplangchain.memory.chat_memory import BaseChatMemory
 from oplangchain.memory.prompt import (
     ENTITY_EXTRACTION_PROMPT,
     KNOWLEDGE_TRIPLE_EXTRACTION_PROMPT,
 )
 from oplangchain.memory.utils import get_prompt_input_key
 from oplangchain.schema import BasePromptTemplate
```

### Comparing `oplangchain-0.1.2/oplangchain/memory/motorhead_memory.py` & `oplangchain-0.1.3/oplangchain/memory/motorhead_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/prompt.py` & `oplangchain-0.1.3/oplangchain/memory/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/readonly.py` & `oplangchain-0.1.3/oplangchain/memory/readonly.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/simple.py` & `oplangchain-0.1.3/oplangchain/memory/simple.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/summary.py` & `oplangchain-0.1.3/oplangchain/memory/summary.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/summary_buffer.py` & `oplangchain-0.1.3/oplangchain/memory/summary_buffer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/token_buffer.py` & `oplangchain-0.1.3/oplangchain/memory/token_buffer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/utils.py` & `oplangchain-0.1.3/oplangchain/memory/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/vectorstore.py` & `oplangchain-0.1.3/oplangchain/memory/vectorstore.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/memory/zep_memory.py` & `oplangchain-0.1.3/oplangchain/memory/zep_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/model_laboratory.py` & `oplangchain-0.1.3/oplangchain/model_laboratory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/__init__.py` & `oplangchain-0.1.3/oplangchain/output_parsers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,18 @@
     CommaSeparatedListOutputParser,
     ListOutputParser,
 )
 from oplangchain.output_parsers.pydantic import PydanticOutputParser
 from oplangchain.output_parsers.rail_parser import GuardrailsOutputParser
 from oplangchain.output_parsers.regex import RegexParser
 from oplangchain.output_parsers.regex_dict import RegexDictParser
-from oplangchain.output_parsers.retry import RetryOutputParser, RetryWithErrorOutputParser
+from oplangchain.output_parsers.retry import (
+    RetryOutputParser,
+    RetryWithErrorOutputParser,
+)
 from oplangchain.output_parsers.structured import ResponseSchema, StructuredOutputParser
 
 __all__ = [
     "BooleanOutputParser",
     "CombiningOutputParser",
     "CommaSeparatedListOutputParser",
     "DatetimeOutputParser",
```

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/boolean.py` & `oplangchain-0.1.3/oplangchain/output_parsers/boolean.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/combining.py` & `oplangchain-0.1.3/oplangchain/output_parsers/combining.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/datetime.py` & `oplangchain-0.1.3/oplangchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/enum.py` & `oplangchain-0.1.3/oplangchain/output_parsers/enum.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/fix.py` & `oplangchain-0.1.3/oplangchain/output_parsers/fix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
 from typing import TypeVar
 
 from oplangchain.chains.llm import LLMChain
 from oplangchain.output_parsers.prompts import NAIVE_FIX_PROMPT
-from oplangchain.schema import BaseOutputParser, BasePromptTemplate, OutputParserException
+from oplangchain.schema import (
+    BaseOutputParser,
+    BasePromptTemplate,
+    OutputParserException,
+)
 from oplangchain.schema.language_model import BaseLanguageModel
 
 T = TypeVar("T")
 
 
 class OutputFixingParser(BaseOutputParser[T]):
     """Wraps a parser and tries to fix parsing errors."""
```

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/format_instructions.py` & `oplangchain-0.1.3/oplangchain/output_parsers/format_instructions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/json.py` & `oplangchain-0.1.3/oplangchain/output_parsers/json.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/list.py` & `oplangchain-0.1.3/oplangchain/output_parsers/list.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/loading.py` & `oplangchain-0.1.3/oplangchain/output_parsers/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/openai_functions.py` & `oplangchain-0.1.3/oplangchain/output_parsers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/pydantic.py` & `oplangchain-0.1.3/oplangchain/output_parsers/pydantic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/rail_parser.py` & `oplangchain-0.1.3/oplangchain/output_parsers/rail_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/regex.py` & `oplangchain-0.1.3/oplangchain/output_parsers/regex.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/regex_dict.py` & `oplangchain-0.1.3/oplangchain/output_parsers/regex_dict.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/retry.py` & `oplangchain-0.1.3/oplangchain/output_parsers/retry.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/output_parsers/structured.py` & `oplangchain-0.1.3/oplangchain/output_parsers/structured.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/__init__.py` & `oplangchain-0.1.3/oplangchain/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/base.py` & `oplangchain-0.1.3/oplangchain/prompts/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/chat.py` & `oplangchain-0.1.3/oplangchain/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/example_selector/__init__.py` & `oplangchain-0.1.3/oplangchain/prompts/example_selector/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Logic for selecting examples to include in prompts."""
 from oplangchain.prompts.example_selector.length_based import LengthBasedExampleSelector
-from oplangchain.prompts.example_selector.ngram_overlap import NGramOverlapExampleSelector
+from oplangchain.prompts.example_selector.ngram_overlap import (
+    NGramOverlapExampleSelector,
+)
 from oplangchain.prompts.example_selector.semantic_similarity import (
     MaxMarginalRelevanceExampleSelector,
     SemanticSimilarityExampleSelector,
 )
 
 __all__ = [
     "LengthBasedExampleSelector",
```

### Comparing `oplangchain-0.1.2/oplangchain/prompts/example_selector/base.py` & `oplangchain-0.1.3/oplangchain/prompts/example_selector/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/example_selector/length_based.py` & `oplangchain-0.1.3/oplangchain/prompts/example_selector/length_based.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/example_selector/ngram_overlap.py` & `oplangchain-0.1.3/oplangchain/prompts/example_selector/ngram_overlap.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/example_selector/semantic_similarity.py` & `oplangchain-0.1.3/oplangchain/prompts/example_selector/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/few_shot.py` & `oplangchain-0.1.3/oplangchain/prompts/few_shot.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/few_shot_with_templates.py` & `oplangchain-0.1.3/oplangchain/prompts/few_shot_with_templates.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/loading.py` & `oplangchain-0.1.3/oplangchain/prompts/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/pipeline.py` & `oplangchain-0.1.3/oplangchain/prompts/pipeline.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/prompts/prompt.py` & `oplangchain-0.1.3/oplangchain/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/__init__.py` & `oplangchain-0.1.3/oplangchain/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/arxiv.py` & `oplangchain-0.1.3/oplangchain/retrievers/arxiv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/azure_cognitive_search.py` & `oplangchain-0.1.3/oplangchain/retrievers/azure_cognitive_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/bm25.py` & `oplangchain-0.1.3/oplangchain/retrievers/bm25.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/chaindesk.py` & `oplangchain-0.1.3/oplangchain/retrievers/chaindesk.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/chatgpt_plugin_retriever.py` & `oplangchain-0.1.3/oplangchain/retrievers/chatgpt_plugin_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/contextual_compression.py` & `oplangchain-0.1.3/oplangchain/retrievers/contextual_compression.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/databerry.py` & `oplangchain-0.1.3/oplangchain/retrievers/databerry.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/docarray.py` & `oplangchain-0.1.3/oplangchain/retrievers/docarray.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/document_compressors/__init__.py` & `oplangchain-0.1.3/oplangchain/retrievers/document_compressors/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/document_compressors/base.py` & `oplangchain-0.1.3/oplangchain/retrievers/document_compressors/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/document_compressors/chain_extract.py` & `oplangchain-0.1.3/oplangchain/retrievers/document_compressors/chain_extract.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/document_compressors/chain_filter.py` & `oplangchain-0.1.3/oplangchain/retrievers/document_compressors/chain_filter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/document_compressors/cohere_rerank.py` & `oplangchain-0.1.3/oplangchain/retrievers/document_compressors/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/document_compressors/embeddings_filter.py` & `oplangchain-0.1.3/oplangchain/retrievers/document_compressors/embeddings_filter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/elastic_search_bm25.py` & `oplangchain-0.1.3/oplangchain/retrievers/elastic_search_bm25.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/ensemble.py` & `oplangchain-0.1.3/oplangchain/retrievers/ensemble.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/google_cloud_enterprise_search.py` & `oplangchain-0.1.3/oplangchain/retrievers/google_cloud_enterprise_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/kendra.py` & `oplangchain-0.1.3/oplangchain/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/knn.py` & `oplangchain-0.1.3/oplangchain/retrievers/knn.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/llama_index.py` & `oplangchain-0.1.3/oplangchain/retrievers/llama_index.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/merger_retriever.py` & `oplangchain-0.1.3/oplangchain/retrievers/merger_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/metal.py` & `oplangchain-0.1.3/oplangchain/retrievers/metal.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/milvus.py` & `oplangchain-0.1.3/oplangchain/retrievers/milvus.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/multi_query.py` & `oplangchain-0.1.3/oplangchain/retrievers/multi_query.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/pinecone_hybrid_search.py` & `oplangchain-0.1.3/oplangchain/retrievers/pinecone_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/pubmed.py` & `oplangchain-0.1.3/oplangchain/retrievers/pubmed.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/re_phraser.py` & `oplangchain-0.1.3/oplangchain/retrievers/re_phraser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/remote_retriever.py` & `oplangchain-0.1.3/oplangchain/retrievers/remote_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/self_query/base.py` & `oplangchain-0.1.3/oplangchain/retrievers/self_query/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/self_query/chroma.py` & `oplangchain-0.1.3/oplangchain/retrievers/self_query/chroma.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/self_query/deeplake.py` & `oplangchain-0.1.3/oplangchain/retrievers/self_query/deeplake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/self_query/myscale.py` & `oplangchain-0.1.3/oplangchain/retrievers/self_query/myscale.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/self_query/pinecone.py` & `oplangchain-0.1.3/oplangchain/retrievers/self_query/pinecone.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/self_query/qdrant.py` & `oplangchain-0.1.3/oplangchain/retrievers/self_query/qdrant.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/self_query/weaviate.py` & `oplangchain-0.1.3/oplangchain/retrievers/self_query/weaviate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/svm.py` & `oplangchain-0.1.3/oplangchain/retrievers/svm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/tfidf.py` & `oplangchain-0.1.3/oplangchain/retrievers/tfidf.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/time_weighted_retriever.py` & `oplangchain-0.1.3/oplangchain/retrievers/time_weighted_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/vespa_retriever.py` & `oplangchain-0.1.3/oplangchain/retrievers/vespa_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/weaviate_hybrid_search.py` & `oplangchain-0.1.3/oplangchain/retrievers/weaviate_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/web_research.py` & `oplangchain-0.1.3/oplangchain/retrievers/web_research.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/wikipedia.py` & `oplangchain-0.1.3/oplangchain/retrievers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/zep.py` & `oplangchain-0.1.3/oplangchain/retrievers/zep.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/retrievers/zilliz.py` & `oplangchain-0.1.3/oplangchain/retrievers/zilliz.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/__init__.py` & `oplangchain-0.1.3/oplangchain/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/agent.py` & `oplangchain-0.1.3/oplangchain/schema/agent.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/document.py` & `oplangchain-0.1.3/oplangchain/schema/document.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/language_model.py` & `oplangchain-0.1.3/oplangchain/schema/language_model.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/memory.py` & `oplangchain-0.1.3/oplangchain/schema/memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/messages.py` & `oplangchain-0.1.3/oplangchain/schema/messages.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/output.py` & `oplangchain-0.1.3/oplangchain/schema/output.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/output_parser.py` & `oplangchain-0.1.3/oplangchain/schema/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/prompt.py` & `oplangchain-0.1.3/oplangchain/schema/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/prompt_template.py` & `oplangchain-0.1.3/oplangchain/schema/prompt_template.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/retriever.py` & `oplangchain-0.1.3/oplangchain/schema/retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/schema/runnable.py` & `oplangchain-0.1.3/oplangchain/schema/runnable.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/server.py` & `oplangchain-0.1.3/oplangchain/server.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/smith/__init__.py` & `oplangchain-0.1.3/oplangchain/smith/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/smith/evaluation/__init__.py` & `oplangchain-0.1.3/oplangchain/smith/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/smith/evaluation/config.py` & `oplangchain-0.1.3/oplangchain/smith/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/smith/evaluation/runner_utils.py` & `oplangchain-0.1.3/oplangchain/smith/evaluation/runner_utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/smith/evaluation/string_run_evaluator.py` & `oplangchain-0.1.3/oplangchain/smith/evaluation/string_run_evaluator.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/text_splitter.py` & `oplangchain-0.1.3/oplangchain/text_splitter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/__init__.py` & `oplangchain-0.1.3/oplangchain/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     AzureCogsSpeech2TextTool,
     AzureCogsText2SpeechTool,
 )
 from oplangchain.tools.base import BaseTool, StructuredTool, Tool, tool
 from oplangchain.tools.bing_search.tool import BingSearchResults, BingSearchRun
 from oplangchain.tools.brave_search.tool import BraveSearch
 from oplangchain.tools.convert_to_openai import format_tool_to_openai_function
-from oplangchain.tools.ddg_search.tool import DuckDuckGoSearchResults, DuckDuckGoSearchRun
+from oplangchain.tools.ddg_search.tool import (
+    DuckDuckGoSearchResults,
+    DuckDuckGoSearchRun,
+)
 from oplangchain.tools.file_management import (
     CopyFileTool,
     DeleteFileTool,
     FileSearchTool,
     ListDirectoryTool,
     MoveFileTool,
     ReadFileTool,
```

### Comparing `oplangchain-0.1.2/oplangchain/tools/amadeus/closest_airport.py` & `oplangchain-0.1.3/oplangchain/tools/amadeus/closest_airport.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/amadeus/flight_search.py` & `oplangchain-0.1.3/oplangchain/tools/amadeus/flight_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/amadeus/utils.py` & `oplangchain-0.1.3/oplangchain/tools/amadeus/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/arxiv/tool.py` & `oplangchain-0.1.3/oplangchain/tools/arxiv/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/__init__.py` & `oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/form_recognizer.py` & `oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/image_analysis.py` & `oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/image_analysis.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/speech2text.py` & `oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/speech2text.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/text2speech.py` & `oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/text2speech.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/azure_cognitive_services/utils.py` & `oplangchain-0.1.3/oplangchain/tools/azure_cognitive_services/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/base.py` & `oplangchain-0.1.3/oplangchain/tools/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/bing_search/tool.py` & `oplangchain-0.1.3/oplangchain/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/brave_search/tool.py` & `oplangchain-0.1.3/oplangchain/tools/brave_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/convert_to_openai.py` & `oplangchain-0.1.3/oplangchain/tools/convert_to_openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/dataforseo_api_search/tool.py` & `oplangchain-0.1.3/oplangchain/tools/dataforseo_api_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/ddg_search/tool.py` & `oplangchain-0.1.3/oplangchain/tools/ddg_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/__init__.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/copy.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/copy.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/delete.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/delete.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/file_search.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/file_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/list_dir.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/list_dir.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/move.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/move.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/read.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/read.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/utils.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/file_management/write.py` & `oplangchain-0.1.3/oplangchain/tools/file_management/write.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/github/prompt.py` & `oplangchain-0.1.3/oplangchain/tools/github/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/github/tool.py` & `oplangchain-0.1.3/oplangchain/tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/gmail/__init__.py` & `oplangchain-0.1.3/oplangchain/tools/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/gmail/base.py` & `oplangchain-0.1.3/oplangchain/tools/gmail/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/gmail/create_draft.py` & `oplangchain-0.1.3/oplangchain/tools/gmail/create_draft.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/gmail/get_message.py` & `oplangchain-0.1.3/oplangchain/tools/gmail/get_message.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/gmail/get_thread.py` & `oplangchain-0.1.3/oplangchain/tools/gmail/get_thread.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/gmail/search.py` & `oplangchain-0.1.3/oplangchain/tools/gmail/search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/gmail/send_message.py` & `oplangchain-0.1.3/oplangchain/tools/gmail/send_message.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/gmail/utils.py` & `oplangchain-0.1.3/oplangchain/tools/gmail/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/golden_query/tool.py` & `oplangchain-0.1.3/oplangchain/tools/golden_query/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/google_places/tool.py` & `oplangchain-0.1.3/oplangchain/tools/google_places/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/google_search/tool.py` & `oplangchain-0.1.3/oplangchain/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/google_serper/tool.py` & `oplangchain-0.1.3/oplangchain/tools/google_serper/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/graphql/tool.py` & `oplangchain-0.1.3/oplangchain/tools/graphql/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/human/tool.py` & `oplangchain-0.1.3/oplangchain/tools/human/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/ifttt.py` & `oplangchain-0.1.3/oplangchain/tools/ifttt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/jira/prompt.py` & `oplangchain-0.1.3/oplangchain/tools/jira/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/jira/tool.py` & `oplangchain-0.1.3/oplangchain/tools/jira/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/json/tool.py` & `oplangchain-0.1.3/oplangchain/tools/json/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/metaphor_search/tool.py` & `oplangchain-0.1.3/oplangchain/tools/metaphor_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/multion/create_session.py` & `oplangchain-0.1.3/oplangchain/tools/multion/create_session.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/multion/update_session.py` & `oplangchain-0.1.3/oplangchain/tools/multion/update_session.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/nuclia/tool.py` & `oplangchain-0.1.3/oplangchain/tools/nuclia/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/office365/__init__.py` & `oplangchain-0.1.3/oplangchain/tools/office365/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/office365/create_draft_message.py` & `oplangchain-0.1.3/oplangchain/tools/office365/create_draft_message.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/office365/events_search.py` & `oplangchain-0.1.3/oplangchain/tools/office365/events_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/office365/messages_search.py` & `oplangchain-0.1.3/oplangchain/tools/office365/messages_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/office365/send_event.py` & `oplangchain-0.1.3/oplangchain/tools/office365/send_event.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/office365/send_message.py` & `oplangchain-0.1.3/oplangchain/tools/office365/send_message.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/office365/utils.py` & `oplangchain-0.1.3/oplangchain/tools/office365/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/openapi/utils/api_models.py` & `oplangchain-0.1.3/oplangchain/tools/openapi/utils/api_models.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/openweathermap/tool.py` & `oplangchain-0.1.3/oplangchain/tools/openweathermap/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/__init__.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/base.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/click.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/click.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/current_page.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/current_page.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/extract_hyperlinks.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/extract_hyperlinks.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/extract_text.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/extract_text.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/get_elements.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/get_elements.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/navigate.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/navigate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/navigate_back.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/navigate_back.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/playwright/utils.py` & `oplangchain-0.1.3/oplangchain/tools/playwright/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/plugin.py` & `oplangchain-0.1.3/oplangchain/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/powerbi/prompt.py` & `oplangchain-0.1.3/oplangchain/tools/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/powerbi/tool.py` & `oplangchain-0.1.3/oplangchain/tools/powerbi/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/pubmed/tool.py` & `oplangchain-0.1.3/oplangchain/tools/pubmed/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/python/tool.py` & `oplangchain-0.1.3/oplangchain/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/requests/tool.py` & `oplangchain-0.1.3/oplangchain/tools/requests/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/scenexplain/tool.py` & `oplangchain-0.1.3/oplangchain/tools/scenexplain/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/searx_search/tool.py` & `oplangchain-0.1.3/oplangchain/tools/searx_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/shell/tool.py` & `oplangchain-0.1.3/oplangchain/tools/shell/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/sleep/tool.py` & `oplangchain-0.1.3/oplangchain/tools/sleep/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/spark_sql/prompt.py` & `oplangchain-0.1.3/oplangchain/tools/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/spark_sql/tool.py` & `oplangchain-0.1.3/oplangchain/tools/spark_sql/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/sql_database/prompt.py` & `oplangchain-0.1.3/oplangchain/tools/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/sql_database/tool.py` & `oplangchain-0.1.3/oplangchain/tools/sql_database/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/steamship_image_generation/tool.py` & `oplangchain-0.1.3/oplangchain/tools/steamship_image_generation/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/steamship_image_generation/utils.py` & `oplangchain-0.1.3/oplangchain/tools/steamship_image_generation/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/vectorstore/tool.py` & `oplangchain-0.1.3/oplangchain/tools/vectorstore/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/wikipedia/tool.py` & `oplangchain-0.1.3/oplangchain/tools/wikipedia/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/wolfram_alpha/tool.py` & `oplangchain-0.1.3/oplangchain/tools/wolfram_alpha/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/youtube/search.py` & `oplangchain-0.1.3/oplangchain/tools/youtube/search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/zapier/prompt.py` & `oplangchain-0.1.3/oplangchain/tools/zapier/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/tools/zapier/tool.py` & `oplangchain-0.1.3/oplangchain/tools/zapier/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/__init__.py` & `oplangchain-0.1.3/oplangchain/utilities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 from oplangchain.utilities.max_compute import MaxComputeAPIWrapper
 from oplangchain.utilities.metaphor_search import MetaphorSearchAPIWrapper
 from oplangchain.utilities.openweathermap import OpenWeatherMapAPIWrapper
 from oplangchain.utilities.portkey import Portkey
 from oplangchain.utilities.powerbi import PowerBIDataset
 from oplangchain.utilities.pupmed import PubMedAPIWrapper
 from oplangchain.utilities.python import PythonREPL
-from oplangchain.utilities.requests import Requests, RequestsWrapper, TextRequestsWrapper
+from oplangchain.utilities.requests import (
+    Requests,
+    RequestsWrapper,
+    TextRequestsWrapper,
+)
 from oplangchain.utilities.scenexplain import SceneXplainAPIWrapper
 from oplangchain.utilities.searx_search import SearxSearchWrapper
 from oplangchain.utilities.serpapi import SerpAPIWrapper
 from oplangchain.utilities.spark_sql import SparkSQL
 from oplangchain.utilities.sql_database import SQLDatabase
 from oplangchain.utilities.twilio import TwilioAPIWrapper
 from oplangchain.utilities.wikipedia import WikipediaAPIWrapper
```

### Comparing `oplangchain-0.1.2/oplangchain/utilities/arxiv.py` & `oplangchain-0.1.3/oplangchain/utilities/arxiv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/awslambda.py` & `oplangchain-0.1.3/oplangchain/utilities/awslambda.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/bash.py` & `oplangchain-0.1.3/oplangchain/utilities/bash.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/bibtex.py` & `oplangchain-0.1.3/oplangchain/utilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/bing_search.py` & `oplangchain-0.1.3/oplangchain/utilities/bing_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/brave_search.py` & `oplangchain-0.1.3/oplangchain/utilities/brave_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/dataforseo_api_search.py` & `oplangchain-0.1.3/oplangchain/utilities/dataforseo_api_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/duckduckgo_search.py` & `oplangchain-0.1.3/oplangchain/utilities/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/github.py` & `oplangchain-0.1.3/oplangchain/utilities/github.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/golden_query.py` & `oplangchain-0.1.3/oplangchain/utilities/golden_query.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/google_places_api.py` & `oplangchain-0.1.3/oplangchain/utilities/google_places_api.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/google_search.py` & `oplangchain-0.1.3/oplangchain/utilities/google_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/google_serper.py` & `oplangchain-0.1.3/oplangchain/utilities/google_serper.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/graphql.py` & `oplangchain-0.1.3/oplangchain/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/jira.py` & `oplangchain-0.1.3/oplangchain/utilities/jira.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/loading.py` & `oplangchain-0.1.3/oplangchain/utilities/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/max_compute.py` & `oplangchain-0.1.3/oplangchain/utilities/max_compute.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/metaphor_search.py` & `oplangchain-0.1.3/oplangchain/utilities/metaphor_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/openapi.py` & `oplangchain-0.1.3/oplangchain/utilities/openapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     PathItem,
     Paths,
     Reference,
     RequestBody,
     Schema,
 )
 from pydantic import ValidationError
+from urllib.parse import urlparse
 
 logger = logging.getLogger(__name__)
 
 
 class HTTPVerb(str, Enum):
     """Enumerator of the HTTP verbs."""
 
@@ -194,20 +195,26 @@
 
     @classmethod
     def from_spec_dict(cls, spec_dict: dict) -> "OpenAPISpec":
         """Get an OpenAPI spec from a dict."""
         return cls.parse_obj(spec_dict)
 
     @classmethod
-    def from_text(cls, text: str) -> "OpenAPISpec":
+    def from_text(cls, text: str, openapi_url: str = "") -> "OpenAPISpec":
         """Get an OpenAPI spec from a text."""
         try:
             spec_dict = json.loads(text)
         except json.JSONDecodeError:
             spec_dict = yaml.safe_load(text)
+
+        if "servers" not in spec_dict and openapi_url:
+            parsed_url = urlparse(openapi_url)
+            root_url = f"{parsed_url.scheme}://{parsed_url.netloc}"
+            spec_dict["servers"] = [{"url": root_url}]
+
         return cls.from_spec_dict(spec_dict)
 
     @classmethod
     def from_file(cls, path: Union[str, Path]) -> "OpenAPISpec":
         """Get an OpenAPI spec from a file path."""
         path_ = path if isinstance(path, Path) else Path(path)
         if not path_.exists():
@@ -215,15 +222,15 @@
         with path_.open("r") as f:
             return cls.from_text(f.read())
 
     @classmethod
     def from_url(cls, url: str) -> "OpenAPISpec":
         """Get an OpenAPI spec from a URL."""
         response = requests.get(url)
-        return cls.from_text(response.text)
+        return cls.from_text(response.text, url)
 
     @property
     def base_url(self) -> str:
         """Get the base url."""
         return self.servers[0].url
 
     def get_methods_for_path(self, path: str) -> List[str]:
```

### Comparing `oplangchain-0.1.2/oplangchain/utilities/openweathermap.py` & `oplangchain-0.1.3/oplangchain/utilities/openweathermap.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/portkey.py` & `oplangchain-0.1.3/oplangchain/utilities/portkey.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/powerbi.py` & `oplangchain-0.1.3/oplangchain/utilities/powerbi.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/pupmed.py` & `oplangchain-0.1.3/oplangchain/utilities/pupmed.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/python.py` & `oplangchain-0.1.3/oplangchain/utilities/python.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/redis.py` & `oplangchain-0.1.3/oplangchain/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/requests.py` & `oplangchain-0.1.3/oplangchain/utilities/requests.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/scenexplain.py` & `oplangchain-0.1.3/oplangchain/utilities/scenexplain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/searx_search.py` & `oplangchain-0.1.3/oplangchain/utilities/searx_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/serpapi.py` & `oplangchain-0.1.3/oplangchain/utilities/serpapi.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/spark_sql.py` & `oplangchain-0.1.3/oplangchain/utilities/spark_sql.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/sql_database.py` & `oplangchain-0.1.3/oplangchain/utilities/sql_database.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/twilio.py` & `oplangchain-0.1.3/oplangchain/utilities/twilio.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/vertexai.py` & `oplangchain-0.1.3/oplangchain/utilities/vertexai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/wikipedia.py` & `oplangchain-0.1.3/oplangchain/utilities/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/wolfram_alpha.py` & `oplangchain-0.1.3/oplangchain/utilities/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utilities/zapier.py` & `oplangchain-0.1.3/oplangchain/utilities/zapier.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utils/__init__.py` & `oplangchain-0.1.3/oplangchain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utils/env.py` & `oplangchain-0.1.3/oplangchain/utils/env.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utils/formatting.py` & `oplangchain-0.1.3/oplangchain/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utils/input.py` & `oplangchain-0.1.3/oplangchain/utils/input.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utils/math.py` & `oplangchain-0.1.3/oplangchain/utils/math.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utils/strings.py` & `oplangchain-0.1.3/oplangchain/utils/strings.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/utils/utils.py` & `oplangchain-0.1.3/oplangchain/utils/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/__init__.py` & `oplangchain-0.1.3/oplangchain/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/_pgvector_data_models.py` & `oplangchain-0.1.3/oplangchain/vectorstores/_pgvector_data_models.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/alibabacloud_opensearch.py` & `oplangchain-0.1.3/oplangchain/vectorstores/alibabacloud_opensearch.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/analyticdb.py` & `oplangchain-0.1.3/oplangchain/vectorstores/analyticdb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/annoy.py` & `oplangchain-0.1.3/oplangchain/vectorstores/annoy.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/atlas.py` & `oplangchain-0.1.3/oplangchain/vectorstores/atlas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/awadb.py` & `oplangchain-0.1.3/oplangchain/vectorstores/awadb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/azuresearch.py` & `oplangchain-0.1.3/oplangchain/vectorstores/azuresearch.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/base.py` & `oplangchain-0.1.3/oplangchain/vectorstores/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/cassandra.py` & `oplangchain-0.1.3/oplangchain/vectorstores/cassandra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/chroma.py` & `oplangchain-0.1.3/oplangchain/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/clarifai.py` & `oplangchain-0.1.3/oplangchain/vectorstores/clarifai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/clickhouse.py` & `oplangchain-0.1.3/oplangchain/vectorstores/clickhouse.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/deeplake.py` & `oplangchain-0.1.3/oplangchain/vectorstores/deeplake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/docarray/base.py` & `oplangchain-0.1.3/oplangchain/vectorstores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/docarray/hnsw.py` & `oplangchain-0.1.3/oplangchain/vectorstores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/docarray/in_memory.py` & `oplangchain-0.1.3/oplangchain/vectorstores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/elastic_vector_search.py` & `oplangchain-0.1.3/oplangchain/vectorstores/elastic_vector_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/faiss.py` & `oplangchain-0.1.3/oplangchain/vectorstores/faiss.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/hologres.py` & `oplangchain-0.1.3/oplangchain/vectorstores/hologres.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/lancedb.py` & `oplangchain-0.1.3/oplangchain/vectorstores/lancedb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/marqo.py` & `oplangchain-0.1.3/oplangchain/vectorstores/marqo.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/matching_engine.py` & `oplangchain-0.1.3/oplangchain/vectorstores/matching_engine.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/meilisearch.py` & `oplangchain-0.1.3/oplangchain/vectorstores/meilisearch.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/milvus.py` & `oplangchain-0.1.3/oplangchain/vectorstores/milvus.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/mongodb_atlas.py` & `oplangchain-0.1.3/oplangchain/vectorstores/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/myscale.py` & `oplangchain-0.1.3/oplangchain/vectorstores/myscale.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/opensearch_vector_search.py` & `oplangchain-0.1.3/oplangchain/vectorstores/opensearch_vector_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/pgembedding.py` & `oplangchain-0.1.3/oplangchain/vectorstores/pgembedding.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/pgvector.py` & `oplangchain-0.1.3/oplangchain/vectorstores/pgvector.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/pinecone.py` & `oplangchain-0.1.3/oplangchain/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/qdrant.py` & `oplangchain-0.1.3/oplangchain/vectorstores/qdrant.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/redis.py` & `oplangchain-0.1.3/oplangchain/vectorstores/redis.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/rocksetdb.py` & `oplangchain-0.1.3/oplangchain/vectorstores/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/scann.py` & `oplangchain-0.1.3/oplangchain/vectorstores/scann.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/singlestoredb.py` & `oplangchain-0.1.3/oplangchain/vectorstores/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/sklearn.py` & `oplangchain-0.1.3/oplangchain/vectorstores/sklearn.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/starrocks.py` & `oplangchain-0.1.3/oplangchain/vectorstores/starrocks.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/supabase.py` & `oplangchain-0.1.3/oplangchain/vectorstores/supabase.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/tair.py` & `oplangchain-0.1.3/oplangchain/vectorstores/tair.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/tigris.py` & `oplangchain-0.1.3/oplangchain/vectorstores/tigris.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/typesense.py` & `oplangchain-0.1.3/oplangchain/vectorstores/typesense.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/utils.py` & `oplangchain-0.1.3/oplangchain/vectorstores/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/vectara.py` & `oplangchain-0.1.3/oplangchain/vectorstores/vectara.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/weaviate.py` & `oplangchain-0.1.3/oplangchain/vectorstores/weaviate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/oplangchain/vectorstores/zilliz.py` & `oplangchain-0.1.3/oplangchain/vectorstores/zilliz.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/pyproject.toml` & `oplangchain-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oplangchain"
-version = "0.1.2"
+version = "0.1.3"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/hwchase17/langchain"
 
 [tool.poetry.scripts]
```

### Comparing `oplangchain-0.1.2/README.md` & `oplangchain-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oplangchain-0.1.2/PKG-INFO` & `oplangchain-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oplangchain
-Version: 0.1.2
+Version: 0.1.3
 Summary: Building applications with LLMs through composability
 Home-page: https://www.github.com/hwchase17/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

