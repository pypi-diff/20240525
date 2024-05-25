# Comparing `tmp/pymemgpt_nightly-0.3.9.dev20240411103902.tar.gz` & `tmp/pymemgpt_nightly-0.3.9.dev20240412103904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemgpt_nightly-0.3.9.dev20240411103902.tar", max compression
+gzip compressed data, was "pymemgpt_nightly-0.3.9.dev20240412103904.tar", max compression
```

## Comparing `pymemgpt_nightly-0.3.9.dev20240411103902.tar` & `pymemgpt_nightly-0.3.9.dev20240412103904.tar`

### file list

```diff
@@ -1,171 +1,172 @@
--rw-r--r--   0        0        0    10760 2024-04-11 10:38:55.455901 pymemgpt_nightly-0.3.9.dev20240411103902/LICENSE
--rw-r--r--   0        0        0     8441 2024-04-11 10:38:55.455901 pymemgpt_nightly-0.3.9.dev20240411103902/README.md
--rw-r--r--   0        0        0      108 2024-04-11 10:39:02.663830 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/__init__.py
--rw-r--r--   0        0        0       29 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/__main__.py
--rw-r--r--   0        0        0    55434 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent.py
--rw-r--r--   0        0        0    10728 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/chroma.py
--rw-r--r--   0        0        0    25552 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/db.py
--rw-r--r--   0        0        0     5288 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/lancedb.py
--rw-r--r--   0        0        0     6390 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/storage.py
--rw-r--r--   0        0        0      169 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/README.md
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/__init__.py
--rw-r--r--   0        0        0     7088 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_autoreply.py
--rw-r--r--   0        0        0     6813 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_docs.py
--rw-r--r--   0        0        0     7929 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_groupchat.py
--rw-r--r--   0        0        0     7375 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
--rw-r--r--   0        0        0     9346 2024-04-11 10:38:55.459901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/interface.py
--rw-r--r--   0        0        0    20931 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/memgpt_agent.py
--rw-r--r--   0        0        0     3644 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/benchmark/benchmark.py
--rw-r--r--   0        0        0      536 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/benchmark/constants.py
--rw-r--r--   0        0        0    34724 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli.py
--rw-r--r--   0        0        0    45520 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli_config.py
--rw-r--r--   0        0        0    10453 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli_load.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/__init__.py
--rw-r--r--   0        0        0     3239 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/admin.py
--rw-r--r--   0        0        0    26894 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/client.py
--rw-r--r--   0        0        0    18729 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/config.py
--rw-r--r--   0        0        0      390 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/configs/memgpt_hosted.json
--rw-r--r--   0        0        0      373 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/configs/openai.json
--rw-r--r--   0        0        0     5606 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/constants.py
--rw-r--r--   0        0        0     5390 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/credentials.py
--rw-r--r--   0        0        0     9529 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/data_sources/connectors.py
--rw-r--r--   0        0        0    28513 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/data_types.py
--rw-r--r--   0        0        0     7601 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/embeddings.py
--rw-r--r--   0        0        0      820 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/errors.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/__init__.py
--rw-r--r--   0        0        0     7343 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/function_sets/base.py
--rw-r--r--   0        0        0     4775 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/function_sets/extras.py
--rw-r--r--   0        0        0     7403 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/functions.py
--rw-r--r--   0        0        0     5433 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/schema_generator.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/humans/__init__.py
--rw-r--r--   0        0        0       17 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/humans/examples/basic.txt
--rw-r--r--   0        0        0      305 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/humans/examples/cs_phd.txt
--rw-r--r--   0        0        0    12994 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/interface.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/__init__.py
--rw-r--r--   0        0        0     6816 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/azure_openai.py
--rw-r--r--   0        0        0    19315 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/google_ai.py
--rw-r--r--   0        0        0    10622 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/llm_api_tools.py
--rw-r--r--   0        0        0     5972 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/openai.py
--rw-r--r--   0        0        0      175 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/README.md
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/__init__.py
--rw-r--r--   0        0        0    13519 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/chat_completion_proxy.py
--rw-r--r--   0        0        0     1032 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/constants.py
--rw-r--r--   0        0        0     2788 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/function_parser.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/__init__.py
--rw-r--r--   0        0        0    56322 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/gbnf_grammar_generator.py
--rw-r--r--   0        0        0      667 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/json.gbnf
--rw-r--r--   0        0        0     3255 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
--rw-r--r--   0        0        0     3562 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/groq/api.py
--rw-r--r--   0        0        0     7793 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/json_parser.py
--rw-r--r--   0        0        0     2586 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/koboldcpp/api.py
--rw-r--r--   0        0        0      557 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/koboldcpp/settings.py
--rw-r--r--   0        0        0     2492 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llamacpp/api.py
--rw-r--r--   0        0        0      548 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llamacpp/settings.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
--rw-r--r--   0        0        0    19913 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
--rw-r--r--   0        0        0    21457 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
--rw-r--r--   0        0        0    19975 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
--rw-r--r--   0        0        0    10300 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
--rw-r--r--   0        0        0     6144 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
--rw-r--r--   0        0        0      419 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
--rw-r--r--   0        0        0    14956 2024-04-11 10:38:55.463901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
--rw-r--r--   0        0        0     4630 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/lmstudio/api.py
--rw-r--r--   0        0        0      857 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/lmstudio/settings.py
--rw-r--r--   0        0        0     3660 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/ollama/api.py
--rw-r--r--   0        0        0      894 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/ollama/settings.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/__init__.py
--rw-r--r--   0        0        0     1222 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/deterministic_mirostat.py
--rw-r--r--   0        0        0     3058 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/settings.py
--rw-r--r--   0        0        0      719 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/simple.py
--rw-r--r--   0        0        0     4846 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/utils.py
--rw-r--r--   0        0        0     2612 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/vllm/api.py
--rw-r--r--   0        0        0     2658 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/api.py
--rw-r--r--   0        0        0     2354 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/legacy_api.py
--rw-r--r--   0        0        0      579 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/legacy_settings.py
--rw-r--r--   0        0        0      593 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/settings.py
--rw-r--r--   0        0        0     1211 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/log.py
--rw-r--r--   0        0        0    20047 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/main.py
--rw-r--r--   0        0        0    20376 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/memory.py
--rw-r--r--   0        0        0    29420 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/metadata.py
--rw-r--r--   0        0        0    31537 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/migrate.py
--rw-r--r--   0        0        0     3295 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/chat_completion_request.py
--rw-r--r--   0        0        0     1562 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/chat_completion_response.py
--rw-r--r--   0        0        0      356 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/embedding_response.py
--rw-r--r--   0        0        0     7977 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/openai.py
--rw-r--r--   0        0        0     8957 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/pydantic_models.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/openai_backcompat/__init__.py
--rw-r--r--   0        0        0    13692 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/openai_backcompat/openai_object.py
--rw-r--r--   0        0        0     5882 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/persistence_manager.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/__init__.py
--rw-r--r--   0        0        0     1849 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/anna_pa.txt
--rw-r--r--   0        0        0     1196 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/google_search_persona.txt
--rw-r--r--   0        0        0      431 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/memgpt_doc.txt
--rw-r--r--   0        0        0      164 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/memgpt_starter.txt
--rw-r--r--   0        0        0     1236 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam.txt
--rw-r--r--   0        0        0     1171 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam_pov.txt
--rw-r--r--   0        0        0     1053 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam_simple_pov_gpt35.txt
--rw-r--r--   0        0        0     8192 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sqldb/test.db
--rw-r--r--   0        0        0      248 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/examples/memgpt_chat.yaml
--rw-r--r--   0        0        0      247 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/examples/memgpt_docs.yaml
--rw-r--r--   0        0        0      374 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/examples/memgpt_extras.yaml
--rw-r--r--   0        0        0     7575 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/presets.py
--rw-r--r--   0        0        0     2789 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/__init__.py
--rw-r--r--   0        0        0    12907 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_functions.py
--rw-r--r--   0        0        0     1139 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_summarize.py
--rw-r--r--   0        0        0     1045 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_system.py
--rw-r--r--   0        0        0     4758 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_base.txt
--rw-r--r--   0        0        0     5479 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_chat.txt
--rw-r--r--   0        0        0     1057 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_chat_compressed.txt
--rw-r--r--   0        0        0     4819 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_doc.txt
--rw-r--r--   0        0        0     5047 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_gpt35_extralong.txt
--rw-r--r--   0        0        0     2967 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
--rw-r--r--   0        0        0     4663 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_modified_chat.txt
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/__init__.py
--rw-r--r--   0        0        0       92 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/constants.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/admin/__init__.py
--rw-r--r--   0        0        0     6130 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/admin/users.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/command.py
--rw-r--r--   0        0        0     6138 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/config.py
--rw-r--r--   0        0        0     5114 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/index.py
--rw-r--r--   0        0        0     7640 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/memory.py
--rw-r--r--   0        0        0     8583 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/message.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth/__init__.py
--rw-r--r--   0        0        0     1303 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth/index.py
--rw-r--r--   0        0        0      775 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth_token.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/config/__init__.py
--rw-r--r--   0        0        0     1136 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/config/index.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/humans/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/humans/index.py
--rw-r--r--   0        0        0     5482 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/interface.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/models/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-11 10:38:55.467901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/models/index.py
--rw-r--r--   0        0        0    23956 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/openai_assistants/assistants.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/personas/__init__.py
--rw-r--r--   0        0        0     1795 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/personas/index.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/presets/__init__.py
--rw-r--r--   0        0        0     5014 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/presets/index.py
--rw-r--r--   0        0        0     9580 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/server.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/sources/__init__.py
--rw-r--r--   0        0        0     8218 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/sources/index.py
--rw-r--r--   0        0        0      914 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/static_files.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/tools/__init__.py
--rw-r--r--   0        0        0     2560 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/tools/index.py
--rw-r--r--   0        0        0    63646 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/server.py
--rw-r--r--   0        0        0    43424 2024-04-11 10:38:55.471901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/assets/index-0c5d3001.css
--rw-r--r--   0        0        0   725155 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/assets/index-bf421135.js
--rw-r--r--   0        0        0    28783 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/favicon.ico
--rw-r--r--   0        0        0     1199 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/index.html
--rw-r--r--   0        0        0    85383 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/memgpt_logo_transparent.png
--rw-r--r--   0        0        0     1667 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/__init__.py
--rw-r--r--   0        0        0     4264 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/example_client.py
--rw-r--r--   0        0        0     4124 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/interface.py
--rw-r--r--   0        0        0     2257 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/protocol.py
--rw-r--r--   0        0        0     6122 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/server.py
--rw-r--r--   0        0        0     7281 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/system.py
--rw-r--r--   0        0        0    31426 2024-04-11 10:38:55.475901 pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/utils.py
--rw-r--r--   0        0        0     2285 2024-04-11 10:39:02.663830 pymemgpt_nightly-0.3.9.dev20240411103902/pyproject.toml
--rw-r--r--   0        0        0    11046 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.9.dev20240411103902/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-12 10:38:56.330371 pymemgpt_nightly-0.3.9.dev20240412103904/LICENSE
+-rw-r--r--   0        0        0     8441 2024-04-12 10:38:56.330371 pymemgpt_nightly-0.3.9.dev20240412103904/README.md
+-rw-r--r--   0        0        0      108 2024-04-12 10:39:04.982238 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/__main__.py
+-rw-r--r--   0        0        0    55434 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent.py
+-rw-r--r--   0        0        0    10728 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent_store/chroma.py
+-rw-r--r--   0        0        0    25552 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent_store/db.py
+-rw-r--r--   0        0        0     5288 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent_store/lancedb.py
+-rw-r--r--   0        0        0     6390 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent_store/storage.py
+-rw-r--r--   0        0        0      169 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/__init__.py
+-rw-r--r--   0        0        0     7088 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/examples/agent_autoreply.py
+-rw-r--r--   0        0        0     6813 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/examples/agent_docs.py
+-rw-r--r--   0        0        0     7929 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/examples/agent_groupchat.py
+-rw-r--r--   0        0        0     7375 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
+-rw-r--r--   0        0        0     9346 2024-04-12 10:38:56.334371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/interface.py
+-rw-r--r--   0        0        0    20931 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/memgpt_agent.py
+-rw-r--r--   0        0        0     3644 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/benchmark/benchmark.py
+-rw-r--r--   0        0        0      536 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/benchmark/constants.py
+-rw-r--r--   0        0        0    34724 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/cli/cli.py
+-rw-r--r--   0        0        0    49820 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/cli/cli_config.py
+-rw-r--r--   0        0        0    10453 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/cli/cli_load.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/client/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/client/admin.py
+-rw-r--r--   0        0        0    26894 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/client/client.py
+-rw-r--r--   0        0        0    18729 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/config.py
+-rw-r--r--   0        0        0      390 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/configs/memgpt_hosted.json
+-rw-r--r--   0        0        0      373 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/configs/openai.json
+-rw-r--r--   0        0        0     5606 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/constants.py
+-rw-r--r--   0        0        0     5641 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/credentials.py
+-rw-r--r--   0        0        0     9529 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/data_sources/connectors.py
+-rw-r--r--   0        0        0    31248 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/data_types.py
+-rw-r--r--   0        0        0     7601 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/embeddings.py
+-rw-r--r--   0        0        0      820 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/errors.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/__init__.py
+-rw-r--r--   0        0        0     7343 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/function_sets/base.py
+-rw-r--r--   0        0        0     4775 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/function_sets/extras.py
+-rw-r--r--   0        0        0     7403 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/functions.py
+-rw-r--r--   0        0        0     5433 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/schema_generator.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/humans/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/humans/examples/basic.txt
+-rw-r--r--   0        0        0      305 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/humans/examples/cs_phd.txt
+-rw-r--r--   0        0        0    12994 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/interface.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/__init__.py
+-rw-r--r--   0        0        0    13539 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/anthropic.py
+-rw-r--r--   0        0        0     6816 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/azure_openai.py
+-rw-r--r--   0        0        0    19315 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/google_ai.py
+-rw-r--r--   0        0        0    11874 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/llm_api_tools.py
+-rw-r--r--   0        0        0     5972 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/openai.py
+-rw-r--r--   0        0        0      175 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/__init__.py
+-rw-r--r--   0        0        0    13519 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/chat_completion_proxy.py
+-rw-r--r--   0        0        0     1078 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/constants.py
+-rw-r--r--   0        0        0     2788 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/function_parser.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/grammars/__init__.py
+-rw-r--r--   0        0        0    56322 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/grammars/gbnf_grammar_generator.py
+-rw-r--r--   0        0        0      667 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/grammars/json.gbnf
+-rw-r--r--   0        0        0     3255 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
+-rw-r--r--   0        0        0     3562 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/groq/api.py
+-rw-r--r--   0        0        0     7793 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/json_parser.py
+-rw-r--r--   0        0        0     2586 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/koboldcpp/api.py
+-rw-r--r--   0        0        0      557 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/koboldcpp/settings.py
+-rw-r--r--   0        0        0     2492 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llamacpp/api.py
+-rw-r--r--   0        0        0      548 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llamacpp/settings.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
+-rw-r--r--   0        0        0    19913 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
+-rw-r--r--   0        0        0    21457 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
+-rw-r--r--   0        0        0    19975 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
+-rw-r--r--   0        0        0    10300 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
+-rw-r--r--   0        0        0     6144 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
+-rw-r--r--   0        0        0      419 2024-04-12 10:38:56.338371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
+-rw-r--r--   0        0        0    14956 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
+-rw-r--r--   0        0        0     4630 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/lmstudio/api.py
+-rw-r--r--   0        0        0      857 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/lmstudio/settings.py
+-rw-r--r--   0        0        0     3660 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/ollama/api.py
+-rw-r--r--   0        0        0      894 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/ollama/settings.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/settings/__init__.py
+-rw-r--r--   0        0        0     1222 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/settings/deterministic_mirostat.py
+-rw-r--r--   0        0        0     3058 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/settings/settings.py
+-rw-r--r--   0        0        0      719 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/settings/simple.py
+-rw-r--r--   0        0        0     4846 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/utils.py
+-rw-r--r--   0        0        0     2612 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/vllm/api.py
+-rw-r--r--   0        0        0     2658 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/webui/api.py
+-rw-r--r--   0        0        0     2354 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/webui/legacy_api.py
+-rw-r--r--   0        0        0      579 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/webui/legacy_settings.py
+-rw-r--r--   0        0        0      593 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/webui/settings.py
+-rw-r--r--   0        0        0     1211 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/log.py
+-rw-r--r--   0        0        0    20047 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/main.py
+-rw-r--r--   0        0        0    20376 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/memory.py
+-rw-r--r--   0        0        0    29420 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/metadata.py
+-rw-r--r--   0        0        0    31537 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/migrate.py
+-rw-r--r--   0        0        0     3295 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/chat_completion_request.py
+-rw-r--r--   0        0        0     1562 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/chat_completion_response.py
+-rw-r--r--   0        0        0      356 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/embedding_response.py
+-rw-r--r--   0        0        0     7977 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/openai.py
+-rw-r--r--   0        0        0     8957 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/pydantic_models.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/openai_backcompat/__init__.py
+-rw-r--r--   0        0        0    13692 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/openai_backcompat/openai_object.py
+-rw-r--r--   0        0        0     5882 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/persistence_manager.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/__init__.py
+-rw-r--r--   0        0        0     1849 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/anna_pa.txt
+-rw-r--r--   0        0        0     1196 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/google_search_persona.txt
+-rw-r--r--   0        0        0      431 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/memgpt_doc.txt
+-rw-r--r--   0        0        0      164 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/memgpt_starter.txt
+-rw-r--r--   0        0        0     1236 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/sam.txt
+-rw-r--r--   0        0        0     1171 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/sam_pov.txt
+-rw-r--r--   0        0        0     1053 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/sam_simple_pov_gpt35.txt
+-rw-r--r--   0        0        0     8192 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/sqldb/test.db
+-rw-r--r--   0        0        0      248 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/presets/examples/memgpt_chat.yaml
+-rw-r--r--   0        0        0      247 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/presets/examples/memgpt_docs.yaml
+-rw-r--r--   0        0        0      374 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/presets/examples/memgpt_extras.yaml
+-rw-r--r--   0        0        0     7575 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/presets/presets.py
+-rw-r--r--   0        0        0     2789 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/presets/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/__init__.py
+-rw-r--r--   0        0        0    12907 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/gpt_functions.py
+-rw-r--r--   0        0        0     1139 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/gpt_summarize.py
+-rw-r--r--   0        0        0     1045 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/gpt_system.py
+-rw-r--r--   0        0        0     4758 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_base.txt
+-rw-r--r--   0        0        0     5479 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_chat.txt
+-rw-r--r--   0        0        0     1057 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_chat_compressed.txt
+-rw-r--r--   0        0        0     4819 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_doc.txt
+-rw-r--r--   0        0        0     5047 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_gpt35_extralong.txt
+-rw-r--r--   0        0        0     2967 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
+-rw-r--r--   0        0        0     4663 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_modified_chat.txt
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/constants.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/admin/__init__.py
+-rw-r--r--   0        0        0     6130 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/admin/users.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/__init__.py
+-rw-r--r--   0        0        0     1757 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/command.py
+-rw-r--r--   0        0        0     6138 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/config.py
+-rw-r--r--   0        0        0     5114 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/index.py
+-rw-r--r--   0        0        0     7640 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/memory.py
+-rw-r--r--   0        0        0     8583 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/message.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/auth/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/auth/index.py
+-rw-r--r--   0        0        0      775 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/auth_token.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/config/__init__.py
+-rw-r--r--   0        0        0     1136 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/config/index.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/humans/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/humans/index.py
+-rw-r--r--   0        0        0     5482 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/interface.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/models/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-12 10:38:56.342371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/models/index.py
+-rw-r--r--   0        0        0    23956 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/openai_assistants/assistants.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/personas/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/personas/index.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/presets/__init__.py
+-rw-r--r--   0        0        0     5014 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/presets/index.py
+-rw-r--r--   0        0        0     9580 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/server.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/sources/__init__.py
+-rw-r--r--   0        0        0     8218 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/sources/index.py
+-rw-r--r--   0        0        0      914 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/static_files.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/tools/__init__.py
+-rw-r--r--   0        0        0     2560 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/tools/index.py
+-rw-r--r--   0        0        0    63646 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/server.py
+-rw-r--r--   0        0        0    43424 2024-04-12 10:38:56.346371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/assets/index-0c5d3001.css
+-rw-r--r--   0        0        0   725155 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/assets/index-bf421135.js
+-rw-r--r--   0        0        0    28783 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/favicon.ico
+-rw-r--r--   0        0        0     1199 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/index.html
+-rw-r--r--   0        0        0    85383 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/memgpt_logo_transparent.png
+-rw-r--r--   0        0        0     1667 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/__init__.py
+-rw-r--r--   0        0        0     4264 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/example_client.py
+-rw-r--r--   0        0        0     4124 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/interface.py
+-rw-r--r--   0        0        0     2257 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/protocol.py
+-rw-r--r--   0        0        0     6122 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/server.py
+-rw-r--r--   0        0        0     7281 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/system.py
+-rw-r--r--   0        0        0    31426 2024-04-12 10:38:56.350371 pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/utils.py
+-rw-r--r--   0        0        0     2285 2024-04-12 10:39:04.978238 pymemgpt_nightly-0.3.9.dev20240412103904/pyproject.toml
+-rw-r--r--   0        0        0    11046 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.9.dev20240412103904/PKG-INFO
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/LICENSE` & `pymemgpt_nightly-0.3.9.dev20240412103904/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/README.md` & `pymemgpt_nightly-0.3.9.dev20240412103904/README.md`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/chroma.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent_store/chroma.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/db.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent_store/db.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/lancedb.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/agent_store/storage.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/agent_store/storage.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_autoreply.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/examples/agent_autoreply.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_docs.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/examples/agent_docs.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/agent_groupchat.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/examples/agent_groupchat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/examples/memgpt_coder_autogen.ipynb` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/examples/memgpt_coder_autogen.ipynb`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/interface.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/autogen/memgpt_agent.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/autogen/memgpt_agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/benchmark/benchmark.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/benchmark/constants.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/benchmark/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli_config.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/cli/cli_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from memgpt.constants import LLM_MAX_TOKENS
 from memgpt.constants import MEMGPT_DIR
 from memgpt.credentials import MemGPTCredentials, SUPPORTED_AUTH_TYPES
 from memgpt.data_types import User, LLMConfig, EmbeddingConfig
 from memgpt.llm_api.openai import openai_get_model_list
 from memgpt.llm_api.azure_openai import azure_openai_get_model_list
 from memgpt.llm_api.google_ai import google_ai_get_model_list, google_ai_get_model_context_window
+from memgpt.llm_api.anthropic import anthropic_get_model_list, antropic_get_model_context_window
+from memgpt.llm_api.llm_api_tools import LLM_API_PROVIDER_OPTIONS
 from memgpt.local_llm.constants import DEFAULT_ENDPOINTS, DEFAULT_OLLAMA_MODEL, DEFAULT_WRAPPER_NAME
 from memgpt.local_llm.utils import get_available_wrappers
 from memgpt.server.utils import shorten_key_middle
 from memgpt.data_types import User, LLMConfig, EmbeddingConfig, Source
 from memgpt.metadata import MetadataStore
 from memgpt.server.utils import shorten_key_middle
 from memgpt.models.pydantic_models import HumanModel, PersonaModel, PresetModel
@@ -60,22 +62,22 @@
 def configure_llm_endpoint(config: MemGPTConfig, credentials: MemGPTCredentials):
     # configure model endpoint
     model_endpoint_type, model_endpoint = None, None
 
     # get default
     default_model_endpoint_type = config.default_llm_config.model_endpoint_type
     if config.default_llm_config.model_endpoint_type is not None and config.default_llm_config.model_endpoint_type not in [
-        "openai",
-        "azure",
-        "google_ai",
+        provider for provider in LLM_API_PROVIDER_OPTIONS if provider != "local"
     ]:  # local model
         default_model_endpoint_type = "local"
 
     provider = questionary.select(
-        "Select LLM inference provider:", choices=["openai", "azure", "google_ai", "local"], default=default_model_endpoint_type
+        "Select LLM inference provider:",
+        choices=LLM_API_PROVIDER_OPTIONS,
+        default=default_model_endpoint_type,
     ).ask()
     if provider is None:
         raise KeyboardInterrupt
 
     # set: model_endpoint_type, model_endpoint
     if provider == "openai":
         # check for key
@@ -180,14 +182,54 @@
         credentials.google_ai_service_endpoint = google_ai_service_endpoint
 
         # write out the credentials
         credentials.save()
 
         model_endpoint_type = "google_ai"
 
+    elif provider == "anthropic":
+        # check for key
+        if credentials.anthropic_key is None:
+            # allow key to get pulled from env vars
+            anthropic_api_key = os.getenv("ANTHROPIC_API_KEY", None)
+            # if we still can't find it, ask for it as input
+            if anthropic_api_key is None:
+                while anthropic_api_key is None or len(anthropic_api_key) == 0:
+                    # Ask for API key as input
+                    anthropic_api_key = questionary.password(
+                        "Enter your Anthropic API key (starts with 'sk-', see https://console.anthropic.com/settings/keys):"
+                    ).ask()
+                    if anthropic_api_key is None:
+                        raise KeyboardInterrupt
+            credentials.anthropic_key = anthropic_api_key
+            credentials.save()
+        else:
+            # Give the user an opportunity to overwrite the key
+            anthropic_api_key = None
+            default_input = (
+                shorten_key_middle(credentials.anthropic_key) if credentials.anthropic_key.startswith("sk-") else credentials.anthropic_key
+            )
+            anthropic_api_key = questionary.password(
+                "Enter your Anthropic API key (starts with 'sk-', see https://console.anthropic.com/settings/keys):",
+                default=default_input,
+            ).ask()
+            if anthropic_api_key is None:
+                raise KeyboardInterrupt
+            # If the user modified it, use the new one
+            if anthropic_api_key != default_input:
+                credentials.anthropic_key = anthropic_api_key
+                credentials.save()
+
+        model_endpoint_type = "anthropic"
+        model_endpoint = "https://api.anthropic.com/v1"
+        model_endpoint = questionary.text("Override default endpoint:", default=model_endpoint).ask()
+        if model_endpoint is None:
+            raise KeyboardInterrupt
+        provider = "anthropic"
+
     else:  # local models
         # backend_options_old = ["webui", "webui-legacy", "llamacpp", "koboldcpp", "ollama", "lmstudio", "lmstudio-legacy", "vllm", "openai"]
         backend_options = builtins.list(DEFAULT_ENDPOINTS.keys())
         # assert backend_options_old == backend_options, (backend_options_old, backend_options)
         default_model_endpoint_type = None
         if config.default_llm_config.model_endpoint_type in backend_options:
             # set from previous config
@@ -287,14 +329,20 @@
             model_options = [str(m["name"]) for m in model_options]
             model_options = [mo[len("models/") :] if mo.startswith("models/") else mo for mo in model_options]
 
             # TODO remove manual filtering for gemini-pro
             model_options = [mo for mo in model_options if str(mo).startswith("gemini") and "-pro" in str(mo)]
             # model_options = ["gemini-pro"]
 
+        elif model_endpoint_type == "anthropic":
+            if credentials.anthropic_key is None:
+                raise ValueError("Missing Anthropic API key")
+            fetched_model_options = anthropic_get_model_list(url=model_endpoint, api_key=credentials.anthropic_key)
+            model_options = [obj["name"] for obj in fetched_model_options]
+
         else:
             # Attempt to do OpenAI endpoint style model fetching
             # TODO support local auth with api-key header
             if credentials.openllm_auth_type == "bearer_token":
                 api_key = credentials.openllm_key
             else:
                 api_key = None
@@ -378,14 +426,34 @@
             "Select default model:",
             choices=fetched_model_options,
             default=fetched_model_options[0],
         ).ask()
         if model is None:
             raise KeyboardInterrupt
 
+    elif model_endpoint_type == "anthropic":
+        try:
+            fetched_model_options = get_model_options(
+                credentials=credentials, model_endpoint_type=model_endpoint_type, model_endpoint=model_endpoint
+            )
+        except Exception as e:
+            # NOTE: if this fails, it means the user's key is probably bad
+            typer.secho(
+                f"Failed to get model list from {model_endpoint} - make sure your API key and endpoints are correct!", fg=typer.colors.RED
+            )
+            raise e
+
+        model = questionary.select(
+            "Select default model:",
+            choices=fetched_model_options,
+            default=fetched_model_options[0],
+        ).ask()
+        if model is None:
+            raise KeyboardInterrupt
+
     else:  # local models
 
         # ask about local auth
         if model_endpoint_type in ["groq"]:  # TODO all llm engines under 'local' that will require api keys
             use_local_auth = True
             local_auth_type = "bearer_token"
             local_auth_key = questionary.password(
@@ -518,25 +586,46 @@
                     )
                 )
                 print(f"Got context window {fetched_context_window} for model {model} (from Google API)")
                 context_length_options = [
                     fetched_context_window,
                     "custom",
                 ]
-            except:
-                print(f"Failed to get model details for model '{model}' on Google AI API")
+            except Exception as e:
+                print(f"Failed to get model details for model '{model}' on Google AI API ({str(e)})")
 
             context_window_input = questionary.select(
                 "Select your model's context window (see https://cloud.google.com/vertex-ai/generative-ai/docs/learn/model-versioning#gemini-model-versions):",
                 choices=context_length_options,
                 default=context_length_options[0],
             ).ask()
             if context_window_input is None:
                 raise KeyboardInterrupt
 
+        elif model_endpoint_type == "anthropic":
+            try:
+                fetched_context_window = str(
+                    antropic_get_model_context_window(url=model_endpoint, api_key=credentials.anthropic_key, model=model)
+                )
+                print(f"Got context window {fetched_context_window} for model {model}")
+                context_length_options = [
+                    fetched_context_window,
+                    "custom",
+                ]
+            except Exception as e:
+                print(f"Failed to get model details for model '{model}' ({str(e)})")
+
+            context_window_input = questionary.select(
+                "Select your model's context window (see https://docs.anthropic.com/claude/docs/models-overview):",
+                choices=context_length_options,
+                default=context_length_options[0],
+            ).ask()
+            if context_window_input is None:
+                raise KeyboardInterrupt
+
         else:
 
             # Ask the user to specify the context length
             context_window_input = questionary.select(
                 "Select your model's context window (for Mistral 7B models, this is probably 8k / 8192):",
                 choices=context_length_options,
                 default=str(LLM_MAX_TOKENS["DEFAULT"]),
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/cli/cli_load.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/cli/cli_load.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/admin.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/client/admin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/client/client.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/client/client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/config.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/constants.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/credentials.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     openai_auth_type: str = "bearer_token"
     openai_key: Optional[str] = None
 
     # gemini config
     google_ai_key: Optional[str] = None
     google_ai_service_endpoint: Optional[str] = None
 
+    # anthropic config
+    anthropic_key: Optional[str] = None
+
     # azure config
     azure_auth_type: str = "api_key"
     azure_key: Optional[str] = None
     # base llm / model
     azure_version: Optional[str] = None
     azure_endpoint: Optional[str] = None
     azure_deployment: Optional[str] = None
@@ -73,14 +76,16 @@
                 "azure_deployment": get_field(config, "azure", "deployment"),
                 "azure_embedding_version": get_field(config, "azure", "embedding_version"),
                 "azure_embedding_endpoint": get_field(config, "azure", "embedding_endpoint"),
                 "azure_embedding_deployment": get_field(config, "azure", "embedding_deployment"),
                 # gemini
                 "google_ai_key": get_field(config, "google_ai", "key"),
                 "google_ai_service_endpoint": get_field(config, "google_ai", "service_endpoint"),
+                # anthropic
+                "anthropic_key": get_field(config, "anthropic", "key"),
                 # open llm
                 "openllm_auth_type": get_field(config, "openllm", "auth_type"),
                 "openllm_key": get_field(config, "openllm", "key"),
                 # path
                 "credentials_path": credentials_path,
             }
             config_dict = {k: v for k, v in config_dict.items() if v is not None}
@@ -109,14 +114,17 @@
         set_field(config, "azure", "embedding_endpoint", self.azure_embedding_endpoint)
         set_field(config, "azure", "embedding_deployment", self.azure_embedding_deployment)
 
         # gemini
         set_field(config, "google_ai", "key", self.google_ai_key)
         set_field(config, "google_ai", "service_endpoint", self.google_ai_service_endpoint)
 
+        # anthropic
+        set_field(config, "anthropic", "key", self.anthropic_key)
+
         # openllm config
         set_field(config, "openllm", "auth_type", self.openllm_auth_type)
         set_field(config, "openllm", "key", self.openllm_key)
 
         if not os.path.exists(MEMGPT_DIR):
             os.makedirs(MEMGPT_DIR, exist_ok=True)
         with open(self.credentials_path, "w", encoding="utf-8") as f:
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/data_sources/connectors.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/data_sources/connectors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/data_types.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -290,14 +290,86 @@
             }
 
         else:
             raise ValueError(self.role)
 
         return openai_message
 
+    def to_anthropic_dict(self, inner_thoughts_xml_tag="thinking") -> dict:
+        # raise NotImplementedError
+
+        def add_xml_tag(string: str, xml_tag: Optional[str]):
+            # NOTE: Anthropic docs recommends using <thinking> tag when using CoT + tool use
+            return f"<{xml_tag}>{string}</{xml_tag}" if xml_tag else string
+
+        if self.role == "system":
+            raise ValueError(f"Anthropic 'system' role not supported")
+
+        elif self.role == "user":
+            assert all([v is not None for v in [self.text, self.role]]), vars(self)
+            anthropic_message = {
+                "content": self.text,
+                "role": self.role,
+            }
+            # Optional field, do not include if null
+            if self.name is not None:
+                anthropic_message["name"] = self.name
+
+        elif self.role == "assistant":
+            assert self.tool_calls is not None or self.text is not None
+            anthropic_message = {
+                "role": self.role,
+            }
+            content = []
+            if self.text is not None:
+                content.append(
+                    {
+                        "type": "text",
+                        "text": add_xml_tag(string=self.text, xml_tag=inner_thoughts_xml_tag),
+                    }
+                )
+            if self.tool_calls is not None:
+                for tool_call in self.tool_calls:
+                    content.append(
+                        {
+                            "type": "tool_use",
+                            "id": tool_call.id,
+                            "name": tool_call.function["name"],
+                            "input": json.loads(tool_call.function["arguments"]),
+                        }
+                    )
+
+            # If the only content was text, unpack it back into a singleton
+            # TODO
+            anthropic_message["content"] = content
+
+            # Optional fields, do not include if null
+            if self.name is not None:
+                anthropic_message["name"] = self.name
+
+        elif self.role == "tool":
+            # NOTE: Anthropic uses role "user" for "tool" responses
+            assert all([v is not None for v in [self.role, self.tool_call_id]]), vars(self)
+            anthropic_message = {
+                "role": "user",  # NOTE: diff
+                "content": [
+                    # TODO support error types etc
+                    {
+                        "type": "tool_result",
+                        "tool_use_id": self.tool_call_id,
+                        "content": self.text,
+                    }
+                ],
+            }
+
+        else:
+            raise ValueError(self.role)
+
+        return anthropic_message
+
     def to_google_ai_dict(self, put_inner_thoughts_in_kwargs: bool = True) -> dict:
         """Go from Message class to Google AI REST message object
 
         type Content: https://ai.google.dev/api/rest/v1/Content / https://ai.google.dev/api/rest/v1beta/Content
             parts[]: Part
             role: str ('user' or 'model')
         """
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/embeddings.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/embeddings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/errors.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/errors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/function_sets/base.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/function_sets/base.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/function_sets/extras.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/function_sets/extras.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/functions.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/functions/schema_generator.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/functions/schema_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/interface.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/azure_openai.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/google_ai.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/google_ai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/llm_api_tools.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/llm_api_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 
 from memgpt.llm_api.openai import openai_chat_completions_request
 from memgpt.llm_api.azure_openai import azure_openai_chat_completions_request, MODEL_TO_AZURE_ENGINE
 from memgpt.llm_api.google_ai import (
     google_ai_chat_completions_request,
     convert_tools_to_google_ai_format,
 )
+from memgpt.llm_api.anthropic import anthropic_chat_completions_request
+
+
+LLM_API_PROVIDER_OPTIONS = ["openai", "azure", "anthropic", "google_ai", "local"]
 
 
 def is_context_overflow_error(exception: requests.exceptions.RequestException) -> bool:
     """Checks if an exception is due to context overflow (based on common OpenAI response messages)"""
     from memgpt.utils import printd
 
     match_string = "maximum context length"
@@ -210,15 +214,15 @@
         # NOTE: until Google AI supports CoT / text alongside function calls,
         # we need to put it in a kwarg (unless we want to split the message into two)
         google_ai_inner_thoughts_in_kwarg = True
 
         if functions is not None:
             tools = [{"type": "function", "function": f} for f in functions]
             tools = [Tool(**t) for t in tools]
-            tools = (convert_tools_to_google_ai_format(tools, inner_thoughts_in_kwargs=google_ai_inner_thoughts_in_kwarg),)
+            tools = convert_tools_to_google_ai_format(tools, inner_thoughts_in_kwargs=google_ai_inner_thoughts_in_kwarg)
         else:
             tools = None
 
         return google_ai_chat_completions_request(
             inner_thoughts_in_kwargs=google_ai_inner_thoughts_in_kwarg,
             service_endpoint=credentials.google_ai_service_endpoint,
             model=agent_state.llm_config.model,
@@ -226,14 +230,38 @@
             # see structure of payload here: https://ai.google.dev/docs/function_calling
             data=dict(
                 contents=[m.to_google_ai_dict() for m in messages],
                 tools=tools,
             ),
         )
 
+    elif agent_state.llm_config.model_endpoint_type == "anthropic":
+        if not use_tool_naming:
+            raise NotImplementedError("Only tool calling supported on Anthropic API requests")
+
+        if functions is not None:
+            tools = [{"type": "function", "function": f} for f in functions]
+            tools = [Tool(**t) for t in tools]
+        else:
+            tools = None
+
+        return anthropic_chat_completions_request(
+            url=agent_state.llm_config.model_endpoint,
+            api_key=credentials.anthropic_key,
+            data=ChatCompletionRequest(
+                model=agent_state.llm_config.model,
+                messages=[cast_message_to_subtype(m.to_openai_dict()) for m in messages],
+                tools=[{"type": "function", "function": f} for f in functions] if functions else None,
+                # tool_choice=function_call,
+                # user=str(agent_state.user_id),
+                # NOTE: max_tokens is required for Anthropic API
+                max_tokens=1024,  # TODO make dynamic
+            ),
+        )
+
     # local model
     else:
         return get_chat_completion(
             model=agent_state.llm_config.model,
             messages=messages,
             functions=functions,
             functions_python=functions_python,
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/llm_api/openai.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/llm_api/openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/chat_completion_proxy.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/chat_completion_proxy.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/constants.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "lmstudio-legacy": "http://localhost:1234",
     "ollama": "http://localhost:11434",
     "webui-legacy": "http://localhost:5000",
     "webui": "http://localhost:5000",
     "vllm": "http://localhost:8000",
     # APIs
     "openai": "https://api.openai.com",
+    "anthropic": "https://api.anthropic.com",
     "groq": "https://api.groq.com/openai",
 }
 
 DEFAULT_OLLAMA_MODEL = "dolphin2.2-mistral:7b-q6_K"
 
 # DEFAULT_WRAPPER = airoboros.Airoboros21InnerMonologueWrapper
 # DEFAULT_WRAPPER_NAME = "airoboros-l2-70b-2.1"
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/function_parser.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/function_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/gbnf_grammar_generator.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/grammars/gbnf_grammar_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/json.gbnf` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/groq/api.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/groq/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/json_parser.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/json_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/koboldcpp/api.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/koboldcpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/koboldcpp/settings.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/koboldcpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llamacpp/api.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llamacpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llamacpp/settings.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llamacpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/lmstudio/api.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/lmstudio/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/lmstudio/settings.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/lmstudio/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/ollama/api.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/ollama/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/ollama/settings.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/ollama/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/deterministic_mirostat.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/settings/deterministic_mirostat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/settings.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/settings/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/settings/simple.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/settings/simple.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/utils.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/vllm/api.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/vllm/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/api.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/webui/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/legacy_api.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/webui/legacy_api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/legacy_settings.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/webui/legacy_settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/local_llm/webui/settings.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/local_llm/webui/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/log.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/log.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/main.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/main.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/memory.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/metadata.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/metadata.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/migrate.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/migrate.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/chat_completion_request.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/chat_completion_response.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/openai.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/models/pydantic_models.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/models/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/openai_backcompat/openai_object.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/openai_backcompat/openai_object.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/persistence_manager.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/anna_pa.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/anna_pa.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/google_search_persona.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/google_search_persona.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/sam.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam_pov.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/sam_pov.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sam_simple_pov_gpt35.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/sam_simple_pov_gpt35.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/personas/examples/sqldb/test.db` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/personas/examples/sqldb/test.db`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/presets.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/presets/presets.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/presets/utils.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/presets/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_functions.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/gpt_functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_summarize.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/gpt_summarize.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/gpt_system.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/gpt_system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_base.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_base.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_chat.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_chat_compressed.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_chat_compressed.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_doc.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_doc.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_gpt35_extralong.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_gpt35_extralong.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_intuitive_knowledge.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_intuitive_knowledge.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/prompts/system/memgpt_modified_chat.txt` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/prompts/system/memgpt_modified_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/admin/users.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/admin/users.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/command.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/command.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/config.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/memory.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/agents/message.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/agents/message.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/auth/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/auth_token.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/auth_token.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/config/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/config/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/humans/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/humans/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/interface.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/models/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/models/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/openai_assistants/assistants.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/openai_assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/personas/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/personas/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/presets/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/presets/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/server.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/sources/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/sources/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/static_files.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/static_files.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/rest_api/tools/index.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/rest_api/tools/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/server.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/assets/index-0c5d3001.css` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/assets/index-0c5d3001.css`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/assets/index-bf421135.js` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/assets/index-bf421135.js`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/favicon.ico` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/index.html` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/index.html`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/static_files/memgpt_logo_transparent.png` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/static_files/memgpt_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/utils.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/example_client.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/example_client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/interface.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/protocol.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/protocol.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/server/ws_api/server.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/server/ws_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/system.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/memgpt/utils.py` & `pymemgpt_nightly-0.3.9.dev20240412103904/memgpt/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/pyproject.toml` & `pymemgpt_nightly-0.3.9.dev20240412103904/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymemgpt-nightly"
-version = "0.3.9.dev20240411103902"
+version = "0.3.9.dev20240412103904"
 packages = [
     {include = "memgpt"}
 ]
 description = "Teaching LLMs memory management for unbounded context"
 authors = [
     "MemGPT Team <hi@memgpt.ai>",
 ]
```

### Comparing `pymemgpt_nightly-0.3.9.dev20240411103902/PKG-INFO` & `pymemgpt_nightly-0.3.9.dev20240412103904/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemgpt-nightly
-Version: 0.3.9.dev20240411103902
+Version: 0.3.9.dev20240412103904
 Summary: Teaching LLMs memory management for unbounded context
 License: Apache License
 Author: MemGPT Team
 Author-email: hi@memgpt.ai
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.9.dev20240411103902
+Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.9.dev20240412103904
 Summary: Teaching LLMs memory management for unbounded context License: Apache
 License Author: MemGPT Team Author-email: hi@memgpt.ai Requires-Python:
 >=3.10,<3.13 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Provides-Extra: autogen Provides-Extra:
 dev Provides-Extra: local Provides-Extra: postgres Provides-Extra: server
```

