# Comparing `tmp/promptulate-1.9.0.tar.gz` & `tmp/promptulate-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptulate-1.9.0.tar", max compression
+gzip compressed data, was "promptulate-1.9.1.tar", max compression
```

## Comparing `promptulate-1.9.0.tar` & `promptulate-1.9.1.tar`

### file list

```diff
@@ -1,93 +1,92 @@
--rw-r--r--   0        0        0    11357 2023-11-09 05:03:16.922496 promptulate-1.9.0/LICENSE
--rw-r--r--   0        0        0     9013 2023-11-09 05:03:16.922496 promptulate-1.9.0/README.md
--rw-r--r--   0        0        0     1211 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/__init__.py
--rw-r--r--   0        0        0      210 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/auto_agent.py
--rw-r--r--   0        0        0     1768 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/base.py
--rw-r--r--   0        0        0       83 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/tool_agent/__init__.py
--rw-r--r--   0        0        0     6400 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/tool_agent/agent.py
--rw-r--r--   0        0        0     1523 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/tool_agent/prompt.py
--rw-r--r--   0        0        0        0 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/web_agent/__init__.py
--rw-r--r--   0        0        0     2392 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/web_agent/agent.py
--rw-r--r--   0        0        0      727 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/agents/web_agent/prompt.py
--rw-r--r--   0        0        0     2824 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/chat.py
--rw-r--r--   0        0        0        0 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/client/__init__.py
--rw-r--r--   0        0        0     5696 2023-11-09 05:03:16.930496 promptulate-1.9.0/promptulate/client/chat.py
--rw-r--r--   0        0        0     6519 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/config.py
--rw-r--r--   0        0        0      846 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/frameworks/__init__.py
--rw-r--r--   0        0        0      859 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/frameworks/conversation/__init__.py
--rw-r--r--   0        0        0     5488 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/frameworks/conversation/conversation.py
--rw-r--r--   0        0        0     1737 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/frameworks/prompt.py
--rw-r--r--   0        0        0     1116 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/frameworks/schema.py
--rw-r--r--   0        0        0       83 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/hook/__init__.py
--rw-r--r--   0        0        0     9317 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/hook/base.py
--rw-r--r--   0        0        0     1727 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/hook/stdout_hook.py
--rw-r--r--   0        0        0      968 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/llms/__init__.py
--rw-r--r--   0        0        0     2122 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/llms/base.py
--rw-r--r--   0        0        0        0 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/llms/erniebot/__init__.py
--rw-r--r--   0        0        0     3376 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/llms/erniebot/erniebot.py
--rw-r--r--   0        0        0       59 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/llms/erniebot/schema.py
--rw-r--r--   0        0        0       98 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/llms/openai/__init__.py
--rw-r--r--   0        0        0    10220 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/llms/openai/openai.py
--rw-r--r--   0        0        0      228 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/llms/openai/schema.py
--rw-r--r--   0        0        0      912 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/memory/__init__.py
--rw-r--r--   0        0        0     2305 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/memory/base.py
--rw-r--r--   0        0        0     2072 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/memory/buffer.py
--rw-r--r--   0        0        0     2230 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/memory/file.py
--rw-r--r--   0        0        0      213 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/output_formatter/__init__.py
--rw-r--r--   0        0        0     2247 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/output_formatter/formatter.py
--rw-r--r--   0        0        0      501 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/output_formatter/prompt.py
--rw-r--r--   0        0        0      894 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/preset_roles/__init__.py
--rw-r--r--   0        0        0     2717 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/preset_roles/prompt.py
--rw-r--r--   0        0        0     5707 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/preset_roles/roles.py
--rw-r--r--   0        0        0     1033 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/provider/__init__.py
--rw-r--r--   0        0        0      655 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/provider/base.py
--rw-r--r--   0        0        0     4687 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/provider/mixins.py
--rw-r--r--   0        0        0     5175 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/schema.py
--rw-r--r--   0        0        0     1860 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tips.py
--rw-r--r--   0        0        0     1394 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/__init__.py
--rw-r--r--   0        0        0      276 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/arxiv/__init__.py
--rw-r--r--   0        0        0     4753 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/arxiv/api_wrapper.py
--rw-r--r--   0        0        0      387 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/arxiv/toolkit.py
--rw-r--r--   0        0        0     9567 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/arxiv/tools.py
--rw-r--r--   0        0        0     4357 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/base.py
--rw-r--r--   0        0        0      155 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/duckduckgo/__init__.py
--rw-r--r--   0        0        0     3376 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/duckduckgo/api_wrapper.py
--rw-r--r--   0        0        0     2643 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/duckduckgo/tools.py
--rw-r--r--   0        0        0        0 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/huggingface/__init__.py
--rw-r--r--   0        0        0      604 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/huggingface/tools.py
--rw-r--r--   0        0        0      102 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/human_feedback/__init__.py
--rw-r--r--   0        0        0     1191 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/human_feedback/tools.py
--rw-r--r--   0        0        0       94 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/iot_swith_mqtt/__init__.py
--rw-r--r--   0        0        0      146 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/iot_swith_mqtt/api_wrapper.py
--rw-r--r--   0        0        0      474 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/iot_swith_mqtt/prompt.py
--rw-r--r--   0        0        0     2678 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/iot_swith_mqtt/tools.py
--rw-r--r--   0        0        0        0 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/langchain/__init__.py
--rw-r--r--   0        0        0      613 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/langchain/tools.py
--rw-r--r--   0        0        0     1167 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/manager.py
--rw-r--r--   0        0        0       78 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/math/__init__.py
--rw-r--r--   0        0        0      814 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/math/prompt.py
--rw-r--r--   0        0        0     2428 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/math/tools.py
--rw-r--r--   0        0        0       91 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/paper/__init__.py
--rw-r--r--   0        0        0     7858 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/paper/tools.py
--rw-r--r--   0        0        0       93 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/python_repl/__init__.py
--rw-r--r--   0        0        0      803 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/python_repl/api_wrapper.py
--rw-r--r--   0        0        0      704 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/python_repl/tools.py
--rw-r--r--   0        0        0      272 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/semantic_scholar/__init__.py
--rw-r--r--   0        0        0     7222 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/semantic_scholar/api_wrapper.py
--rw-r--r--   0        0        0     2276 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/semantic_scholar/tools.py
--rw-r--r--   0        0        0       77 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/shell/__init__.py
--rw-r--r--   0        0        0      630 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/shell/api_wrapper.py
--rw-r--r--   0        0        0      752 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/shell/tools.py
--rw-r--r--   0        0        0       76 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/sleep/__init__.py
--rw-r--r--   0        0        0      524 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/tools/sleep/tool.py
--rw-r--r--   0        0        0     1358 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/utils/__init__.py
--rw-r--r--   0        0        0      564 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/utils/color_print.py
--rw-r--r--   0        0        0     4293 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/utils/core_utils.py
--rw-r--r--   0        0        0     1775 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/utils/logger.py
--rw-r--r--   0        0        0     5461 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/utils/openai_key_pool.py
--rw-r--r--   0        0        0     1880 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/utils/proxy.py
--rw-r--r--   0        0        0     1306 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/utils/singleton.py
--rw-r--r--   0        0        0      703 2023-11-09 05:03:16.934496 promptulate-1.9.0/promptulate/utils/string_template.py
--rw-r--r--   0        0        0     1684 2023-11-09 05:03:16.934496 promptulate-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    10097 1970-01-01 00:00:00.000000 promptulate-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-19 06:26:24.372632 promptulate-1.9.1/LICENSE
+-rw-r--r--   0        0        0     9013 2023-11-19 06:26:24.372632 promptulate-1.9.1/README.md
+-rw-r--r--   0        0        0     1211 2023-11-19 06:26:24.380632 promptulate-1.9.1/promptulate/__init__.py
+-rw-r--r--   0        0        0      210 2023-11-19 06:26:24.380632 promptulate-1.9.1/promptulate/agents/__init__.py
+-rw-r--r--   0        0        0     1768 2023-11-19 06:26:24.380632 promptulate-1.9.1/promptulate/agents/base.py
+-rw-r--r--   0        0        0       83 2023-11-19 06:26:24.380632 promptulate-1.9.1/promptulate/agents/tool_agent/__init__.py
+-rw-r--r--   0        0        0     6400 2023-11-19 06:26:24.380632 promptulate-1.9.1/promptulate/agents/tool_agent/agent.py
+-rw-r--r--   0        0        0     1904 2023-11-19 06:26:24.380632 promptulate-1.9.1/promptulate/agents/tool_agent/prompt.py
+-rw-r--r--   0        0        0        0 2023-11-19 06:26:24.380632 promptulate-1.9.1/promptulate/agents/web_agent/__init__.py
+-rw-r--r--   0        0        0     2541 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/agents/web_agent/agent.py
+-rw-r--r--   0        0        0      735 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/agents/web_agent/prompt.py
+-rw-r--r--   0        0        0     2824 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/chat.py
+-rw-r--r--   0        0        0        0 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/client/__init__.py
+-rw-r--r--   0        0        0     5678 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/client/chat.py
+-rw-r--r--   0        0        0     6494 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/config.py
+-rw-r--r--   0        0        0      846 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/frameworks/__init__.py
+-rw-r--r--   0        0        0      859 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/frameworks/conversation/__init__.py
+-rw-r--r--   0        0        0     5488 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/frameworks/conversation/conversation.py
+-rw-r--r--   0        0        0     1737 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/frameworks/prompt.py
+-rw-r--r--   0        0        0     1116 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/frameworks/schema.py
+-rw-r--r--   0        0        0       83 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/hook/__init__.py
+-rw-r--r--   0        0        0     9317 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/hook/base.py
+-rw-r--r--   0        0        0     1727 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/hook/stdout_hook.py
+-rw-r--r--   0        0        0      968 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/llms/__init__.py
+-rw-r--r--   0        0        0     2122 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/llms/base.py
+-rw-r--r--   0        0        0        0 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/llms/erniebot/__init__.py
+-rw-r--r--   0        0        0     3292 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/llms/erniebot/erniebot.py
+-rw-r--r--   0        0        0       59 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/llms/erniebot/schema.py
+-rw-r--r--   0        0        0       98 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/llms/openai/__init__.py
+-rw-r--r--   0        0        0    10220 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/llms/openai/openai.py
+-rw-r--r--   0        0        0      228 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/llms/openai/schema.py
+-rw-r--r--   0        0        0      912 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/memory/__init__.py
+-rw-r--r--   0        0        0     2305 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/memory/base.py
+-rw-r--r--   0        0        0     2072 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/memory/buffer.py
+-rw-r--r--   0        0        0     2230 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/memory/file.py
+-rw-r--r--   0        0        0      213 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/output_formatter/__init__.py
+-rw-r--r--   0        0        0     2247 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/output_formatter/formatter.py
+-rw-r--r--   0        0        0      501 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/output_formatter/prompt.py
+-rw-r--r--   0        0        0      894 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/preset_roles/__init__.py
+-rw-r--r--   0        0        0     2717 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/preset_roles/prompt.py
+-rw-r--r--   0        0        0     5707 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/preset_roles/roles.py
+-rw-r--r--   0        0        0     1033 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/provider/__init__.py
+-rw-r--r--   0        0        0      655 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/provider/base.py
+-rw-r--r--   0        0        0     4687 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/provider/mixins.py
+-rw-r--r--   0        0        0     5175 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/schema.py
+-rw-r--r--   0        0        0     1860 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tips.py
+-rw-r--r--   0        0        0     1394 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/__init__.py
+-rw-r--r--   0        0        0      276 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0     4753 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/arxiv/api_wrapper.py
+-rw-r--r--   0        0        0      387 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/arxiv/toolkit.py
+-rw-r--r--   0        0        0     9567 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/arxiv/tools.py
+-rw-r--r--   0        0        0     4357 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/base.py
+-rw-r--r--   0        0        0      155 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/duckduckgo/__init__.py
+-rw-r--r--   0        0        0     3376 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/duckduckgo/api_wrapper.py
+-rw-r--r--   0        0        0     2643 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/duckduckgo/tools.py
+-rw-r--r--   0        0        0        0 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/huggingface/__init__.py
+-rw-r--r--   0        0        0      604 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/huggingface/tools.py
+-rw-r--r--   0        0        0      102 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/human_feedback/__init__.py
+-rw-r--r--   0        0        0     1191 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/human_feedback/tools.py
+-rw-r--r--   0        0        0       94 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/iot_swith_mqtt/__init__.py
+-rw-r--r--   0        0        0      146 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/iot_swith_mqtt/api_wrapper.py
+-rw-r--r--   0        0        0      474 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/iot_swith_mqtt/prompt.py
+-rw-r--r--   0        0        0     2678 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/iot_swith_mqtt/tools.py
+-rw-r--r--   0        0        0        0 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/langchain/__init__.py
+-rw-r--r--   0        0        0      613 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/langchain/tools.py
+-rw-r--r--   0        0        0     1167 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/manager.py
+-rw-r--r--   0        0        0       78 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/math/__init__.py
+-rw-r--r--   0        0        0      814 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/math/prompt.py
+-rw-r--r--   0        0        0     2428 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/math/tools.py
+-rw-r--r--   0        0        0       91 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/paper/__init__.py
+-rw-r--r--   0        0        0     7858 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/paper/tools.py
+-rw-r--r--   0        0        0       93 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/python_repl/__init__.py
+-rw-r--r--   0        0        0      803 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/python_repl/api_wrapper.py
+-rw-r--r--   0        0        0      704 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/python_repl/tools.py
+-rw-r--r--   0        0        0      272 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/semantic_scholar/__init__.py
+-rw-r--r--   0        0        0     7222 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/semantic_scholar/api_wrapper.py
+-rw-r--r--   0        0        0     2276 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/semantic_scholar/tools.py
+-rw-r--r--   0        0        0       77 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/shell/__init__.py
+-rw-r--r--   0        0        0      630 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/shell/api_wrapper.py
+-rw-r--r--   0        0        0      752 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/shell/tools.py
+-rw-r--r--   0        0        0       76 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/sleep/__init__.py
+-rw-r--r--   0        0        0      524 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/tools/sleep/tool.py
+-rw-r--r--   0        0        0     1358 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/utils/__init__.py
+-rw-r--r--   0        0        0      564 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/utils/color_print.py
+-rw-r--r--   0        0        0     4293 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/utils/core_utils.py
+-rw-r--r--   0        0        0     1775 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/utils/logger.py
+-rw-r--r--   0        0        0     5461 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/utils/openai_key_pool.py
+-rw-r--r--   0        0        0     1880 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/utils/proxy.py
+-rw-r--r--   0        0        0     1306 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/utils/singleton.py
+-rw-r--r--   0        0        0      703 2023-11-19 06:26:24.384632 promptulate-1.9.1/promptulate/utils/string_template.py
+-rw-r--r--   0        0        0     1685 2023-11-19 06:26:24.384632 promptulate-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    10098 1970-01-01 00:00:00.000000 promptulate-1.9.1/PKG-INFO
```

### Comparing `promptulate-1.9.0/LICENSE` & `promptulate-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/README.md` & `promptulate-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/__init__.py` & `promptulate-1.9.1/promptulate/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/agents/base.py` & `promptulate-1.9.1/promptulate/agents/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/agents/tool_agent/agent.py` & `promptulate-1.9.1/promptulate/agents/tool_agent/agent.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/agents/tool_agent/prompt.py` & `promptulate-1.9.1/promptulate/agents/tool_agent/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 REACT_ZERO_SHOT_PROMPT = """
 Answer the following questions as best you can. You have access to the following tools:
-
 {tool_descriptions}
-Use the following format:
+
+Your output format if as follows:
 Question: the input question you must answer
 Thought: you should always think about what to do
 Action: the action to take, must be one of [{tool_names}]
 Action Input: the input to the action
 Observation: the result of the action
-... (this Thought/Action/Action Input/Observation can repeat N times)
+... (this behavior of Thought/Action/Action Input/Observation can repeat N times)
 Thought: I now know the final answer
 Final Answer: the final answer to the original input question
 
+**Attention**
+- let's take a deep breathe and think it step by step
+- You can only output one behavior in one step
+- Minimize the number of websearch, but ensure that all necessary online searches are aimed at answering user questions.
+- Your final answer output language should be consistent with the language used by the user. Middle step output is English.
+
 Begin!
 
 Question: {prompt}
 Thought:
 """
 PREFIX_TEMPLATE = """You are a {agent_identity}, named {agent_name}, your goal is {agent_goal}, and the constraint is {agent_constraints}. """
```

### Comparing `promptulate-1.9.0/promptulate/agents/web_agent/agent.py` & `promptulate-1.9.1/promptulate/agents/web_agent/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,32 +42,38 @@
             return self.llm(prompt)
 
         self.conversation_prompt = _build_system_prompt(prompt)
         iterations = 0
 
         # Loop search until find the answer
         while True:
-            answer: str = self.llm(self.conversation_prompt, stop=self.stop_sequences)
+            llm_output: str = self.llm(
+                self.conversation_prompt, stop=self.stop_sequences
+            )
             logger.info(
                 f"[pne] tool agent <{iterations}> current prompt: {self.conversation_prompt}"
             )
 
-            if "Final Answer" in answer:
-                return answer.split("Final Answer:")[-1]
+            if "Final Answer" in llm_output:
+                return llm_output.split("Final Answer:")[-1]
+
+            self.conversation_prompt += llm_output
 
-            query_words: str = self._find_query_words(answer)
+            # get keywords and query by websearch
+            query_words: str = self._find_query_words(llm_output)
             Hook.call_hook(
                 HookTable.ON_AGENT_ACTION,
                 self,
                 action="websearch",
                 action_input=query_words,
             )
 
             query_result: str = self.websearch.run(query_words)
             Hook.call_hook(
                 HookTable.ON_AGENT_OBSERVATION, self, observation=query_result
             )
+
             self.conversation_prompt += f"Observation: {query_result}\nThought: "
             iterations += 1
 
     def _find_query_words(self, answer: str) -> str:
         return answer.split("Query:")[-1].replace('"', "")
```

### Comparing `promptulate-1.9.0/promptulate/agents/web_agent/prompt.py` & `promptulate-1.9.1/promptulate/agents/web_agent/prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from promptulate.utils.string_template import StringTemplate
 
 SYSTEM_PROMPT = """
 Answer the following questions as best you can. You have access use web search.
 After the user enters a question, you need to generate keywords for web search,
 and then summarize until you think you can answer the user's answer.
 
-Use the following format:
+Your output format is as follows:
 Question: the input question you must answer
 Thought: The next you should do
 Query: web search query words
 Observation: the result of query
 ... (this Thought/Query/Observation can repeat N times) 
 Thought: I know the final answer
 Final Answer: the final answer to the original input question
```

### Comparing `promptulate-1.9.0/promptulate/chat.py` & `promptulate-1.9.1/promptulate/chat.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/client/chat.py` & `promptulate-1.9.1/promptulate/client/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,34 +37,25 @@
     SleepTool,
 )
 from promptulate.tools.shell import ShellTool
 from promptulate.utils.color_print import print_text
 from promptulate.utils.proxy import set_proxy_mode
 
 CFG = Config()
-MODEL_MAPPING = {"OpenAI": ChatOpenAI, "ErnieBot": ErnieBot}
 TOOL_MAPPING = {
     "Calculator": Calculator,
     "WebSearch": DuckDuckGoTool,
     "Python Script Executor": PythonREPLTool,
     "Arxiv Query": ArxivQueryTool,
     "Sleep": SleepTool,
     "Shell Executor": ShellTool,
     "HumanFeedBackTool": HumanFeedBackTool,
 }
 
 
-def check_key(model_type: str):
-    model_key_mapping = {
-        "OpenAI": CFG.get_openai_api_key,
-        "ErnieBot": CFG.get_ernie_api_key,
-    }
-    model_key_mapping[model_type]()
-
-
 def get_user_input() -> Optional[str]:
     marker = (
         "# You input are here (please delete this line)\n"
         "You should save it and close the notebook after writing the prompt. (please delete this line)\n"
         "Reply 'exit' to exit the chat.\n"
     )
     message = click.edit(marker)
@@ -166,20 +157,29 @@
     ).ask()
 
     if terminal_mode == "exit":
         exit(0)
 
     model = questionary.select(
         "Choose a llm model:",
-        choices=list(MODEL_MAPPING.keys()),
+        choices=[
+            "gpt-3.5-turbo",
+            "gpt-4",
+            "gpt-3.5-turbo-16k",
+            "ernie-bot-turbo",
+            "ernie-bot",
+        ],
     ).ask()
 
-    check_key(model)
+    # init model
+    if "gpt" in model:
+        llm = ChatOpenAI(model=model, temperature=0.0)
+    elif "ernie" in model:
+        llm = ErnieBot(model=model, temperature=0.0)
 
-    llm = MODEL_MAPPING[model](temperature=0.2)
     if terminal_mode == "Simple Chat":
         simple_chat(llm)
     elif terminal_mode == "Agent Chat":
         str_tools = questionary.checkbox(
             "Choose tools you want:", choices=list(TOOL_MAPPING.keys())
         ).ask()
         tools = []
```

### Comparing `promptulate-1.9.0/promptulate/config.py` & `promptulate-1.9.1/promptulate/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 def turn_off_stdout_hook():
     Config().turn_off_stdout_hook()
 
 
 class Config(metaclass=Singleton):
     def __init__(self):
-        logger.info(f"[pne config] Config initialization")
+        logger.info("[pne config] Config initialization")
         self.enable_cache: bool = True
         self._proxy_mode: str = PROXY_MODE[0]
         self._proxies: Optional[dict] = None
 
         self.openai_chat_api_url = "https://api.openai.com/v1/chat/completions"
         self.openai_completion_api_url = "https://api.openai.com/v1/completions"
         self.openai_proxy_url = "https://chatgpt-api.shn.hk/v1/"  # FREE API
@@ -67,35 +67,33 @@
             StdOutHook.registry_stdout_hooks()
 
     def turn_off_stdout_hook(self):
         if self.enable_stdout_hook:
             self.enable_stdout_hook = False
             StdOutHook.unregister_stdout_hooks()
 
-    @property
-    def openai_api_key(self):
-        """This attribution has deprecated to use. Using `get_openai_api_key`"""
+    def get_openai_api_key(self, model: str = "gpt-3.5-turbo") -> str:
+        """Get openai key from KeyPool and environment variable. The priority of obtaining the key:
+        environment variable, cache of OpenAIKeyPool, cache of OEPNAI_API_KEY,"""
         if "OPENAI_API_KEY" in os.environ.keys():
             if self.enable_cache:
                 get_cache()["OPENAI_API_KEY"] = os.getenv("OPENAI_API_KEY")
             return os.getenv("OPENAI_API_KEY")
-        if self.enable_cache and "OPENAI_API_KEY" in get_cache():
-            return get_cache()["OPENAI_API_KEY"]
-        raise ValueError("OPENAI API key is not provided. Please set your key.")
 
-    def get_openai_api_key(self, model: str) -> str:
-        """Get openai key from KeyPool and environ"""
         if self.enable_cache:
             openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
             key = openai_key_pool.get(model)
             if key:
                 return key
-        return self.openai_api_key
 
-    @property
+        if self.enable_cache and "OPENAI_API_KEY" in get_cache():
+            return get_cache()["OPENAI_API_KEY"]
+
+        raise ValueError("OPENAI API key is not provided. Please set your key.")
+
     def get_ernie_api_key(self) -> str:
         if "ERNIE_API_KEY" in os.environ.keys():
             if self.enable_cache:
                 get_cache()["ERNIE_API_KEY"] = os.getenv("ERNIE_API_KEY")
             return os.getenv("ERNIE_API_KEY")
         if self.enable_cache and "ERNIE_API_KEY" in get_cache():
             return get_cache()["ERNIE_API_KEY"]
@@ -111,15 +109,15 @@
             return get_cache()["ERNIE_API_SECRET"]
         raise ValueError("ERNIE_API_SECRET is not provided. Please set your secret.")
 
     def get_ernie_token(self) -> str:
         url = self.ernie_bot_token_url
         params = {
             "grant_type": "client_credentials",
-            "client_id": self.get_ernie_api_key,
+            "client_id": self.get_ernie_api_key(),
             "client_secret": self.get_ernie_api_secret,
         }
         return str(requests.post(url, params=params).json().get("access_token"))
 
     def get_key_retry_times(self, model: str) -> int:
         if self.enable_cache:
             openai_key_pool: OpenAIKeyPool = OpenAIKeyPool()
```

### Comparing `promptulate-1.9.0/promptulate/frameworks/__init__.py` & `promptulate-1.9.1/promptulate/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/frameworks/conversation/__init__.py` & `promptulate-1.9.1/promptulate/frameworks/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/frameworks/conversation/conversation.py` & `promptulate-1.9.1/promptulate/frameworks/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/frameworks/prompt.py` & `promptulate-1.9.1/promptulate/frameworks/prompt.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/frameworks/schema.py` & `promptulate-1.9.1/promptulate/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/hook/base.py` & `promptulate-1.9.1/promptulate/hook/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/hook/stdout_hook.py` & `promptulate-1.9.1/promptulate/hook/stdout_hook.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/llms/__init__.py` & `promptulate-1.9.1/promptulate/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/llms/base.py` & `promptulate-1.9.1/promptulate/llms/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/llms/erniebot/erniebot.py` & `promptulate-1.9.1/promptulate/llms/erniebot/erniebot.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,14 @@
         message_set = MessageSet(
             messages=[
                 UserMessage(content=prompt),
             ]
         )
         return self.predict(message_set, stop).content
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
     def _predict(
         self, prompts: MessageSet, stop: Optional[List[str]] = None, *args, **kwargs
     ) -> AssistantMessage:
         """llm generate prompt"""
         headers = {"Content-Type": "application/json"}
         if self.model == "ernie-bot-turbo":
             logging.debug("[pne use ernie-bot-turbo]")
```

### Comparing `promptulate-1.9.0/promptulate/llms/openai/openai.py` & `promptulate-1.9.1/promptulate/llms/openai/openai.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/memory/__init__.py` & `promptulate-1.9.1/promptulate/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/memory/base.py` & `promptulate-1.9.1/promptulate/memory/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/memory/buffer.py` & `promptulate-1.9.1/promptulate/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/memory/file.py` & `promptulate-1.9.1/promptulate/memory/file.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/output_formatter/formatter.py` & `promptulate-1.9.1/promptulate/output_formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/preset_roles/__init__.py` & `promptulate-1.9.1/promptulate/preset_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/preset_roles/prompt.py` & `promptulate-1.9.1/promptulate/preset_roles/prompt.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/preset_roles/roles.py` & `promptulate-1.9.1/promptulate/preset_roles/roles.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/provider/__init__.py` & `promptulate-1.9.1/promptulate/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/provider/base.py` & `promptulate-1.9.1/promptulate/provider/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/provider/mixins.py` & `promptulate-1.9.1/promptulate/provider/mixins.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/schema.py` & `promptulate-1.9.1/promptulate/schema.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tips.py` & `promptulate-1.9.1/promptulate/tips.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/__init__.py` & `promptulate-1.9.1/promptulate/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/arxiv/api_wrapper.py` & `promptulate-1.9.1/promptulate/tools/arxiv/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/arxiv/tools.py` & `promptulate-1.9.1/promptulate/tools/arxiv/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/base.py` & `promptulate-1.9.1/promptulate/tools/base.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/duckduckgo/api_wrapper.py` & `promptulate-1.9.1/promptulate/tools/duckduckgo/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/duckduckgo/tools.py` & `promptulate-1.9.1/promptulate/tools/duckduckgo/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/huggingface/tools.py` & `promptulate-1.9.1/promptulate/tools/huggingface/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/human_feedback/tools.py` & `promptulate-1.9.1/promptulate/tools/human_feedback/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/iot_swith_mqtt/tools.py` & `promptulate-1.9.1/promptulate/tools/iot_swith_mqtt/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/langchain/tools.py` & `promptulate-1.9.1/promptulate/tools/langchain/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/manager.py` & `promptulate-1.9.1/promptulate/tools/manager.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/math/prompt.py` & `promptulate-1.9.1/promptulate/tools/math/prompt.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/math/tools.py` & `promptulate-1.9.1/promptulate/tools/math/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/paper/tools.py` & `promptulate-1.9.1/promptulate/tools/paper/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/python_repl/api_wrapper.py` & `promptulate-1.9.1/promptulate/tools/python_repl/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/python_repl/tools.py` & `promptulate-1.9.1/promptulate/tools/python_repl/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/semantic_scholar/api_wrapper.py` & `promptulate-1.9.1/promptulate/tools/semantic_scholar/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/semantic_scholar/tools.py` & `promptulate-1.9.1/promptulate/tools/semantic_scholar/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/shell/api_wrapper.py` & `promptulate-1.9.1/promptulate/tools/shell/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/shell/tools.py` & `promptulate-1.9.1/promptulate/tools/shell/tools.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/tools/sleep/tool.py` & `promptulate-1.9.1/promptulate/tools/sleep/tool.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/utils/__init__.py` & `promptulate-1.9.1/promptulate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/utils/color_print.py` & `promptulate-1.9.1/promptulate/utils/color_print.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/utils/core_utils.py` & `promptulate-1.9.1/promptulate/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/utils/logger.py` & `promptulate-1.9.1/promptulate/utils/logger.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/utils/openai_key_pool.py` & `promptulate-1.9.1/promptulate/utils/openai_key_pool.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/utils/proxy.py` & `promptulate-1.9.1/promptulate/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/utils/singleton.py` & `promptulate-1.9.1/promptulate/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/promptulate/utils/string_template.py` & `promptulate-1.9.1/promptulate/utils/string_template.py`

 * *Files identical despite different names*

### Comparing `promptulate-1.9.0/pyproject.toml` & `promptulate-1.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 [build-system]
-requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
 
 [tool.poetry]
-name = "promptulate"
-version = "1.9.0"
+authors = ["Zeeland <zeeland4work@gmail.com>"]
 description = "A powerful LLM Application development framework."
-authors = ["Zeeland <zeeland@foxmail.com>"]
+name = "promptulate"
 readme = "README.md"
 repository = "https://github.com/Undertone0809/promptulate"
+version = "1.9.1"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+arxiv = "^1.4.7"
+broadcast-service = "1.3.2"
 click = "^8.1.7"
-pydantic = "^1.10.0"
-questionary = "^2.0.1"
-python-dotenv = "^1.0.0"
 cushy-storage = "^1.2.5"
-requests = "^2.31.0"
-arxiv = "^1.4.7"
 duckduckgo_search = "^3.8.3"
+litellm = "^1.1.1"
 numexpr = "^2.8.4"
-litellm = "^0.12.5"
-broadcast-service = "1.3.2"
+pydantic = "^1.10.0"
+python = ">=3.8.1,<4.0"
+python-dotenv = "^1.0.0"
+questionary = "^2.0.1"
+requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12"
+coverage = "^6.1.2"
+coverage-badge = "^1.1.0"
 isort = {extras = ["colors"], version = "^5.10.1"}
+langchain = "^0.0.338"
+pre-commit = "^3.5.0"
 pytest = "^6.2.5"
-pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
-coverage = "^6.1.2"
-pre-commit = "^3.5.0"
-coverage-badge = "^1.1.0"
-langchain = "^0.0.324"
+pytest-html = "^3.1.1"
 
 [tool.poetry.scripts]
 pne-chat = "promptulate.client.chat:main"
 
 [[tool.poetry.source]]
 name = "tsinghua"
-url = "https://pypi.tuna.tsinghua.edu.cn/simple"
 priority = "default"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple"
 
 [tool.black]
 # https://github.com/psf/black
-target-version = ["py310"]
-line-length = 88
 color = true
+line-length = 88
+target-version = ["py310"]
 
 exclude = '''
 /(
     \.git
     | \.hg
     | \.mypy_cache
     | \.tox
@@ -63,24 +63,23 @@
     | env
     | venv
 )/
 '''
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
-py_version = 37
 line_length = 88
+py_version = 37
 
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
-profile = "black"
+color_output = true
 include_trailing_comma = true
-multi_line_output = 3
 indent = 4
-color_output = true
+multi_line_output = 3
+profile = "black"
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 
 [tool.coverage.run]
 source = ["tests"]
 
 [coverage.report]
 fail_under = 50
 show_missing = true
-
```

### Comparing `promptulate-1.9.0/PKG-INFO` & `promptulate-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: promptulate
-Version: 1.9.0
+Version: 1.9.1
 Summary: A powerful LLM Application development framework.
 Home-page: https://github.com/Undertone0809/promptulate
 Author: Zeeland
-Author-email: zeeland@foxmail.com
+Author-email: zeeland4work@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: arxiv (>=1.4.7,<2.0.0)
 Requires-Dist: broadcast-service (==1.3.2)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cushy-storage (>=1.2.5,<2.0.0)
 Requires-Dist: duckduckgo_search (>=3.8.3,<4.0.0)
-Requires-Dist: litellm (>=0.12.5,<0.13.0)
+Requires-Dist: litellm (>=1.1.1,<2.0.0)
 Requires-Dist: numexpr (>=2.8.4,<3.0.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/Undertone0809/promptulate
 Description-Content-Type: text/markdown
```

