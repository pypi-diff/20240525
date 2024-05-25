# Comparing `tmp/llama_index_core-0.9.55.tar.gz` & `tmp/llama_index_core-0.9.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_core-0.9.55.tar", max compression
+gzip compressed data, was "llama_index_core-0.9.56.tar", max compression
```

## Comparing `llama_index_core-0.9.55.tar` & `llama_index_core-0.9.56.tar`

### file list

```diff
@@ -1,437 +1,437 @@
--rw-r--r--   0        0        0     1065 2024-02-08 06:51:54.186119 llama_index_core-0.9.55/LICENSE
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.186218 llama_index_core-0.9.55/README.md
--rw-r--r--   0        0        0       13 2024-02-08 06:51:54.186391 llama_index_core-0.9.55/llama_index/core/VERSION
--rw-r--r--   0        0        0     3975 2024-02-08 06:51:54.186475 llama_index_core-0.9.55/llama_index/core/__init__.py
--rw-r--r--   0        0        0       46 2024-02-08 06:51:54.186596 llama_index_core-0.9.55/llama_index/core/_static/.gitignore
--rw-r--r--   0        0        0       32 2024-02-08 06:51:54.186722 llama_index_core-0.9.55/llama_index/core/_static/nltk_cache/.gitignore
--rw-r--r--   0        0        0       32 2024-02-08 06:51:54.186831 llama_index_core-0.9.55/llama_index/core/_static/tiktoken_cache/.gitignore
--rw-r--r--   0        0        0     1031 2024-02-08 06:51:54.186974 llama_index_core-0.9.55/llama_index/core/agent/__init__.py
--rw-r--r--   0        0        0       19 2024-02-08 06:51:54.187096 llama_index_core-0.9.55/llama_index/core/agent/custom/__init__.py
--rw-r--r--   0        0        0     6424 2024-02-08 06:51:54.187200 llama_index_core-0.9.55/llama_index/core/agent/custom/pipeline_worker.py
--rw-r--r--   0        0        0     8533 2024-02-08 06:51:54.187286 llama_index_core-0.9.55/llama_index/core/agent/custom/simple.py
--rw-r--r--   0        0        0       19 2024-02-08 06:51:54.187395 llama_index_core-0.9.55/llama_index/core/agent/legacy/__init__.py
--rw-r--r--   0        0        0       19 2024-02-08 06:51:54.187499 llama_index_core-0.9.55/llama_index/core/agent/legacy/react/__init__.py
--rw-r--r--   0        0        0    19427 2024-02-08 06:51:54.187609 llama_index_core-0.9.55/llama_index/core/agent/legacy/react/base.py
--rw-r--r--   0        0        0      258 2024-02-08 06:51:54.187750 llama_index_core-0.9.55/llama_index/core/agent/react/__init__.py
--rw-r--r--   0        0        0      190 2024-02-08 06:51:54.188236 llama_index_core-0.9.55/llama_index/core/agent/react/agent.py
--rw-r--r--   0        0        0     4290 2024-02-08 06:51:54.188320 llama_index_core-0.9.55/llama_index/core/agent/react/base.py
--rw-r--r--   0        0        0     4107 2024-02-08 06:51:54.188410 llama_index_core-0.9.55/llama_index/core/agent/react/formatter.py
--rw-r--r--   0        0        0     3733 2024-02-08 06:51:54.188479 llama_index_core-0.9.55/llama_index/core/agent/react/output_parser.py
--rw-r--r--   0        0        0     3408 2024-02-08 06:51:54.188732 llama_index_core-0.9.55/llama_index/core/agent/react/prompts.py
--rw-r--r--   0        0        0    23654 2024-02-08 06:51:54.188846 llama_index_core-0.9.55/llama_index/core/agent/react/step.py
--rw-r--r--   0        0        0     1797 2024-02-08 06:51:54.188928 llama_index_core-0.9.55/llama_index/core/agent/react/types.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.189004 llama_index_core-0.9.55/llama_index/core/agent/react_multimodal/__init__.py
--rw-r--r--   0        0        0     2839 2024-02-08 06:51:54.189094 llama_index_core-0.9.55/llama_index/core/agent/react_multimodal/prompts.py
--rw-r--r--   0        0        0    18603 2024-02-08 06:51:54.189181 llama_index_core-0.9.55/llama_index/core/agent/react_multimodal/step.py
--rw-r--r--   0        0        0       19 2024-02-08 06:51:54.189412 llama_index_core-0.9.55/llama_index/core/agent/runner/__init__.py
--rw-r--r--   0        0        0    20460 2024-02-08 06:51:54.189513 llama_index_core-0.9.55/llama_index/core/agent/runner/base.py
--rw-r--r--   0        0        0    15699 2024-02-08 06:51:54.189662 llama_index_core-0.9.55/llama_index/core/agent/runner/parallel.py
--rw-r--r--   0        0        0     7147 2024-02-08 06:51:54.189756 llama_index_core-0.9.55/llama_index/core/agent/types.py
--rw-r--r--   0        0        0      545 2024-02-08 06:51:54.189837 llama_index_core-0.9.55/llama_index/core/agent/utils.py
--rw-r--r--   0        0        0     2926 2024-02-08 06:51:54.189921 llama_index_core-0.9.55/llama_index/core/async_utils.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.189999 llama_index_core-0.9.55/llama_index/core/base/__init__.py
--rw-r--r--   0        0        0     1627 2024-02-08 06:51:54.190097 llama_index_core-0.9.55/llama_index/core/base/base_auto_retriever.py
--rw-r--r--   0        0        0     1788 2024-02-08 06:51:54.190203 llama_index_core-0.9.55/llama_index/core/base/base_multi_modal_retriever.py
--rw-r--r--   0        0        0     4216 2024-02-08 06:51:54.190278 llama_index_core-0.9.55/llama_index/core/base/base_query_engine.py
--rw-r--r--   0        0        0    11946 2024-02-08 06:51:54.190378 llama_index_core-0.9.55/llama_index/core/base/base_retriever.py
--rw-r--r--   0        0        0     3333 2024-02-08 06:51:54.190451 llama_index_core-0.9.55/llama_index/core/base/base_selector.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.190534 llama_index_core-0.9.55/llama_index/core/base/embeddings/__init__.py
--rw-r--r--   0        0        0    12474 2024-02-08 06:51:54.191211 llama_index_core-0.9.55/llama_index/core/base/embeddings/base.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.191300 llama_index_core-0.9.55/llama_index/core/base/llms/__init__.py
--rw-r--r--   0        0        0     3778 2024-02-08 06:51:54.191398 llama_index_core-0.9.55/llama_index/core/base/llms/types.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.191465 llama_index_core-0.9.55/llama_index/core/base/query_pipeline/__init__.py
--rw-r--r--   0        0        0    10619 2024-02-08 06:51:54.191568 llama_index_core-0.9.55/llama_index/core/base/query_pipeline/query.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.191644 llama_index_core-0.9.55/llama_index/core/base/response/__init__.py
--rw-r--r--   0        0        0     4748 2024-02-08 06:51:54.191746 llama_index_core-0.9.55/llama_index/core/base/response/schema.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.191815 llama_index_core-0.9.55/llama_index/core/bridge/__init__.py
--rw-r--r--   0        0        0     2809 2024-02-08 06:51:54.191913 llama_index_core-0.9.55/llama_index/core/bridge/langchain.py
--rw-r--r--   0        0        0     1132 2024-02-08 06:51:54.191997 llama_index_core-0.9.55/llama_index/core/bridge/pydantic.py
--rw-r--r--   0        0        0      378 2024-02-08 06:51:54.192106 llama_index_core-0.9.55/llama_index/core/callbacks/__init__.py
--rw-r--r--   0        0        0    10389 2024-02-08 06:51:54.192180 llama_index_core-0.9.55/llama_index/core/callbacks/base.py
--rw-r--r--   0        0        0     1664 2024-02-08 06:51:54.192253 llama_index_core-0.9.55/llama_index/core/callbacks/base_handler.py
--rw-r--r--   0        0        0     3726 2024-02-08 06:51:54.192308 llama_index_core-0.9.55/llama_index/core/callbacks/global_handlers.py
--rw-r--r--   0        0        0     7866 2024-02-08 06:51:54.192381 llama_index_core-0.9.55/llama_index/core/callbacks/llama_debug.py
--rw-r--r--   0        0        0     3572 2024-02-08 06:51:54.192454 llama_index_core-0.9.55/llama_index/core/callbacks/schema.py
--rw-r--r--   0        0        0     2161 2024-02-08 06:51:54.192533 llama_index_core-0.9.55/llama_index/core/callbacks/simple_llm_handler.py
--rw-r--r--   0        0        0     7679 2024-02-08 06:51:54.192598 llama_index_core-0.9.55/llama_index/core/callbacks/token_counting.py
--rw-r--r--   0        0        0     2174 2024-02-08 06:51:54.192657 llama_index_core-0.9.55/llama_index/core/callbacks/utils.py
--rw-r--r--   0        0        0      464 2024-02-08 06:51:54.192754 llama_index_core-0.9.55/llama_index/core/chat_engine/__init__.py
--rw-r--r--   0        0        0    14037 2024-02-08 06:51:54.192864 llama_index_core-0.9.55/llama_index/core/chat_engine/condense_plus_context.py
--rw-r--r--   0        0        0    14398 2024-02-08 06:51:54.192980 llama_index_core-0.9.55/llama_index/core/chat_engine/condense_question.py
--rw-r--r--   0        0        0    11385 2024-02-08 06:51:54.193065 llama_index_core-0.9.55/llama_index/core/chat_engine/context.py
--rw-r--r--   0        0        0     6274 2024-02-08 06:51:54.193152 llama_index_core-0.9.55/llama_index/core/chat_engine/simple.py
--rw-r--r--   0        0        0    11130 2024-02-08 06:51:54.193261 llama_index_core-0.9.55/llama_index/core/chat_engine/types.py
--rw-r--r--   0        0        0      476 2024-02-08 06:51:54.193351 llama_index_core-0.9.55/llama_index/core/chat_engine/utils.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.193434 llama_index_core-0.9.55/llama_index/core/command_line/__init__.py
--rw-r--r--   0        0        0     7000 2024-02-08 06:51:54.193543 llama_index_core-0.9.55/llama_index/core/command_line/command_line.py
--rw-r--r--   0        0        0    45435 2024-02-08 06:51:54.193662 llama_index_core-0.9.55/llama_index/core/command_line/mappings.json
--rw-r--r--   0        0        0    15052 2024-02-08 06:51:54.193800 llama_index_core-0.9.55/llama_index/core/command_line/rag.py
--rw-r--r--   0        0        0     8428 2024-02-08 06:51:54.193880 llama_index_core-0.9.55/llama_index/core/command_line/upgrade.py
--rw-r--r--   0        0        0      251 2024-02-08 06:51:54.194027 llama_index_core-0.9.55/llama_index/core/composability/__init__.py
--rw-r--r--   0        0        0      170 2024-02-08 06:51:54.194134 llama_index_core-0.9.55/llama_index/core/composability/base.py
--rw-r--r--   0        0        0     4762 2024-02-08 06:51:54.194211 llama_index_core-0.9.55/llama_index/core/composability/joint_qa_summary.py
--rw-r--r--   0        0        0      703 2024-02-08 06:51:54.194300 llama_index_core-0.9.55/llama_index/core/constants.py
--rw-r--r--   0        0        0      337 2024-02-08 06:51:54.194633 llama_index_core-0.9.55/llama_index/core/data_structs/__init__.py
--rw-r--r--   0        0        0     8110 2024-02-08 06:51:54.194726 llama_index_core-0.9.55/llama_index/core/data_structs/data_structs.py
--rw-r--r--   0        0        0     2518 2024-02-08 06:51:54.194803 llama_index_core-0.9.55/llama_index/core/data_structs/document_summary.py
--rw-r--r--   0        0        0     1026 2024-02-08 06:51:54.194869 llama_index_core-0.9.55/llama_index/core/data_structs/registry.py
--rw-r--r--   0        0        0     4292 2024-02-08 06:51:54.194951 llama_index_core-0.9.55/llama_index/core/data_structs/struct_type.py
--rw-r--r--   0        0        0     1035 2024-02-08 06:51:54.195037 llama_index_core-0.9.55/llama_index/core/data_structs/table.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.195112 llama_index_core-0.9.55/llama_index/core/download/__init__.py
--rw-r--r--   0        0        0     8995 2024-02-08 06:51:54.195222 llama_index_core-0.9.55/llama_index/core/download/dataset.py
--rw-r--r--   0        0        0      975 2024-02-08 06:51:54.195291 llama_index_core-0.9.55/llama_index/core/download/integration.py
--rw-r--r--   0        0        0     9553 2024-02-08 06:51:54.195363 llama_index_core-0.9.55/llama_index/core/download/module.py
--rw-r--r--   0        0        0     4702 2024-02-08 06:51:54.195443 llama_index_core-0.9.55/llama_index/core/download/pack.py
--rw-r--r--   0        0        0     3239 2024-02-08 06:51:54.195517 llama_index_core-0.9.55/llama_index/core/download/utils.py
--rw-r--r--   0        0        0      348 2024-02-08 06:51:54.195606 llama_index_core-0.9.55/llama_index/core/embeddings/__init__.py
--rw-r--r--   0        0        0      708 2024-02-08 06:51:54.195667 llama_index_core-0.9.55/llama_index/core/embeddings/loading.py
--rw-r--r--   0        0        0     1081 2024-02-08 06:51:54.195737 llama_index_core-0.9.55/llama_index/core/embeddings/mock_embed_model.py
--rw-r--r--   0        0        0     6837 2024-02-08 06:51:54.195813 llama_index_core-0.9.55/llama_index/core/embeddings/multi_modal_base.py
--rw-r--r--   0        0        0     1452 2024-02-08 06:51:54.195879 llama_index_core-0.9.55/llama_index/core/embeddings/pooling.py
--rw-r--r--   0        0        0     4804 2024-02-08 06:51:54.195947 llama_index_core-0.9.55/llama_index/core/embeddings/utils.py
--rw-r--r--   0        0        0     2636 2024-02-08 06:51:54.196071 llama_index_core-0.9.55/llama_index/core/evaluation/__init__.py
--rw-r--r--   0        0        0     5550 2024-02-08 06:51:54.196208 llama_index_core-0.9.55/llama_index/core/evaluation/answer_relevancy.py
--rw-r--r--   0        0        0     4070 2024-02-08 06:51:54.196297 llama_index_core-0.9.55/llama_index/core/evaluation/base.py
--rw-r--r--   0        0        0    11242 2024-02-08 06:51:54.196387 llama_index_core-0.9.55/llama_index/core/evaluation/batch_runner.py
--rw-r--r--   0        0        0      198 2024-02-08 06:51:54.196526 llama_index_core-0.9.55/llama_index/core/evaluation/benchmarks/__init__.py
--rw-r--r--   0        0        0     4195 2024-02-08 06:51:54.196653 llama_index_core-0.9.55/llama_index/core/evaluation/benchmarks/beir.py
--rw-r--r--   0        0        0     7602 2024-02-08 06:51:54.196737 llama_index_core-0.9.55/llama_index/core/evaluation/benchmarks/hotpotqa.py
--rw-r--r--   0        0        0     7011 2024-02-08 06:51:54.196821 llama_index_core-0.9.55/llama_index/core/evaluation/context_relevancy.py
--rw-r--r--   0        0        0     5162 2024-02-08 06:51:54.196901 llama_index_core-0.9.55/llama_index/core/evaluation/correctness.py
--rw-r--r--   0        0        0    12903 2024-02-08 06:51:54.197033 llama_index_core-0.9.55/llama_index/core/evaluation/dataset_generation.py
--rw-r--r--   0        0        0     2199 2024-02-08 06:51:54.197115 llama_index_core-0.9.55/llama_index/core/evaluation/eval_utils.py
--rw-r--r--   0        0        0     6276 2024-02-08 06:51:54.197198 llama_index_core-0.9.55/llama_index/core/evaluation/faithfulness.py
--rw-r--r--   0        0        0     4453 2024-02-08 06:51:54.197274 llama_index_core-0.9.55/llama_index/core/evaluation/guideline.py
--rw-r--r--   0        0        0      324 2024-02-08 06:51:54.197414 llama_index_core-0.9.55/llama_index/core/evaluation/multi_modal/__init__.py
--rw-r--r--   0        0        0     8140 2024-02-08 06:51:54.197501 llama_index_core-0.9.55/llama_index/core/evaluation/multi_modal/faithfulness.py
--rw-r--r--   0        0        0     7206 2024-02-08 06:51:54.197601 llama_index_core-0.9.55/llama_index/core/evaluation/multi_modal/relevancy.py
--rw-r--r--   0        0        0     2321 2024-02-08 06:51:54.197694 llama_index_core-0.9.55/llama_index/core/evaluation/notebook_utils.py
--rw-r--r--   0        0        0    10344 2024-02-08 06:51:54.197785 llama_index_core-0.9.55/llama_index/core/evaluation/pairwise.py
--rw-r--r--   0        0        0     5357 2024-02-08 06:51:54.197869 llama_index_core-0.9.55/llama_index/core/evaluation/relevancy.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.197949 llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/__init__.py
--rw-r--r--   0        0        0     6353 2024-02-08 06:51:54.198045 llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/base.py
--rw-r--r--   0        0        0     4606 2024-02-08 06:51:54.198148 llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/evaluator.py
--rw-r--r--   0        0        0     4571 2024-02-08 06:51:54.198231 llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/metrics.py
--rw-r--r--   0        0        0     1557 2024-02-08 06:51:54.198308 llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/metrics_base.py
--rw-r--r--   0        0        0     3110 2024-02-08 06:51:54.198387 llama_index_core-0.9.55/llama_index/core/evaluation/semantic_similarity.py
--rw-r--r--   0        0        0     3892 2024-02-08 06:51:54.198480 llama_index_core-0.9.55/llama_index/core/exec_utils.py
--rw-r--r--   0        0        0      426 2024-02-08 06:51:54.198600 llama_index_core-0.9.55/llama_index/core/extractors/__init__.py
--rw-r--r--   0        0        0     5472 2024-02-08 06:51:54.198678 llama_index_core-0.9.55/llama_index/core/extractors/interface.py
--rw-r--r--   0        0        0      966 2024-02-08 06:51:54.198941 llama_index_core-0.9.55/llama_index/core/extractors/loading.py
--rw-r--r--   0        0        0    16864 2024-02-08 06:51:54.199065 llama_index_core-0.9.55/llama_index/core/extractors/metadata_extractors.py
--rw-r--r--   0        0        0      126 2024-02-08 06:51:54.199218 llama_index_core-0.9.55/llama_index/core/graph_stores/__init__.py
--rw-r--r--   0        0        0      535 2024-02-08 06:51:54.199297 llama_index_core-0.9.55/llama_index/core/graph_stores/registry.py
--rw-r--r--   0        0        0     6107 2024-02-08 06:51:54.199380 llama_index_core-0.9.55/llama_index/core/graph_stores/simple.py
--rw-r--r--   0        0        0     2096 2024-02-08 06:51:54.199464 llama_index_core-0.9.55/llama_index/core/graph_stores/types.py
--rw-r--r--   0        0        0     3226 2024-02-08 06:51:54.199560 llama_index_core-0.9.55/llama_index/core/image_retriever.py
--rw-r--r--   0        0        0      522 2024-02-08 06:51:54.199629 llama_index_core-0.9.55/llama_index/core/img_utils.py
--rw-r--r--   0        0        0     2360 2024-02-08 06:51:54.199746 llama_index_core-0.9.55/llama_index/core/indices/__init__.py
--rw-r--r--   0        0        0    17484 2024-02-08 06:51:54.199844 llama_index_core-0.9.55/llama_index/core/indices/base.py
--rw-r--r--   0        0        0      129 2024-02-08 06:51:54.199928 llama_index_core-0.9.55/llama_index/core/indices/base_retriever.py
--rw-r--r--   0        0        0       17 2024-02-08 06:51:54.200032 llama_index_core-0.9.55/llama_index/core/indices/common/__init__.py
--rw-r--r--   0        0        0       19 2024-02-08 06:51:54.200145 llama_index_core-0.9.55/llama_index/core/indices/common/struct_store/__init__.py
--rw-r--r--   0        0        0     8944 2024-02-08 06:51:54.200238 llama_index_core-0.9.55/llama_index/core/indices/common/struct_store/base.py
--rw-r--r--   0        0        0      776 2024-02-08 06:51:54.200315 llama_index_core-0.9.55/llama_index/core/indices/common/struct_store/schema.py
--rw-r--r--   0        0        0     2687 2024-02-08 06:51:54.200384 llama_index_core-0.9.55/llama_index/core/indices/common/struct_store/sql.py
--rw-r--r--   0        0        0       19 2024-02-08 06:51:54.200494 llama_index_core-0.9.55/llama_index/core/indices/common_tree/__init__.py
--rw-r--r--   0        0        0     8868 2024-02-08 06:51:54.200586 llama_index_core-0.9.55/llama_index/core/indices/common_tree/base.py
--rw-r--r--   0        0        0      185 2024-02-08 06:51:54.200884 llama_index_core-0.9.55/llama_index/core/indices/composability/__init__.py
--rw-r--r--   0        0        0     4953 2024-02-08 06:51:54.200977 llama_index_core-0.9.55/llama_index/core/indices/composability/graph.py
--rw-r--r--   0        0        0      546 2024-02-08 06:51:54.201386 llama_index_core-0.9.55/llama_index/core/indices/document_summary/__init__.py
--rw-r--r--   0        0        0    11179 2024-02-08 06:51:54.201507 llama_index_core-0.9.55/llama_index/core/indices/document_summary/base.py
--rw-r--r--   0        0        0     7213 2024-02-08 06:51:54.201612 llama_index_core-0.9.55/llama_index/core/indices/document_summary/retrievers.py
--rw-r--r--   0        0        0      234 2024-02-08 06:51:54.201758 llama_index_core-0.9.55/llama_index/core/indices/empty/__init__.py
--rw-r--r--   0        0        0     3065 2024-02-08 06:51:54.201847 llama_index_core-0.9.55/llama_index/core/indices/empty/base.py
--rw-r--r--   0        0        0     1285 2024-02-08 06:51:54.201946 llama_index_core-0.9.55/llama_index/core/indices/empty/retrievers.py
--rw-r--r--   0        0        0     2379 2024-02-08 06:51:54.202314 llama_index_core-0.9.55/llama_index/core/indices/keyword_table/README.md
--rw-r--r--   0        0        0      880 2024-02-08 06:51:54.202423 llama_index_core-0.9.55/llama_index/core/indices/keyword_table/__init__.py
--rw-r--r--   0        0        0     9273 2024-02-08 06:51:54.202517 llama_index_core-0.9.55/llama_index/core/indices/keyword_table/base.py
--rw-r--r--   0        0        0     1098 2024-02-08 06:51:54.202597 llama_index_core-0.9.55/llama_index/core/indices/keyword_table/rake_base.py
--rw-r--r--   0        0        0     7142 2024-02-08 06:51:54.202701 llama_index_core-0.9.55/llama_index/core/indices/keyword_table/retrievers.py
--rw-r--r--   0        0        0     1312 2024-02-08 06:51:54.202786 llama_index_core-0.9.55/llama_index/core/indices/keyword_table/simple_base.py
--rw-r--r--   0        0        0     2360 2024-02-08 06:51:54.202887 llama_index_core-0.9.55/llama_index/core/indices/keyword_table/utils.py
--rw-r--r--   0        0        0      342 2024-02-08 06:51:54.203018 llama_index_core-0.9.55/llama_index/core/indices/knowledge_graph/__init__.py
--rw-r--r--   0        0        0    13153 2024-02-08 06:51:54.203152 llama_index_core-0.9.55/llama_index/core/indices/knowledge_graph/base.py
--rw-r--r--   0        0        0    34765 2024-02-08 06:51:54.203284 llama_index_core-0.9.55/llama_index/core/indices/knowledge_graph/retrievers.py
--rw-r--r--   0        0        0     1022 2024-02-08 06:51:54.203643 llama_index_core-0.9.55/llama_index/core/indices/list/README.md
--rw-r--r--   0        0        0      645 2024-02-08 06:51:54.203773 llama_index_core-0.9.55/llama_index/core/indices/list/__init__.py
--rw-r--r--   0        0        0     5446 2024-02-08 06:51:54.203854 llama_index_core-0.9.55/llama_index/core/indices/list/base.py
--rw-r--r--   0        0        0     8249 2024-02-08 06:51:54.203939 llama_index_core-0.9.55/llama_index/core/indices/list/retrievers.py
--rw-r--r--   0        0        0     3602 2024-02-08 06:51:54.204029 llama_index_core-0.9.55/llama_index/core/indices/loading.py
--rw-r--r--   0        0        0      106 2024-02-08 06:51:54.204360 llama_index_core-0.9.55/llama_index/core/indices/managed/__init__.py
--rw-r--r--   0        0        0     3718 2024-02-08 06:51:54.204451 llama_index_core-0.9.55/llama_index/core/indices/managed/base.py
--rw-r--r--   0        0        0      172 2024-02-08 06:51:54.204541 llama_index_core-0.9.55/llama_index/core/indices/managed/types.py
--rw-r--r--   0        0        0      310 2024-02-08 06:51:54.204660 llama_index_core-0.9.55/llama_index/core/indices/multi_modal/__init__.py
--rw-r--r--   0        0        0    16441 2024-02-08 06:51:54.204758 llama_index_core-0.9.55/llama_index/core/indices/multi_modal/base.py
--rw-r--r--   0        0        0    15510 2024-02-08 06:51:54.204917 llama_index_core-0.9.55/llama_index/core/indices/multi_modal/retriever.py
--rw-r--r--   0        0        0     1361 2024-02-08 06:51:54.204990 llama_index_core-0.9.55/llama_index/core/indices/postprocessor.py
--rw-r--r--   0        0        0    10492 2024-02-08 06:51:54.205077 llama_index_core-0.9.55/llama_index/core/indices/prompt_helper.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.205146 llama_index_core-0.9.55/llama_index/core/indices/query/__init__.py
--rw-r--r--   0        0        0      136 2024-02-08 06:51:54.205232 llama_index_core-0.9.55/llama_index/core/indices/query/base.py
--rw-r--r--   0        0        0     6109 2024-02-08 06:51:54.205313 llama_index_core-0.9.55/llama_index/core/indices/query/embedding_utils.py
--rw-r--r--   0        0        0      286 2024-02-08 06:51:54.205438 llama_index_core-0.9.55/llama_index/core/indices/query/query_transform/__init__.py
--rw-r--r--   0        0        0    12479 2024-02-08 06:51:54.205572 llama_index_core-0.9.55/llama_index/core/indices/query/query_transform/base.py
--rw-r--r--   0        0        0     4548 2024-02-08 06:51:54.205646 llama_index_core-0.9.55/llama_index/core/indices/query/query_transform/feedback_transform.py
--rw-r--r--   0        0        0     5200 2024-02-08 06:51:54.205719 llama_index_core-0.9.55/llama_index/core/indices/query/query_transform/prompts.py
--rw-r--r--   0        0        0      129 2024-02-08 06:51:54.205780 llama_index_core-0.9.55/llama_index/core/indices/query/schema.py
--rw-r--r--   0        0        0     1442 2024-02-08 06:51:54.205843 llama_index_core-0.9.55/llama_index/core/indices/registry.py
--rw-r--r--   0        0        0      127 2024-02-08 06:51:54.205908 llama_index_core-0.9.55/llama_index/core/indices/service_context.py
--rw-r--r--   0        0        0      988 2024-02-08 06:51:54.206009 llama_index_core-0.9.55/llama_index/core/indices/struct_store/__init__.py
--rw-r--r--   0        0        0     2411 2024-02-08 06:51:54.206090 llama_index_core-0.9.55/llama_index/core/indices/struct_store/base.py
--rw-r--r--   0        0        0     5761 2024-02-08 06:51:54.206162 llama_index_core-0.9.55/llama_index/core/indices/struct_store/container_builder.py
--rw-r--r--   0        0        0     8036 2024-02-08 06:51:54.206246 llama_index_core-0.9.55/llama_index/core/indices/struct_store/json_query.py
--rw-r--r--   0        0        0     2610 2024-02-08 06:51:54.206323 llama_index_core-0.9.55/llama_index/core/indices/struct_store/pandas.py
--rw-r--r--   0        0        0     6472 2024-02-08 06:51:54.206403 llama_index_core-0.9.55/llama_index/core/indices/struct_store/sql.py
--rw-r--r--   0        0        0    20387 2024-02-08 06:51:54.206502 llama_index_core-0.9.55/llama_index/core/indices/struct_store/sql_query.py
--rw-r--r--   0        0        0    15704 2024-02-08 06:51:54.206633 llama_index_core-0.9.55/llama_index/core/indices/struct_store/sql_retriever.py
--rw-r--r--   0        0        0     2645 2024-02-08 06:51:54.206770 llama_index_core-0.9.55/llama_index/core/indices/tree/README.md
--rw-r--r--   0        0        0      691 2024-02-08 06:51:54.206846 llama_index_core-0.9.55/llama_index/core/indices/tree/__init__.py
--rw-r--r--   0        0        0     1902 2024-02-08 06:51:54.206918 llama_index_core-0.9.55/llama_index/core/indices/tree/all_leaf_retriever.py
--rw-r--r--   0        0        0     7767 2024-02-08 06:51:54.207000 llama_index_core-0.9.55/llama_index/core/indices/tree/base.py
--rw-r--r--   0        0        0     8060 2024-02-08 06:51:54.207078 llama_index_core-0.9.55/llama_index/core/indices/tree/inserter.py
--rw-r--r--   0        0        0     6090 2024-02-08 06:51:54.207167 llama_index_core-0.9.55/llama_index/core/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0        0        0    15756 2024-02-08 06:51:54.207288 llama_index_core-0.9.55/llama_index/core/indices/tree/select_leaf_retriever.py
--rw-r--r--   0        0        0     1744 2024-02-08 06:51:54.207360 llama_index_core-0.9.55/llama_index/core/indices/tree/tree_root_retriever.py
--rw-r--r--   0        0        0      795 2024-02-08 06:51:54.207437 llama_index_core-0.9.55/llama_index/core/indices/tree/utils.py
--rw-r--r--   0        0        0     8309 2024-02-08 06:51:54.207528 llama_index_core-0.9.55/llama_index/core/indices/utils.py
--rw-r--r--   0        0        0      409 2024-02-08 06:51:54.207650 llama_index_core-0.9.55/llama_index/core/indices/vector_store/__init__.py
--rw-r--r--   0        0        0    14505 2024-02-08 06:51:54.207882 llama_index_core-0.9.55/llama_index/core/indices/vector_store/base.py
--rw-r--r--   0        0        0      300 2024-02-08 06:51:54.208004 llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/__init__.py
--rw-r--r--   0        0        0      172 2024-02-08 06:51:54.208132 llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0        0        0    10055 2024-02-08 06:51:54.208220 llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0        0        0      665 2024-02-08 06:51:54.208511 llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0        0        0     3989 2024-02-08 06:51:54.208825 llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0        0        0     7531 2024-02-08 06:51:54.208919 llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/retriever.py
--rw-r--r--   0        0        0      349 2024-02-08 06:51:54.209205 llama_index_core-0.9.55/llama_index/core/ingestion/__init__.py
--rw-r--r--   0        0        0     2635 2024-02-08 06:51:54.209296 llama_index_core-0.9.55/llama_index/core/ingestion/cache.py
--rw-r--r--   0        0        0    23537 2024-02-08 06:51:54.209402 llama_index_core-0.9.55/llama_index/core/ingestion/pipeline.py
--rw-r--r--   0        0        0      237 2024-02-08 06:51:54.209554 llama_index_core-0.9.55/llama_index/core/langchain_helpers/__init__.py
--rw-r--r--   0        0        0      529 2024-02-08 06:51:54.209689 llama_index_core-0.9.55/llama_index/core/langchain_helpers/agents/__init__.py
--rw-r--r--   0        0        0     2933 2024-02-08 06:51:54.209775 llama_index_core-0.9.55/llama_index/core/langchain_helpers/agents/agents.py
--rw-r--r--   0        0        0      835 2024-02-08 06:51:54.209853 llama_index_core-0.9.55/llama_index/core/langchain_helpers/agents/toolkits.py
--rw-r--r--   0        0        0     2517 2024-02-08 06:51:54.209941 llama_index_core-0.9.55/llama_index/core/langchain_helpers/agents/tools.py
--rw-r--r--   0        0        0     7653 2024-02-08 06:51:54.210027 llama_index_core-0.9.55/llama_index/core/langchain_helpers/memory_wrapper.py
--rw-r--r--   0        0        0     1352 2024-02-08 06:51:54.210110 llama_index_core-0.9.55/llama_index/core/langchain_helpers/streaming.py
--rw-r--r--   0        0        0       70 2024-02-08 06:51:54.210189 llama_index_core-0.9.55/llama_index/core/langchain_helpers/text_splitter.py
--rw-r--r--   0        0        0     1819 2024-02-08 06:51:54.210312 llama_index_core-0.9.55/llama_index/core/llama_dataset/__init__.py
--rw-r--r--   0        0        0    10610 2024-02-08 06:51:54.210403 llama_index_core-0.9.55/llama_index/core/llama_dataset/base.py
--rw-r--r--   0        0        0     3885 2024-02-08 06:51:54.211989 llama_index_core-0.9.55/llama_index/core/llama_dataset/download.py
--rw-r--r--   0        0        0    15965 2024-02-08 06:51:54.212388 llama_index_core-0.9.55/llama_index/core/llama_dataset/evaluator_evaluation.py
--rw-r--r--   0        0        0    10480 2024-02-08 06:51:54.212464 llama_index_core-0.9.55/llama_index/core/llama_dataset/generator.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.212518 llama_index_core-0.9.55/llama_index/core/llama_dataset/legacy/__init__.py
--rw-r--r--   0        0        0     3128 2024-02-08 06:51:54.212597 llama_index_core-0.9.55/llama_index/core/llama_dataset/legacy/embedding.py
--rw-r--r--   0        0        0     5384 2024-02-08 06:51:54.212667 llama_index_core-0.9.55/llama_index/core/llama_dataset/rag.py
--rw-r--r--   0        0        0      208 2024-02-08 06:51:54.212757 llama_index_core-0.9.55/llama_index/core/llama_pack/__init__.py
--rw-r--r--   0        0        0      293 2024-02-08 06:51:54.212810 llama_index_core-0.9.55/llama_index/core/llama_pack/base.py
--rw-r--r--   0        0        0     2314 2024-02-08 06:51:54.212868 llama_index_core-0.9.55/llama_index/core/llama_pack/download.py
--rw-r--r--   0        0        0      601 2024-02-08 06:51:54.212962 llama_index_core-0.9.55/llama_index/core/llms/__init__.py
--rw-r--r--   0        0        0     2594 2024-02-08 06:51:54.213019 llama_index_core-0.9.55/llama_index/core/llms/base.py
--rw-r--r--   0        0        0    10272 2024-02-08 06:51:54.213079 llama_index_core-0.9.55/llama_index/core/llms/callbacks.py
--rw-r--r--   0        0        0     2659 2024-02-08 06:51:54.213138 llama_index_core-0.9.55/llama_index/core/llms/custom.py
--rw-r--r--   0        0        0    10263 2024-02-08 06:51:54.213201 llama_index_core-0.9.55/llama_index/core/llms/generic_utils.py
--rw-r--r--   0        0        0    15383 2024-02-08 06:51:54.213314 llama_index_core-0.9.55/llama_index/core/llms/llm.py
--rw-r--r--   0        0        0      687 2024-02-08 06:51:54.213373 llama_index_core-0.9.55/llama_index/core/llms/loading.py
--rw-r--r--   0        0        0     2606 2024-02-08 06:51:54.213434 llama_index_core-0.9.55/llama_index/core/llms/mock.py
--rw-r--r--   0        0        0     3475 2024-02-08 06:51:54.213488 llama_index_core-0.9.55/llama_index/core/llms/utils.py
--rw-r--r--   0        0        0      171 2024-02-08 06:51:54.213760 llama_index_core-0.9.55/llama_index/core/memory/__init__.py
--rw-r--r--   0        0        0     5843 2024-02-08 06:51:54.213821 llama_index_core-0.9.55/llama_index/core/memory/chat_memory_buffer.py
--rw-r--r--   0        0        0     1279 2024-02-08 06:51:54.213887 llama_index_core-0.9.55/llama_index/core/memory/types.py
--rw-r--r--   0        0        0      166 2024-02-08 06:51:54.213998 llama_index_core-0.9.55/llama_index/core/multi_modal_llms/__init__.py
--rw-r--r--   0        0        0     7895 2024-02-08 06:51:54.214072 llama_index_core-0.9.55/llama_index/core/multi_modal_llms/base.py
--rw-r--r--   0        0        0     1772 2024-02-08 06:51:54.214135 llama_index_core-0.9.55/llama_index/core/multi_modal_llms/generic_utils.py
--rw-r--r--   0        0        0     1896 2024-02-08 06:51:54.214241 llama_index_core-0.9.55/llama_index/core/node_parser/__init__.py
--rw-r--r--   0        0        0      398 2024-02-08 06:51:54.214340 llama_index_core-0.9.55/llama_index/core/node_parser/file/__init__.py
--rw-r--r--   0        0        0     4202 2024-02-08 06:51:54.214402 llama_index_core-0.9.55/llama_index/core/node_parser/file/html.py
--rw-r--r--   0        0        0     3598 2024-02-08 06:51:54.214515 llama_index_core-0.9.55/llama_index/core/node_parser/file/json.py
--rw-r--r--   0        0        0     3974 2024-02-08 06:51:54.214589 llama_index_core-0.9.55/llama_index/core/node_parser/file/markdown.py
--rw-r--r--   0        0        0     2776 2024-02-08 06:51:54.214669 llama_index_core-0.9.55/llama_index/core/node_parser/file/simple_file.py
--rw-r--r--   0        0        0     6315 2024-02-08 06:51:54.214777 llama_index_core-0.9.55/llama_index/core/node_parser/interface.py
--rw-r--r--   0        0        0     1762 2024-02-08 06:51:54.214849 llama_index_core-0.9.55/llama_index/core/node_parser/loading.py
--rw-r--r--   0        0        0     3287 2024-02-08 06:51:54.214934 llama_index_core-0.9.55/llama_index/core/node_parser/node_utils.py
--rw-r--r--   0        0        0      428 2024-02-08 06:51:54.215063 llama_index_core-0.9.55/llama_index/core/node_parser/relational/__init__.py
--rw-r--r--   0        0        0    12471 2024-02-08 06:51:54.215213 llama_index_core-0.9.55/llama_index/core/node_parser/relational/base_element.py
--rw-r--r--   0        0        0     7649 2024-02-08 06:51:54.215305 llama_index_core-0.9.55/llama_index/core/node_parser/relational/hierarchical.py
--rw-r--r--   0        0        0     7995 2024-02-08 06:51:54.215385 llama_index_core-0.9.55/llama_index/core/node_parser/relational/markdown_element.py
--rw-r--r--   0        0        0     4432 2024-02-08 06:51:54.215661 llama_index_core-0.9.55/llama_index/core/node_parser/relational/unstructured_element.py
--rw-r--r--   0        0        0      655 2024-02-08 06:51:54.215792 llama_index_core-0.9.55/llama_index/core/node_parser/text/__init__.py
--rw-r--r--   0        0        0     5879 2024-02-08 06:51:54.215873 llama_index_core-0.9.55/llama_index/core/node_parser/text/code.py
--rw-r--r--   0        0        0     1767 2024-02-08 06:51:54.215949 llama_index_core-0.9.55/llama_index/core/node_parser/text/langchain.py
--rw-r--r--   0        0        0     8761 2024-02-08 06:51:54.216030 llama_index_core-0.9.55/llama_index/core/node_parser/text/semantic_splitter.py
--rw-r--r--   0        0        0    12203 2024-02-08 06:51:54.216131 llama_index_core-0.9.55/llama_index/core/node_parser/text/sentence.py
--rw-r--r--   0        0        0     5055 2024-02-08 06:51:54.216214 llama_index_core-0.9.55/llama_index/core/node_parser/text/sentence_window.py
--rw-r--r--   0        0        0     8604 2024-02-08 06:51:54.216297 llama_index_core-0.9.55/llama_index/core/node_parser/text/token.py
--rw-r--r--   0        0        0     2430 2024-02-08 06:51:54.216379 llama_index_core-0.9.55/llama_index/core/node_parser/text/utils.py
--rw-r--r--   0        0        0      600 2024-02-08 06:51:54.216525 llama_index_core-0.9.55/llama_index/core/objects/__init__.py
--rw-r--r--   0        0        0     6423 2024-02-08 06:51:54.216599 llama_index_core-0.9.55/llama_index/core/objects/base.py
--rw-r--r--   0        0        0     5404 2024-02-08 06:51:54.216677 llama_index_core-0.9.55/llama_index/core/objects/base_node_mapping.py
--rw-r--r--   0        0        0     3045 2024-02-08 06:51:54.216760 llama_index_core-0.9.55/llama_index/core/objects/table_node_mapping.py
--rw-r--r--   0        0        0     4878 2024-02-08 06:51:54.216852 llama_index_core-0.9.55/llama_index/core/objects/tool_node_mapping.py
--rw-r--r--   0        0        0      450 2024-02-08 06:51:54.216960 llama_index_core-0.9.55/llama_index/core/output_parsers/__init__.py
--rw-r--r--   0        0        0     2051 2024-02-08 06:51:54.217030 llama_index_core-0.9.55/llama_index/core/output_parsers/base.py
--rw-r--r--   0        0        0     1916 2024-02-08 06:51:54.217101 llama_index_core-0.9.55/llama_index/core/output_parsers/langchain.py
--rw-r--r--   0        0        0     2083 2024-02-08 06:51:54.217194 llama_index_core-0.9.55/llama_index/core/output_parsers/pydantic.py
--rw-r--r--   0        0        0     3343 2024-02-08 06:51:54.217274 llama_index_core-0.9.55/llama_index/core/output_parsers/selection.py
--rw-r--r--   0        0        0     3801 2024-02-08 06:51:54.217357 llama_index_core-0.9.55/llama_index/core/output_parsers/utils.py
--rw-r--r--   0        0        0      224 2024-02-08 06:51:54.217464 llama_index_core-0.9.55/llama_index/core/playground/__init__.py
--rw-r--r--   0        0        0     6957 2024-02-08 06:51:54.217549 llama_index_core-0.9.55/llama_index/core/playground/base.py
--rw-r--r--   0        0        0     1291 2024-02-08 06:51:54.217849 llama_index_core-0.9.55/llama_index/core/postprocessor/__init__.py
--rw-r--r--   0        0        0     4299 2024-02-08 06:51:54.217939 llama_index_core-0.9.55/llama_index/core/postprocessor/llm_rerank.py
--rw-r--r--   0        0        0     1067 2024-02-08 06:51:54.218035 llama_index_core-0.9.55/llama_index/core/postprocessor/metadata_replacement.py
--rw-r--r--   0        0        0    13644 2024-02-08 06:51:54.218180 llama_index_core-0.9.55/llama_index/core/postprocessor/node.py
--rw-r--r--   0        0        0     7114 2024-02-08 06:51:54.218263 llama_index_core-0.9.55/llama_index/core/postprocessor/node_recency.py
--rw-r--r--   0        0        0     6131 2024-02-08 06:51:54.218340 llama_index_core-0.9.55/llama_index/core/postprocessor/optimizer.py
--rw-r--r--   0        0        0     5312 2024-02-08 06:51:54.218412 llama_index_core-0.9.55/llama_index/core/postprocessor/pii.py
--rw-r--r--   0        0        0     6035 2024-02-08 06:51:54.218510 llama_index_core-0.9.55/llama_index/core/postprocessor/rankGPT_rerank.py
--rw-r--r--   0        0        0     3354 2024-02-08 06:51:54.218593 llama_index_core-0.9.55/llama_index/core/postprocessor/sbert_rerank.py
--rw-r--r--   0        0        0     4117 2024-02-08 06:51:54.218665 llama_index_core-0.9.55/llama_index/core/postprocessor/types.py
--rw-r--r--   0        0        0      342 2024-02-08 06:51:54.218782 llama_index_core-0.9.55/llama_index/core/program/__init__.py
--rw-r--r--   0        0        0     4564 2024-02-08 06:51:54.218882 llama_index_core-0.9.55/llama_index/core/program/llm_program.py
--rw-r--r--   0        0        0      983 2024-02-08 06:51:54.218953 llama_index_core-0.9.55/llama_index/core/program/llm_prompt_program.py
--rw-r--r--   0        0        0     4373 2024-02-08 06:51:54.219022 llama_index_core-0.9.55/llama_index/core/program/multi_modal_llm_program.py
--rw-r--r--   0        0        0     3631 2024-02-08 06:51:54.219093 llama_index_core-0.9.55/llama_index/core/program/utils.py
--rw-r--r--   0        0        0      608 2024-02-08 06:51:54.219223 llama_index_core-0.9.55/llama_index/core/prompts/__init__.py
--rw-r--r--   0        0        0    20346 2024-02-08 06:51:54.219326 llama_index_core-0.9.55/llama_index/core/prompts/base.py
--rw-r--r--   0        0        0     3620 2024-02-08 06:51:54.219427 llama_index_core-0.9.55/llama_index/core/prompts/chat_prompts.py
--rw-r--r--   0        0        0     1199 2024-02-08 06:51:54.219507 llama_index_core-0.9.55/llama_index/core/prompts/default_prompt_selectors.py
--rw-r--r--   0        0        0    16240 2024-02-08 06:51:54.219651 llama_index_core-0.9.55/llama_index/core/prompts/default_prompts.py
--rw-r--r--   0        0        0      524 2024-02-08 06:51:54.219726 llama_index_core-0.9.55/llama_index/core/prompts/display_utils.py
--rw-r--r--   0        0        0     5582 2024-02-08 06:51:54.219806 llama_index_core-0.9.55/llama_index/core/prompts/guidance_utils.py
--rw-r--r--   0        0        0     3277 2024-02-08 06:51:54.219884 llama_index_core-0.9.55/llama_index/core/prompts/mixin.py
--rw-r--r--   0        0        0     1780 2024-02-08 06:51:54.219984 llama_index_core-0.9.55/llama_index/core/prompts/prompt_type.py
--rw-r--r--   0        0        0     1098 2024-02-08 06:51:54.220059 llama_index_core-0.9.55/llama_index/core/prompts/prompt_utils.py
--rw-r--r--   0        0        0     3915 2024-02-08 06:51:54.220128 llama_index_core-0.9.55/llama_index/core/prompts/prompts.py
--rw-r--r--   0        0        0     4790 2024-02-08 06:51:54.220230 llama_index_core-0.9.55/llama_index/core/prompts/system.py
--rw-r--r--   0        0        0      501 2024-02-08 06:51:54.220322 llama_index_core-0.9.55/llama_index/core/prompts/utils.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.220354 llama_index_core-0.9.55/llama_index/core/py.typed
--rw-r--r--   0        0        0     2816 2024-02-08 06:51:54.220493 llama_index_core-0.9.55/llama_index/core/query_engine/__init__.py
--rw-r--r--   0        0        0    13229 2024-02-08 06:51:54.220615 llama_index_core-0.9.55/llama_index/core/query_engine/citation_query_engine.py
--rw-r--r--   0        0        0     2059 2024-02-08 06:51:54.220696 llama_index_core-0.9.55/llama_index/core/query_engine/cogniswitch_query_engine.py
--rw-r--r--   0        0        0     2955 2024-02-08 06:51:54.220780 llama_index_core-0.9.55/llama_index/core/query_engine/custom.py
--rw-r--r--   0        0        0       19 2024-02-08 06:51:54.220892 llama_index_core-0.9.55/llama_index/core/query_engine/flare/__init__.py
--rw-r--r--   0        0        0     6976 2024-02-08 06:51:54.220981 llama_index_core-0.9.55/llama_index/core/query_engine/flare/answer_inserter.py
--rw-r--r--   0        0        0    10753 2024-02-08 06:51:54.221080 llama_index_core-0.9.55/llama_index/core/query_engine/flare/base.py
--rw-r--r--   0        0        0     2088 2024-02-08 06:51:54.221161 llama_index_core-0.9.55/llama_index/core/query_engine/flare/output_parser.py
--rw-r--r--   0        0        0      163 2024-02-08 06:51:54.221229 llama_index_core-0.9.55/llama_index/core/query_engine/flare/schema.py
--rw-r--r--   0        0        0     4819 2024-02-08 06:51:54.221307 llama_index_core-0.9.55/llama_index/core/query_engine/graph_query_engine.py
--rw-r--r--   0        0        0    13068 2024-02-08 06:51:54.221449 llama_index_core-0.9.55/llama_index/core/query_engine/jsonalyze_query_engine.py
--rw-r--r--   0        0        0    10575 2024-02-08 06:51:54.221536 llama_index_core-0.9.55/llama_index/core/query_engine/knowledge_graph_query_engine.py
--rw-r--r--   0        0        0     9492 2024-02-08 06:51:54.221624 llama_index_core-0.9.55/llama_index/core/query_engine/multi_modal.py
--rw-r--r--   0        0        0     6755 2024-02-08 06:51:54.221699 llama_index_core-0.9.55/llama_index/core/query_engine/multistep_query_engine.py
--rw-r--r--   0        0        0      270 2024-02-08 06:51:54.221824 llama_index_core-0.9.55/llama_index/core/query_engine/pandas/__init__.py
--rw-r--r--   0        0        0     2963 2024-02-08 06:51:54.221911 llama_index_core-0.9.55/llama_index/core/query_engine/pandas/output_parser.py
--rw-r--r--   0        0        0     7191 2024-02-08 06:51:54.221990 llama_index_core-0.9.55/llama_index/core/query_engine/pandas/pandas_query_engine.py
--rw-r--r--   0        0        0     8428 2024-02-08 06:51:54.222071 llama_index_core-0.9.55/llama_index/core/query_engine/retriever_query_engine.py
--rw-r--r--   0        0        0     5363 2024-02-08 06:51:54.222160 llama_index_core-0.9.55/llama_index/core/query_engine/retry_query_engine.py
--rw-r--r--   0        0        0     3812 2024-02-08 06:51:54.222250 llama_index_core-0.9.55/llama_index/core/query_engine/retry_source_query_engine.py
--rw-r--r--   0        0        0    15724 2024-02-08 06:51:54.222366 llama_index_core-0.9.55/llama_index/core/query_engine/router_query_engine.py
--rw-r--r--   0        0        0    13916 2024-02-08 06:51:54.222491 llama_index_core-0.9.55/llama_index/core/query_engine/sql_join_query_engine.py
--rw-r--r--   0        0        0     7267 2024-02-08 06:51:54.222585 llama_index_core-0.9.55/llama_index/core/query_engine/sql_vector_query_engine.py
--rw-r--r--   0        0        0    11106 2024-02-08 06:51:54.222671 llama_index_core-0.9.55/llama_index/core/query_engine/sub_question_query_engine.py
--rw-r--r--   0        0        0     3427 2024-02-08 06:51:54.222746 llama_index_core-0.9.55/llama_index/core/query_engine/transform_query_engine.py
--rw-r--r--   0        0        0      793 2024-02-08 06:51:54.222857 llama_index_core-0.9.55/llama_index/core/query_pipeline/__init__.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.222947 llama_index_core-0.9.55/llama_index/core/query_pipeline/components/__init__.py
--rw-r--r--   0        0        0    10506 2024-02-08 06:51:54.223044 llama_index_core-0.9.55/llama_index/core/query_pipeline/components/agent.py
--rw-r--r--   0        0        0     3657 2024-02-08 06:51:54.223125 llama_index_core-0.9.55/llama_index/core/query_pipeline/components/argpacks.py
--rw-r--r--   0        0        0     3839 2024-02-08 06:51:54.223213 llama_index_core-0.9.55/llama_index/core/query_pipeline/components/function.py
--rw-r--r--   0        0        0     1563 2024-02-08 06:51:54.223311 llama_index_core-0.9.55/llama_index/core/query_pipeline/components/input.py
--rw-r--r--   0        0        0     6850 2024-02-08 06:51:54.223400 llama_index_core-0.9.55/llama_index/core/query_pipeline/components/router.py
--rw-r--r--   0        0        0     3780 2024-02-08 06:51:54.223490 llama_index_core-0.9.55/llama_index/core/query_pipeline/components/tool_runner.py
--rw-r--r--   0        0        0    21914 2024-02-08 06:51:54.223617 llama_index_core-0.9.55/llama_index/core/query_pipeline/query.py
--rw-r--r--   0        0        0      232 2024-02-08 06:51:54.223783 llama_index_core-0.9.55/llama_index/core/question_gen/__init__.py
--rw-r--r--   0        0        0     3803 2024-02-08 06:51:54.223873 llama_index_core-0.9.55/llama_index/core/question_gen/llm_generators.py
--rw-r--r--   0        0        0     1024 2024-02-08 06:51:54.223965 llama_index_core-0.9.55/llama_index/core/question_gen/output_parser.py
--rw-r--r--   0        0        0     1974 2024-02-08 06:51:54.224058 llama_index_core-0.9.55/llama_index/core/question_gen/prompts.py
--rw-r--r--   0        0        0     1009 2024-02-08 06:51:54.224154 llama_index_core-0.9.55/llama_index/core/question_gen/types.py
--rw-r--r--   0        0        0      929 2024-02-08 06:51:54.224294 llama_index_core-0.9.55/llama_index/core/readers/__init__.py
--rw-r--r--   0        0        0     2446 2024-02-08 06:51:54.224387 llama_index_core-0.9.55/llama_index/core/readers/base.py
--rw-r--r--   0        0        0     2438 2024-02-08 06:51:54.224472 llama_index_core-0.9.55/llama_index/core/readers/download.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.224575 llama_index_core-0.9.55/llama_index/core/readers/file/__init__.py
--rw-r--r--   0        0        0    15958 2024-02-08 06:51:54.224754 llama_index_core-0.9.55/llama_index/core/readers/file/base.py
--rw-r--r--   0        0        0     4665 2024-02-08 06:51:54.224872 llama_index_core-0.9.55/llama_index/core/readers/json.py
--rw-r--r--   0        0        0      784 2024-02-08 06:51:54.224959 llama_index_core-0.9.55/llama_index/core/readers/loading.py
--rw-r--r--   0        0        0     1196 2024-02-08 06:51:54.225060 llama_index_core-0.9.55/llama_index/core/readers/string_iterable.py
--rw-r--r--   0        0        0       83 2024-02-08 06:51:54.225179 llama_index_core-0.9.55/llama_index/core/response/__init__.py
--rw-r--r--   0        0        0     4904 2024-02-08 06:51:54.225260 llama_index_core-0.9.55/llama_index/core/response/notebook_utils.py
--rw-r--r--   0        0        0     1589 2024-02-08 06:51:54.225332 llama_index_core-0.9.55/llama_index/core/response/pprint_utils.py
--rw-r--r--   0        0        0      262 2024-02-08 06:51:54.225605 llama_index_core-0.9.55/llama_index/core/response/utils.py
--rw-r--r--   0        0        0      922 2024-02-08 06:51:54.225747 llama_index_core-0.9.55/llama_index/core/response_synthesizers/__init__.py
--rw-r--r--   0        0        0     5296 2024-02-08 06:51:54.225843 llama_index_core-0.9.55/llama_index/core/response_synthesizers/accumulate.py
--rw-r--r--   0        0        0     9574 2024-02-08 06:51:54.225932 llama_index_core-0.9.55/llama_index/core/response_synthesizers/base.py
--rw-r--r--   0        0        0     1823 2024-02-08 06:51:54.226014 llama_index_core-0.9.55/llama_index/core/response_synthesizers/compact_and_accumulate.py
--rw-r--r--   0        0        0     2004 2024-02-08 06:51:54.226100 llama_index_core-0.9.55/llama_index/core/response_synthesizers/compact_and_refine.py
--rw-r--r--   0        0        0     6672 2024-02-08 06:51:54.226180 llama_index_core-0.9.55/llama_index/core/response_synthesizers/factory.py
--rw-r--r--   0        0        0     2902 2024-02-08 06:51:54.226254 llama_index_core-0.9.55/llama_index/core/response_synthesizers/generation.py
--rw-r--r--   0        0        0      796 2024-02-08 06:51:54.226334 llama_index_core-0.9.55/llama_index/core/response_synthesizers/no_text.py
--rw-r--r--   0        0        0    18085 2024-02-08 06:51:54.226419 llama_index_core-0.9.55/llama_index/core/response_synthesizers/refine.py
--rw-r--r--   0        0        0     3766 2024-02-08 06:51:54.226526 llama_index_core-0.9.55/llama_index/core/response_synthesizers/simple_summarize.py
--rw-r--r--   0        0        0     8896 2024-02-08 06:51:54.226612 llama_index_core-0.9.55/llama_index/core/response_synthesizers/tree_summarize.py
--rw-r--r--   0        0        0     2011 2024-02-08 06:51:54.226694 llama_index_core-0.9.55/llama_index/core/response_synthesizers/type.py
--rw-r--r--   0        0        0     2419 2024-02-08 06:51:54.226828 llama_index_core-0.9.55/llama_index/core/retrievers/__init__.py
--rw-r--r--   0        0        0     7122 2024-02-08 06:51:54.226919 llama_index_core-0.9.55/llama_index/core/retrievers/auto_merging_retriever.py
--rw-r--r--   0        0        0     7926 2024-02-08 06:51:54.227013 llama_index_core-0.9.55/llama_index/core/retrievers/fusion_retriever.py
--rw-r--r--   0        0        0     7525 2024-02-08 06:51:54.227097 llama_index_core-0.9.55/llama_index/core/retrievers/recursive_retriever.py
--rw-r--r--   0        0        0     6104 2024-02-08 06:51:54.227197 llama_index_core-0.9.55/llama_index/core/retrievers/router_retriever.py
--rw-r--r--   0        0        0     1581 2024-02-08 06:51:54.227280 llama_index_core-0.9.55/llama_index/core/retrievers/transform_retriever.py
--rw-r--r--   0        0        0    23388 2024-02-08 06:51:54.227394 llama_index_core-0.9.55/llama_index/core/schema.py
--rw-r--r--   0        0        0      456 2024-02-08 06:51:54.227583 llama_index_core-0.9.55/llama_index/core/selectors/__init__.py
--rw-r--r--   0        0        0     3052 2024-02-08 06:51:54.227678 llama_index_core-0.9.55/llama_index/core/selectors/embedding_selectors.py
--rw-r--r--   0        0        0     7898 2024-02-08 06:51:54.227769 llama_index_core-0.9.55/llama_index/core/selectors/llm_selectors.py
--rw-r--r--   0        0        0     2985 2024-02-08 06:51:54.227862 llama_index_core-0.9.55/llama_index/core/selectors/prompts.py
--rw-r--r--   0        0        0     5496 2024-02-08 06:51:54.227958 llama_index_core-0.9.55/llama_index/core/selectors/pydantic_selectors.py
--rw-r--r--   0        0        0     3333 2024-02-08 06:51:54.228046 llama_index_core-0.9.55/llama_index/core/selectors/types.py
--rw-r--r--   0        0        0     1021 2024-02-08 06:51:54.228128 llama_index_core-0.9.55/llama_index/core/selectors/utils.py
--rw-r--r--   0        0        0    15655 2024-02-08 06:51:54.228275 llama_index_core-0.9.55/llama_index/core/service_context.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.228372 llama_index_core-0.9.55/llama_index/core/service_context_elements/__init__.py
--rw-r--r--   0        0        0      995 2024-02-08 06:51:54.228479 llama_index_core-0.9.55/llama_index/core/service_context_elements/llama_logger.py
--rw-r--r--   0        0        0    11826 2024-02-08 06:51:54.228588 llama_index_core-0.9.55/llama_index/core/service_context_elements/llm_predictor.py
--rw-r--r--   0        0        0     9970 2024-02-08 06:51:54.228685 llama_index_core-0.9.55/llama_index/core/settings.py
--rw-r--r--   0        0        0      129 2024-02-08 06:51:54.228824 llama_index_core-0.9.55/llama_index/core/storage/__init__.py
--rw-r--r--   0        0        0      197 2024-02-08 06:51:54.228990 llama_index_core-0.9.55/llama_index/core/storage/chat_store/__init__.py
--rw-r--r--   0        0        0     1336 2024-02-08 06:51:54.229292 llama_index_core-0.9.55/llama_index/core/storage/chat_store/base.py
--rw-r--r--   0        0        0      668 2024-02-08 06:51:54.229387 llama_index_core-0.9.55/llama_index/core/storage/chat_store/loading.py
--rw-r--r--   0        0        0     2821 2024-02-08 06:51:54.229473 llama_index_core-0.9.55/llama_index/core/storage/chat_store/simple_chat_store.py
--rw-r--r--   0        0        0      304 2024-02-08 06:51:54.229610 llama_index_core-0.9.55/llama_index/core/storage/docstore/__init__.py
--rw-r--r--   0        0        0    20499 2024-02-08 06:51:54.229717 llama_index_core-0.9.55/llama_index/core/storage/docstore/keyval_docstore.py
--rw-r--r--   0        0        0     2497 2024-02-08 06:51:54.229842 llama_index_core-0.9.55/llama_index/core/storage/docstore/postgres_docstore.py
--rw-r--r--   0        0        0      648 2024-02-08 06:51:54.229928 llama_index_core-0.9.55/llama_index/core/storage/docstore/registry.py
--rw-r--r--   0        0        0     3292 2024-02-08 06:51:54.230014 llama_index_core-0.9.55/llama_index/core/storage/docstore/simple_docstore.py
--rw-r--r--   0        0        0     6635 2024-02-08 06:51:54.230101 llama_index_core-0.9.55/llama_index/core/storage/docstore/types.py
--rw-r--r--   0        0        0     2606 2024-02-08 06:51:54.230188 llama_index_core-0.9.55/llama_index/core/storage/docstore/utils.py
--rw-r--r--   0        0        0      133 2024-02-08 06:51:54.230320 llama_index_core-0.9.55/llama_index/core/storage/index_store/__init__.py
--rw-r--r--   0        0        0     2242 2024-02-08 06:51:54.230422 llama_index_core-0.9.55/llama_index/core/storage/index_store/keyval_index_store.py
--rw-r--r--   0        0        0     2280 2024-02-08 06:51:54.230502 llama_index_core-0.9.55/llama_index/core/storage/index_store/postgres_index_store.py
--rw-r--r--   0        0        0     2365 2024-02-08 06:51:54.230591 llama_index_core-0.9.55/llama_index/core/storage/index_store/simple_index_store.py
--rw-r--r--   0        0        0      959 2024-02-08 06:51:54.230672 llama_index_core-0.9.55/llama_index/core/storage/index_store/types.py
--rw-r--r--   0        0        0      692 2024-02-08 06:51:54.230757 llama_index_core-0.9.55/llama_index/core/storage/index_store/utils.py
--rw-r--r--   0        0        0      157 2024-02-08 06:51:54.230905 llama_index_core-0.9.55/llama_index/core/storage/kvstore/__init__.py
--rw-r--r--   0        0        0    14770 2024-02-08 06:51:54.231249 llama_index_core-0.9.55/llama_index/core/storage/kvstore/postgres_kvstore.py
--rw-r--r--   0        0        0     3482 2024-02-08 06:51:54.231336 llama_index_core-0.9.55/llama_index/core/storage/kvstore/simple_kvstore.py
--rw-r--r--   0        0        0     2533 2024-02-08 06:51:54.231419 llama_index_core-0.9.55/llama_index/core/storage/kvstore/types.py
--rw-r--r--   0        0        0     8902 2024-02-08 06:51:54.231513 llama_index_core-0.9.55/llama_index/core/storage/storage_context.py
--rw-r--r--   0        0        0      356 2024-02-08 06:51:54.231659 llama_index_core-0.9.55/llama_index/core/text_splitter/__init__.py
--rw-r--r--   0        0        0      682 2024-02-08 06:51:54.231931 llama_index_core-0.9.55/llama_index/core/tools/__init__.py
--rw-r--r--   0        0        0     1898 2024-02-08 06:51:54.232023 llama_index_core-0.9.55/llama_index/core/tools/download.py
--rw-r--r--   0        0        0     4099 2024-02-08 06:51:54.232106 llama_index_core-0.9.55/llama_index/core/tools/function_tool.py
--rw-r--r--   0        0        0     5861 2024-02-08 06:51:54.232190 llama_index_core-0.9.55/llama_index/core/tools/ondemand_loader_tool.py
--rw-r--r--   0        0        0     3791 2024-02-08 06:51:54.232276 llama_index_core-0.9.55/llama_index/core/tools/query_engine.py
--rw-r--r--   0        0        0     7692 2024-02-08 06:51:54.232385 llama_index_core-0.9.55/llama_index/core/tools/query_plan.py
--rw-r--r--   0        0        0     3600 2024-02-08 06:51:54.232467 llama_index_core-0.9.55/llama_index/core/tools/retriever_tool.py
--rw-r--r--   0        0        0       19 2024-02-08 06:51:54.232597 llama_index_core-0.9.55/llama_index/core/tools/tool_spec/__init__.py
--rw-r--r--   0        0        0     4575 2024-02-08 06:51:54.232693 llama_index_core-0.9.55/llama_index/core/tools/tool_spec/base.py
--rw-r--r--   0        0        0     1139 2024-02-08 06:51:54.232844 llama_index_core-0.9.55/llama_index/core/tools/tool_spec/load_and_search/README.md
--rw-r--r--   0        0        0      134 2024-02-08 06:51:54.232931 llama_index_core-0.9.55/llama_index/core/tools/tool_spec/load_and_search/__init__.py
--rw-r--r--   0        0        0     5061 2024-02-08 06:51:54.233036 llama_index_core-0.9.55/llama_index/core/tools/tool_spec/load_and_search/base.py
--rw-r--r--   0        0        0     5659 2024-02-08 06:51:54.233124 llama_index_core-0.9.55/llama_index/core/tools/types.py
--rw-r--r--   0        0        0     1925 2024-02-08 06:51:54.233198 llama_index_core-0.9.55/llama_index/core/tools/utils.py
--rw-r--r--   0        0        0     2208 2024-02-08 06:51:54.233283 llama_index_core-0.9.55/llama_index/core/types.py
--rw-r--r--   0        0        0        0 2024-02-08 06:51:54.233354 llama_index_core-0.9.55/llama_index/core/utilities/__init__.py
--rw-r--r--   0        0        0     1644 2024-02-08 06:51:54.233443 llama_index_core-0.9.55/llama_index/core/utilities/aws_utils.py
--rw-r--r--   0        0        0     9634 2024-02-08 06:51:54.233527 llama_index_core-0.9.55/llama_index/core/utilities/sql_wrapper.py
--rw-r--r--   0        0        0     2674 2024-02-08 06:51:54.233599 llama_index_core-0.9.55/llama_index/core/utilities/token_counting.py
--rw-r--r--   0        0        0    14400 2024-02-08 06:51:54.233730 llama_index_core-0.9.55/llama_index/core/utils.py
--rw-r--r--   0        0        0      506 2024-02-08 06:51:54.233871 llama_index_core-0.9.55/llama_index/core/vector_stores/__init__.py
--rw-r--r--   0        0        0    11220 2024-02-08 06:51:54.234181 llama_index_core-0.9.55/llama_index/core/vector_stores/simple.py
--rw-r--r--   0        0        0    10662 2024-02-08 06:51:54.234255 llama_index_core-0.9.55/llama_index/core/vector_stores/types.py
--rw-r--r--   0        0        0     4593 2024-02-08 06:51:54.234337 llama_index_core-0.9.55/llama_index/core/vector_stores/utils.py
--rw-r--r--   0        0        0     6376 2024-02-08 06:59:24.874507 llama_index_core-0.9.55/pyproject.toml
--rw-r--r--   0        0        0     2957 1970-01-01 00:00:00.000000 llama_index_core-0.9.55/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-02-08 20:02:33.965952 llama_index_core-0.9.56/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.966050 llama_index_core-0.9.56/README.md
+-rw-r--r--   0        0        0       13 2024-02-08 20:02:33.966406 llama_index_core-0.9.56/llama_index/core/VERSION
+-rw-r--r--   0        0        0     3975 2024-02-08 20:02:33.966795 llama_index_core-0.9.56/llama_index/core/__init__.py
+-rw-r--r--   0        0        0       46 2024-02-08 20:02:33.966894 llama_index_core-0.9.56/llama_index/core/_static/.gitignore
+-rw-r--r--   0        0        0       32 2024-02-08 20:02:33.967171 llama_index_core-0.9.56/llama_index/core/_static/nltk_cache/.gitignore
+-rw-r--r--   0        0        0       32 2024-02-08 20:02:33.967266 llama_index_core-0.9.56/llama_index/core/_static/tiktoken_cache/.gitignore
+-rw-r--r--   0        0        0     1031 2024-02-08 20:02:33.967545 llama_index_core-0.9.56/llama_index/core/agent/__init__.py
+-rw-r--r--   0        0        0       19 2024-02-08 20:02:33.967718 llama_index_core-0.9.56/llama_index/core/agent/custom/__init__.py
+-rw-r--r--   0        0        0     6424 2024-02-08 20:02:33.967836 llama_index_core-0.9.56/llama_index/core/agent/custom/pipeline_worker.py
+-rw-r--r--   0        0        0     8533 2024-02-08 20:02:33.967994 llama_index_core-0.9.56/llama_index/core/agent/custom/simple.py
+-rw-r--r--   0        0        0       19 2024-02-08 20:02:33.968093 llama_index_core-0.9.56/llama_index/core/agent/legacy/__init__.py
+-rw-r--r--   0        0        0       19 2024-02-08 20:02:33.968205 llama_index_core-0.9.56/llama_index/core/agent/legacy/react/__init__.py
+-rw-r--r--   0        0        0    19427 2024-02-08 20:02:33.968309 llama_index_core-0.9.56/llama_index/core/agent/legacy/react/base.py
+-rw-r--r--   0        0        0      258 2024-02-08 20:02:33.968793 llama_index_core-0.9.56/llama_index/core/agent/react/__init__.py
+-rw-r--r--   0        0        0      190 2024-02-08 20:02:33.969338 llama_index_core-0.9.56/llama_index/core/agent/react/agent.py
+-rw-r--r--   0        0        0     4290 2024-02-08 20:02:33.969426 llama_index_core-0.9.56/llama_index/core/agent/react/base.py
+-rw-r--r--   0        0        0     4107 2024-02-08 20:02:33.969509 llama_index_core-0.9.56/llama_index/core/agent/react/formatter.py
+-rw-r--r--   0        0        0     3733 2024-02-08 20:02:33.969587 llama_index_core-0.9.56/llama_index/core/agent/react/output_parser.py
+-rw-r--r--   0        0        0     3408 2024-02-08 20:02:33.969799 llama_index_core-0.9.56/llama_index/core/agent/react/prompts.py
+-rw-r--r--   0        0        0    23654 2024-02-08 20:02:33.969923 llama_index_core-0.9.56/llama_index/core/agent/react/step.py
+-rw-r--r--   0        0        0     1797 2024-02-08 20:02:33.970239 llama_index_core-0.9.56/llama_index/core/agent/react/types.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.970305 llama_index_core-0.9.56/llama_index/core/agent/react_multimodal/__init__.py
+-rw-r--r--   0        0        0     2839 2024-02-08 20:02:33.970565 llama_index_core-0.9.56/llama_index/core/agent/react_multimodal/prompts.py
+-rw-r--r--   0        0        0    18603 2024-02-08 20:02:33.970675 llama_index_core-0.9.56/llama_index/core/agent/react_multimodal/step.py
+-rw-r--r--   0        0        0       19 2024-02-08 20:02:33.970970 llama_index_core-0.9.56/llama_index/core/agent/runner/__init__.py
+-rw-r--r--   0        0        0    20460 2024-02-08 20:02:33.971065 llama_index_core-0.9.56/llama_index/core/agent/runner/base.py
+-rw-r--r--   0        0        0    15699 2024-02-08 20:02:33.971505 llama_index_core-0.9.56/llama_index/core/agent/runner/parallel.py
+-rw-r--r--   0        0        0     7147 2024-02-08 20:02:33.971588 llama_index_core-0.9.56/llama_index/core/agent/types.py
+-rw-r--r--   0        0        0      545 2024-02-08 20:02:33.971663 llama_index_core-0.9.56/llama_index/core/agent/utils.py
+-rw-r--r--   0        0        0     2926 2024-02-08 20:02:33.971740 llama_index_core-0.9.56/llama_index/core/async_utils.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.971802 llama_index_core-0.9.56/llama_index/core/base/__init__.py
+-rw-r--r--   0        0        0     1627 2024-02-08 20:02:33.971881 llama_index_core-0.9.56/llama_index/core/base/base_auto_retriever.py
+-rw-r--r--   0        0        0     1788 2024-02-08 20:02:33.971959 llama_index_core-0.9.56/llama_index/core/base/base_multi_modal_retriever.py
+-rw-r--r--   0        0        0     4216 2024-02-08 20:02:33.972043 llama_index_core-0.9.56/llama_index/core/base/base_query_engine.py
+-rw-r--r--   0        0        0    11946 2024-02-08 20:02:33.972155 llama_index_core-0.9.56/llama_index/core/base/base_retriever.py
+-rw-r--r--   0        0        0     3333 2024-02-08 20:02:33.972226 llama_index_core-0.9.56/llama_index/core/base/base_selector.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.972283 llama_index_core-0.9.56/llama_index/core/base/embeddings/__init__.py
+-rw-r--r--   0        0        0    12474 2024-02-08 20:02:33.972759 llama_index_core-0.9.56/llama_index/core/base/embeddings/base.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.972866 llama_index_core-0.9.56/llama_index/core/base/llms/__init__.py
+-rw-r--r--   0        0        0     3778 2024-02-08 20:02:33.973873 llama_index_core-0.9.56/llama_index/core/base/llms/types.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.973947 llama_index_core-0.9.56/llama_index/core/base/query_pipeline/__init__.py
+-rw-r--r--   0        0        0    10619 2024-02-08 20:02:33.974051 llama_index_core-0.9.56/llama_index/core/base/query_pipeline/query.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.974120 llama_index_core-0.9.56/llama_index/core/base/response/__init__.py
+-rw-r--r--   0        0        0     4748 2024-02-08 20:02:33.974511 llama_index_core-0.9.56/llama_index/core/base/response/schema.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.974586 llama_index_core-0.9.56/llama_index/core/bridge/__init__.py
+-rw-r--r--   0        0        0     2809 2024-02-08 20:02:33.974690 llama_index_core-0.9.56/llama_index/core/bridge/langchain.py
+-rw-r--r--   0        0        0     1132 2024-02-08 20:02:33.974751 llama_index_core-0.9.56/llama_index/core/bridge/pydantic.py
+-rw-r--r--   0        0        0      378 2024-02-08 20:02:33.974993 llama_index_core-0.9.56/llama_index/core/callbacks/__init__.py
+-rw-r--r--   0        0        0    10389 2024-02-08 20:02:33.975326 llama_index_core-0.9.56/llama_index/core/callbacks/base.py
+-rw-r--r--   0        0        0     1664 2024-02-08 20:02:33.975520 llama_index_core-0.9.56/llama_index/core/callbacks/base_handler.py
+-rw-r--r--   0        0        0     3726 2024-02-08 20:02:33.975590 llama_index_core-0.9.56/llama_index/core/callbacks/global_handlers.py
+-rw-r--r--   0        0        0     7866 2024-02-08 20:02:33.975675 llama_index_core-0.9.56/llama_index/core/callbacks/llama_debug.py
+-rw-r--r--   0        0        0     3572 2024-02-08 20:02:33.975749 llama_index_core-0.9.56/llama_index/core/callbacks/schema.py
+-rw-r--r--   0        0        0     2161 2024-02-08 20:02:33.975953 llama_index_core-0.9.56/llama_index/core/callbacks/simple_llm_handler.py
+-rw-r--r--   0        0        0     7679 2024-02-08 20:02:33.976086 llama_index_core-0.9.56/llama_index/core/callbacks/token_counting.py
+-rw-r--r--   0        0        0     2174 2024-02-08 20:02:33.976180 llama_index_core-0.9.56/llama_index/core/callbacks/utils.py
+-rw-r--r--   0        0        0      464 2024-02-08 20:02:33.976328 llama_index_core-0.9.56/llama_index/core/chat_engine/__init__.py
+-rw-r--r--   0        0        0    14037 2024-02-08 20:02:33.976417 llama_index_core-0.9.56/llama_index/core/chat_engine/condense_plus_context.py
+-rw-r--r--   0        0        0    14398 2024-02-08 20:02:33.976503 llama_index_core-0.9.56/llama_index/core/chat_engine/condense_question.py
+-rw-r--r--   0        0        0    11385 2024-02-08 20:02:33.976589 llama_index_core-0.9.56/llama_index/core/chat_engine/context.py
+-rw-r--r--   0        0        0     6274 2024-02-08 20:02:33.976666 llama_index_core-0.9.56/llama_index/core/chat_engine/simple.py
+-rw-r--r--   0        0        0    11130 2024-02-08 20:02:33.976756 llama_index_core-0.9.56/llama_index/core/chat_engine/types.py
+-rw-r--r--   0        0        0      476 2024-02-08 20:02:33.976819 llama_index_core-0.9.56/llama_index/core/chat_engine/utils.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.976884 llama_index_core-0.9.56/llama_index/core/command_line/__init__.py
+-rw-r--r--   0        0        0     7000 2024-02-08 20:02:33.976976 llama_index_core-0.9.56/llama_index/core/command_line/command_line.py
+-rw-r--r--   0        0        0    45435 2024-02-08 20:02:33.977110 llama_index_core-0.9.56/llama_index/core/command_line/mappings.json
+-rw-r--r--   0        0        0    15052 2024-02-08 20:02:33.977237 llama_index_core-0.9.56/llama_index/core/command_line/rag.py
+-rw-r--r--   0        0        0     8428 2024-02-08 20:02:33.977334 llama_index_core-0.9.56/llama_index/core/command_line/upgrade.py
+-rw-r--r--   0        0        0      251 2024-02-08 20:02:33.977460 llama_index_core-0.9.56/llama_index/core/composability/__init__.py
+-rw-r--r--   0        0        0      170 2024-02-08 20:02:33.977535 llama_index_core-0.9.56/llama_index/core/composability/base.py
+-rw-r--r--   0        0        0     4762 2024-02-08 20:02:33.977757 llama_index_core-0.9.56/llama_index/core/composability/joint_qa_summary.py
+-rw-r--r--   0        0        0      703 2024-02-08 20:02:33.977844 llama_index_core-0.9.56/llama_index/core/constants.py
+-rw-r--r--   0        0        0      337 2024-02-08 20:02:33.978135 llama_index_core-0.9.56/llama_index/core/data_structs/__init__.py
+-rw-r--r--   0        0        0     8110 2024-02-08 20:02:33.978474 llama_index_core-0.9.56/llama_index/core/data_structs/data_structs.py
+-rw-r--r--   0        0        0     2518 2024-02-08 20:02:33.978563 llama_index_core-0.9.56/llama_index/core/data_structs/document_summary.py
+-rw-r--r--   0        0        0     1026 2024-02-08 20:02:33.978848 llama_index_core-0.9.56/llama_index/core/data_structs/registry.py
+-rw-r--r--   0        0        0     4292 2024-02-08 20:02:33.978958 llama_index_core-0.9.56/llama_index/core/data_structs/struct_type.py
+-rw-r--r--   0        0        0     1035 2024-02-08 20:02:33.979051 llama_index_core-0.9.56/llama_index/core/data_structs/table.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.979113 llama_index_core-0.9.56/llama_index/core/download/__init__.py
+-rw-r--r--   0        0        0     8995 2024-02-08 20:02:33.979236 llama_index_core-0.9.56/llama_index/core/download/dataset.py
+-rw-r--r--   0        0        0      975 2024-02-08 20:02:33.979313 llama_index_core-0.9.56/llama_index/core/download/integration.py
+-rw-r--r--   0        0        0     9553 2024-02-08 20:02:33.979425 llama_index_core-0.9.56/llama_index/core/download/module.py
+-rw-r--r--   0        0        0     4702 2024-02-08 20:02:33.979514 llama_index_core-0.9.56/llama_index/core/download/pack.py
+-rw-r--r--   0        0        0     3239 2024-02-08 20:02:33.979580 llama_index_core-0.9.56/llama_index/core/download/utils.py
+-rw-r--r--   0        0        0      348 2024-02-08 20:02:33.979672 llama_index_core-0.9.56/llama_index/core/embeddings/__init__.py
+-rw-r--r--   0        0        0      708 2024-02-08 20:02:33.979736 llama_index_core-0.9.56/llama_index/core/embeddings/loading.py
+-rw-r--r--   0        0        0     1081 2024-02-08 20:02:33.979796 llama_index_core-0.9.56/llama_index/core/embeddings/mock_embed_model.py
+-rw-r--r--   0        0        0     6837 2024-02-08 20:02:33.979873 llama_index_core-0.9.56/llama_index/core/embeddings/multi_modal_base.py
+-rw-r--r--   0        0        0     1452 2024-02-08 20:02:33.979936 llama_index_core-0.9.56/llama_index/core/embeddings/pooling.py
+-rw-r--r--   0        0        0     4804 2024-02-08 20:02:33.980000 llama_index_core-0.9.56/llama_index/core/embeddings/utils.py
+-rw-r--r--   0        0        0     2636 2024-02-08 20:02:33.980253 llama_index_core-0.9.56/llama_index/core/evaluation/__init__.py
+-rw-r--r--   0        0        0     5550 2024-02-08 20:02:33.980335 llama_index_core-0.9.56/llama_index/core/evaluation/answer_relevancy.py
+-rw-r--r--   0        0        0     4070 2024-02-08 20:02:33.980591 llama_index_core-0.9.56/llama_index/core/evaluation/base.py
+-rw-r--r--   0        0        0    11242 2024-02-08 20:02:33.980673 llama_index_core-0.9.56/llama_index/core/evaluation/batch_runner.py
+-rw-r--r--   0        0        0      198 2024-02-08 20:02:33.980952 llama_index_core-0.9.56/llama_index/core/evaluation/benchmarks/__init__.py
+-rw-r--r--   0        0        0     4195 2024-02-08 20:02:33.981018 llama_index_core-0.9.56/llama_index/core/evaluation/benchmarks/beir.py
+-rw-r--r--   0        0        0     7602 2024-02-08 20:02:33.981087 llama_index_core-0.9.56/llama_index/core/evaluation/benchmarks/hotpotqa.py
+-rw-r--r--   0        0        0     7011 2024-02-08 20:02:33.981160 llama_index_core-0.9.56/llama_index/core/evaluation/context_relevancy.py
+-rw-r--r--   0        0        0     5162 2024-02-08 20:02:33.981227 llama_index_core-0.9.56/llama_index/core/evaluation/correctness.py
+-rw-r--r--   0        0        0    12903 2024-02-08 20:02:33.981291 llama_index_core-0.9.56/llama_index/core/evaluation/dataset_generation.py
+-rw-r--r--   0        0        0     2199 2024-02-08 20:02:33.981351 llama_index_core-0.9.56/llama_index/core/evaluation/eval_utils.py
+-rw-r--r--   0        0        0     6276 2024-02-08 20:02:33.981421 llama_index_core-0.9.56/llama_index/core/evaluation/faithfulness.py
+-rw-r--r--   0        0        0     4453 2024-02-08 20:02:33.981502 llama_index_core-0.9.56/llama_index/core/evaluation/guideline.py
+-rw-r--r--   0        0        0      324 2024-02-08 20:02:33.981595 llama_index_core-0.9.56/llama_index/core/evaluation/multi_modal/__init__.py
+-rw-r--r--   0        0        0     8140 2024-02-08 20:02:33.981671 llama_index_core-0.9.56/llama_index/core/evaluation/multi_modal/faithfulness.py
+-rw-r--r--   0        0        0     7206 2024-02-08 20:02:33.981753 llama_index_core-0.9.56/llama_index/core/evaluation/multi_modal/relevancy.py
+-rw-r--r--   0        0        0     2321 2024-02-08 20:02:33.981825 llama_index_core-0.9.56/llama_index/core/evaluation/notebook_utils.py
+-rw-r--r--   0        0        0    10344 2024-02-08 20:02:33.981903 llama_index_core-0.9.56/llama_index/core/evaluation/pairwise.py
+-rw-r--r--   0        0        0     5357 2024-02-08 20:02:33.981968 llama_index_core-0.9.56/llama_index/core/evaluation/relevancy.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.982023 llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/__init__.py
+-rw-r--r--   0        0        0     6353 2024-02-08 20:02:33.982104 llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/base.py
+-rw-r--r--   0        0        0     4606 2024-02-08 20:02:33.982165 llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/evaluator.py
+-rw-r--r--   0        0        0     4571 2024-02-08 20:02:33.982230 llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/metrics.py
+-rw-r--r--   0        0        0     1557 2024-02-08 20:02:33.982515 llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/metrics_base.py
+-rw-r--r--   0        0        0     3110 2024-02-08 20:02:33.982581 llama_index_core-0.9.56/llama_index/core/evaluation/semantic_similarity.py
+-rw-r--r--   0        0        0     3892 2024-02-08 20:02:33.982644 llama_index_core-0.9.56/llama_index/core/exec_utils.py
+-rw-r--r--   0        0        0      426 2024-02-08 20:02:33.982736 llama_index_core-0.9.56/llama_index/core/extractors/__init__.py
+-rw-r--r--   0        0        0     5472 2024-02-08 20:02:33.982801 llama_index_core-0.9.56/llama_index/core/extractors/interface.py
+-rw-r--r--   0        0        0      966 2024-02-08 20:02:33.983093 llama_index_core-0.9.56/llama_index/core/extractors/loading.py
+-rw-r--r--   0        0        0    16864 2024-02-08 20:02:33.983181 llama_index_core-0.9.56/llama_index/core/extractors/metadata_extractors.py
+-rw-r--r--   0        0        0      126 2024-02-08 20:02:33.983406 llama_index_core-0.9.56/llama_index/core/graph_stores/__init__.py
+-rw-r--r--   0        0        0      535 2024-02-08 20:02:33.983465 llama_index_core-0.9.56/llama_index/core/graph_stores/registry.py
+-rw-r--r--   0        0        0     6107 2024-02-08 20:02:33.983672 llama_index_core-0.9.56/llama_index/core/graph_stores/simple.py
+-rw-r--r--   0        0        0     2096 2024-02-08 20:02:33.983736 llama_index_core-0.9.56/llama_index/core/graph_stores/types.py
+-rw-r--r--   0        0        0     3226 2024-02-08 20:02:33.983820 llama_index_core-0.9.56/llama_index/core/image_retriever.py
+-rw-r--r--   0        0        0      522 2024-02-08 20:02:33.983876 llama_index_core-0.9.56/llama_index/core/img_utils.py
+-rw-r--r--   0        0        0     2360 2024-02-08 20:02:33.983966 llama_index_core-0.9.56/llama_index/core/indices/__init__.py
+-rw-r--r--   0        0        0    17484 2024-02-08 20:02:33.984043 llama_index_core-0.9.56/llama_index/core/indices/base.py
+-rw-r--r--   0        0        0      129 2024-02-08 20:02:33.984237 llama_index_core-0.9.56/llama_index/core/indices/base_retriever.py
+-rw-r--r--   0        0        0       17 2024-02-08 20:02:33.984359 llama_index_core-0.9.56/llama_index/core/indices/common/__init__.py
+-rw-r--r--   0        0        0       19 2024-02-08 20:02:33.984448 llama_index_core-0.9.56/llama_index/core/indices/common/struct_store/__init__.py
+-rw-r--r--   0        0        0     8944 2024-02-08 20:02:33.984527 llama_index_core-0.9.56/llama_index/core/indices/common/struct_store/base.py
+-rw-r--r--   0        0        0      776 2024-02-08 20:02:33.984596 llama_index_core-0.9.56/llama_index/core/indices/common/struct_store/schema.py
+-rw-r--r--   0        0        0     2687 2024-02-08 20:02:33.984662 llama_index_core-0.9.56/llama_index/core/indices/common/struct_store/sql.py
+-rw-r--r--   0        0        0       19 2024-02-08 20:02:33.984750 llama_index_core-0.9.56/llama_index/core/indices/common_tree/__init__.py
+-rw-r--r--   0        0        0     8868 2024-02-08 20:02:33.984827 llama_index_core-0.9.56/llama_index/core/indices/common_tree/base.py
+-rw-r--r--   0        0        0      185 2024-02-08 20:02:33.985058 llama_index_core-0.9.56/llama_index/core/indices/composability/__init__.py
+-rw-r--r--   0        0        0     4953 2024-02-08 20:02:33.985134 llama_index_core-0.9.56/llama_index/core/indices/composability/graph.py
+-rw-r--r--   0        0        0      546 2024-02-08 20:02:33.985366 llama_index_core-0.9.56/llama_index/core/indices/document_summary/__init__.py
+-rw-r--r--   0        0        0    11179 2024-02-08 20:02:33.985448 llama_index_core-0.9.56/llama_index/core/indices/document_summary/base.py
+-rw-r--r--   0        0        0     7213 2024-02-08 20:02:33.985519 llama_index_core-0.9.56/llama_index/core/indices/document_summary/retrievers.py
+-rw-r--r--   0        0        0      234 2024-02-08 20:02:33.985626 llama_index_core-0.9.56/llama_index/core/indices/empty/__init__.py
+-rw-r--r--   0        0        0     3065 2024-02-08 20:02:33.985700 llama_index_core-0.9.56/llama_index/core/indices/empty/base.py
+-rw-r--r--   0        0        0     1285 2024-02-08 20:02:33.985760 llama_index_core-0.9.56/llama_index/core/indices/empty/retrievers.py
+-rw-r--r--   0        0        0     2379 2024-02-08 20:02:33.985997 llama_index_core-0.9.56/llama_index/core/indices/keyword_table/README.md
+-rw-r--r--   0        0        0      880 2024-02-08 20:02:33.986056 llama_index_core-0.9.56/llama_index/core/indices/keyword_table/__init__.py
+-rw-r--r--   0        0        0     9273 2024-02-08 20:02:33.986136 llama_index_core-0.9.56/llama_index/core/indices/keyword_table/base.py
+-rw-r--r--   0        0        0     1098 2024-02-08 20:02:33.986199 llama_index_core-0.9.56/llama_index/core/indices/keyword_table/rake_base.py
+-rw-r--r--   0        0        0     7142 2024-02-08 20:02:33.986272 llama_index_core-0.9.56/llama_index/core/indices/keyword_table/retrievers.py
+-rw-r--r--   0        0        0     1312 2024-02-08 20:02:33.986326 llama_index_core-0.9.56/llama_index/core/indices/keyword_table/simple_base.py
+-rw-r--r--   0        0        0     2360 2024-02-08 20:02:33.986386 llama_index_core-0.9.56/llama_index/core/indices/keyword_table/utils.py
+-rw-r--r--   0        0        0      342 2024-02-08 20:02:33.986476 llama_index_core-0.9.56/llama_index/core/indices/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0    13153 2024-02-08 20:02:33.986552 llama_index_core-0.9.56/llama_index/core/indices/knowledge_graph/base.py
+-rw-r--r--   0        0        0    34765 2024-02-08 20:02:33.986719 llama_index_core-0.9.56/llama_index/core/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0        0        0     1022 2024-02-08 20:02:33.987001 llama_index_core-0.9.56/llama_index/core/indices/list/README.md
+-rw-r--r--   0        0        0      645 2024-02-08 20:02:33.987058 llama_index_core-0.9.56/llama_index/core/indices/list/__init__.py
+-rw-r--r--   0        0        0     5446 2024-02-08 20:02:33.987124 llama_index_core-0.9.56/llama_index/core/indices/list/base.py
+-rw-r--r--   0        0        0     8249 2024-02-08 20:02:33.987206 llama_index_core-0.9.56/llama_index/core/indices/list/retrievers.py
+-rw-r--r--   0        0        0     3602 2024-02-08 20:02:33.987407 llama_index_core-0.9.56/llama_index/core/indices/loading.py
+-rw-r--r--   0        0        0      106 2024-02-08 20:02:33.987626 llama_index_core-0.9.56/llama_index/core/indices/managed/__init__.py
+-rw-r--r--   0        0        0     3718 2024-02-08 20:02:33.987686 llama_index_core-0.9.56/llama_index/core/indices/managed/base.py
+-rw-r--r--   0        0        0      172 2024-02-08 20:02:33.987758 llama_index_core-0.9.56/llama_index/core/indices/managed/types.py
+-rw-r--r--   0        0        0      310 2024-02-08 20:02:33.987860 llama_index_core-0.9.56/llama_index/core/indices/multi_modal/__init__.py
+-rw-r--r--   0        0        0    16441 2024-02-08 20:02:33.987934 llama_index_core-0.9.56/llama_index/core/indices/multi_modal/base.py
+-rw-r--r--   0        0        0    15510 2024-02-08 20:02:33.988022 llama_index_core-0.9.56/llama_index/core/indices/multi_modal/retriever.py
+-rw-r--r--   0        0        0     1361 2024-02-08 20:02:33.988082 llama_index_core-0.9.56/llama_index/core/indices/postprocessor.py
+-rw-r--r--   0        0        0    10492 2024-02-08 20:02:33.988163 llama_index_core-0.9.56/llama_index/core/indices/prompt_helper.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.988222 llama_index_core-0.9.56/llama_index/core/indices/query/__init__.py
+-rw-r--r--   0        0        0      136 2024-02-08 20:02:33.988293 llama_index_core-0.9.56/llama_index/core/indices/query/base.py
+-rw-r--r--   0        0        0     6109 2024-02-08 20:02:33.988364 llama_index_core-0.9.56/llama_index/core/indices/query/embedding_utils.py
+-rw-r--r--   0        0        0      286 2024-02-08 20:02:33.988462 llama_index_core-0.9.56/llama_index/core/indices/query/query_transform/__init__.py
+-rw-r--r--   0        0        0    12479 2024-02-08 20:02:33.988540 llama_index_core-0.9.56/llama_index/core/indices/query/query_transform/base.py
+-rw-r--r--   0        0        0     4548 2024-02-08 20:02:33.988611 llama_index_core-0.9.56/llama_index/core/indices/query/query_transform/feedback_transform.py
+-rw-r--r--   0        0        0     5200 2024-02-08 20:02:33.988790 llama_index_core-0.9.56/llama_index/core/indices/query/query_transform/prompts.py
+-rw-r--r--   0        0        0      129 2024-02-08 20:02:33.988981 llama_index_core-0.9.56/llama_index/core/indices/query/schema.py
+-rw-r--r--   0        0        0     1442 2024-02-08 20:02:33.989042 llama_index_core-0.9.56/llama_index/core/indices/registry.py
+-rw-r--r--   0        0        0      127 2024-02-08 20:02:33.989099 llama_index_core-0.9.56/llama_index/core/indices/service_context.py
+-rw-r--r--   0        0        0      988 2024-02-08 20:02:33.989182 llama_index_core-0.9.56/llama_index/core/indices/struct_store/__init__.py
+-rw-r--r--   0        0        0     2411 2024-02-08 20:02:33.989248 llama_index_core-0.9.56/llama_index/core/indices/struct_store/base.py
+-rw-r--r--   0        0        0     5761 2024-02-08 20:02:33.989540 llama_index_core-0.9.56/llama_index/core/indices/struct_store/container_builder.py
+-rw-r--r--   0        0        0     8036 2024-02-08 20:02:33.989628 llama_index_core-0.9.56/llama_index/core/indices/struct_store/json_query.py
+-rw-r--r--   0        0        0     2610 2024-02-08 20:02:33.989702 llama_index_core-0.9.56/llama_index/core/indices/struct_store/pandas.py
+-rw-r--r--   0        0        0     6472 2024-02-08 20:02:33.989772 llama_index_core-0.9.56/llama_index/core/indices/struct_store/sql.py
+-rw-r--r--   0        0        0    20387 2024-02-08 20:02:33.989867 llama_index_core-0.9.56/llama_index/core/indices/struct_store/sql_query.py
+-rw-r--r--   0        0        0    15704 2024-02-08 20:02:33.990400 llama_index_core-0.9.56/llama_index/core/indices/struct_store/sql_retriever.py
+-rw-r--r--   0        0        0     2645 2024-02-08 20:02:33.990666 llama_index_core-0.9.56/llama_index/core/indices/tree/README.md
+-rw-r--r--   0        0        0      691 2024-02-08 20:02:33.990742 llama_index_core-0.9.56/llama_index/core/indices/tree/__init__.py
+-rw-r--r--   0        0        0     1902 2024-02-08 20:02:33.990813 llama_index_core-0.9.56/llama_index/core/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0        0        0     7767 2024-02-08 20:02:33.990893 llama_index_core-0.9.56/llama_index/core/indices/tree/base.py
+-rw-r--r--   0        0        0     8060 2024-02-08 20:02:33.990977 llama_index_core-0.9.56/llama_index/core/indices/tree/inserter.py
+-rw-r--r--   0        0        0     6090 2024-02-08 20:02:33.991069 llama_index_core-0.9.56/llama_index/core/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0        0        0    15756 2024-02-08 20:02:33.991149 llama_index_core-0.9.56/llama_index/core/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0        0        0     1744 2024-02-08 20:02:33.991222 llama_index_core-0.9.56/llama_index/core/indices/tree/tree_root_retriever.py
+-rw-r--r--   0        0        0      795 2024-02-08 20:02:33.991296 llama_index_core-0.9.56/llama_index/core/indices/tree/utils.py
+-rw-r--r--   0        0        0     8309 2024-02-08 20:02:33.991394 llama_index_core-0.9.56/llama_index/core/indices/utils.py
+-rw-r--r--   0        0        0      409 2024-02-08 20:02:33.991508 llama_index_core-0.9.56/llama_index/core/indices/vector_store/__init__.py
+-rw-r--r--   0        0        0    14505 2024-02-08 20:02:33.991618 llama_index_core-0.9.56/llama_index/core/indices/vector_store/base.py
+-rw-r--r--   0        0        0      300 2024-02-08 20:02:33.991735 llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/__init__.py
+-rw-r--r--   0        0        0      172 2024-02-08 20:02:33.991845 llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0        0        0    10055 2024-02-08 20:02:33.991936 llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0        0        0      665 2024-02-08 20:02:33.992153 llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0        0        0     3989 2024-02-08 20:02:33.992409 llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0        0        0     7531 2024-02-08 20:02:33.992509 llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/retriever.py
+-rw-r--r--   0        0        0      349 2024-02-08 20:02:33.992759 llama_index_core-0.9.56/llama_index/core/ingestion/__init__.py
+-rw-r--r--   0        0        0     2635 2024-02-08 20:02:33.992838 llama_index_core-0.9.56/llama_index/core/ingestion/cache.py
+-rw-r--r--   0        0        0    23537 2024-02-08 20:02:33.992937 llama_index_core-0.9.56/llama_index/core/ingestion/pipeline.py
+-rw-r--r--   0        0        0      237 2024-02-08 20:02:33.993072 llama_index_core-0.9.56/llama_index/core/langchain_helpers/__init__.py
+-rw-r--r--   0        0        0      529 2024-02-08 20:02:33.993185 llama_index_core-0.9.56/llama_index/core/langchain_helpers/agents/__init__.py
+-rw-r--r--   0        0        0     2933 2024-02-08 20:02:33.993275 llama_index_core-0.9.56/llama_index/core/langchain_helpers/agents/agents.py
+-rw-r--r--   0        0        0      835 2024-02-08 20:02:33.993353 llama_index_core-0.9.56/llama_index/core/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0        0        0     2517 2024-02-08 20:02:33.993425 llama_index_core-0.9.56/llama_index/core/langchain_helpers/agents/tools.py
+-rw-r--r--   0        0        0     7653 2024-02-08 20:02:33.993509 llama_index_core-0.9.56/llama_index/core/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0        0        0     1352 2024-02-08 20:02:33.993581 llama_index_core-0.9.56/llama_index/core/langchain_helpers/streaming.py
+-rw-r--r--   0        0        0       70 2024-02-08 20:02:33.993642 llama_index_core-0.9.56/llama_index/core/langchain_helpers/text_splitter.py
+-rw-r--r--   0        0        0     1819 2024-02-08 20:02:33.993749 llama_index_core-0.9.56/llama_index/core/llama_dataset/__init__.py
+-rw-r--r--   0        0        0    10610 2024-02-08 20:02:33.993962 llama_index_core-0.9.56/llama_index/core/llama_dataset/base.py
+-rw-r--r--   0        0        0     3885 2024-02-08 20:02:33.994165 llama_index_core-0.9.56/llama_index/core/llama_dataset/download.py
+-rw-r--r--   0        0        0    15965 2024-02-08 20:02:33.994384 llama_index_core-0.9.56/llama_index/core/llama_dataset/evaluator_evaluation.py
+-rw-r--r--   0        0        0    10480 2024-02-08 20:02:33.994475 llama_index_core-0.9.56/llama_index/core/llama_dataset/generator.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:33.994532 llama_index_core-0.9.56/llama_index/core/llama_dataset/legacy/__init__.py
+-rw-r--r--   0        0        0     3128 2024-02-08 20:02:33.994604 llama_index_core-0.9.56/llama_index/core/llama_dataset/legacy/embedding.py
+-rw-r--r--   0        0        0     5384 2024-02-08 20:02:33.994669 llama_index_core-0.9.56/llama_index/core/llama_dataset/rag.py
+-rw-r--r--   0        0        0      208 2024-02-08 20:02:33.994754 llama_index_core-0.9.56/llama_index/core/llama_pack/__init__.py
+-rw-r--r--   0        0        0      293 2024-02-08 20:02:33.994808 llama_index_core-0.9.56/llama_index/core/llama_pack/base.py
+-rw-r--r--   0        0        0     2314 2024-02-08 20:02:33.994869 llama_index_core-0.9.56/llama_index/core/llama_pack/download.py
+-rw-r--r--   0        0        0      601 2024-02-08 20:02:33.994950 llama_index_core-0.9.56/llama_index/core/llms/__init__.py
+-rw-r--r--   0        0        0     2594 2024-02-08 20:02:33.995005 llama_index_core-0.9.56/llama_index/core/llms/base.py
+-rw-r--r--   0        0        0    10272 2024-02-08 20:02:33.995075 llama_index_core-0.9.56/llama_index/core/llms/callbacks.py
+-rw-r--r--   0        0        0     2659 2024-02-08 20:02:33.995133 llama_index_core-0.9.56/llama_index/core/llms/custom.py
+-rw-r--r--   0        0        0    10263 2024-02-08 20:02:33.995209 llama_index_core-0.9.56/llama_index/core/llms/generic_utils.py
+-rw-r--r--   0        0        0    15383 2024-02-08 20:02:33.995283 llama_index_core-0.9.56/llama_index/core/llms/llm.py
+-rw-r--r--   0        0        0      687 2024-02-08 20:02:33.995348 llama_index_core-0.9.56/llama_index/core/llms/loading.py
+-rw-r--r--   0        0        0     2606 2024-02-08 20:02:33.995413 llama_index_core-0.9.56/llama_index/core/llms/mock.py
+-rw-r--r--   0        0        0     3475 2024-02-08 20:02:33.995483 llama_index_core-0.9.56/llama_index/core/llms/utils.py
+-rw-r--r--   0        0        0      171 2024-02-08 20:02:33.995720 llama_index_core-0.9.56/llama_index/core/memory/__init__.py
+-rw-r--r--   0        0        0     5843 2024-02-08 20:02:33.995793 llama_index_core-0.9.56/llama_index/core/memory/chat_memory_buffer.py
+-rw-r--r--   0        0        0     1279 2024-02-08 20:02:33.995844 llama_index_core-0.9.56/llama_index/core/memory/types.py
+-rw-r--r--   0        0        0      166 2024-02-08 20:02:33.995935 llama_index_core-0.9.56/llama_index/core/multi_modal_llms/__init__.py
+-rw-r--r--   0        0        0     7895 2024-02-08 20:02:33.996003 llama_index_core-0.9.56/llama_index/core/multi_modal_llms/base.py
+-rw-r--r--   0        0        0     1772 2024-02-08 20:02:33.996067 llama_index_core-0.9.56/llama_index/core/multi_modal_llms/generic_utils.py
+-rw-r--r--   0        0        0     1896 2024-02-08 20:02:33.996169 llama_index_core-0.9.56/llama_index/core/node_parser/__init__.py
+-rw-r--r--   0        0        0      398 2024-02-08 20:02:33.996265 llama_index_core-0.9.56/llama_index/core/node_parser/file/__init__.py
+-rw-r--r--   0        0        0     4202 2024-02-08 20:02:33.996331 llama_index_core-0.9.56/llama_index/core/node_parser/file/html.py
+-rw-r--r--   0        0        0     3598 2024-02-08 20:02:33.996416 llama_index_core-0.9.56/llama_index/core/node_parser/file/json.py
+-rw-r--r--   0        0        0     3974 2024-02-08 20:02:33.996478 llama_index_core-0.9.56/llama_index/core/node_parser/file/markdown.py
+-rw-r--r--   0        0        0     2776 2024-02-08 20:02:33.996547 llama_index_core-0.9.56/llama_index/core/node_parser/file/simple_file.py
+-rw-r--r--   0        0        0     6315 2024-02-08 20:02:33.996626 llama_index_core-0.9.56/llama_index/core/node_parser/interface.py
+-rw-r--r--   0        0        0     1762 2024-02-08 20:02:33.996693 llama_index_core-0.9.56/llama_index/core/node_parser/loading.py
+-rw-r--r--   0        0        0     3287 2024-02-08 20:02:33.996878 llama_index_core-0.9.56/llama_index/core/node_parser/node_utils.py
+-rw-r--r--   0        0        0      428 2024-02-08 20:02:33.996970 llama_index_core-0.9.56/llama_index/core/node_parser/relational/__init__.py
+-rw-r--r--   0        0        0    13027 2024-02-08 20:02:33.997491 llama_index_core-0.9.56/llama_index/core/node_parser/relational/base_element.py
+-rw-r--r--   0        0        0     7649 2024-02-08 20:02:33.997583 llama_index_core-0.9.56/llama_index/core/node_parser/relational/hierarchical.py
+-rw-r--r--   0        0        0     8780 2024-02-08 20:02:33.998070 llama_index_core-0.9.56/llama_index/core/node_parser/relational/markdown_element.py
+-rw-r--r--   0        0        0     4432 2024-02-08 20:02:33.998364 llama_index_core-0.9.56/llama_index/core/node_parser/relational/unstructured_element.py
+-rw-r--r--   0        0        0      655 2024-02-08 20:02:33.998455 llama_index_core-0.9.56/llama_index/core/node_parser/text/__init__.py
+-rw-r--r--   0        0        0     5879 2024-02-08 20:02:33.998634 llama_index_core-0.9.56/llama_index/core/node_parser/text/code.py
+-rw-r--r--   0        0        0     1767 2024-02-08 20:02:33.998698 llama_index_core-0.9.56/llama_index/core/node_parser/text/langchain.py
+-rw-r--r--   0        0        0     8761 2024-02-08 20:02:33.998776 llama_index_core-0.9.56/llama_index/core/node_parser/text/semantic_splitter.py
+-rw-r--r--   0        0        0    12203 2024-02-08 20:02:33.999028 llama_index_core-0.9.56/llama_index/core/node_parser/text/sentence.py
+-rw-r--r--   0        0        0     5055 2024-02-08 20:02:33.999114 llama_index_core-0.9.56/llama_index/core/node_parser/text/sentence_window.py
+-rw-r--r--   0        0        0     8604 2024-02-08 20:02:33.999189 llama_index_core-0.9.56/llama_index/core/node_parser/text/token.py
+-rw-r--r--   0        0        0     2430 2024-02-08 20:02:33.999251 llama_index_core-0.9.56/llama_index/core/node_parser/text/utils.py
+-rw-r--r--   0        0        0      600 2024-02-08 20:02:33.999336 llama_index_core-0.9.56/llama_index/core/objects/__init__.py
+-rw-r--r--   0        0        0     6423 2024-02-08 20:02:33.999403 llama_index_core-0.9.56/llama_index/core/objects/base.py
+-rw-r--r--   0        0        0     5404 2024-02-08 20:02:33.999470 llama_index_core-0.9.56/llama_index/core/objects/base_node_mapping.py
+-rw-r--r--   0        0        0     3045 2024-02-08 20:02:33.999638 llama_index_core-0.9.56/llama_index/core/objects/table_node_mapping.py
+-rw-r--r--   0        0        0     4878 2024-02-08 20:02:33.999703 llama_index_core-0.9.56/llama_index/core/objects/tool_node_mapping.py
+-rw-r--r--   0        0        0      450 2024-02-08 20:02:33.999799 llama_index_core-0.9.56/llama_index/core/output_parsers/__init__.py
+-rw-r--r--   0        0        0     2051 2024-02-08 20:02:33.999857 llama_index_core-0.9.56/llama_index/core/output_parsers/base.py
+-rw-r--r--   0        0        0     1916 2024-02-08 20:02:33.999911 llama_index_core-0.9.56/llama_index/core/output_parsers/langchain.py
+-rw-r--r--   0        0        0     2083 2024-02-08 20:02:33.999969 llama_index_core-0.9.56/llama_index/core/output_parsers/pydantic.py
+-rw-r--r--   0        0        0     3343 2024-02-08 20:02:34.000032 llama_index_core-0.9.56/llama_index/core/output_parsers/selection.py
+-rw-r--r--   0        0        0     3801 2024-02-08 20:02:34.000089 llama_index_core-0.9.56/llama_index/core/output_parsers/utils.py
+-rw-r--r--   0        0        0      224 2024-02-08 20:02:34.000301 llama_index_core-0.9.56/llama_index/core/playground/__init__.py
+-rw-r--r--   0        0        0     6957 2024-02-08 20:02:34.000370 llama_index_core-0.9.56/llama_index/core/playground/base.py
+-rw-r--r--   0        0        0     1291 2024-02-08 20:02:34.000594 llama_index_core-0.9.56/llama_index/core/postprocessor/__init__.py
+-rw-r--r--   0        0        0     4299 2024-02-08 20:02:34.000661 llama_index_core-0.9.56/llama_index/core/postprocessor/llm_rerank.py
+-rw-r--r--   0        0        0     1067 2024-02-08 20:02:34.000727 llama_index_core-0.9.56/llama_index/core/postprocessor/metadata_replacement.py
+-rw-r--r--   0        0        0    13644 2024-02-08 20:02:34.000831 llama_index_core-0.9.56/llama_index/core/postprocessor/node.py
+-rw-r--r--   0        0        0     7114 2024-02-08 20:02:34.000917 llama_index_core-0.9.56/llama_index/core/postprocessor/node_recency.py
+-rw-r--r--   0        0        0     6131 2024-02-08 20:02:34.000990 llama_index_core-0.9.56/llama_index/core/postprocessor/optimizer.py
+-rw-r--r--   0        0        0     5312 2024-02-08 20:02:34.001063 llama_index_core-0.9.56/llama_index/core/postprocessor/pii.py
+-rw-r--r--   0        0        0     6035 2024-02-08 20:02:34.001132 llama_index_core-0.9.56/llama_index/core/postprocessor/rankGPT_rerank.py
+-rw-r--r--   0        0        0     3354 2024-02-08 20:02:34.001196 llama_index_core-0.9.56/llama_index/core/postprocessor/sbert_rerank.py
+-rw-r--r--   0        0        0     4117 2024-02-08 20:02:34.001258 llama_index_core-0.9.56/llama_index/core/postprocessor/types.py
+-rw-r--r--   0        0        0      342 2024-02-08 20:02:34.001348 llama_index_core-0.9.56/llama_index/core/program/__init__.py
+-rw-r--r--   0        0        0     4564 2024-02-08 20:02:34.001417 llama_index_core-0.9.56/llama_index/core/program/llm_program.py
+-rw-r--r--   0        0        0      983 2024-02-08 20:02:34.001575 llama_index_core-0.9.56/llama_index/core/program/llm_prompt_program.py
+-rw-r--r--   0        0        0     4373 2024-02-08 20:02:34.001638 llama_index_core-0.9.56/llama_index/core/program/multi_modal_llm_program.py
+-rw-r--r--   0        0        0     3631 2024-02-08 20:02:34.001698 llama_index_core-0.9.56/llama_index/core/program/utils.py
+-rw-r--r--   0        0        0      608 2024-02-08 20:02:34.001794 llama_index_core-0.9.56/llama_index/core/prompts/__init__.py
+-rw-r--r--   0        0        0    20346 2024-02-08 20:02:34.001887 llama_index_core-0.9.56/llama_index/core/prompts/base.py
+-rw-r--r--   0        0        0     3620 2024-02-08 20:02:34.001968 llama_index_core-0.9.56/llama_index/core/prompts/chat_prompts.py
+-rw-r--r--   0        0        0     1199 2024-02-08 20:02:34.002151 llama_index_core-0.9.56/llama_index/core/prompts/default_prompt_selectors.py
+-rw-r--r--   0        0        0    16240 2024-02-08 20:02:34.002222 llama_index_core-0.9.56/llama_index/core/prompts/default_prompts.py
+-rw-r--r--   0        0        0      524 2024-02-08 20:02:34.002276 llama_index_core-0.9.56/llama_index/core/prompts/display_utils.py
+-rw-r--r--   0        0        0     5582 2024-02-08 20:02:34.002479 llama_index_core-0.9.56/llama_index/core/prompts/guidance_utils.py
+-rw-r--r--   0        0        0     3277 2024-02-08 20:02:34.002540 llama_index_core-0.9.56/llama_index/core/prompts/mixin.py
+-rw-r--r--   0        0        0     1780 2024-02-08 20:02:34.003742 llama_index_core-0.9.56/llama_index/core/prompts/prompt_type.py
+-rw-r--r--   0        0        0     1098 2024-02-08 20:02:34.003797 llama_index_core-0.9.56/llama_index/core/prompts/prompt_utils.py
+-rw-r--r--   0        0        0     3915 2024-02-08 20:02:34.003858 llama_index_core-0.9.56/llama_index/core/prompts/prompts.py
+-rw-r--r--   0        0        0     4790 2024-02-08 20:02:34.003927 llama_index_core-0.9.56/llama_index/core/prompts/system.py
+-rw-r--r--   0        0        0      501 2024-02-08 20:02:34.003986 llama_index_core-0.9.56/llama_index/core/prompts/utils.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:34.004005 llama_index_core-0.9.56/llama_index/core/py.typed
+-rw-r--r--   0        0        0     2816 2024-02-08 20:02:34.004105 llama_index_core-0.9.56/llama_index/core/query_engine/__init__.py
+-rw-r--r--   0        0        0    13229 2024-02-08 20:02:34.004174 llama_index_core-0.9.56/llama_index/core/query_engine/citation_query_engine.py
+-rw-r--r--   0        0        0     2059 2024-02-08 20:02:34.004228 llama_index_core-0.9.56/llama_index/core/query_engine/cogniswitch_query_engine.py
+-rw-r--r--   0        0        0     2955 2024-02-08 20:02:34.004289 llama_index_core-0.9.56/llama_index/core/query_engine/custom.py
+-rw-r--r--   0        0        0       19 2024-02-08 20:02:34.004365 llama_index_core-0.9.56/llama_index/core/query_engine/flare/__init__.py
+-rw-r--r--   0        0        0     6976 2024-02-08 20:02:34.004441 llama_index_core-0.9.56/llama_index/core/query_engine/flare/answer_inserter.py
+-rw-r--r--   0        0        0    10753 2024-02-08 20:02:34.004521 llama_index_core-0.9.56/llama_index/core/query_engine/flare/base.py
+-rw-r--r--   0        0        0     2088 2024-02-08 20:02:34.004685 llama_index_core-0.9.56/llama_index/core/query_engine/flare/output_parser.py
+-rw-r--r--   0        0        0      163 2024-02-08 20:02:34.004740 llama_index_core-0.9.56/llama_index/core/query_engine/flare/schema.py
+-rw-r--r--   0        0        0     4819 2024-02-08 20:02:34.004807 llama_index_core-0.9.56/llama_index/core/query_engine/graph_query_engine.py
+-rw-r--r--   0        0        0    13068 2024-02-08 20:02:34.004880 llama_index_core-0.9.56/llama_index/core/query_engine/jsonalyze_query_engine.py
+-rw-r--r--   0        0        0    10575 2024-02-08 20:02:34.004957 llama_index_core-0.9.56/llama_index/core/query_engine/knowledge_graph_query_engine.py
+-rw-r--r--   0        0        0     9492 2024-02-08 20:02:34.005027 llama_index_core-0.9.56/llama_index/core/query_engine/multi_modal.py
+-rw-r--r--   0        0        0     6755 2024-02-08 20:02:34.005092 llama_index_core-0.9.56/llama_index/core/query_engine/multistep_query_engine.py
+-rw-r--r--   0        0        0      270 2024-02-08 20:02:34.005182 llama_index_core-0.9.56/llama_index/core/query_engine/pandas/__init__.py
+-rw-r--r--   0        0        0     2963 2024-02-08 20:02:34.005247 llama_index_core-0.9.56/llama_index/core/query_engine/pandas/output_parser.py
+-rw-r--r--   0        0        0     7191 2024-02-08 20:02:34.005317 llama_index_core-0.9.56/llama_index/core/query_engine/pandas/pandas_query_engine.py
+-rw-r--r--   0        0        0     8428 2024-02-08 20:02:34.005413 llama_index_core-0.9.56/llama_index/core/query_engine/retriever_query_engine.py
+-rw-r--r--   0        0        0     5363 2024-02-08 20:02:34.005479 llama_index_core-0.9.56/llama_index/core/query_engine/retry_query_engine.py
+-rw-r--r--   0        0        0     3812 2024-02-08 20:02:34.005554 llama_index_core-0.9.56/llama_index/core/query_engine/retry_source_query_engine.py
+-rw-r--r--   0        0        0    15724 2024-02-08 20:02:34.005626 llama_index_core-0.9.56/llama_index/core/query_engine/router_query_engine.py
+-rw-r--r--   0        0        0    13916 2024-02-08 20:02:34.005692 llama_index_core-0.9.56/llama_index/core/query_engine/sql_join_query_engine.py
+-rw-r--r--   0        0        0     7267 2024-02-08 20:02:34.005761 llama_index_core-0.9.56/llama_index/core/query_engine/sql_vector_query_engine.py
+-rw-r--r--   0        0        0    11106 2024-02-08 20:02:34.005838 llama_index_core-0.9.56/llama_index/core/query_engine/sub_question_query_engine.py
+-rw-r--r--   0        0        0     3427 2024-02-08 20:02:34.005906 llama_index_core-0.9.56/llama_index/core/query_engine/transform_query_engine.py
+-rw-r--r--   0        0        0      793 2024-02-08 20:02:34.005999 llama_index_core-0.9.56/llama_index/core/query_pipeline/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:34.006060 llama_index_core-0.9.56/llama_index/core/query_pipeline/components/__init__.py
+-rw-r--r--   0        0        0    10506 2024-02-08 20:02:34.006163 llama_index_core-0.9.56/llama_index/core/query_pipeline/components/agent.py
+-rw-r--r--   0        0        0     3657 2024-02-08 20:02:34.006229 llama_index_core-0.9.56/llama_index/core/query_pipeline/components/argpacks.py
+-rw-r--r--   0        0        0     3839 2024-02-08 20:02:34.006301 llama_index_core-0.9.56/llama_index/core/query_pipeline/components/function.py
+-rw-r--r--   0        0        0     1563 2024-02-08 20:02:34.006374 llama_index_core-0.9.56/llama_index/core/query_pipeline/components/input.py
+-rw-r--r--   0        0        0     6850 2024-02-08 20:02:34.006453 llama_index_core-0.9.56/llama_index/core/query_pipeline/components/router.py
+-rw-r--r--   0        0        0     3780 2024-02-08 20:02:34.006527 llama_index_core-0.9.56/llama_index/core/query_pipeline/components/tool_runner.py
+-rw-r--r--   0        0        0    21914 2024-02-08 20:02:34.006608 llama_index_core-0.9.56/llama_index/core/query_pipeline/query.py
+-rw-r--r--   0        0        0      232 2024-02-08 20:02:34.006732 llama_index_core-0.9.56/llama_index/core/question_gen/__init__.py
+-rw-r--r--   0        0        0     3803 2024-02-08 20:02:34.006797 llama_index_core-0.9.56/llama_index/core/question_gen/llm_generators.py
+-rw-r--r--   0        0        0     1024 2024-02-08 20:02:34.006855 llama_index_core-0.9.56/llama_index/core/question_gen/output_parser.py
+-rw-r--r--   0        0        0     1974 2024-02-08 20:02:34.007027 llama_index_core-0.9.56/llama_index/core/question_gen/prompts.py
+-rw-r--r--   0        0        0     1009 2024-02-08 20:02:34.007091 llama_index_core-0.9.56/llama_index/core/question_gen/types.py
+-rw-r--r--   0        0        0      929 2024-02-08 20:02:34.007186 llama_index_core-0.9.56/llama_index/core/readers/__init__.py
+-rw-r--r--   0        0        0     2446 2024-02-08 20:02:34.007256 llama_index_core-0.9.56/llama_index/core/readers/base.py
+-rw-r--r--   0        0        0     2438 2024-02-08 20:02:34.007327 llama_index_core-0.9.56/llama_index/core/readers/download.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:34.007391 llama_index_core-0.9.56/llama_index/core/readers/file/__init__.py
+-rw-r--r--   0        0        0    15958 2024-02-08 20:02:34.007477 llama_index_core-0.9.56/llama_index/core/readers/file/base.py
+-rw-r--r--   0        0        0     4665 2024-02-08 20:02:34.007650 llama_index_core-0.9.56/llama_index/core/readers/json.py
+-rw-r--r--   0        0        0      784 2024-02-08 20:02:34.007714 llama_index_core-0.9.56/llama_index/core/readers/loading.py
+-rw-r--r--   0        0        0     1196 2024-02-08 20:02:34.007914 llama_index_core-0.9.56/llama_index/core/readers/string_iterable.py
+-rw-r--r--   0        0        0       83 2024-02-08 20:02:34.008008 llama_index_core-0.9.56/llama_index/core/response/__init__.py
+-rw-r--r--   0        0        0     4904 2024-02-08 20:02:34.008073 llama_index_core-0.9.56/llama_index/core/response/notebook_utils.py
+-rw-r--r--   0        0        0     1589 2024-02-08 20:02:34.008126 llama_index_core-0.9.56/llama_index/core/response/pprint_utils.py
+-rw-r--r--   0        0        0      262 2024-02-08 20:02:34.008285 llama_index_core-0.9.56/llama_index/core/response/utils.py
+-rw-r--r--   0        0        0      922 2024-02-08 20:02:34.008386 llama_index_core-0.9.56/llama_index/core/response_synthesizers/__init__.py
+-rw-r--r--   0        0        0     5296 2024-02-08 20:02:34.008458 llama_index_core-0.9.56/llama_index/core/response_synthesizers/accumulate.py
+-rw-r--r--   0        0        0     9574 2024-02-08 20:02:34.008533 llama_index_core-0.9.56/llama_index/core/response_synthesizers/base.py
+-rw-r--r--   0        0        0     1823 2024-02-08 20:02:34.008590 llama_index_core-0.9.56/llama_index/core/response_synthesizers/compact_and_accumulate.py
+-rw-r--r--   0        0        0     2004 2024-02-08 20:02:34.008643 llama_index_core-0.9.56/llama_index/core/response_synthesizers/compact_and_refine.py
+-rw-r--r--   0        0        0     6672 2024-02-08 20:02:34.008710 llama_index_core-0.9.56/llama_index/core/response_synthesizers/factory.py
+-rw-r--r--   0        0        0     2902 2024-02-08 20:02:34.008765 llama_index_core-0.9.56/llama_index/core/response_synthesizers/generation.py
+-rw-r--r--   0        0        0      796 2024-02-08 20:02:34.008845 llama_index_core-0.9.56/llama_index/core/response_synthesizers/no_text.py
+-rw-r--r--   0        0        0    18085 2024-02-08 20:02:34.008911 llama_index_core-0.9.56/llama_index/core/response_synthesizers/refine.py
+-rw-r--r--   0        0        0     3766 2024-02-08 20:02:34.008984 llama_index_core-0.9.56/llama_index/core/response_synthesizers/simple_summarize.py
+-rw-r--r--   0        0        0     8896 2024-02-08 20:02:34.009055 llama_index_core-0.9.56/llama_index/core/response_synthesizers/tree_summarize.py
+-rw-r--r--   0        0        0     2011 2024-02-08 20:02:34.009147 llama_index_core-0.9.56/llama_index/core/response_synthesizers/type.py
+-rw-r--r--   0        0        0     2419 2024-02-08 20:02:34.009237 llama_index_core-0.9.56/llama_index/core/retrievers/__init__.py
+-rw-r--r--   0        0        0     7122 2024-02-08 20:02:34.009303 llama_index_core-0.9.56/llama_index/core/retrievers/auto_merging_retriever.py
+-rw-r--r--   0        0        0     7926 2024-02-08 20:02:34.009373 llama_index_core-0.9.56/llama_index/core/retrievers/fusion_retriever.py
+-rw-r--r--   0        0        0     7525 2024-02-08 20:02:34.009446 llama_index_core-0.9.56/llama_index/core/retrievers/recursive_retriever.py
+-rw-r--r--   0        0        0     6104 2024-02-08 20:02:34.009514 llama_index_core-0.9.56/llama_index/core/retrievers/router_retriever.py
+-rw-r--r--   0        0        0     1581 2024-02-08 20:02:34.009571 llama_index_core-0.9.56/llama_index/core/retrievers/transform_retriever.py
+-rw-r--r--   0        0        0    23388 2024-02-08 20:02:34.009655 llama_index_core-0.9.56/llama_index/core/schema.py
+-rw-r--r--   0        0        0      456 2024-02-08 20:02:34.009768 llama_index_core-0.9.56/llama_index/core/selectors/__init__.py
+-rw-r--r--   0        0        0     3052 2024-02-08 20:02:34.009828 llama_index_core-0.9.56/llama_index/core/selectors/embedding_selectors.py
+-rw-r--r--   0        0        0     7898 2024-02-08 20:02:34.009898 llama_index_core-0.9.56/llama_index/core/selectors/llm_selectors.py
+-rw-r--r--   0        0        0     2985 2024-02-08 20:02:34.009968 llama_index_core-0.9.56/llama_index/core/selectors/prompts.py
+-rw-r--r--   0        0        0     5496 2024-02-08 20:02:34.010033 llama_index_core-0.9.56/llama_index/core/selectors/pydantic_selectors.py
+-rw-r--r--   0        0        0     3333 2024-02-08 20:02:34.010101 llama_index_core-0.9.56/llama_index/core/selectors/types.py
+-rw-r--r--   0        0        0     1021 2024-02-08 20:02:34.010164 llama_index_core-0.9.56/llama_index/core/selectors/utils.py
+-rw-r--r--   0        0        0    15655 2024-02-08 20:02:34.010247 llama_index_core-0.9.56/llama_index/core/service_context.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:34.010319 llama_index_core-0.9.56/llama_index/core/service_context_elements/__init__.py
+-rw-r--r--   0        0        0      995 2024-02-08 20:02:34.010403 llama_index_core-0.9.56/llama_index/core/service_context_elements/llama_logger.py
+-rw-r--r--   0        0        0    11826 2024-02-08 20:02:34.010497 llama_index_core-0.9.56/llama_index/core/service_context_elements/llm_predictor.py
+-rw-r--r--   0        0        0     9970 2024-02-08 20:02:34.010739 llama_index_core-0.9.56/llama_index/core/settings.py
+-rw-r--r--   0        0        0      129 2024-02-08 20:02:34.010861 llama_index_core-0.9.56/llama_index/core/storage/__init__.py
+-rw-r--r--   0        0        0      197 2024-02-08 20:02:34.010975 llama_index_core-0.9.56/llama_index/core/storage/chat_store/__init__.py
+-rw-r--r--   0        0        0     1336 2024-02-08 20:02:34.011201 llama_index_core-0.9.56/llama_index/core/storage/chat_store/base.py
+-rw-r--r--   0        0        0      668 2024-02-08 20:02:34.011263 llama_index_core-0.9.56/llama_index/core/storage/chat_store/loading.py
+-rw-r--r--   0        0        0     2821 2024-02-08 20:02:34.011329 llama_index_core-0.9.56/llama_index/core/storage/chat_store/simple_chat_store.py
+-rw-r--r--   0        0        0      304 2024-02-08 20:02:34.011561 llama_index_core-0.9.56/llama_index/core/storage/docstore/__init__.py
+-rw-r--r--   0        0        0    20499 2024-02-08 20:02:34.011650 llama_index_core-0.9.56/llama_index/core/storage/docstore/keyval_docstore.py
+-rw-r--r--   0        0        0     2497 2024-02-08 20:02:34.011754 llama_index_core-0.9.56/llama_index/core/storage/docstore/postgres_docstore.py
+-rw-r--r--   0        0        0      648 2024-02-08 20:02:34.011821 llama_index_core-0.9.56/llama_index/core/storage/docstore/registry.py
+-rw-r--r--   0        0        0     3292 2024-02-08 20:02:34.011898 llama_index_core-0.9.56/llama_index/core/storage/docstore/simple_docstore.py
+-rw-r--r--   0        0        0     6635 2024-02-08 20:02:34.011971 llama_index_core-0.9.56/llama_index/core/storage/docstore/types.py
+-rw-r--r--   0        0        0     2606 2024-02-08 20:02:34.012040 llama_index_core-0.9.56/llama_index/core/storage/docstore/utils.py
+-rw-r--r--   0        0        0      133 2024-02-08 20:02:34.012143 llama_index_core-0.9.56/llama_index/core/storage/index_store/__init__.py
+-rw-r--r--   0        0        0     2242 2024-02-08 20:02:34.012343 llama_index_core-0.9.56/llama_index/core/storage/index_store/keyval_index_store.py
+-rw-r--r--   0        0        0     2280 2024-02-08 20:02:34.012406 llama_index_core-0.9.56/llama_index/core/storage/index_store/postgres_index_store.py
+-rw-r--r--   0        0        0     2365 2024-02-08 20:02:34.012475 llama_index_core-0.9.56/llama_index/core/storage/index_store/simple_index_store.py
+-rw-r--r--   0        0        0      959 2024-02-08 20:02:34.012543 llama_index_core-0.9.56/llama_index/core/storage/index_store/types.py
+-rw-r--r--   0        0        0      692 2024-02-08 20:02:34.012603 llama_index_core-0.9.56/llama_index/core/storage/index_store/utils.py
+-rw-r--r--   0        0        0      157 2024-02-08 20:02:34.012701 llama_index_core-0.9.56/llama_index/core/storage/kvstore/__init__.py
+-rw-r--r--   0        0        0    14770 2024-02-08 20:02:34.012915 llama_index_core-0.9.56/llama_index/core/storage/kvstore/postgres_kvstore.py
+-rw-r--r--   0        0        0     3482 2024-02-08 20:02:34.013023 llama_index_core-0.9.56/llama_index/core/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0        0        0     2533 2024-02-08 20:02:34.013109 llama_index_core-0.9.56/llama_index/core/storage/kvstore/types.py
+-rw-r--r--   0        0        0     8902 2024-02-08 20:02:34.013203 llama_index_core-0.9.56/llama_index/core/storage/storage_context.py
+-rw-r--r--   0        0        0      356 2024-02-08 20:02:34.013334 llama_index_core-0.9.56/llama_index/core/text_splitter/__init__.py
+-rw-r--r--   0        0        0      682 2024-02-08 20:02:34.013526 llama_index_core-0.9.56/llama_index/core/tools/__init__.py
+-rw-r--r--   0        0        0     1898 2024-02-08 20:02:34.013602 llama_index_core-0.9.56/llama_index/core/tools/download.py
+-rw-r--r--   0        0        0     4099 2024-02-08 20:02:34.013684 llama_index_core-0.9.56/llama_index/core/tools/function_tool.py
+-rw-r--r--   0        0        0     5861 2024-02-08 20:02:34.013757 llama_index_core-0.9.56/llama_index/core/tools/ondemand_loader_tool.py
+-rw-r--r--   0        0        0     3791 2024-02-08 20:02:34.013823 llama_index_core-0.9.56/llama_index/core/tools/query_engine.py
+-rw-r--r--   0        0        0     7692 2024-02-08 20:02:34.014006 llama_index_core-0.9.56/llama_index/core/tools/query_plan.py
+-rw-r--r--   0        0        0     3600 2024-02-08 20:02:34.014078 llama_index_core-0.9.56/llama_index/core/tools/retriever_tool.py
+-rw-r--r--   0        0        0       19 2024-02-08 20:02:34.014167 llama_index_core-0.9.56/llama_index/core/tools/tool_spec/__init__.py
+-rw-r--r--   0        0        0     4575 2024-02-08 20:02:34.014232 llama_index_core-0.9.56/llama_index/core/tools/tool_spec/base.py
+-rw-r--r--   0        0        0     1139 2024-02-08 20:02:34.014320 llama_index_core-0.9.56/llama_index/core/tools/tool_spec/load_and_search/README.md
+-rw-r--r--   0        0        0      134 2024-02-08 20:02:34.014383 llama_index_core-0.9.56/llama_index/core/tools/tool_spec/load_and_search/__init__.py
+-rw-r--r--   0        0        0     5061 2024-02-08 20:02:34.014462 llama_index_core-0.9.56/llama_index/core/tools/tool_spec/load_and_search/base.py
+-rw-r--r--   0        0        0     5659 2024-02-08 20:02:34.014527 llama_index_core-0.9.56/llama_index/core/tools/types.py
+-rw-r--r--   0        0        0     1925 2024-02-08 20:02:34.014585 llama_index_core-0.9.56/llama_index/core/tools/utils.py
+-rw-r--r--   0        0        0     2208 2024-02-08 20:02:34.014642 llama_index_core-0.9.56/llama_index/core/types.py
+-rw-r--r--   0        0        0        0 2024-02-08 20:02:34.014696 llama_index_core-0.9.56/llama_index/core/utilities/__init__.py
+-rw-r--r--   0        0        0     1644 2024-02-08 20:02:34.014902 llama_index_core-0.9.56/llama_index/core/utilities/aws_utils.py
+-rw-r--r--   0        0        0     9634 2024-02-08 20:02:34.015085 llama_index_core-0.9.56/llama_index/core/utilities/sql_wrapper.py
+-rw-r--r--   0        0        0     2674 2024-02-08 20:02:34.015146 llama_index_core-0.9.56/llama_index/core/utilities/token_counting.py
+-rw-r--r--   0        0        0    14400 2024-02-08 20:02:34.015219 llama_index_core-0.9.56/llama_index/core/utils.py
+-rw-r--r--   0        0        0      506 2024-02-08 20:02:34.015308 llama_index_core-0.9.56/llama_index/core/vector_stores/__init__.py
+-rw-r--r--   0        0        0    11220 2024-02-08 20:02:34.015491 llama_index_core-0.9.56/llama_index/core/vector_stores/simple.py
+-rw-r--r--   0        0        0    10662 2024-02-08 20:02:34.015554 llama_index_core-0.9.56/llama_index/core/vector_stores/types.py
+-rw-r--r--   0        0        0     4593 2024-02-08 20:02:34.015724 llama_index_core-0.9.56/llama_index/core/vector_stores/utils.py
+-rw-r--r--   0        0        0     6376 2024-02-08 20:03:05.998483 llama_index_core-0.9.56/pyproject.toml
+-rw-r--r--   0        0        0     2957 1970-01-01 00:00:00.000000 llama_index_core-0.9.56/PKG-INFO
```

### Comparing `llama_index_core-0.9.55/LICENSE` & `llama_index_core-0.9.56/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/__init__.py` & `llama_index_core-0.9.56/llama_index/core/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/__init__.py` & `llama_index_core-0.9.56/llama_index/core/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/custom/pipeline_worker.py` & `llama_index_core-0.9.56/llama_index/core/agent/custom/pipeline_worker.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/custom/simple.py` & `llama_index_core-0.9.56/llama_index/core/agent/custom/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/legacy/react/base.py` & `llama_index_core-0.9.56/llama_index/core/agent/legacy/react/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/react/base.py` & `llama_index_core-0.9.56/llama_index/core/agent/react/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/react/formatter.py` & `llama_index_core-0.9.56/llama_index/core/agent/react/formatter.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/react/output_parser.py` & `llama_index_core-0.9.56/llama_index/core/agent/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/react/prompts.py` & `llama_index_core-0.9.56/llama_index/core/agent/react/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/react/step.py` & `llama_index_core-0.9.56/llama_index/core/agent/react/step.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/react/types.py` & `llama_index_core-0.9.56/llama_index/core/agent/react/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/react_multimodal/prompts.py` & `llama_index_core-0.9.56/llama_index/core/agent/react_multimodal/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/react_multimodal/step.py` & `llama_index_core-0.9.56/llama_index/core/agent/react_multimodal/step.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/runner/base.py` & `llama_index_core-0.9.56/llama_index/core/agent/runner/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/runner/parallel.py` & `llama_index_core-0.9.56/llama_index/core/agent/runner/parallel.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/types.py` & `llama_index_core-0.9.56/llama_index/core/agent/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/agent/utils.py` & `llama_index_core-0.9.56/llama_index/core/agent/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/async_utils.py` & `llama_index_core-0.9.56/llama_index/core/async_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/base_auto_retriever.py` & `llama_index_core-0.9.56/llama_index/core/base/base_auto_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/base_multi_modal_retriever.py` & `llama_index_core-0.9.56/llama_index/core/base/base_multi_modal_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/base_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/base/base_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/base_retriever.py` & `llama_index_core-0.9.56/llama_index/core/base/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/base_selector.py` & `llama_index_core-0.9.56/llama_index/core/base/base_selector.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/embeddings/base.py` & `llama_index_core-0.9.56/llama_index/core/base/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/llms/types.py` & `llama_index_core-0.9.56/llama_index/core/base/llms/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/query_pipeline/query.py` & `llama_index_core-0.9.56/llama_index/core/base/query_pipeline/query.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/base/response/schema.py` & `llama_index_core-0.9.56/llama_index/core/base/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/bridge/langchain.py` & `llama_index_core-0.9.56/llama_index/core/bridge/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/bridge/pydantic.py` & `llama_index_core-0.9.56/llama_index/core/bridge/pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/callbacks/base.py` & `llama_index_core-0.9.56/llama_index/core/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/callbacks/base_handler.py` & `llama_index_core-0.9.56/llama_index/core/callbacks/base_handler.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/callbacks/global_handlers.py` & `llama_index_core-0.9.56/llama_index/core/callbacks/global_handlers.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/callbacks/llama_debug.py` & `llama_index_core-0.9.56/llama_index/core/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/callbacks/schema.py` & `llama_index_core-0.9.56/llama_index/core/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/callbacks/simple_llm_handler.py` & `llama_index_core-0.9.56/llama_index/core/callbacks/simple_llm_handler.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/callbacks/token_counting.py` & `llama_index_core-0.9.56/llama_index/core/callbacks/token_counting.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/callbacks/utils.py` & `llama_index_core-0.9.56/llama_index/core/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/chat_engine/condense_plus_context.py` & `llama_index_core-0.9.56/llama_index/core/chat_engine/condense_plus_context.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/chat_engine/condense_question.py` & `llama_index_core-0.9.56/llama_index/core/chat_engine/condense_question.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/chat_engine/context.py` & `llama_index_core-0.9.56/llama_index/core/chat_engine/context.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/chat_engine/simple.py` & `llama_index_core-0.9.56/llama_index/core/chat_engine/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/chat_engine/types.py` & `llama_index_core-0.9.56/llama_index/core/chat_engine/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/command_line/command_line.py` & `llama_index_core-0.9.56/llama_index/core/command_line/command_line.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/command_line/mappings.json` & `llama_index_core-0.9.56/llama_index/core/command_line/mappings.json`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/command_line/rag.py` & `llama_index_core-0.9.56/llama_index/core/command_line/rag.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/command_line/upgrade.py` & `llama_index_core-0.9.56/llama_index/core/command_line/upgrade.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/composability/joint_qa_summary.py` & `llama_index_core-0.9.56/llama_index/core/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/constants.py` & `llama_index_core-0.9.56/llama_index/core/constants.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/data_structs/data_structs.py` & `llama_index_core-0.9.56/llama_index/core/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/data_structs/document_summary.py` & `llama_index_core-0.9.56/llama_index/core/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/data_structs/registry.py` & `llama_index_core-0.9.56/llama_index/core/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/data_structs/struct_type.py` & `llama_index_core-0.9.56/llama_index/core/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/data_structs/table.py` & `llama_index_core-0.9.56/llama_index/core/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/download/dataset.py` & `llama_index_core-0.9.56/llama_index/core/download/dataset.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/download/integration.py` & `llama_index_core-0.9.56/llama_index/core/download/integration.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/download/module.py` & `llama_index_core-0.9.56/llama_index/core/download/module.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/download/pack.py` & `llama_index_core-0.9.56/llama_index/core/download/pack.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/download/utils.py` & `llama_index_core-0.9.56/llama_index/core/download/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/embeddings/loading.py` & `llama_index_core-0.9.56/llama_index/core/embeddings/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/embeddings/mock_embed_model.py` & `llama_index_core-0.9.56/llama_index/core/embeddings/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/embeddings/multi_modal_base.py` & `llama_index_core-0.9.56/llama_index/core/embeddings/multi_modal_base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/embeddings/pooling.py` & `llama_index_core-0.9.56/llama_index/core/embeddings/pooling.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/embeddings/utils.py` & `llama_index_core-0.9.56/llama_index/core/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/__init__.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/answer_relevancy.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/answer_relevancy.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/base.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/batch_runner.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/batch_runner.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/benchmarks/beir.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/benchmarks/beir.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/benchmarks/hotpotqa.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/benchmarks/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/context_relevancy.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/context_relevancy.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/correctness.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/correctness.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/dataset_generation.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/eval_utils.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/eval_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/faithfulness.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/faithfulness.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/guideline.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/guideline.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/multi_modal/faithfulness.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/multi_modal/faithfulness.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/multi_modal/relevancy.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/multi_modal/relevancy.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/notebook_utils.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/pairwise.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/pairwise.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/relevancy.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/relevancy.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/base.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/evaluator.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/evaluator.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/metrics.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/metrics.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/retrieval/metrics_base.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/retrieval/metrics_base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/evaluation/semantic_similarity.py` & `llama_index_core-0.9.56/llama_index/core/evaluation/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/exec_utils.py` & `llama_index_core-0.9.56/llama_index/core/exec_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/extractors/interface.py` & `llama_index_core-0.9.56/llama_index/core/extractors/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/extractors/loading.py` & `llama_index_core-0.9.56/llama_index/core/extractors/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/extractors/metadata_extractors.py` & `llama_index_core-0.9.56/llama_index/core/extractors/metadata_extractors.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/graph_stores/registry.py` & `llama_index_core-0.9.56/llama_index/core/graph_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/graph_stores/simple.py` & `llama_index_core-0.9.56/llama_index/core/graph_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/graph_stores/types.py` & `llama_index_core-0.9.56/llama_index/core/graph_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/image_retriever.py` & `llama_index_core-0.9.56/llama_index/core/image_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/img_utils.py` & `llama_index_core-0.9.56/llama_index/core/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/__init__.py` & `llama_index_core-0.9.56/llama_index/core/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/common/struct_store/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/common/struct_store/schema.py` & `llama_index_core-0.9.56/llama_index/core/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/common/struct_store/sql.py` & `llama_index_core-0.9.56/llama_index/core/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/common_tree/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/composability/graph.py` & `llama_index_core-0.9.56/llama_index/core/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/document_summary/__init__.py` & `llama_index_core-0.9.56/llama_index/core/indices/document_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/document_summary/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/document_summary/retrievers.py` & `llama_index_core-0.9.56/llama_index/core/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/empty/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/empty/retrievers.py` & `llama_index_core-0.9.56/llama_index/core/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/keyword_table/README.md` & `llama_index_core-0.9.56/llama_index/core/indices/keyword_table/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/keyword_table/__init__.py` & `llama_index_core-0.9.56/llama_index/core/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/keyword_table/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/keyword_table/rake_base.py` & `llama_index_core-0.9.56/llama_index/core/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/keyword_table/retrievers.py` & `llama_index_core-0.9.56/llama_index/core/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/keyword_table/simple_base.py` & `llama_index_core-0.9.56/llama_index/core/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/keyword_table/utils.py` & `llama_index_core-0.9.56/llama_index/core/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/knowledge_graph/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/knowledge_graph/retrievers.py` & `llama_index_core-0.9.56/llama_index/core/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/list/README.md` & `llama_index_core-0.9.56/llama_index/core/indices/list/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/list/__init__.py` & `llama_index_core-0.9.56/llama_index/core/indices/list/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/list/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/list/retrievers.py` & `llama_index_core-0.9.56/llama_index/core/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/loading.py` & `llama_index_core-0.9.56/llama_index/core/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/managed/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/managed/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/multi_modal/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/multi_modal/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/multi_modal/retriever.py` & `llama_index_core-0.9.56/llama_index/core/indices/multi_modal/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/postprocessor.py` & `llama_index_core-0.9.56/llama_index/core/indices/postprocessor.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/prompt_helper.py` & `llama_index_core-0.9.56/llama_index/core/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/query/embedding_utils.py` & `llama_index_core-0.9.56/llama_index/core/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/query/query_transform/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/query/query_transform/feedback_transform.py` & `llama_index_core-0.9.56/llama_index/core/indices/query/query_transform/feedback_transform.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/query/query_transform/prompts.py` & `llama_index_core-0.9.56/llama_index/core/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/registry.py` & `llama_index_core-0.9.56/llama_index/core/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/struct_store/__init__.py` & `llama_index_core-0.9.56/llama_index/core/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/struct_store/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/struct_store/container_builder.py` & `llama_index_core-0.9.56/llama_index/core/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/struct_store/json_query.py` & `llama_index_core-0.9.56/llama_index/core/indices/struct_store/json_query.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/struct_store/pandas.py` & `llama_index_core-0.9.56/llama_index/core/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/struct_store/sql.py` & `llama_index_core-0.9.56/llama_index/core/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/struct_store/sql_query.py` & `llama_index_core-0.9.56/llama_index/core/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/struct_store/sql_retriever.py` & `llama_index_core-0.9.56/llama_index/core/indices/struct_store/sql_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/README.md` & `llama_index_core-0.9.56/llama_index/core/indices/tree/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/__init__.py` & `llama_index_core-0.9.56/llama_index/core/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/all_leaf_retriever.py` & `llama_index_core-0.9.56/llama_index/core/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/inserter.py` & `llama_index_core-0.9.56/llama_index/core/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/select_leaf_embedding_retriever.py` & `llama_index_core-0.9.56/llama_index/core/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/select_leaf_retriever.py` & `llama_index_core-0.9.56/llama_index/core/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/tree_root_retriever.py` & `llama_index_core-0.9.56/llama_index/core/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/tree/utils.py` & `llama_index_core-0.9.56/llama_index/core/indices/tree/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/utils.py` & `llama_index_core-0.9.56/llama_index/core/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/vector_store/base.py` & `llama_index_core-0.9.56/llama_index/core/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/auto_retriever/output_parser.py` & `llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/auto_retriever/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/auto_retriever/prompts.py` & `llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/indices/vector_store/retrievers/retriever.py` & `llama_index_core-0.9.56/llama_index/core/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/ingestion/cache.py` & `llama_index_core-0.9.56/llama_index/core/ingestion/cache.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/ingestion/pipeline.py` & `llama_index_core-0.9.56/llama_index/core/ingestion/pipeline.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/langchain_helpers/agents/__init__.py` & `llama_index_core-0.9.56/llama_index/core/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/langchain_helpers/agents/agents.py` & `llama_index_core-0.9.56/llama_index/core/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/langchain_helpers/agents/toolkits.py` & `llama_index_core-0.9.56/llama_index/core/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/langchain_helpers/agents/tools.py` & `llama_index_core-0.9.56/llama_index/core/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/langchain_helpers/memory_wrapper.py` & `llama_index_core-0.9.56/llama_index/core/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/langchain_helpers/streaming.py` & `llama_index_core-0.9.56/llama_index/core/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llama_dataset/__init__.py` & `llama_index_core-0.9.56/llama_index/core/llama_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llama_dataset/base.py` & `llama_index_core-0.9.56/llama_index/core/llama_dataset/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llama_dataset/download.py` & `llama_index_core-0.9.56/llama_index/core/llama_dataset/download.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llama_dataset/evaluator_evaluation.py` & `llama_index_core-0.9.56/llama_index/core/llama_dataset/evaluator_evaluation.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llama_dataset/generator.py` & `llama_index_core-0.9.56/llama_index/core/llama_dataset/generator.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llama_dataset/legacy/embedding.py` & `llama_index_core-0.9.56/llama_index/core/llama_dataset/legacy/embedding.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llama_dataset/rag.py` & `llama_index_core-0.9.56/llama_index/core/llama_dataset/rag.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llama_pack/download.py` & `llama_index_core-0.9.56/llama_index/core/llama_pack/download.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/__init__.py` & `llama_index_core-0.9.56/llama_index/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/base.py` & `llama_index_core-0.9.56/llama_index/core/llms/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/callbacks.py` & `llama_index_core-0.9.56/llama_index/core/llms/callbacks.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/custom.py` & `llama_index_core-0.9.56/llama_index/core/llms/custom.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/generic_utils.py` & `llama_index_core-0.9.56/llama_index/core/llms/generic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/llm.py` & `llama_index_core-0.9.56/llama_index/core/llms/llm.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/loading.py` & `llama_index_core-0.9.56/llama_index/core/llms/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/mock.py` & `llama_index_core-0.9.56/llama_index/core/llms/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/llms/utils.py` & `llama_index_core-0.9.56/llama_index/core/llms/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/memory/chat_memory_buffer.py` & `llama_index_core-0.9.56/llama_index/core/memory/chat_memory_buffer.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/memory/types.py` & `llama_index_core-0.9.56/llama_index/core/memory/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/multi_modal_llms/base.py` & `llama_index_core-0.9.56/llama_index/core/multi_modal_llms/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/multi_modal_llms/generic_utils.py` & `llama_index_core-0.9.56/llama_index/core/multi_modal_llms/generic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/__init__.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/file/html.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/file/html.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/file/json.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/file/json.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/file/markdown.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/file/markdown.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/file/simple_file.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/file/simple_file.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/interface.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/loading.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/node_utils.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/relational/base_element.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/relational/base_element.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     @abstractmethod
     def extract_elements(self, text: str, **kwargs: Any) -> List[Element]:
         """Extract elements from text."""
 
     def get_table_elements(self, elements: List[Element]) -> List[Element]:
         """Get table elements."""
-        return [e for e in elements if e.type == "table"]
+        return [e for e in elements if e.type == "table" or e.type == "table_text"]
 
     def get_text_elements(self, elements: List[Element]) -> List[Element]:
         """Get text elements."""
         # TODO: There we should maybe do something with titles
         # and other elements in the future?
         return [e for e in elements if e.type != "table"]
 
@@ -151,15 +151,15 @@
             llm = OpenAI()
         llm = cast(LLM, llm)
 
         service_context = ServiceContext.from_defaults(llm=llm, embed_model=None)
 
         table_context_list = []
         for idx, element in tqdm(enumerate(elements)):
-            if element.type != "table":
+            if element.type not in ("table", "table_text"):
                 continue
             table_context = str(element.element)
             if idx > 0 and str(elements[idx - 1].element).lower().strip().startswith(
                 "table"
             ):
                 table_context = str(elements[idx - 1].element) + "\n" + table_context
             if idx < len(elements) + 1 and str(
@@ -254,25 +254,45 @@
         from llama_index.core.node_parser import SentenceSplitter
 
         node_parser = SentenceSplitter()
 
         nodes = []
         cur_text_el_buffer: List[str] = []
         for element in elements:
-            if element.type == "table":
-                # flush text buffer
+            if element.type == "table" or element.type == "table_text":
+                # flush text buffer for table
                 if len(cur_text_el_buffer) > 0:
                     cur_text_nodes = self._get_nodes_from_buffer(
                         cur_text_el_buffer, node_parser
                     )
                     nodes.extend(cur_text_nodes)
                     cur_text_el_buffer = []
 
                 table_output = cast(TableOutput, element.table_output)
-                table_df = cast(pd.DataFrame, element.table)
+                table_md = ""
+                if element.type == "table":
+                    table_df = cast(pd.DataFrame, element.table)
+                    # We serialize the table as markdown as it allow better accuracy
+                    # We do not use the table_df.to_markdown() method as it generate
+                    # a table with a token hungry format.
+                    table_md = "|"
+                    for col_name, col in table_df.items():
+                        table_md += f"{col_name}|"
+                    table_md += "\n|"
+                    for col_name, col in table_df.items():
+                        table_md += f"---|"
+                    table_md += "\n"
+                    for row in table_df.itertuples():
+                        table_md += "|"
+                        for col in row[1:]:
+                            table_md += f"{col}|"
+                        table_md += "\n"
+                elif element.type == "table_text":
+                    # if the table is non-perfect table, we still want to keep the original text of table
+                    table_md = str(element.element)
                 table_id = element.id + "_table"
                 table_ref_id = element.id + "_table_ref"
 
                 col_schema = "\n\n".join([str(col) for col in table_output.columns])
 
                 # We build a summary of the table containing the extracted summary, and a description of the columns
                 table_summary = str(table_output.summary)
@@ -289,37 +309,24 @@
                     text=table_summary,
                     metadata={"col_schema": col_schema},
                     excluded_embed_metadata_keys=["col_schema"],
                     id_=table_ref_id,
                     index_id=table_id,
                 )
 
-                # We serialize the table as markdown as it allow better accuracy
-                # We do not use the table_df.to_markdown() method as it generate
-                # a table with a token hngry format.
-                table_md = "|"
-                for col_name, col in table_df.items():
-                    table_md += f"{col_name}|"
-                table_md += "\n|"
-                for col_name, col in table_df.items():
-                    table_md += f"---|"
-                table_md += "\n"
-                for row in table_df.itertuples():
-                    table_md += "|"
-                    for col in row[1:]:
-                        table_md += f"{col}|"
-                    table_md += "\n"
-
                 table_str = table_summary + "\n" + table_md
+
                 text_node = TextNode(
                     text=table_str,
                     id_=table_id,
                     metadata={
-                        # serialize the table as a dictionary string
-                        "table_df": str(table_df.to_dict()),
+                        # serialize the table as a dictionary string for dataframe of perfect table
+                        "table_df": str(table_df.to_dict())
+                        if element.type == "table"
+                        else table_md,
                         # add table summary for retrieval purposes
                         "table_summary": table_summary,
                     },
                     excluded_embed_metadata_keys=["table_df", "table_summary"],
                     excluded_llm_metadata_keys=["table_df", "table_summary"],
                 )
                 nodes.extend([index_node, text_node])
```

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/relational/hierarchical.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/relational/hierarchical.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/relational/markdown_element.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/relational/markdown_element.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,35 +140,49 @@
                     )
         if currentElement is not None:
             elements.append(currentElement)
 
         for idx, element in enumerate(elements):
             if element.type == "table":
                 should_keep = True
+                perfect_table = True
 
                 # verify that the table (markdown) have the same number of columns on each rows
                 table_lines = element.element.split("\n")
                 table_columns = [len(line.split("|")) for line in table_lines]
                 if len(set(table_columns)) > 1:
-                    should_keep = False
+                    # if the table have different number of columns on each rows, it's not a perfect table
+                    # we will store the raw text for such tables instead of converting them to a dataframe
+                    perfect_table = False
 
                 # verify that the table (markdown) have at least 2 rows
                 if len(table_lines) < 2:
                     should_keep = False
 
                 # apply the table filter, now only filter empty tables
-                if should_keep and table_filters is not None:
+                if should_keep and perfect_table and table_filters is not None:
                     should_keep = all(tf(element) for tf in table_filters)
 
                 # if the element is a table, convert it to a dataframe
                 if should_keep:
-                    table = md_to_df(element.element)
-                    elements[idx] = Element(
-                        id=f"id_{idx}", type="table", element=element, table=table
-                    )
+                    if perfect_table:
+                        table = md_to_df(element.element)
+
+                        elements[idx] = Element(
+                            id=f"id_{idx}", type="table", element=element, table=table
+                        )
+                    else:
+                        # for non-perfect tables, we will store the raw text
+                        # and give it a different type to differentiate it from perfect tables
+                        elements[idx] = Element(
+                            id=f"id_{idx}",
+                            type="table_text",
+                            element=element.element,
+                            # table=table
+                        )
                 else:
                     elements[idx] = Element(
                         id=f"id_{idx}",
                         type="text",
                         element=element.element,
                     )
             else:
```

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/relational/unstructured_element.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/relational/unstructured_element.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/text/__init__.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/text/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/text/code.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/text/code.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/text/langchain.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/text/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/text/semantic_splitter.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/text/semantic_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/text/sentence.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/text/sentence.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/text/sentence_window.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/text/sentence_window.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/text/token.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/text/token.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/node_parser/text/utils.py` & `llama_index_core-0.9.56/llama_index/core/node_parser/text/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/objects/__init__.py` & `llama_index_core-0.9.56/llama_index/core/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/objects/base.py` & `llama_index_core-0.9.56/llama_index/core/objects/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/objects/base_node_mapping.py` & `llama_index_core-0.9.56/llama_index/core/objects/base_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/objects/table_node_mapping.py` & `llama_index_core-0.9.56/llama_index/core/objects/table_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/objects/tool_node_mapping.py` & `llama_index_core-0.9.56/llama_index/core/objects/tool_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/output_parsers/base.py` & `llama_index_core-0.9.56/llama_index/core/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/output_parsers/langchain.py` & `llama_index_core-0.9.56/llama_index/core/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/output_parsers/pydantic.py` & `llama_index_core-0.9.56/llama_index/core/output_parsers/pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/output_parsers/selection.py` & `llama_index_core-0.9.56/llama_index/core/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/output_parsers/utils.py` & `llama_index_core-0.9.56/llama_index/core/output_parsers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/playground/base.py` & `llama_index_core-0.9.56/llama_index/core/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/__init__.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/llm_rerank.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/llm_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/metadata_replacement.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/metadata_replacement.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/node.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/node_recency.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/optimizer.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/pii.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/rankGPT_rerank.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/rankGPT_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/sbert_rerank.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/sbert_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/postprocessor/types.py` & `llama_index_core-0.9.56/llama_index/core/postprocessor/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/program/llm_program.py` & `llama_index_core-0.9.56/llama_index/core/program/llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/program/llm_prompt_program.py` & `llama_index_core-0.9.56/llama_index/core/program/llm_prompt_program.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/program/multi_modal_llm_program.py` & `llama_index_core-0.9.56/llama_index/core/program/multi_modal_llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/program/utils.py` & `llama_index_core-0.9.56/llama_index/core/program/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/__init__.py` & `llama_index_core-0.9.56/llama_index/core/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/base.py` & `llama_index_core-0.9.56/llama_index/core/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/chat_prompts.py` & `llama_index_core-0.9.56/llama_index/core/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/default_prompt_selectors.py` & `llama_index_core-0.9.56/llama_index/core/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/default_prompts.py` & `llama_index_core-0.9.56/llama_index/core/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/display_utils.py` & `llama_index_core-0.9.56/llama_index/core/prompts/display_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/guidance_utils.py` & `llama_index_core-0.9.56/llama_index/core/prompts/guidance_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/mixin.py` & `llama_index_core-0.9.56/llama_index/core/prompts/mixin.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/prompt_type.py` & `llama_index_core-0.9.56/llama_index/core/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/prompt_utils.py` & `llama_index_core-0.9.56/llama_index/core/prompts/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/prompts.py` & `llama_index_core-0.9.56/llama_index/core/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/prompts/system.py` & `llama_index_core-0.9.56/llama_index/core/prompts/system.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/__init__.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/citation_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/citation_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/cogniswitch_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/cogniswitch_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/custom.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/custom.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/flare/answer_inserter.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/flare/answer_inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/flare/base.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/flare/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/flare/output_parser.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/flare/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/graph_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/jsonalyze_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/jsonalyze_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/knowledge_graph_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/knowledge_graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/multi_modal.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/multi_modal.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/multistep_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/pandas/output_parser.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/pandas/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/pandas/pandas_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/pandas/pandas_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/retriever_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/retry_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/retry_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/retry_source_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/retry_source_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/router_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/sql_join_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/sql_join_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/sql_vector_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/sql_vector_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/sub_question_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/sub_question_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_engine/transform_query_engine.py` & `llama_index_core-0.9.56/llama_index/core/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_pipeline/__init__.py` & `llama_index_core-0.9.56/llama_index/core/query_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_pipeline/components/agent.py` & `llama_index_core-0.9.56/llama_index/core/query_pipeline/components/agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_pipeline/components/argpacks.py` & `llama_index_core-0.9.56/llama_index/core/query_pipeline/components/argpacks.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_pipeline/components/function.py` & `llama_index_core-0.9.56/llama_index/core/query_pipeline/components/function.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_pipeline/components/input.py` & `llama_index_core-0.9.56/llama_index/core/query_pipeline/components/input.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_pipeline/components/router.py` & `llama_index_core-0.9.56/llama_index/core/query_pipeline/components/router.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_pipeline/components/tool_runner.py` & `llama_index_core-0.9.56/llama_index/core/query_pipeline/components/tool_runner.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/query_pipeline/query.py` & `llama_index_core-0.9.56/llama_index/core/query_pipeline/query.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/question_gen/llm_generators.py` & `llama_index_core-0.9.56/llama_index/core/question_gen/llm_generators.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/question_gen/output_parser.py` & `llama_index_core-0.9.56/llama_index/core/question_gen/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/question_gen/prompts.py` & `llama_index_core-0.9.56/llama_index/core/question_gen/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/question_gen/types.py` & `llama_index_core-0.9.56/llama_index/core/question_gen/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/readers/__init__.py` & `llama_index_core-0.9.56/llama_index/core/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/readers/base.py` & `llama_index_core-0.9.56/llama_index/core/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/readers/download.py` & `llama_index_core-0.9.56/llama_index/core/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/readers/file/base.py` & `llama_index_core-0.9.56/llama_index/core/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/readers/json.py` & `llama_index_core-0.9.56/llama_index/core/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/readers/loading.py` & `llama_index_core-0.9.56/llama_index/core/readers/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/readers/string_iterable.py` & `llama_index_core-0.9.56/llama_index/core/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response/notebook_utils.py` & `llama_index_core-0.9.56/llama_index/core/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response/pprint_utils.py` & `llama_index_core-0.9.56/llama_index/core/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/__init__.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/accumulate.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/base.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/compact_and_accumulate.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/compact_and_accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/compact_and_refine.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/compact_and_refine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/factory.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/factory.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/generation.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/generation.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/no_text.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/no_text.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/refine.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/refine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/simple_summarize.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/simple_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/tree_summarize.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/response_synthesizers/type.py` & `llama_index_core-0.9.56/llama_index/core/response_synthesizers/type.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/retrievers/__init__.py` & `llama_index_core-0.9.56/llama_index/core/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/retrievers/auto_merging_retriever.py` & `llama_index_core-0.9.56/llama_index/core/retrievers/auto_merging_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/retrievers/fusion_retriever.py` & `llama_index_core-0.9.56/llama_index/core/retrievers/fusion_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/retrievers/recursive_retriever.py` & `llama_index_core-0.9.56/llama_index/core/retrievers/recursive_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/retrievers/router_retriever.py` & `llama_index_core-0.9.56/llama_index/core/retrievers/router_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/retrievers/transform_retriever.py` & `llama_index_core-0.9.56/llama_index/core/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/schema.py` & `llama_index_core-0.9.56/llama_index/core/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/selectors/embedding_selectors.py` & `llama_index_core-0.9.56/llama_index/core/selectors/embedding_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/selectors/llm_selectors.py` & `llama_index_core-0.9.56/llama_index/core/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/selectors/prompts.py` & `llama_index_core-0.9.56/llama_index/core/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/selectors/pydantic_selectors.py` & `llama_index_core-0.9.56/llama_index/core/selectors/pydantic_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/selectors/types.py` & `llama_index_core-0.9.56/llama_index/core/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/selectors/utils.py` & `llama_index_core-0.9.56/llama_index/core/selectors/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/service_context.py` & `llama_index_core-0.9.56/llama_index/core/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/service_context_elements/llama_logger.py` & `llama_index_core-0.9.56/llama_index/core/service_context_elements/llama_logger.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/service_context_elements/llm_predictor.py` & `llama_index_core-0.9.56/llama_index/core/service_context_elements/llm_predictor.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/settings.py` & `llama_index_core-0.9.56/llama_index/core/settings.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/chat_store/base.py` & `llama_index_core-0.9.56/llama_index/core/storage/chat_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/chat_store/loading.py` & `llama_index_core-0.9.56/llama_index/core/storage/chat_store/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/chat_store/simple_chat_store.py` & `llama_index_core-0.9.56/llama_index/core/storage/chat_store/simple_chat_store.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/docstore/keyval_docstore.py` & `llama_index_core-0.9.56/llama_index/core/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/docstore/postgres_docstore.py` & `llama_index_core-0.9.56/llama_index/core/storage/docstore/postgres_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/docstore/registry.py` & `llama_index_core-0.9.56/llama_index/core/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/docstore/simple_docstore.py` & `llama_index_core-0.9.56/llama_index/core/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/docstore/types.py` & `llama_index_core-0.9.56/llama_index/core/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/docstore/utils.py` & `llama_index_core-0.9.56/llama_index/core/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/index_store/keyval_index_store.py` & `llama_index_core-0.9.56/llama_index/core/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/index_store/postgres_index_store.py` & `llama_index_core-0.9.56/llama_index/core/storage/index_store/postgres_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/index_store/simple_index_store.py` & `llama_index_core-0.9.56/llama_index/core/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/index_store/types.py` & `llama_index_core-0.9.56/llama_index/core/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/index_store/utils.py` & `llama_index_core-0.9.56/llama_index/core/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/kvstore/postgres_kvstore.py` & `llama_index_core-0.9.56/llama_index/core/storage/kvstore/postgres_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/kvstore/simple_kvstore.py` & `llama_index_core-0.9.56/llama_index/core/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/kvstore/types.py` & `llama_index_core-0.9.56/llama_index/core/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/storage/storage_context.py` & `llama_index_core-0.9.56/llama_index/core/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/__init__.py` & `llama_index_core-0.9.56/llama_index/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/download.py` & `llama_index_core-0.9.56/llama_index/core/tools/download.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/function_tool.py` & `llama_index_core-0.9.56/llama_index/core/tools/function_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/ondemand_loader_tool.py` & `llama_index_core-0.9.56/llama_index/core/tools/ondemand_loader_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/query_engine.py` & `llama_index_core-0.9.56/llama_index/core/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/query_plan.py` & `llama_index_core-0.9.56/llama_index/core/tools/query_plan.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/retriever_tool.py` & `llama_index_core-0.9.56/llama_index/core/tools/retriever_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/tool_spec/base.py` & `llama_index_core-0.9.56/llama_index/core/tools/tool_spec/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/tool_spec/load_and_search/README.md` & `llama_index_core-0.9.56/llama_index/core/tools/tool_spec/load_and_search/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/tool_spec/load_and_search/base.py` & `llama_index_core-0.9.56/llama_index/core/tools/tool_spec/load_and_search/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/types.py` & `llama_index_core-0.9.56/llama_index/core/tools/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/tools/utils.py` & `llama_index_core-0.9.56/llama_index/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/types.py` & `llama_index_core-0.9.56/llama_index/core/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/utilities/aws_utils.py` & `llama_index_core-0.9.56/llama_index/core/utilities/aws_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/utilities/sql_wrapper.py` & `llama_index_core-0.9.56/llama_index/core/utilities/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/utilities/token_counting.py` & `llama_index_core-0.9.56/llama_index/core/utilities/token_counting.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/utils.py` & `llama_index_core-0.9.56/llama_index/core/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/vector_stores/simple.py` & `llama_index_core-0.9.56/llama_index/core/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/vector_stores/types.py` & `llama_index_core-0.9.56/llama_index/core/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/llama_index/core/vector_stores/utils.py` & `llama_index_core-0.9.56/llama_index/core/vector_stores/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_core-0.9.55/pyproject.toml` & `llama_index_core-0.9.56/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   "Simon Suo <simon@llamaindex.ai>",
   "Sourabh Desai <sourabh@llamaindex.ai>"
 ]
 name = "llama-index-core"
 packages = [{include = "llama_index"}]
 readme = "README.md"
 repository = "https://github.com/run-llama/llama_index"
-version = "0.9.55"
+version = "0.9.56"
 
 [tool.poetry.dependencies]
 SQLAlchemy = {extras = ["asyncio"], version = ">=1.4.49"}
 beautifulsoup4 = {optional = true, version = "^4.12.2"}
 dataclasses-json = "*"
 deprecated = ">=1.2.9.3"
 fsspec = ">=2023.5.0"
```

### Comparing `llama_index_core-0.9.55/PKG-INFO` & `llama_index_core-0.9.56/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-core
-Version: 0.9.55
+Version: 0.9.56
 Summary: Interface between LLMs and your data
 Home-page: https://llamaindex.ai
 License: MIT
 Keywords: LLM,NLP,RAG,data,devtools,index,retrieval
 Author: Jerry Liu
 Author-email: jerry@llamaindex.ai
 Maintainer: Andrei Fajardo
```

