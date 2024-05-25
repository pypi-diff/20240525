# Comparing `tmp/llama_index-0.9.8.post1.tar.gz` & `tmp/llama_index-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.9.8.post1.tar", max compression
+gzip compressed data, was "llama_index-0.9.9.tar", max compression
```

## Comparing `llama_index-0.9.8.post1.tar` & `llama_index-0.9.9.tar`

### file list

```diff
@@ -1,626 +1,631 @@
--rw-r--r--   0        0        0     1065 2023-11-27 17:22:19.557165 llama_index-0.9.8.post1/LICENSE
--rw-r--r--   0        0        0     5541 2023-11-27 17:22:19.557165 llama_index-0.9.8.post1/README.md
--rw-r--r--   0        0        0       12 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/VERSION
--rw-r--r--   0        0        0     4859 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/__init__.py
--rw-r--r--   0        0        0      620 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/__init__.py
--rw-r--r--   0        0        0     7343 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/context_retriever_agent.py
--rw-r--r--   0        0        0    22887 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/openai_agent.py
--rw-r--r--   0        0        0    13320 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/openai_assistant_agent.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/react/__init__.py
--rw-r--r--   0        0        0    19759 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/react/base.py
--rw-r--r--   0        0        0     2841 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/react/formatter.py
--rw-r--r--   0        0        0     3174 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/react/output_parser.py
--rw-r--r--   0        0        0     1728 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/react/prompts.py
--rw-r--r--   0        0        0     1796 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/react/types.py
--rw-r--r--   0        0        0      833 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/retriever_openai_agent.py
--rw-r--r--   0        0        0     2062 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/agent/types.py
--rw-r--r--   0        0        0     2715 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/async_utils.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/bridge/__init__.py
--rw-r--r--   0        0        0     2769 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/bridge/langchain.py
--rw-r--r--   0        0        0     1132 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/bridge/pydantic.py
--rw-r--r--   0        0        0      756 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/__init__.py
--rw-r--r--   0        0        0     6808 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/aim.py
--rw-r--r--   0        0        0      596 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/arize_phoenix_callback.py
--rw-r--r--   0        0        0    10124 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/base.py
--rw-r--r--   0        0        0     1659 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/base_handler.py
--rw-r--r--   0        0        0     7532 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/finetuning_handler.py
--rw-r--r--   0        0        0     1430 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/global_handlers.py
--rw-r--r--   0        0        0      406 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/honeyhive_callback.py
--rw-r--r--   0        0        0     7856 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/llama_debug.py
--rw-r--r--   0        0        0     7933 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/open_inference_callback.py
--rw-r--r--   0        0        0     3572 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/schema.py
--rw-r--r--   0        0        0     2146 2023-11-27 17:22:20.053165 llama_index-0.9.8.post1/llama_index/callbacks/simple_llm_handler.py
--rw-r--r--   0        0        0     7421 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/callbacks/token_counting.py
--rw-r--r--   0        0        0     2006 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/callbacks/utils.py
--rw-r--r--   0        0        0    21044 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/callbacks/wandb_callback.py
--rw-r--r--   0        0        0      426 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/chat_engine/__init__.py
--rw-r--r--   0        0        0    14114 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/chat_engine/condense_plus_context.py
--rw-r--r--   0        0        0    13834 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/chat_engine/condense_question.py
--rw-r--r--   0        0        0    11289 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/chat_engine/context.py
--rw-r--r--   0        0        0     6154 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/chat_engine/simple.py
--rw-r--r--   0        0        0    10305 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/chat_engine/types.py
--rw-r--r--   0        0        0      460 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/chat_engine/utils.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/command_line/__init__.py
--rw-r--r--   0        0        0     1851 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/command_line/command_line.py
--rw-r--r--   0        0        0      232 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/composability/__init__.py
--rw-r--r--   0        0        0      165 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/composability/base.py
--rw-r--r--   0        0        0     3411 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0        0        0      672 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/constants.py
--rw-r--r--   0        0        0      373 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/core/__init__.py
--rw-r--r--   0        0        0     1773 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/core/base_multi_modal_retriever.py
--rw-r--r--   0        0        0     2474 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/core/base_query_engine.py
--rw-r--r--   0        0        0     3826 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/core/base_retriever.py
--rw-r--r--   0        0        0     3211 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/core/image_retriever.py
--rw-r--r--   0        0        0      327 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/data_structs/__init__.py
--rw-r--r--   0        0        0     8100 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/data_structs/data_structs.py
--rw-r--r--   0        0        0     2284 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/data_structs/document_summary.py
--rw-r--r--   0        0        0     1006 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/data_structs/registry.py
--rw-r--r--   0        0        0     4240 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/data_structs/struct_type.py
--rw-r--r--   0        0        0     1025 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/data_structs/table.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/download/__init__.py
--rw-r--r--   0        0        0    10834 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/download/download_utils.py
--rw-r--r--   0        0        0     2589 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/__init__.py
--rw-r--r--   0        0        0     4200 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/adapter.py
--rw-r--r--   0        0        0     5487 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/adapter_utils.py
--rw-r--r--   0        0        0     3469 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/azure_openai.py
--rw-r--r--   0        0        0    12407 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/base.py
--rw-r--r--   0        0        0     6580 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/bedrock.py
--rw-r--r--   0        0        0     5132 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/clarifai.py
--rw-r--r--   0        0        0     4763 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/clip.py
--rw-r--r--   0        0        0     6222 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/cohereai.py
--rw-r--r--   0        0        0     6197 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/elasticsearch.py
--rw-r--r--   0        0        0     3546 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/fastembed.py
--rw-r--r--   0        0        0     2075 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/google.py
--rw-r--r--   0        0        0     2655 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/google_palm.py
--rw-r--r--   0        0        0     4782 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/gradient.py
--rw-r--r--   0        0        0    11330 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/huggingface.py
--rw-r--r--   0        0        0     6518 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/huggingface_optimum.py
--rw-r--r--   0        0        0     2488 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/huggingface_utils.py
--rw-r--r--   0        0        0     3603 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/instructor.py
--rw-r--r--   0        0        0     3990 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/jinaai.py
--rw-r--r--   0        0        0     3142 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/langchain.py
--rw-r--r--   0        0        0     3739 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/llm_rails.py
--rw-r--r--   0        0        0     1845 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/loading.py
--rw-r--r--   0        0        0     6812 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/multi_modal_base.py
--rw-r--r--   0        0        0    11864 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/openai.py
--rw-r--r--   0        0        0     1266 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/pooling.py
--rw-r--r--   0        0        0     4493 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/text_embeddings_inference.py
--rw-r--r--   0        0        0     3527 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/utils.py
--rw-r--r--   0        0        0     3171 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/embeddings/voyageai.py
--rw-r--r--   0        0        0     2298 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/__init__.py
--rw-r--r--   0        0        0     3808 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/base.py
--rw-r--r--   0        0        0    11209 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/batch_runner.py
--rw-r--r--   0        0        0      188 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/benchmarks/__init__.py
--rw-r--r--   0        0        0     3686 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/benchmarks/beir.py
--rw-r--r--   0        0        0     7507 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/benchmarks/hotpotqa.py
--rw-r--r--   0        0        0     4677 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/correctness.py
--rw-r--r--   0        0        0    11765 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0        0        0     1804 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/eval_utils.py
--rw-r--r--   0        0        0     5936 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/faithfulness.py
--rw-r--r--   0        0        0     4165 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/guideline.py
--rw-r--r--   0        0        0      305 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/multi_modal/__init__.py
--rw-r--r--   0        0        0     8115 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/multi_modal/faithfulness.py
--rw-r--r--   0        0        0     7181 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/multi_modal/relevancy.py
--rw-r--r--   0        0        0     2096 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/notebook_utils.py
--rw-r--r--   0        0        0     8845 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/pairwise.py
--rw-r--r--   0        0        0     4987 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/relevancy.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.057165 llama_index-0.9.8.post1/llama_index/evaluation/retrieval/__init__.py
--rw-r--r--   0        0        0     5562 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/evaluation/retrieval/base.py
--rw-r--r--   0        0        0     2780 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/evaluation/retrieval/evaluator.py
--rw-r--r--   0        0        0     1963 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/evaluation/retrieval/metrics.py
--rw-r--r--   0        0        0     1378 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/evaluation/retrieval/metrics_base.py
--rw-r--r--   0        0        0     2891 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/evaluation/semantic_similarity.py
--rw-r--r--   0        0        0     2528 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/exec_utils.py
--rw-r--r--   0        0        0      585 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/extractors/__init__.py
--rw-r--r--   0        0        0     5253 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/extractors/interface.py
--rw-r--r--   0        0        0     1086 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/extractors/loading.py
--rw-r--r--   0        0        0     2991 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/extractors/marvin_metadata_extractor.py
--rw-r--r--   0        0        0    22105 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/extractors/metadata_extractors.py
--rw-r--r--   0        0        0     1003 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/__init__.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/cross_encoders/__init__.py
--rw-r--r--   0        0        0     4792 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/cross_encoders/cross_encoder.py
--rw-r--r--   0        0        0     9446 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/cross_encoders/dataset_gen.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/embeddings/__init__.py
--rw-r--r--   0        0        0     6361 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/embeddings/adapter.py
--rw-r--r--   0        0        0     5010 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/embeddings/adapter_utils.py
--rw-r--r--   0        0        0     3113 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/embeddings/common.py
--rw-r--r--   0        0        0     3022 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/gradient/__init__.py
--rw-r--r--   0        0        0     4946 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/gradient/base.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/openai/__init__.py
--rw-r--r--   0        0        0     3836 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/openai/base.py
--rw-r--r--   0        0        0     6562 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/openai/validate_json.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/rerankers/__init__.py
--rw-r--r--   0        0        0     2720 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/rerankers/cohere_reranker.py
--rw-r--r--   0        0        0     4690 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/rerankers/dataset_gen.py
--rw-r--r--   0        0        0     1548 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/finetuning/types.py
--rw-r--r--   0        0        0      463 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/graph_stores/__init__.py
--rw-r--r--   0        0        0     6075 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/graph_stores/falkordb.py
--rw-r--r--   0        0        0     8829 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/graph_stores/kuzu.py
--rw-r--r--   0        0        0    25956 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/graph_stores/nebulagraph.py
--rw-r--r--   0        0        0     9481 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/graph_stores/neo4j.py
--rw-r--r--   0        0        0     1041 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/graph_stores/registry.py
--rw-r--r--   0        0        0     6102 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/graph_stores/simple.py
--rw-r--r--   0        0        0     2096 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/graph_stores/types.py
--rw-r--r--   0        0        0      522 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/img_utils.py
--rw-r--r--   0        0        0     2346 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/__init__.py
--rw-r--r--   0        0        0    16424 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/base.py
--rw-r--r--   0        0        0      109 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/base_retriever.py
--rw-r--r--   0        0        0       17 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/common/__init__.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0        0        0     8572 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0        0        0      776 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0        0        0     2653 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/common/struct_store/sql.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0        0        0     8776 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/common_tree/base.py
--rw-r--r--   0        0        0      180 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/composability/__init__.py
--rw-r--r--   0        0        0     4869 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/composability/graph.py
--rw-r--r--   0        0        0      536 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0        0        0     8938 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/document_summary/base.py
--rw-r--r--   0        0        0     6720 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/document_summary/retrievers.py
--rw-r--r--   0        0        0      224 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/empty/__init__.py
--rw-r--r--   0        0        0     2841 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/empty/base.py
--rw-r--r--   0        0        0     1240 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/empty/retrievers.py
--rw-r--r--   0        0        0     2374 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/keyword_table/README.md
--rw-r--r--   0        0        0      860 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0        0        0     8716 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/keyword_table/base.py
--rw-r--r--   0        0        0     1068 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0        0        0     5836 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0        0        0     1268 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0        0        0     2264 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/keyword_table/utils.py
--rw-r--r--   0        0        0      403 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0        0        0    12094 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0        0        0    33724 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0        0        0     1017 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/list/README.md
--rw-r--r--   0        0        0      618 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/list/__init__.py
--rw-r--r--   0        0        0     4542 2023-11-27 17:22:20.061165 llama_index-0.9.8.post1/llama_index/indices/list/base.py
--rw-r--r--   0        0        0     7397 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/list/retrievers.py
--rw-r--r--   0        0        0     3582 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/loading.py
--rw-r--r--   0        0        0      271 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/managed/__init__.py
--rw-r--r--   0        0        0     3417 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/managed/base.py
--rw-r--r--   0        0        0      172 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/managed/types.py
--rw-r--r--   0        0        0      189 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/managed/vectara/__init__.py
--rw-r--r--   0        0        0    11749 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/managed/vectara/base.py
--rw-r--r--   0        0        0     5336 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/managed/vectara/query.py
--rw-r--r--   0        0        0     8046 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/managed/vectara/retriever.py
--rw-r--r--   0        0        0     4962 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/managed.tar.gz
--rw-r--r--   0        0        0      291 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/multi_modal/__init__.py
--rw-r--r--   0        0        0    13661 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/multi_modal/base.py
--rw-r--r--   0        0        0    13967 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/multi_modal/retriever.py
--rw-r--r--   0        0        0     1052 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/postprocessor.py
--rw-r--r--   0        0        0    10446 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/prompt_helper.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/query/__init__.py
--rw-r--r--   0        0        0      113 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/query/base.py
--rw-r--r--   0        0        0     6094 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/query/embedding_utils.py
--rw-r--r--   0        0        0      281 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0        0        0    10659 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0        0        0     4568 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/query/query_transform/feedback_transform.py
--rw-r--r--   0        0        0     5190 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0        0        0      124 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/query/schema.py
--rw-r--r--   0        0        0     1382 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/registry.py
--rw-r--r--   0        0        0      122 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/service_context.py
--rw-r--r--   0        0        0      955 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0        0        0     2376 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/struct_store/base.py
--rw-r--r--   0        0        0     5722 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0        0        0     7707 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/struct_store/json_query.py
--rw-r--r--   0        0        0     2385 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0        0        0     6115 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/struct_store/sql.py
--rw-r--r--   0        0        0    18002 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/struct_store/sql_query.py
--rw-r--r--   0        0        0    14146 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/struct_store/sql_retriever.py
--rw-r--r--   0        0        0     2640 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/README.md
--rw-r--r--   0        0        0      657 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/__init__.py
--rw-r--r--   0        0        0     1704 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0        0        0     6738 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/base.py
--rw-r--r--   0        0        0     7936 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/inserter.py
--rw-r--r--   0        0        0     4675 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0        0        0    15387 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0        0        0     1546 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0        0        0      780 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/tree/utils.py
--rw-r--r--   0        0        0     8279 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/utils.py
--rw-r--r--   0        0        0      386 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0        0        0    12347 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/vector_store/base.py
--rw-r--r--   0        0        0      290 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/__init__.py
--rw-r--r--   0        0        0      167 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0        0        0     5286 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0        0        0      645 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0        0        0     2701 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0        0        0     7230 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/retriever.py
--rw-r--r--   0        0        0      293 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/ingestion/__init__.py
--rw-r--r--   0        0        0     2824 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/ingestion/cache.py
--rw-r--r--   0        0        0     7915 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/ingestion/pipeline.py
--rw-r--r--   0        0        0      237 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/langchain_helpers/__init__.py
--rw-r--r--   0        0        0      514 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0        0        0     2923 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0        0        0      807 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0        0        0     2469 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0        0        0     7623 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0        0        0     1347 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/langchain_helpers/streaming.py
--rw-r--r--   0        0        0       65 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/langchain_helpers/text_splitter.py
--rw-r--r--   0        0        0      198 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llama_pack/__init__.py
--rw-r--r--   0        0        0      293 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llama_pack/base.py
--rw-r--r--   0        0        0     1173 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llama_pack/download.py
--rw-r--r--   0        0        0      390 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/__init__.py
--rw-r--r--   0        0        0    10984 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/base.py
--rw-r--r--   0        0        0     1088 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/loading.py
--rw-r--r--   0        0        0     5663 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/mock.py
--rw-r--r--   0        0        0     2706 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/structured.py
--rw-r--r--   0        0        0     1478 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/utils.py
--rw-r--r--   0        0        0      386 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/__init__.py
--rw-r--r--   0        0        0      151 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/exceptions.py
--rw-r--r--   0        0        0     7299 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/predictor.py
--rw-r--r--   0        0        0     9841 2023-11-27 17:22:20.065165 llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/prompt_registry.py
--rw-r--r--   0        0        0     1035 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/types.py
--rw-r--r--   0        0        0      238 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/utils.py
--rw-r--r--   0        0        0     2539 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/__init__.py
--rw-r--r--   0        0        0     4009 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/ai21.py
--rw-r--r--   0        0        0      567 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/ai21_utils.py
--rw-r--r--   0        0        0     7864 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/anthropic.py
--rw-r--r--   0        0        0     1758 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/anthropic_utils.py
--rw-r--r--   0        0        0     2009 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/anyscale.py
--rw-r--r--   0        0        0     2312 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/anyscale_utils.py
--rw-r--r--   0        0        0     5886 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/azure_openai.py
--rw-r--r--   0        0        0    15458 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/base.py
--rw-r--r--   0        0        0     8647 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/bedrock.py
--rw-r--r--   0        0        0     7082 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/bedrock_utils.py
--rw-r--r--   0        0        0     5645 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/clarifai.py
--rw-r--r--   0        0        0    10611 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/cohere.py
--rw-r--r--   0        0        0     3166 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/cohere_utils.py
--rw-r--r--   0        0        0     2250 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/custom.py
--rw-r--r--   0        0        0     1854 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/everlyai.py
--rw-r--r--   0        0        0     1082 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/everlyai_utils.py
--rw-r--r--   0        0        0     9582 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/generic_utils.py
--rw-r--r--   0        0        0     4897 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/gradient.py
--rw-r--r--   0        0        0    22189 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/huggingface.py
--rw-r--r--   0        0        0    20175 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/konko.py
--rw-r--r--   0        0        0     7085 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/konko_utils.py
--rw-r--r--   0        0        0     5158 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/langchain.py
--rw-r--r--   0        0        0     5617 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/langchain_utils.py
--rw-r--r--   0        0        0    16128 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/litellm.py
--rw-r--r--   0        0        0     6616 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/litellm_utils.py
--rw-r--r--   0        0        0     3765 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/llama_api.py
--rw-r--r--   0        0        0     9653 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/llama_cpp.py
--rw-r--r--   0        0        0     2237 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/llama_utils.py
--rw-r--r--   0        0        0     1749 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/loading.py
--rw-r--r--   0        0        0     2702 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/localai.py
--rw-r--r--   0        0        0     1856 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/mock.py
--rw-r--r--   0        0        0     5273 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/monsterapi.py
--rw-r--r--   0        0        0     5911 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/ollama.py
--rw-r--r--   0        0        0    20781 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/openai.py
--rw-r--r--   0        0        0     2613 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/openai_like.py
--rw-r--r--   0        0        0    11781 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/openai_utils.py
--rw-r--r--   0        0        0    17159 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/openllm.py
--rw-r--r--   0        0        0     3829 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/palm.py
--rw-r--r--   0        0        0    13900 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/perplexity.py
--rw-r--r--   0        0        0    10116 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/portkey.py
--rw-r--r--   0        0        0     4724 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/portkey_utils.py
--rw-r--r--   0        0        0     3453 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/predibase.py
--rw-r--r--   0        0        0     5664 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/replicate.py
--rw-r--r--   0        0        0    10586 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/rungpt.py
--rw-r--r--   0        0        0     2223 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/utils.py
--rw-r--r--   0        0        0    10657 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/vertex.py
--rw-r--r--   0        0        0     6074 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/vertex_utils.py
--rw-r--r--   0        0        0     6806 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/watsonx.py
--rw-r--r--   0        0        0     1255 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/watsonx_utils.py
--rw-r--r--   0        0        0     8285 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/xinference.py
--rw-r--r--   0        0        0     1020 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/llms/xinference_utils.py
--rw-r--r--   0        0        0       95 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/logger/__init__.py
--rw-r--r--   0        0        0      995 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/logger/base.py
--rw-r--r--   0        0        0      161 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/memory/__init__.py
--rw-r--r--   0        0        0     4733 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/memory/chat_memory_buffer.py
--rw-r--r--   0        0        0     1078 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/memory/types.py
--rw-r--r--   0        0        0      664 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/multi_modal_llms/__init__.py
--rw-r--r--   0        0        0     4393 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/multi_modal_llms/base.py
--rw-r--r--   0        0        0      618 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/multi_modal_llms/generic_utils.py
--rw-r--r--   0        0        0     7164 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/multi_modal_llms/openai.py
--rw-r--r--   0        0        0     2305 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/multi_modal_llms/openai_utils.py
--rw-r--r--   0        0        0     8108 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/multi_modal_llms/replicate_multi_modal.py
--rw-r--r--   0        0        0     1556 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/node_parser/__init__.py
--rw-r--r--   0        0        0      378 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/node_parser/file/__init__.py
--rw-r--r--   0        0        0     4115 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/node_parser/file/html.py
--rw-r--r--   0        0        0     3415 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/node_parser/file/json.py
--rw-r--r--   0        0        0     3927 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/node_parser/file/markdown.py
--rw-r--r--   0        0        0     2741 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/node_parser/file/simple_file.py
--rw-r--r--   0        0        0     6006 2023-11-27 17:22:20.069165 llama_index-0.9.8.post1/llama_index/node_parser/interface.py
--rw-r--r--   0        0        0     1694 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/loading.py
--rw-r--r--   0        0        0     2823 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/node_utils.py
--rw-r--r--   0        0        0      272 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/relational/__init__.py
--rw-r--r--   0        0        0     7498 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/relational/hierarchical.py
--rw-r--r--   0        0        0    10269 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/relational/unstructured_element.py
--rw-r--r--   0        0        0      487 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/text/__init__.py
--rw-r--r--   0        0        0     4225 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/text/code.py
--rw-r--r--   0        0        0     1489 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/text/langchain.py
--rw-r--r--   0        0        0    11636 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/text/sentence.py
--rw-r--r--   0        0        0     4811 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/text/sentence_window.py
--rw-r--r--   0        0        0     8222 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/text/token.py
--rw-r--r--   0        0        0     3126 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/node_parser/text/utils.py
--rw-r--r--   0        0        0      567 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/objects/__init__.py
--rw-r--r--   0        0        0     4254 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/objects/base.py
--rw-r--r--   0        0        0     5389 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/objects/base_node_mapping.py
--rw-r--r--   0        0        0     3021 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/objects/table_node_mapping.py
--rw-r--r--   0        0        0     4858 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/objects/tool_node_mapping.py
--rw-r--r--   0        0        0      438 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/output_parsers/__init__.py
--rw-r--r--   0        0        0      284 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/output_parsers/base.py
--rw-r--r--   0        0        0     2886 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/output_parsers/guardrails.py
--rw-r--r--   0        0        0     1864 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/output_parsers/langchain.py
--rw-r--r--   0        0        0     1670 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/output_parsers/pydantic.py
--rw-r--r--   0        0        0     3315 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/output_parsers/selection.py
--rw-r--r--   0        0        0     2189 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/output_parsers/utils.py
--rw-r--r--   0        0        0      209 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/param_tuner/__init__.py
--rw-r--r--   0        0        0     9088 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/param_tuner/base.py
--rw-r--r--   0        0        0      202 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/playground/__init__.py
--rw-r--r--   0        0        0     7036 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/playground/base.py
--rw-r--r--   0        0        0     1454 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/__init__.py
--rw-r--r--   0        0        0     2513 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/cohere_rerank.py
--rw-r--r--   0        0        0     4101 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/llm_rerank.py
--rw-r--r--   0        0        0     3994 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/longllmlingua.py
--rw-r--r--   0        0        0     1052 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/metadata_replacement.py
--rw-r--r--   0        0        0    13663 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/node.py
--rw-r--r--   0        0        0     7786 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/node_recency.py
--rw-r--r--   0        0        0     6267 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/optimizer.py
--rw-r--r--   0        0        0     5442 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/pii.py
--rw-r--r--   0        0        0     2469 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/sbert_rerank.py
--rw-r--r--   0        0        0     1829 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/postprocessor/types.py
--rw-r--r--   0        0        0      858 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/__init__.py
--rw-r--r--   0        0        0     2752 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/guidance_program.py
--rw-r--r--   0        0        0     3335 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/llm_program.py
--rw-r--r--   0        0        0      968 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/llm_prompt_program.py
--rw-r--r--   0        0        0     3607 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/lmformatenforcer_program.py
--rw-r--r--   0        0        0     3429 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/multi_modal_llm_program.py
--rw-r--r--   0        0        0     8690 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/openai_program.py
--rw-r--r--   0        0        0      321 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/predefined/__init__.py
--rw-r--r--   0        0        0     7620 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/predefined/df.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/predefined/evaporate/__init__.py
--rw-r--r--   0        0        0     9895 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/predefined/evaporate/base.py
--rw-r--r--   0        0        0     9273 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/predefined/evaporate/extractor.py
--rw-r--r--   0        0        0     4722 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/predefined/evaporate/prompts.py
--rw-r--r--   0        0        0     3288 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/program/utils.py
--rw-r--r--   0        0        0      494 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/__init__.py
--rw-r--r--   0        0        0    17219 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/base.py
--rw-r--r--   0        0        0     3604 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/chat_prompts.py
--rw-r--r--   0        0        0     1179 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0        0        0    15151 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/default_prompts.py
--rw-r--r--   0        0        0     5565 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/guidance_utils.py
--rw-r--r--   0        0        0     2132 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/lmformatenforcer_utils.py
--rw-r--r--   0        0        0     3272 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/mixin.py
--rw-r--r--   0        0        0     1720 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/prompt_type.py
--rw-r--r--   0        0        0     1093 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/prompt_utils.py
--rw-r--r--   0        0        0     3910 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/prompts.py
--rw-r--r--   0        0        0     4790 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/system.py
--rw-r--r--   0        0        0      488 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/prompts/utils.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/py.typed
--rw-r--r--   0        0        0     2501 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/query_engine/__init__.py
--rw-r--r--   0        0        0    12418 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/query_engine/citation_query_engine.py
--rw-r--r--   0        0        0     2021 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/query_engine/cogniswitch_query_engine.py
--rw-r--r--   0        0        0     2902 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/query_engine/custom.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/query_engine/flare/__init__.py
--rw-r--r--   0        0        0     6952 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/query_engine/flare/answer_inserter.py
--rw-r--r--   0        0        0    10517 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/query_engine/flare/base.py
--rw-r--r--   0        0        0     2078 2023-11-27 17:22:20.073165 llama_index-0.9.8.post1/llama_index/query_engine/flare/output_parser.py
--rw-r--r--   0        0        0      163 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/flare/schema.py
--rw-r--r--   0        0        0     4593 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0        0        0    12365 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/knowledge_graph_query_engine.py
--rw-r--r--   0        0        0     7012 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/multi_modal.py
--rw-r--r--   0        0        0     6675 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0        0        0     7010 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/pandas_query_engine.py
--rw-r--r--   0        0        0     7785 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0        0        0     5300 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/retry_query_engine.py
--rw-r--r--   0        0        0     3409 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/retry_source_query_engine.py
--rw-r--r--   0        0        0    14634 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0        0        0    13967 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/sql_join_query_engine.py
--rw-r--r--   0        0        0     7105 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/sql_vector_query_engine.py
--rw-r--r--   0        0        0    10787 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/sub_question_query_engine.py
--rw-r--r--   0        0        0     3374 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/query_engine/transform_query_engine.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/question_gen/__init__.py
--rw-r--r--   0        0        0     2324 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/question_gen/guidance_generator.py
--rw-r--r--   0        0        0     3391 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/question_gen/llm_generators.py
--rw-r--r--   0        0        0     3492 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/question_gen/openai_generator.py
--rw-r--r--   0        0        0      731 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/question_gen/output_parser.py
--rw-r--r--   0        0        0     1948 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/question_gen/prompts.py
--rw-r--r--   0        0        0      989 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/question_gen/types.py
--rw-r--r--   0        0        0     3568 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/__init__.py
--rw-r--r--   0        0        0     2078 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/awadb.py
--rw-r--r--   0        0        0     5595 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/bagel.py
--rw-r--r--   0        0        0     2431 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/base.py
--rw-r--r--   0        0        0      145 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0        0        0     2098 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0        0        0     3834 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/chroma.py
--rw-r--r--   0        0        0     2777 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/dashvector.py
--rw-r--r--   0        0        0     3292 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/database.py
--rw-r--r--   0        0        0     3438 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/deeplake.py
--rw-r--r--   0        0        0     5382 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/discord_reader.py
--rw-r--r--   0        0        0     1871 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/download.py
--rw-r--r--   0        0        0     2718 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/elasticsearch.py
--rw-r--r--   0        0        0     2492 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/faiss.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/__init__.py
--rw-r--r--   0        0        0    11447 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/base.py
--rw-r--r--   0        0        0     5052 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/docs_reader.py
--rw-r--r--   0        0        0     1263 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/epub_reader.py
--rw-r--r--   0        0        0      895 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/flat_reader.py
--rw-r--r--   0        0        0     2150 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/html_reader.py
--rw-r--r--   0        0        0     3010 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/image_caption_reader.py
--rw-r--r--   0        0        0     3866 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/image_reader.py
--rw-r--r--   0        0        0     3011 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/image_vision_llm_reader.py
--rw-r--r--   0        0        0     1272 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/ipynb_reader.py
--rw-r--r--   0        0        0     3647 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/markdown_reader.py
--rw-r--r--   0        0        0     3490 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/mbox_reader.py
--rw-r--r--   0        0        0     3563 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/slides_reader.py
--rw-r--r--   0        0        0     3549 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/tabular_reader.py
--rw-r--r--   0        0        0     1830 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/file/video_audio_reader.py
--rw-r--r--   0        0        0       17 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0        0        0    11727 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0        0        0    15507 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0        0        0     5473 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/github_readers/utils.py
--rw-r--r--   0        0        0       17 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0        0        0     5759 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0        0        0     5068 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0        0        0     4655 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/json.py
--rw-r--r--   0        0        0     2188 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/loading.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/make_com/__init__.py
--rw-r--r--   0        0        0     1641 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0        0        0     1223 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/mbox.py
--rw-r--r--   0        0        0     2290 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/metal.py
--rw-r--r--   0        0        0     4535 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/milvus.py
--rw-r--r--   0        0        0     3501 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/mongo.py
--rw-r--r--   0        0        0     5461 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/myscale.py
--rw-r--r--   0        0        0     5919 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/notion.py
--rw-r--r--   0        0        0     1270 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/obsidian.py
--rw-r--r--   0        0        0     2742 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/pinecone.py
--rw-r--r--   0        0        0     2735 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/psychic.py
--rw-r--r--   0        0        0     6888 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/qdrant.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/redis/__init__.py
--rw-r--r--   0        0        0     3498 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/redis/utils.py
--rw-r--r--   0        0        0      204 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/schema/__init__.py
--rw-r--r--   0        0        0      127 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/schema/base.py
--rw-r--r--   0        0        0     8449 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/slack.py
--rw-r--r--   0        0        0       17 2023-11-27 17:22:20.077165 llama_index-0.9.8.post1/llama_index/readers/steamship/__init__.py
--rw-r--r--   0        0        0     3423 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0        0        0     1174 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/readers/string_iterable.py
--rw-r--r--   0        0        0     2226 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/readers/twitter.py
--rw-r--r--   0        0        0       17 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0        0        0     3976 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/readers/weaviate/reader.py
--rw-r--r--   0        0        0     9196 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/readers/web.py
--rw-r--r--   0        0        0     1094 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/readers/wikipedia.py
--rw-r--r--   0        0        0     1390 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/readers/youtube_transcript.py
--rw-r--r--   0        0        0       93 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response/__init__.py
--rw-r--r--   0        0        0     4879 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response/notebook_utils.py
--rw-r--r--   0        0        0     1569 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response/pprint_utils.py
--rw-r--r--   0        0        0     4728 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response/schema.py
--rw-r--r--   0        0        0      262 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response/utils.py
--rw-r--r--   0        0        0      868 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/__init__.py
--rw-r--r--   0        0        0     4359 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/accumulate.py
--rw-r--r--   0        0        0     6394 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/base.py
--rw-r--r--   0        0        0     1932 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/compact_and_accumulate.py
--rw-r--r--   0        0        0     2005 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/compact_and_refine.py
--rw-r--r--   0        0        0     4901 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/factory.py
--rw-r--r--   0        0        0     2440 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/generation.py
--rw-r--r--   0        0        0      781 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/no_text.py
--rw-r--r--   0        0        0    17581 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/refine.py
--rw-r--r--   0        0        0     3327 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/simple_summarize.py
--rw-r--r--   0        0        0     6586 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/tree_summarize.py
--rw-r--r--   0        0        0     2011 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/response_synthesizers/type.py
--rw-r--r--   0        0        0     2507 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/retrievers/__init__.py
--rw-r--r--   0        0        0     6857 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/retrievers/auto_merging_retriever.py
--rw-r--r--   0        0        0     3206 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/retrievers/bm25_retriever.py
--rw-r--r--   0        0        0     7035 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/retrievers/fusion_retriever.py
--rw-r--r--   0        0        0     7467 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/retrievers/recursive_retriever.py
--rw-r--r--   0        0        0     5519 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/retrievers/router_retriever.py
--rw-r--r--   0        0        0     1388 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0        0        0     1169 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/retrievers/you_retriever.py
--rw-r--r--   0        0        0    23063 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/schema.py
--rw-r--r--   0        0        0      539 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/selectors/__init__.py
--rw-r--r--   0        0        0     3038 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/selectors/embedding_selectors.py
--rw-r--r--   0        0        0     7812 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/selectors/llm_selectors.py
--rw-r--r--   0        0        0     2975 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/selectors/prompts.py
--rw-r--r--   0        0        0     4859 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/selectors/pydantic_selectors.py
--rw-r--r--   0        0        0     2902 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/selectors/types.py
--rw-r--r--   0        0        0     1188 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/selectors/utils.py
--rw-r--r--   0        0        0    14910 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/service_context.py
--rw-r--r--   0        0        0      124 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/__init__.py
--rw-r--r--   0        0        0      706 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/__init__.py
--rw-r--r--   0        0        0      704 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/dynamodb_docstore.py
--rw-r--r--   0        0        0     1244 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/firestore_docstore.py
--rw-r--r--   0        0        0     9176 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0        0        0     1409 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0        0        0     1456 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/redis_docstore.py
--rw-r--r--   0        0        0      762 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/registry.py
--rw-r--r--   0        0        0     3164 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0        0        0     3432 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/types.py
--rw-r--r--   0        0        0     2596 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/docstore/utils.py
--rw-r--r--   0        0        0      523 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/__init__.py
--rw-r--r--   0        0        0      773 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/dynamodb_index_store.py
--rw-r--r--   0        0        0     1184 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/firestore_indexstore.py
--rw-r--r--   0        0        0     2222 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0        0        0     1342 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0        0        0     1385 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/redis_index_store.py
--rw-r--r--   0        0        0     2340 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0        0        0      954 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/types.py
--rw-r--r--   0        0        0      668 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/index_store/utils.py
--rw-r--r--   0        0        0      365 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0        0        0     6056 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/kvstore/dynamodb_kvstore.py
--rw-r--r--   0        0        0     3999 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/kvstore/firestore_kvstore.py
--rw-r--r--   0        0        0     4061 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0        0        0     3641 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/kvstore/redis_kvstore.py
--rw-r--r--   0        0        0     3868 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/kvstore/s3_kvstore.py
--rw-r--r--   0        0        0     2728 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0        0        0     1050 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/kvstore/types.py
--rw-r--r--   0        0        0     8116 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/storage/storage_context.py
--rw-r--r--   0        0        0      341 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/text_splitter/__init__.py
--rw-r--r--   0        0        0       17 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/token_counter/__init__.py
--rw-r--r--   0        0        0     1071 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0        0        0      908 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/token_counter/utils.py
--rw-r--r--   0        0        0      652 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/tools/__init__.py
--rw-r--r--   0        0        0     1195 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/tools/download.py
--rw-r--r--   0        0        0     3970 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/tools/function_tool.py
--rw-r--r--   0        0        0     5834 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/tools/ondemand_loader_tool.py
--rw-r--r--   0        0        0     3753 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/tools/query_engine.py
--rw-r--r--   0        0        0     7654 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/tools/query_plan.py
--rw-r--r--   0        0        0     3565 2023-11-27 17:22:20.081165 llama_index-0.9.8.post1/llama_index/tools/retriever_tool.py
--rw-r--r--   0        0        0       19 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/__init__.py
--rw-r--r--   0        0        0     4019 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/base.py
--rw-r--r--   0        0        0     1120 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/load_and_search/README.md
--rw-r--r--   0        0        0      120 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/load_and_search/__init__.py
--rw-r--r--   0        0        0     4939 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/load_and_search/base.py
--rw-r--r--   0        0        0       24 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/notion/__init__.py
--rw-r--r--   0        0        0     3179 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/notion/base.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/slack/__init__.py
--rw-r--r--   0        0        0     2280 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/tool_spec/slack/base.py
--rw-r--r--   0        0        0     5198 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/types.py
--rw-r--r--   0        0        0     1920 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tools/utils.py
--rw-r--r--   0        0        0      154 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tts/__init__.py
--rw-r--r--   0        0        0     2549 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tts/bark.py
--rw-r--r--   0        0        0      631 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tts/base.py
--rw-r--r--   0        0        0     1265 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/tts/elevenlabs.py
--rw-r--r--   0        0        0     2191 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/types.py
--rw-r--r--   0        0        0        0 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/utilities/__init__.py
--rw-r--r--   0        0        0     8383 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/utilities/sql_wrapper.py
--rw-r--r--   0        0        0     2664 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/utilities/token_counting.py
--rw-r--r--   0        0        0    14038 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/utils.py
--rw-r--r--   0        0        0     3646 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/__init__.py
--rw-r--r--   0        0        0     6219 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/astra.py
--rw-r--r--   0        0        0     6026 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/awadb.py
--rw-r--r--   0        0        0     8866 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/azurecosmosmongo.py
--rw-r--r--   0        0        0     5307 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/bagel.py
--rw-r--r--   0        0        0    11943 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/cassandra.py
--rw-r--r--   0        0        0     5660 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0        0        0     9020 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/chroma.py
--rw-r--r--   0        0        0    22520 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/cogsearch.py
--rw-r--r--   0        0        0     5075 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/dashvector.py
--rw-r--r--   0        0        0     7508 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/deeplake.py
--rw-r--r--   0        0        0      242 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/docarray/__init__.py
--rw-r--r--   0        0        0     6657 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/docarray/base.py
--rw-r--r--   0        0        0     4337 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/docarray/hnsw.py
--rw-r--r--   0        0        0     2836 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/docarray/in_memory.py
--rw-r--r--   0        0        0     5174 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/dynamodb.py
--rw-r--r--   0        0        0    20144 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/elasticsearch.py
--rw-r--r--   0        0        0     9514 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/epsilla.py
--rw-r--r--   0        0        0     5626 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/faiss.py
--rw-r--r--   0        0        0     5781 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/lancedb.py
--rw-r--r--   0        0        0    21536 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/lantern.py
--rw-r--r--   0        0        0     2219 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/loading.py
--rw-r--r--   0        0        0     4709 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/metal.py
--rw-r--r--   0        0        0    10614 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/milvus.py
--rw-r--r--   0        0        0     7595 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/mongodb.py
--rw-r--r--   0        0        0    11105 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/myscale.py
--rw-r--r--   0        0        0    10424 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/neo4jvector.py
--rw-r--r--   0        0        0    12863 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/opensearch.py
--rw-r--r--   0        0        0     2616 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/pgvecto_rs.py
--rw-r--r--   0        0        0    12106 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/pinecone.py
--rw-r--r--   0        0        0    20408 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/postgres.py
--rw-r--r--   0        0        0    15858 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/qdrant.py
--rw-r--r--   0        0        0    16796 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/redis.py
--rw-r--r--   0        0        0     2935 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/registry.py
--rw-r--r--   0        0        0    11665 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/rocksetdb.py
--rw-r--r--   0        0        0    11186 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/simple.py
--rw-r--r--   0        0        0     9185 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/singlestoredb.py
--rw-r--r--   0        0        0     5494 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/supabase.py
--rw-r--r--   0        0        0     8855 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/tair.py
--rw-r--r--   0        0        0    19420 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/tencentvectordb.py
--rw-r--r--   0        0        0     9069 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/timescalevector.py
--rw-r--r--   0        0        0     7251 2023-11-27 17:22:20.085165 llama_index-0.9.8.post1/llama_index/vector_stores/types.py
--rw-r--r--   0        0        0     8798 2023-11-27 17:22:20.089165 llama_index-0.9.8.post1/llama_index/vector_stores/typesense.py
--rw-r--r--   0        0        0     4170 2023-11-27 17:22:20.089165 llama_index-0.9.8.post1/llama_index/vector_stores/utils.py
--rw-r--r--   0        0        0     9719 2023-11-27 17:22:20.089165 llama_index-0.9.8.post1/llama_index/vector_stores/weaviate.py
--rw-r--r--   0        0        0     4877 2023-11-27 17:22:20.089165 llama_index-0.9.8.post1/llama_index/vector_stores/weaviate_utils.py
--rw-r--r--   0        0        0    11586 2023-11-27 17:22:20.089165 llama_index-0.9.8.post1/llama_index/vector_stores/zep.py
--rw-r--r--   0        0        0     5894 2023-11-27 17:22:20.089165 llama_index-0.9.8.post1/pyproject.toml
--rw-r--r--   0        0        0     8193 1970-01-01 00:00:00.000000 llama_index-0.9.8.post1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-11-29 21:20:25.487404 llama_index-0.9.9/LICENSE
+-rw-r--r--   0        0        0     5541 2023-11-29 21:20:25.487404 llama_index-0.9.9/README.md
+-rw-r--r--   0        0        0        6 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/VERSION
+-rw-r--r--   0        0        0     4859 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/__init__.py
+-rw-r--r--   0        0        0      620 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/__init__.py
+-rw-r--r--   0        0        0     7343 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/context_retriever_agent.py
+-rw-r--r--   0        0        0    22887 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/openai_agent.py
+-rw-r--r--   0        0        0    13320 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/openai_assistant_agent.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/react/__init__.py
+-rw-r--r--   0        0        0    19759 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/react/base.py
+-rw-r--r--   0        0        0     2841 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/react/formatter.py
+-rw-r--r--   0        0        0     3174 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/react/output_parser.py
+-rw-r--r--   0        0        0     1728 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/react/prompts.py
+-rw-r--r--   0        0        0     1796 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/react/types.py
+-rw-r--r--   0        0        0      833 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/retriever_openai_agent.py
+-rw-r--r--   0        0        0     2062 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/agent/types.py
+-rw-r--r--   0        0        0     2926 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/async_utils.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/bridge/__init__.py
+-rw-r--r--   0        0        0     2769 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/bridge/langchain.py
+-rw-r--r--   0        0        0     1132 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/bridge/pydantic.py
+-rw-r--r--   0        0        0      756 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/__init__.py
+-rw-r--r--   0        0        0     6808 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/aim.py
+-rw-r--r--   0        0        0      596 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/arize_phoenix_callback.py
+-rw-r--r--   0        0        0    10124 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/base.py
+-rw-r--r--   0        0        0     1659 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/base_handler.py
+-rw-r--r--   0        0        0     7532 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/finetuning_handler.py
+-rw-r--r--   0        0        0     1430 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/global_handlers.py
+-rw-r--r--   0        0        0      406 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/honeyhive_callback.py
+-rw-r--r--   0        0        0     7856 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0        0        0     7933 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/open_inference_callback.py
+-rw-r--r--   0        0        0     3572 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/schema.py
+-rw-r--r--   0        0        0     2146 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/simple_llm_handler.py
+-rw-r--r--   0        0        0     7421 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/token_counting.py
+-rw-r--r--   0        0        0     2006 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/utils.py
+-rw-r--r--   0        0        0    21044 2023-11-29 21:20:25.979409 llama_index-0.9.9/llama_index/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0      426 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/chat_engine/__init__.py
+-rw-r--r--   0        0        0    14114 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/chat_engine/condense_plus_context.py
+-rw-r--r--   0        0        0    13834 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/chat_engine/condense_question.py
+-rw-r--r--   0        0        0    11289 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/chat_engine/context.py
+-rw-r--r--   0        0        0     6154 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/chat_engine/simple.py
+-rw-r--r--   0        0        0    10305 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/chat_engine/types.py
+-rw-r--r--   0        0        0      460 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/chat_engine/utils.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/command_line/__init__.py
+-rw-r--r--   0        0        0     3588 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/command_line/command_line.py
+-rw-r--r--   0        0        0      232 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/composability/__init__.py
+-rw-r--r--   0        0        0      165 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/composability/base.py
+-rw-r--r--   0        0        0     3411 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0        0        0      672 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/constants.py
+-rw-r--r--   0        0        0      373 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/core/__init__.py
+-rw-r--r--   0        0        0     1773 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/core/base_multi_modal_retriever.py
+-rw-r--r--   0        0        0     2474 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/core/base_query_engine.py
+-rw-r--r--   0        0        0     3826 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/core/base_retriever.py
+-rw-r--r--   0        0        0     3211 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/core/image_retriever.py
+-rw-r--r--   0        0        0      327 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/data_structs/__init__.py
+-rw-r--r--   0        0        0     8100 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/data_structs/data_structs.py
+-rw-r--r--   0        0        0     2284 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/data_structs/document_summary.py
+-rw-r--r--   0        0        0     1006 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/data_structs/registry.py
+-rw-r--r--   0        0        0     4240 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/data_structs/struct_type.py
+-rw-r--r--   0        0        0     1025 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/data_structs/table.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/download/__init__.py
+-rw-r--r--   0        0        0    11994 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/download/download_utils.py
+-rw-r--r--   0        0        0     2589 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/__init__.py
+-rw-r--r--   0        0        0     4200 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/adapter.py
+-rw-r--r--   0        0        0     5487 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/adapter_utils.py
+-rw-r--r--   0        0        0     3469 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/azure_openai.py
+-rw-r--r--   0        0        0    12407 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/base.py
+-rw-r--r--   0        0        0     6580 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/bedrock.py
+-rw-r--r--   0        0        0     5132 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/clarifai.py
+-rw-r--r--   0        0        0     4763 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/clip.py
+-rw-r--r--   0        0        0     6222 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/cohereai.py
+-rw-r--r--   0        0        0     6197 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0     3546 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/fastembed.py
+-rw-r--r--   0        0        0     2075 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/google.py
+-rw-r--r--   0        0        0     2655 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/google_palm.py
+-rw-r--r--   0        0        0     4782 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/gradient.py
+-rw-r--r--   0        0        0    11330 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/huggingface.py
+-rw-r--r--   0        0        0     6518 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/huggingface_optimum.py
+-rw-r--r--   0        0        0     2488 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/huggingface_utils.py
+-rw-r--r--   0        0        0     3603 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/instructor.py
+-rw-r--r--   0        0        0     3990 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/jinaai.py
+-rw-r--r--   0        0        0     3142 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/langchain.py
+-rw-r--r--   0        0        0     3739 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/llm_rails.py
+-rw-r--r--   0        0        0     1845 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/loading.py
+-rw-r--r--   0        0        0     6812 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/multi_modal_base.py
+-rw-r--r--   0        0        0    11864 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/openai.py
+-rw-r--r--   0        0        0     1266 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/pooling.py
+-rw-r--r--   0        0        0     4493 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/text_embeddings_inference.py
+-rw-r--r--   0        0        0     3527 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/utils.py
+-rw-r--r--   0        0        0     3171 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/embeddings/voyageai.py
+-rw-r--r--   0        0        0     2298 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/__init__.py
+-rw-r--r--   0        0        0     3808 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/base.py
+-rw-r--r--   0        0        0    11199 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/batch_runner.py
+-rw-r--r--   0        0        0      188 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3686 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/benchmarks/beir.py
+-rw-r--r--   0        0        0     7507 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/benchmarks/hotpotqa.py
+-rw-r--r--   0        0        0     4677 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/correctness.py
+-rw-r--r--   0        0        0    12035 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0        0        0     1644 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/eval_utils.py
+-rw-r--r--   0        0        0     5936 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/faithfulness.py
+-rw-r--r--   0        0        0     4165 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/guideline.py
+-rw-r--r--   0        0        0      305 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/multi_modal/__init__.py
+-rw-r--r--   0        0        0     8115 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/multi_modal/faithfulness.py
+-rw-r--r--   0        0        0     7181 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/multi_modal/relevancy.py
+-rw-r--r--   0        0        0     2096 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/notebook_utils.py
+-rw-r--r--   0        0        0     8845 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/pairwise.py
+-rw-r--r--   0        0        0     4987 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/relevancy.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/retrieval/__init__.py
+-rw-r--r--   0        0        0     5562 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/retrieval/base.py
+-rw-r--r--   0        0        0     2780 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/retrieval/evaluator.py
+-rw-r--r--   0        0        0     1963 2023-11-29 21:20:25.983410 llama_index-0.9.9/llama_index/evaluation/retrieval/metrics.py
+-rw-r--r--   0        0        0     1378 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/evaluation/retrieval/metrics_base.py
+-rw-r--r--   0        0        0     2891 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/evaluation/semantic_similarity.py
+-rw-r--r--   0        0        0     2528 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/exec_utils.py
+-rw-r--r--   0        0        0      585 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/extractors/__init__.py
+-rw-r--r--   0        0        0     5253 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/extractors/interface.py
+-rw-r--r--   0        0        0     1086 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/extractors/loading.py
+-rw-r--r--   0        0        0     2991 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/extractors/marvin_metadata_extractor.py
+-rw-r--r--   0        0        0    22122 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/extractors/metadata_extractors.py
+-rw-r--r--   0        0        0     1003 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/__init__.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/cross_encoders/__init__.py
+-rw-r--r--   0        0        0     4792 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/cross_encoders/cross_encoder.py
+-rw-r--r--   0        0        0     9446 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/cross_encoders/dataset_gen.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/embeddings/__init__.py
+-rw-r--r--   0        0        0     6361 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/embeddings/adapter.py
+-rw-r--r--   0        0        0     5010 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/embeddings/adapter_utils.py
+-rw-r--r--   0        0        0     3113 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/embeddings/common.py
+-rw-r--r--   0        0        0     3022 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/gradient/__init__.py
+-rw-r--r--   0        0        0     4946 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/gradient/base.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/openai/__init__.py
+-rw-r--r--   0        0        0     3836 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/openai/base.py
+-rw-r--r--   0        0        0     6562 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/openai/validate_json.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/rerankers/__init__.py
+-rw-r--r--   0        0        0     2720 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/rerankers/cohere_reranker.py
+-rw-r--r--   0        0        0     4690 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/rerankers/dataset_gen.py
+-rw-r--r--   0        0        0     1548 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/finetuning/types.py
+-rw-r--r--   0        0        0      463 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/graph_stores/__init__.py
+-rw-r--r--   0        0        0     6075 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/graph_stores/falkordb.py
+-rw-r--r--   0        0        0     8829 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/graph_stores/kuzu.py
+-rw-r--r--   0        0        0    25956 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/graph_stores/nebulagraph.py
+-rw-r--r--   0        0        0     9481 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/graph_stores/neo4j.py
+-rw-r--r--   0        0        0     1041 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/graph_stores/registry.py
+-rw-r--r--   0        0        0     6102 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/graph_stores/simple.py
+-rw-r--r--   0        0        0     2096 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/graph_stores/types.py
+-rw-r--r--   0        0        0      522 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/img_utils.py
+-rw-r--r--   0        0        0     2346 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/__init__.py
+-rw-r--r--   0        0        0    16424 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/base.py
+-rw-r--r--   0        0        0      109 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/base_retriever.py
+-rw-r--r--   0        0        0       17 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/common/__init__.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0        0        0     8572 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0        0        0      776 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0        0        0     2653 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/common/struct_store/sql.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0        0        0     8776 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/common_tree/base.py
+-rw-r--r--   0        0        0      180 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/composability/__init__.py
+-rw-r--r--   0        0        0     4869 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/composability/graph.py
+-rw-r--r--   0        0        0      536 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0        0        0     8938 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/document_summary/base.py
+-rw-r--r--   0        0        0     6720 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/document_summary/retrievers.py
+-rw-r--r--   0        0        0      224 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/empty/__init__.py
+-rw-r--r--   0        0        0     2841 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/empty/base.py
+-rw-r--r--   0        0        0     1240 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/empty/retrievers.py
+-rw-r--r--   0        0        0     2374 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/keyword_table/README.md
+-rw-r--r--   0        0        0      860 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0        0        0     8716 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0        0        0     1068 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0        0        0     5836 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0        0        0     1268 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0        0        0     2264 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/keyword_table/utils.py
+-rw-r--r--   0        0        0      403 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0    12094 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0        0        0    33724 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/knowledge_graph/retrievers.py
+-rw-r--r--   0        0        0     1017 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/list/README.md
+-rw-r--r--   0        0        0      618 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/list/__init__.py
+-rw-r--r--   0        0        0     4542 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/list/base.py
+-rw-r--r--   0        0        0     7397 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/list/retrievers.py
+-rw-r--r--   0        0        0     3582 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/loading.py
+-rw-r--r--   0        0        0      271 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/managed/__init__.py
+-rw-r--r--   0        0        0     3417 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/managed/base.py
+-rw-r--r--   0        0        0      172 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/managed/types.py
+-rw-r--r--   0        0        0      189 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/managed/vectara/__init__.py
+-rw-r--r--   0        0        0    11749 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/managed/vectara/base.py
+-rw-r--r--   0        0        0     5336 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/managed/vectara/query.py
+-rw-r--r--   0        0        0     8046 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/managed/vectara/retriever.py
+-rw-r--r--   0        0        0     4962 2023-11-29 21:20:25.987409 llama_index-0.9.9/llama_index/indices/managed.tar.gz
+-rw-r--r--   0        0        0      291 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/multi_modal/__init__.py
+-rw-r--r--   0        0        0    13661 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/multi_modal/base.py
+-rw-r--r--   0        0        0    13967 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/multi_modal/retriever.py
+-rw-r--r--   0        0        0     1052 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/postprocessor.py
+-rw-r--r--   0        0        0    10446 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/prompt_helper.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/query/__init__.py
+-rw-r--r--   0        0        0      113 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/query/base.py
+-rw-r--r--   0        0        0     6094 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/query/embedding_utils.py
+-rw-r--r--   0        0        0      281 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0        0        0    10659 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0        0        0     4568 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/query/query_transform/feedback_transform.py
+-rw-r--r--   0        0        0     5190 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0        0        0      124 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/query/schema.py
+-rw-r--r--   0        0        0     1382 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/registry.py
+-rw-r--r--   0        0        0      122 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/service_context.py
+-rw-r--r--   0        0        0      955 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0        0        0     2376 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/struct_store/base.py
+-rw-r--r--   0        0        0     5722 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0        0        0     7707 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/struct_store/json_query.py
+-rw-r--r--   0        0        0     2385 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0        0        0     6115 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0        0        0    18002 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/struct_store/sql_query.py
+-rw-r--r--   0        0        0    14146 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/struct_store/sql_retriever.py
+-rw-r--r--   0        0        0     2640 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/README.md
+-rw-r--r--   0        0        0      657 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/__init__.py
+-rw-r--r--   0        0        0     1704 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0        0        0     6738 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/base.py
+-rw-r--r--   0        0        0     7936 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/inserter.py
+-rw-r--r--   0        0        0     4675 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0        0        0    15387 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0        0        0     1546 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0        0        0      780 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/tree/utils.py
+-rw-r--r--   0        0        0     8279 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/utils.py
+-rw-r--r--   0        0        0      386 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0        0        0    12347 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/vector_store/base.py
+-rw-r--r--   0        0        0      290 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/vector_store/retrievers/__init__.py
+-rw-r--r--   0        0        0      167 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0        0        0     5286 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0        0        0      645 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0        0        0     2701 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0        0        0     7230 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/indices/vector_store/retrievers/retriever.py
+-rw-r--r--   0        0        0      293 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/ingestion/__init__.py
+-rw-r--r--   0        0        0     2824 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/ingestion/cache.py
+-rw-r--r--   0        0        0     7915 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/ingestion/pipeline.py
+-rw-r--r--   0        0        0      237 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/langchain_helpers/__init__.py
+-rw-r--r--   0        0        0      514 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0        0        0     2923 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0        0        0      807 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0        0        0     2469 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0        0        0     7623 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0        0        0     1347 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0        0        0       65 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/langchain_helpers/text_splitter.py
+-rw-r--r--   0        0        0      752 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llama_dataset/__init__.py
+-rw-r--r--   0        0        0     6492 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llama_dataset/base.py
+-rw-r--r--   0        0        0     1621 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llama_dataset/download.py
+-rw-r--r--   0        0        0     9791 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llama_dataset/generator.py
+-rw-r--r--   0        0        0     4561 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llama_dataset/rag.py
+-rw-r--r--   0        0        0      198 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llama_pack/__init__.py
+-rw-r--r--   0        0        0      293 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llama_pack/base.py
+-rw-r--r--   0        0        0     1173 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llama_pack/download.py
+-rw-r--r--   0        0        0      390 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0        0        0    10984 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/base.py
+-rw-r--r--   0        0        0     1088 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/loading.py
+-rw-r--r--   0        0        0     5663 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/mock.py
+-rw-r--r--   0        0        0     2706 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/structured.py
+-rw-r--r--   0        0        0     1478 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/utils.py
+-rw-r--r--   0        0        0      386 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/vellum/__init__.py
+-rw-r--r--   0        0        0      151 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/vellum/exceptions.py
+-rw-r--r--   0        0        0     7299 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/vellum/predictor.py
+-rw-r--r--   0        0        0     9841 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/vellum/prompt_registry.py
+-rw-r--r--   0        0        0     1035 2023-11-29 21:20:25.991409 llama_index-0.9.9/llama_index/llm_predictor/vellum/types.py
+-rw-r--r--   0        0        0      238 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llm_predictor/vellum/utils.py
+-rw-r--r--   0        0        0     2581 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/__init__.py
+-rw-r--r--   0        0        0     4009 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/ai21.py
+-rw-r--r--   0        0        0      567 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/ai21_utils.py
+-rw-r--r--   0        0        0     7864 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/anthropic.py
+-rw-r--r--   0        0        0     1758 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/anthropic_utils.py
+-rw-r--r--   0        0        0     2009 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/anyscale.py
+-rw-r--r--   0        0        0     2312 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/anyscale_utils.py
+-rw-r--r--   0        0        0     5867 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/azure_openai.py
+-rw-r--r--   0        0        0    15458 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/base.py
+-rw-r--r--   0        0        0     8647 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/bedrock.py
+-rw-r--r--   0        0        0     7082 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/bedrock_utils.py
+-rw-r--r--   0        0        0     5645 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/clarifai.py
+-rw-r--r--   0        0        0    10611 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/cohere.py
+-rw-r--r--   0        0        0     3166 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/cohere_utils.py
+-rw-r--r--   0        0        0     2250 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/custom.py
+-rw-r--r--   0        0        0     1854 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/everlyai.py
+-rw-r--r--   0        0        0     1082 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/everlyai_utils.py
+-rw-r--r--   0        0        0     9582 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/generic_utils.py
+-rw-r--r--   0        0        0     4897 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/gradient.py
+-rw-r--r--   0        0        0    22189 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/huggingface.py
+-rw-r--r--   0        0        0    20175 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/konko.py
+-rw-r--r--   0        0        0     7085 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/konko_utils.py
+-rw-r--r--   0        0        0     5158 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/langchain.py
+-rw-r--r--   0        0        0     5617 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/langchain_utils.py
+-rw-r--r--   0        0        0    16128 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/litellm.py
+-rw-r--r--   0        0        0     6616 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/litellm_utils.py
+-rw-r--r--   0        0        0     3765 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/llama_api.py
+-rw-r--r--   0        0        0     9653 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/llama_cpp.py
+-rw-r--r--   0        0        0     2237 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/llama_utils.py
+-rw-r--r--   0        0        0     1749 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/loading.py
+-rw-r--r--   0        0        0     3313 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/localai.py
+-rw-r--r--   0        0        0     1856 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/mock.py
+-rw-r--r--   0        0        0     5273 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/monsterapi.py
+-rw-r--r--   0        0        0     5911 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/ollama.py
+-rw-r--r--   0        0        0    21336 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/openai.py
+-rw-r--r--   0        0        0     2628 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/openai_like.py
+-rw-r--r--   0        0        0    11781 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/openai_utils.py
+-rw-r--r--   0        0        0    17159 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/openllm.py
+-rw-r--r--   0        0        0     3829 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/palm.py
+-rw-r--r--   0        0        0    13900 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/perplexity.py
+-rw-r--r--   0        0        0    10116 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/portkey.py
+-rw-r--r--   0        0        0     4724 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/portkey_utils.py
+-rw-r--r--   0        0        0     3453 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/predibase.py
+-rw-r--r--   0        0        0     5664 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/replicate.py
+-rw-r--r--   0        0        0    10586 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/rungpt.py
+-rw-r--r--   0        0        0     2223 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/utils.py
+-rw-r--r--   0        0        0    10657 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/vertex.py
+-rw-r--r--   0        0        0     6074 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/vertex_utils.py
+-rw-r--r--   0        0        0     6806 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/watsonx.py
+-rw-r--r--   0        0        0     1255 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/watsonx_utils.py
+-rw-r--r--   0        0        0     8285 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/xinference.py
+-rw-r--r--   0        0        0     1020 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/llms/xinference_utils.py
+-rw-r--r--   0        0        0       95 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/logger/__init__.py
+-rw-r--r--   0        0        0      995 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/logger/base.py
+-rw-r--r--   0        0        0      161 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/memory/__init__.py
+-rw-r--r--   0        0        0     4733 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/memory/chat_memory_buffer.py
+-rw-r--r--   0        0        0     1078 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/memory/types.py
+-rw-r--r--   0        0        0      360 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/multi_modal_llms/__init__.py
+-rw-r--r--   0        0        0     3939 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/multi_modal_llms/base.py
+-rw-r--r--   0        0        0      618 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/multi_modal_llms/generic_utils.py
+-rw-r--r--   0        0        0    16815 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/multi_modal_llms/openai.py
+-rw-r--r--   0        0        0     2419 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/multi_modal_llms/openai_utils.py
+-rw-r--r--   0        0        0    10407 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/multi_modal_llms/replicate_multi_modal.py
+-rw-r--r--   0        0        0     1556 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/node_parser/__init__.py
+-rw-r--r--   0        0        0      378 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/node_parser/file/__init__.py
+-rw-r--r--   0        0        0     4115 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/node_parser/file/html.py
+-rw-r--r--   0        0        0     3415 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/node_parser/file/json.py
+-rw-r--r--   0        0        0     3927 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/node_parser/file/markdown.py
+-rw-r--r--   0        0        0     2741 2023-11-29 21:20:25.995410 llama_index-0.9.9/llama_index/node_parser/file/simple_file.py
+-rw-r--r--   0        0        0     6006 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/interface.py
+-rw-r--r--   0        0        0     1694 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/loading.py
+-rw-r--r--   0        0        0     2823 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/node_utils.py
+-rw-r--r--   0        0        0      272 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/relational/__init__.py
+-rw-r--r--   0        0        0     7618 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/relational/hierarchical.py
+-rw-r--r--   0        0        0    10269 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/relational/unstructured_element.py
+-rw-r--r--   0        0        0      487 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/text/__init__.py
+-rw-r--r--   0        0        0     4225 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/text/code.py
+-rw-r--r--   0        0        0     1489 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/text/langchain.py
+-rw-r--r--   0        0        0    11636 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/text/sentence.py
+-rw-r--r--   0        0        0     4811 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/text/sentence_window.py
+-rw-r--r--   0        0        0     8222 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/text/token.py
+-rw-r--r--   0        0        0     3126 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/node_parser/text/utils.py
+-rw-r--r--   0        0        0      567 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/objects/__init__.py
+-rw-r--r--   0        0        0     4254 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/objects/base.py
+-rw-r--r--   0        0        0     5389 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/objects/base_node_mapping.py
+-rw-r--r--   0        0        0     3025 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/objects/table_node_mapping.py
+-rw-r--r--   0        0        0     4858 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/objects/tool_node_mapping.py
+-rw-r--r--   0        0        0      438 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/output_parsers/__init__.py
+-rw-r--r--   0        0        0      284 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/output_parsers/base.py
+-rw-r--r--   0        0        0     2886 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0        0        0     1864 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/output_parsers/langchain.py
+-rw-r--r--   0        0        0     1670 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/output_parsers/pydantic.py
+-rw-r--r--   0        0        0     3315 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/output_parsers/selection.py
+-rw-r--r--   0        0        0     2189 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/output_parsers/utils.py
+-rw-r--r--   0        0        0      209 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/param_tuner/__init__.py
+-rw-r--r--   0        0        0     9088 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/param_tuner/base.py
+-rw-r--r--   0        0        0      202 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/playground/__init__.py
+-rw-r--r--   0        0        0     7036 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/playground/base.py
+-rw-r--r--   0        0        0     1454 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/__init__.py
+-rw-r--r--   0        0        0     2513 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/cohere_rerank.py
+-rw-r--r--   0        0        0     4101 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/llm_rerank.py
+-rw-r--r--   0        0        0     3994 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/longllmlingua.py
+-rw-r--r--   0        0        0     1052 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/metadata_replacement.py
+-rw-r--r--   0        0        0    13663 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/node.py
+-rw-r--r--   0        0        0     7786 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/node_recency.py
+-rw-r--r--   0        0        0     6267 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/optimizer.py
+-rw-r--r--   0        0        0     5442 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/pii.py
+-rw-r--r--   0        0        0     2469 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/sbert_rerank.py
+-rw-r--r--   0        0        0     1829 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/postprocessor/types.py
+-rw-r--r--   0        0        0      858 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/__init__.py
+-rw-r--r--   0        0        0     2752 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/guidance_program.py
+-rw-r--r--   0        0        0     3335 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/llm_program.py
+-rw-r--r--   0        0        0      968 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/llm_prompt_program.py
+-rw-r--r--   0        0        0     3607 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/lmformatenforcer_program.py
+-rw-r--r--   0        0        0     3429 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/multi_modal_llm_program.py
+-rw-r--r--   0        0        0     8690 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/openai_program.py
+-rw-r--r--   0        0        0      321 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/predefined/__init__.py
+-rw-r--r--   0        0        0     7620 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/predefined/df.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/predefined/evaporate/__init__.py
+-rw-r--r--   0        0        0     9895 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/predefined/evaporate/base.py
+-rw-r--r--   0        0        0     9273 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/predefined/evaporate/extractor.py
+-rw-r--r--   0        0        0     4722 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/predefined/evaporate/prompts.py
+-rw-r--r--   0        0        0     3288 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/program/utils.py
+-rw-r--r--   0        0        0      494 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/__init__.py
+-rw-r--r--   0        0        0    17219 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/base.py
+-rw-r--r--   0        0        0     3604 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0        0        0     1179 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0        0        0    15151 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/default_prompts.py
+-rw-r--r--   0        0        0     5565 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/guidance_utils.py
+-rw-r--r--   0        0        0     2132 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/lmformatenforcer_utils.py
+-rw-r--r--   0        0        0     3272 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/mixin.py
+-rw-r--r--   0        0        0     1720 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/prompt_type.py
+-rw-r--r--   0        0        0     1093 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/prompt_utils.py
+-rw-r--r--   0        0        0     3910 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/prompts.py
+-rw-r--r--   0        0        0     4790 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/system.py
+-rw-r--r--   0        0        0      488 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/prompts/utils.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/py.typed
+-rw-r--r--   0        0        0     2501 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/__init__.py
+-rw-r--r--   0        0        0    12418 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/citation_query_engine.py
+-rw-r--r--   0        0        0     2021 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/cogniswitch_query_engine.py
+-rw-r--r--   0        0        0     2902 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/custom.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/flare/__init__.py
+-rw-r--r--   0        0        0     6952 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/flare/answer_inserter.py
+-rw-r--r--   0        0        0    10517 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/flare/base.py
+-rw-r--r--   0        0        0     2078 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/flare/output_parser.py
+-rw-r--r--   0        0        0      163 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/flare/schema.py
+-rw-r--r--   0        0        0     4593 2023-11-29 21:20:25.999410 llama_index-0.9.9/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0        0        0    12365 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/knowledge_graph_query_engine.py
+-rw-r--r--   0        0        0     7012 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/multi_modal.py
+-rw-r--r--   0        0        0     6675 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0        0        0     7010 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/pandas_query_engine.py
+-rw-r--r--   0        0        0     7785 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0        0        0     5300 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/retry_query_engine.py
+-rw-r--r--   0        0        0     3409 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/retry_source_query_engine.py
+-rw-r--r--   0        0        0    14634 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0        0        0    13967 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/sql_join_query_engine.py
+-rw-r--r--   0        0        0     7105 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/sql_vector_query_engine.py
+-rw-r--r--   0        0        0    10787 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/sub_question_query_engine.py
+-rw-r--r--   0        0        0     3374 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/query_engine/transform_query_engine.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/question_gen/__init__.py
+-rw-r--r--   0        0        0     2324 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/question_gen/guidance_generator.py
+-rw-r--r--   0        0        0     3391 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/question_gen/llm_generators.py
+-rw-r--r--   0        0        0     3492 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/question_gen/openai_generator.py
+-rw-r--r--   0        0        0      731 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/question_gen/output_parser.py
+-rw-r--r--   0        0        0     1948 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/question_gen/prompts.py
+-rw-r--r--   0        0        0      989 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/question_gen/types.py
+-rw-r--r--   0        0        0     3568 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/__init__.py
+-rw-r--r--   0        0        0     2078 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/awadb.py
+-rw-r--r--   0        0        0     5595 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/bagel.py
+-rw-r--r--   0        0        0     2431 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/base.py
+-rw-r--r--   0        0        0      145 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0        0        0     2098 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0        0        0     3834 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/chroma.py
+-rw-r--r--   0        0        0     2777 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/dashvector.py
+-rw-r--r--   0        0        0     3292 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/database.py
+-rw-r--r--   0        0        0     3438 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/deeplake.py
+-rw-r--r--   0        0        0     5382 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/discord_reader.py
+-rw-r--r--   0        0        0     1871 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/download.py
+-rw-r--r--   0        0        0     2718 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/elasticsearch.py
+-rw-r--r--   0        0        0     2492 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/faiss.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/__init__.py
+-rw-r--r--   0        0        0    11447 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/base.py
+-rw-r--r--   0        0        0     5052 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/docs_reader.py
+-rw-r--r--   0        0        0     1263 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/epub_reader.py
+-rw-r--r--   0        0        0      895 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/flat_reader.py
+-rw-r--r--   0        0        0     2150 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/html_reader.py
+-rw-r--r--   0        0        0     3010 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/image_caption_reader.py
+-rw-r--r--   0        0        0     3866 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/image_reader.py
+-rw-r--r--   0        0        0     3011 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/image_vision_llm_reader.py
+-rw-r--r--   0        0        0     1272 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/ipynb_reader.py
+-rw-r--r--   0        0        0     3647 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/markdown_reader.py
+-rw-r--r--   0        0        0     3490 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/mbox_reader.py
+-rw-r--r--   0        0        0     3563 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/slides_reader.py
+-rw-r--r--   0        0        0     3549 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/tabular_reader.py
+-rw-r--r--   0        0        0     1830 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/file/video_audio_reader.py
+-rw-r--r--   0        0        0       17 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0        0        0    11727 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0        0        0    15507 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0        0        0     5473 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/github_readers/utils.py
+-rw-r--r--   0        0        0       17 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0        0        0     5759 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0        0        0     5068 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0        0        0     4655 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/json.py
+-rw-r--r--   0        0        0     2188 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/loading.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0        0        0     1641 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0        0        0     1223 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/mbox.py
+-rw-r--r--   0        0        0     2290 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/metal.py
+-rw-r--r--   0        0        0     4535 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/milvus.py
+-rw-r--r--   0        0        0     3501 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/mongo.py
+-rw-r--r--   0        0        0     5461 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/myscale.py
+-rw-r--r--   0        0        0     5919 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/notion.py
+-rw-r--r--   0        0        0     1270 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/obsidian.py
+-rw-r--r--   0        0        0     2742 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/pinecone.py
+-rw-r--r--   0        0        0     2735 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/psychic.py
+-rw-r--r--   0        0        0     6888 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/qdrant.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/redis/__init__.py
+-rw-r--r--   0        0        0     3498 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/redis/utils.py
+-rw-r--r--   0        0        0      204 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/schema/__init__.py
+-rw-r--r--   0        0        0      127 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/schema/base.py
+-rw-r--r--   0        0        0     8449 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/slack.py
+-rw-r--r--   0        0        0       17 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0        0        0     3423 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0        0        0     1174 2023-11-29 21:20:26.003410 llama_index-0.9.9/llama_index/readers/string_iterable.py
+-rw-r--r--   0        0        0     2226 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/readers/twitter.py
+-rw-r--r--   0        0        0       17 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0        0        0     3976 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0        0        0     9196 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/readers/web.py
+-rw-r--r--   0        0        0     1094 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/readers/wikipedia.py
+-rw-r--r--   0        0        0     1390 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/readers/youtube_transcript.py
+-rw-r--r--   0        0        0       93 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response/__init__.py
+-rw-r--r--   0        0        0     4879 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response/notebook_utils.py
+-rw-r--r--   0        0        0     1569 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response/pprint_utils.py
+-rw-r--r--   0        0        0     4728 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response/schema.py
+-rw-r--r--   0        0        0      262 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response/utils.py
+-rw-r--r--   0        0        0      868 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/__init__.py
+-rw-r--r--   0        0        0     4359 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/accumulate.py
+-rw-r--r--   0        0        0     6394 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/base.py
+-rw-r--r--   0        0        0     1932 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/compact_and_accumulate.py
+-rw-r--r--   0        0        0     2005 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/compact_and_refine.py
+-rw-r--r--   0        0        0     4901 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/factory.py
+-rw-r--r--   0        0        0     2440 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/generation.py
+-rw-r--r--   0        0        0      781 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/no_text.py
+-rw-r--r--   0        0        0    17581 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/refine.py
+-rw-r--r--   0        0        0     3327 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/simple_summarize.py
+-rw-r--r--   0        0        0     6586 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/tree_summarize.py
+-rw-r--r--   0        0        0     2011 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/response_synthesizers/type.py
+-rw-r--r--   0        0        0     2507 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/retrievers/__init__.py
+-rw-r--r--   0        0        0     6857 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/retrievers/auto_merging_retriever.py
+-rw-r--r--   0        0        0     3206 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/retrievers/bm25_retriever.py
+-rw-r--r--   0        0        0     7035 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/retrievers/fusion_retriever.py
+-rw-r--r--   0        0        0     7467 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/retrievers/recursive_retriever.py
+-rw-r--r--   0        0        0     5519 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/retrievers/router_retriever.py
+-rw-r--r--   0        0        0     1388 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0        0        0     1169 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/retrievers/you_retriever.py
+-rw-r--r--   0        0        0    23063 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/schema.py
+-rw-r--r--   0        0        0      539 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/selectors/__init__.py
+-rw-r--r--   0        0        0     3038 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/selectors/embedding_selectors.py
+-rw-r--r--   0        0        0     7812 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0        0        0     2975 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/selectors/prompts.py
+-rw-r--r--   0        0        0     4859 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/selectors/pydantic_selectors.py
+-rw-r--r--   0        0        0     2902 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/selectors/types.py
+-rw-r--r--   0        0        0     1188 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/selectors/utils.py
+-rw-r--r--   0        0        0    14910 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/service_context.py
+-rw-r--r--   0        0        0      124 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/__init__.py
+-rw-r--r--   0        0        0      706 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0        0        0      704 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/dynamodb_docstore.py
+-rw-r--r--   0        0        0     1244 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/firestore_docstore.py
+-rw-r--r--   0        0        0     9176 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0        0        0     1409 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0        0        0     1456 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/redis_docstore.py
+-rw-r--r--   0        0        0      762 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/registry.py
+-rw-r--r--   0        0        0     3164 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0        0        0     3432 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/types.py
+-rw-r--r--   0        0        0     2596 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/docstore/utils.py
+-rw-r--r--   0        0        0      523 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0        0        0      773 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/dynamodb_index_store.py
+-rw-r--r--   0        0        0     1184 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/firestore_indexstore.py
+-rw-r--r--   0        0        0     2222 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0        0        0     1342 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0        0        0     1385 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/redis_index_store.py
+-rw-r--r--   0        0        0     2340 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0        0        0      954 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/types.py
+-rw-r--r--   0        0        0      668 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/index_store/utils.py
+-rw-r--r--   0        0        0      365 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0        0        0     6056 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/kvstore/dynamodb_kvstore.py
+-rw-r--r--   0        0        0     3999 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/kvstore/firestore_kvstore.py
+-rw-r--r--   0        0        0     4061 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0        0        0     3641 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/kvstore/redis_kvstore.py
+-rw-r--r--   0        0        0     3868 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/kvstore/s3_kvstore.py
+-rw-r--r--   0        0        0     2728 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0        0        0     1050 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/kvstore/types.py
+-rw-r--r--   0        0        0     8116 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/storage/storage_context.py
+-rw-r--r--   0        0        0      341 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/text_splitter/__init__.py
+-rw-r--r--   0        0        0       17 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/token_counter/__init__.py
+-rw-r--r--   0        0        0     1071 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0        0        0      908 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/token_counter/utils.py
+-rw-r--r--   0        0        0      652 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/__init__.py
+-rw-r--r--   0        0        0     1195 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/download.py
+-rw-r--r--   0        0        0     3970 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/function_tool.py
+-rw-r--r--   0        0        0     5834 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/ondemand_loader_tool.py
+-rw-r--r--   0        0        0     3753 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/query_engine.py
+-rw-r--r--   0        0        0     7654 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/query_plan.py
+-rw-r--r--   0        0        0     3565 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/retriever_tool.py
+-rw-r--r--   0        0        0       19 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/tool_spec/__init__.py
+-rw-r--r--   0        0        0     4019 2023-11-29 21:20:26.007410 llama_index-0.9.9/llama_index/tools/tool_spec/base.py
+-rw-r--r--   0        0        0     1120 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/tool_spec/load_and_search/README.md
+-rw-r--r--   0        0        0      120 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/tool_spec/load_and_search/__init__.py
+-rw-r--r--   0        0        0     4939 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/tool_spec/load_and_search/base.py
+-rw-r--r--   0        0        0       24 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/tool_spec/notion/__init__.py
+-rw-r--r--   0        0        0     3179 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/tool_spec/notion/base.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/tool_spec/slack/__init__.py
+-rw-r--r--   0        0        0     2280 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/tool_spec/slack/base.py
+-rw-r--r--   0        0        0     5198 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/types.py
+-rw-r--r--   0        0        0     1920 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tools/utils.py
+-rw-r--r--   0        0        0      154 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tts/__init__.py
+-rw-r--r--   0        0        0     2549 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tts/bark.py
+-rw-r--r--   0        0        0      631 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tts/base.py
+-rw-r--r--   0        0        0     1265 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/tts/elevenlabs.py
+-rw-r--r--   0        0        0     2191 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/types.py
+-rw-r--r--   0        0        0        0 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/utilities/__init__.py
+-rw-r--r--   0        0        0     8383 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/utilities/sql_wrapper.py
+-rw-r--r--   0        0        0     2664 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/utilities/token_counting.py
+-rw-r--r--   0        0        0    14038 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/utils.py
+-rw-r--r--   0        0        0     3646 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/__init__.py
+-rw-r--r--   0        0        0     9754 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/astra.py
+-rw-r--r--   0        0        0     6026 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/awadb.py
+-rw-r--r--   0        0        0     8866 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/azurecosmosmongo.py
+-rw-r--r--   0        0        0     5307 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/bagel.py
+-rw-r--r--   0        0        0    11943 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/cassandra.py
+-rw-r--r--   0        0        0     5660 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0        0        0     9269 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/chroma.py
+-rw-r--r--   0        0        0    22520 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/cogsearch.py
+-rw-r--r--   0        0        0     5075 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/dashvector.py
+-rw-r--r--   0        0        0     7508 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0        0        0      242 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/docarray/__init__.py
+-rw-r--r--   0        0        0     6657 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/docarray/base.py
+-rw-r--r--   0        0        0     4337 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/docarray/hnsw.py
+-rw-r--r--   0        0        0     2836 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/docarray/in_memory.py
+-rw-r--r--   0        0        0     5174 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/dynamodb.py
+-rw-r--r--   0        0        0    20144 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/elasticsearch.py
+-rw-r--r--   0        0        0     9514 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/epsilla.py
+-rw-r--r--   0        0        0     5626 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/faiss.py
+-rw-r--r--   0        0        0     5814 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0        0        0    21536 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/lantern.py
+-rw-r--r--   0        0        0     2219 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/loading.py
+-rw-r--r--   0        0        0     4709 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/metal.py
+-rw-r--r--   0        0        0    10614 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/milvus.py
+-rw-r--r--   0        0        0     7595 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/mongodb.py
+-rw-r--r--   0        0        0    11105 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/myscale.py
+-rw-r--r--   0        0        0    10424 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/neo4jvector.py
+-rw-r--r--   0        0        0    12863 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0        0        0     2616 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/pgvecto_rs.py
+-rw-r--r--   0        0        0    12106 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0        0        0    20408 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/postgres.py
+-rw-r--r--   0        0        0    15858 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0        0        0    16796 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/redis.py
+-rw-r--r--   0        0        0     2935 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/registry.py
+-rw-r--r--   0        0        0    11665 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/rocksetdb.py
+-rw-r--r--   0        0        0    11186 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/simple.py
+-rw-r--r--   0        0        0     9185 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/singlestoredb.py
+-rw-r--r--   0        0        0     5494 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/supabase.py
+-rw-r--r--   0        0        0     8855 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/tair.py
+-rw-r--r--   0        0        0    19420 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/tencentvectordb.py
+-rw-r--r--   0        0        0     9069 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/timescalevector.py
+-rw-r--r--   0        0        0     7251 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/types.py
+-rw-r--r--   0        0        0     8798 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/typesense.py
+-rw-r--r--   0        0        0     4170 2023-11-29 21:20:26.011410 llama_index-0.9.9/llama_index/vector_stores/utils.py
+-rw-r--r--   0        0        0     9719 2023-11-29 21:20:26.015410 llama_index-0.9.9/llama_index/vector_stores/weaviate.py
+-rw-r--r--   0        0        0     4877 2023-11-29 21:20:26.015410 llama_index-0.9.9/llama_index/vector_stores/weaviate_utils.py
+-rw-r--r--   0        0        0    11586 2023-11-29 21:20:26.015410 llama_index-0.9.9/llama_index/vector_stores/zep.py
+-rw-r--r--   0        0        0     5915 2023-11-29 21:20:26.015410 llama_index-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 llama_index-0.9.9/PKG-INFO
```

### Comparing `llama_index-0.9.8.post1/LICENSE` & `llama_index-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/README.md` & `llama_index-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/__init__.py` & `llama_index-0.9.9/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/__init__.py` & `llama_index-0.9.9/llama_index/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/context_retriever_agent.py` & `llama_index-0.9.9/llama_index/agent/context_retriever_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/openai_agent.py` & `llama_index-0.9.9/llama_index/agent/openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/openai_assistant_agent.py` & `llama_index-0.9.9/llama_index/agent/openai_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/react/base.py` & `llama_index-0.9.9/llama_index/agent/react/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/react/formatter.py` & `llama_index-0.9.9/llama_index/agent/react/formatter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/react/output_parser.py` & `llama_index-0.9.9/llama_index/agent/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/react/prompts.py` & `llama_index-0.9.9/llama_index/agent/react/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/react/types.py` & `llama_index-0.9.9/llama_index/agent/react/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/retriever_openai_agent.py` & `llama_index-0.9.9/llama_index/agent/retriever_openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/agent/types.py` & `llama_index-0.9.9/llama_index/agent/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/async_utils.py` & `llama_index-0.9.9/llama_index/async_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 """Async utils."""
 import asyncio
 from itertools import zip_longest
 from typing import Any, Coroutine, Iterable, List
 
 
+def asyncio_module(show_progress: bool = False) -> Any:
+    if show_progress:
+        from tqdm.asyncio import tqdm_asyncio
+
+        module = tqdm_asyncio
+    else:
+        module = asyncio
+
+    return module
+
+
 def run_async_tasks(
     tasks: List[Coroutine],
     show_progress: bool = False,
     progress_bar_desc: str = "Running async tasks",
 ) -> List[Any]:
     """Run a list of async tasks."""
     tasks_to_execute: List[Any] = tasks
```

### Comparing `llama_index-0.9.8.post1/llama_index/bridge/langchain.py` & `llama_index-0.9.9/llama_index/bridge/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/bridge/pydantic.py` & `llama_index-0.9.9/llama_index/bridge/pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/__init__.py` & `llama_index-0.9.9/llama_index/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/aim.py` & `llama_index-0.9.9/llama_index/callbacks/aim.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/arize_phoenix_callback.py` & `llama_index-0.9.9/llama_index/callbacks/arize_phoenix_callback.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/base.py` & `llama_index-0.9.9/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/base_handler.py` & `llama_index-0.9.9/llama_index/callbacks/base_handler.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/finetuning_handler.py` & `llama_index-0.9.9/llama_index/callbacks/finetuning_handler.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/global_handlers.py` & `llama_index-0.9.9/llama_index/callbacks/global_handlers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/llama_debug.py` & `llama_index-0.9.9/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/open_inference_callback.py` & `llama_index-0.9.9/llama_index/callbacks/open_inference_callback.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/schema.py` & `llama_index-0.9.9/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/simple_llm_handler.py` & `llama_index-0.9.9/llama_index/callbacks/simple_llm_handler.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/token_counting.py` & `llama_index-0.9.9/llama_index/callbacks/token_counting.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/utils.py` & `llama_index-0.9.9/llama_index/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/callbacks/wandb_callback.py` & `llama_index-0.9.9/llama_index/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/chat_engine/condense_plus_context.py` & `llama_index-0.9.9/llama_index/chat_engine/condense_plus_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/chat_engine/condense_question.py` & `llama_index-0.9.9/llama_index/chat_engine/condense_question.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/chat_engine/context.py` & `llama_index-0.9.9/llama_index/chat_engine/context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/chat_engine/simple.py` & `llama_index-0.9.9/llama_index/chat_engine/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/chat_engine/types.py` & `llama_index-0.9.9/llama_index/chat_engine/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/composability/joint_qa_summary.py` & `llama_index-0.9.9/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/constants.py` & `llama_index-0.9.9/llama_index/constants.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/core/base_multi_modal_retriever.py` & `llama_index-0.9.9/llama_index/core/base_multi_modal_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/core/base_query_engine.py` & `llama_index-0.9.9/llama_index/core/base_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/core/base_retriever.py` & `llama_index-0.9.9/llama_index/core/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/core/image_retriever.py` & `llama_index-0.9.9/llama_index/core/image_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/data_structs/data_structs.py` & `llama_index-0.9.9/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/data_structs/document_summary.py` & `llama_index-0.9.9/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/data_structs/registry.py` & `llama_index-0.9.9/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/data_structs/struct_type.py` & `llama_index-0.9.9/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/data_structs/table.py` & `llama_index-0.9.9/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/download/download_utils.py` & `llama_index-0.9.9/llama_index/download/download_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,32 @@
 
 import json
 import os
 import subprocess
 import sys
 from importlib import util
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pkg_resources
 import requests
 from pkg_resources import DistributionNotFound
 
-LLAMA_HUB_CONTENTS_URL = "https://raw.githubusercontent.com/run-llama/llama-hub/main"
+LLAMA_HUB_CONTENTS_URL = f"https://raw.githubusercontent.com/run-llama/llama-hub/main"
 LLAMA_HUB_PATH = "/llama_hub"
 LLAMA_HUB_URL = LLAMA_HUB_CONTENTS_URL + LLAMA_HUB_PATH
 
+REPO = "llama_datasets"
+BRANCH = "main"
+LLAMA_DATASETS_URL = (
+    f"https://media.githubusercontent.com/media/run-llama/{REPO}/{BRANCH}"
+)
+LLAMA_RAG_DATASET_FILENAME = "rag_dataset.json"
+
+
 PATH_TYPE = Union[str, Path]
 
 
 def _get_file_content(loader_hub_url: str, path: str) -> Tuple[str, int]:
     """Get the content of a file from the GitHub REST API."""
     resp = requests.get(loader_hub_url + path)
     return resp.text, resp.status_code
@@ -160,14 +168,15 @@
     remote_dir_path: PATH_TYPE,
     module_id: str,
     extra_files: List[str],
     refresh_cache: bool = False,
     use_gpt_index_import: bool = False,
     base_file_name: str = "base.py",
     override_path: bool = False,
+    is_dataset: bool = False,
 ) -> None:
     """Load module."""
     if isinstance(local_dir_path, str):
         local_dir_path = Path(local_dir_path)
 
     if override_path:
         module_path = str(local_dir_path)
@@ -205,51 +214,54 @@
                 with open(local_dir_path / "__init__.py", "r+") as f:
                     f.write(f"from .{module_id} import {', '.join(loader_exports)}")
                     existing_exports = get_exports(f.read())
                 rewrite_exports(existing_exports + loader_exports, str(local_dir_path))
             with open(f"{module_path}/{extra_file}", "w") as f:
                 f.write(extra_file_raw_content)
 
-    # install requirements
-    requirements_path = f"{local_dir_path}/requirements.txt"
-
-    if not os.path.exists(requirements_path):
-        # NOTE: need to check the status code
-        response_txt, status_code = _get_file_content(
-            str(remote_dir_path), f"/{module_id}/requirements.txt"
-        )
-        if status_code == 200:
-            with open(requirements_path, "w") as f:
-                f.write(response_txt)
-
-    # Install dependencies if there are any and not already installed
-    if os.path.exists(requirements_path):
-        try:
-            requirements = pkg_resources.parse_requirements(
-                Path(requirements_path).open()
-            )
-            pkg_resources.require([str(r) for r in requirements])
-        except DistributionNotFound:
-            subprocess.check_call(
-                [sys.executable, "-m", "pip", "install", "-r", requirements_path]
+    if not is_dataset:
+        # install requirements
+        requirements_path = f"{local_dir_path}/requirements.txt"
+
+        if not os.path.exists(requirements_path):
+            # NOTE: need to check the status code
+            response_txt, status_code = _get_file_content(
+                str(remote_dir_path), f"/{module_id}/requirements.txt"
             )
+            if status_code == 200:
+                with open(requirements_path, "w") as f:
+                    f.write(response_txt)
+
+        # Install dependencies if there are any and not already installed
+        if os.path.exists(requirements_path):
+            try:
+                requirements = pkg_resources.parse_requirements(
+                    Path(requirements_path).open()
+                )
+                pkg_resources.require([str(r) for r in requirements])
+            except DistributionNotFound:
+                subprocess.check_call(
+                    [sys.executable, "-m", "pip", "install", "-r", requirements_path]
+                )
 
 
 def download_llama_module(
     module_class: str,
     llama_hub_url: str = LLAMA_HUB_URL,
     refresh_cache: bool = False,
     custom_dir: Optional[str] = None,
     custom_path: Optional[str] = None,
     library_path: str = "library.json",
     base_file_name: str = "base.py",
     use_gpt_index_import: bool = False,
     disable_library_cache: bool = False,
     override_path: bool = False,
-) -> Type:
+    llama_datasets_url: str = LLAMA_DATASETS_URL,
+    is_dataset: bool = False,
+) -> Any:
     """Download a module from LlamaHub.
 
     Can be a loader, tool, pack, or more.
 
     Args:
         loader_class: The name of the llama module class you want to download,
             such as `GmailOpenAIAgentPack`.
@@ -259,17 +271,18 @@
         custom_path: Custom dirpath to download loader into.
         library_path: File name of the library file.
         use_gpt_index_import: If true, the loader files will use
             llama_index as the base dependency. By default (False),
             the loader files use llama_index as the base dependency.
             NOTE: this is a temporary workaround while we fully migrate all usages
             to llama_index.
+        is_dataset: whether or not downloading a LlamaDataset
 
     Returns:
-        A Loader.
+        A Loader, A Pack, An Agent, or A Dataset
     """
     # create directory / get path
     dirpath = initialize_directory(custom_path=custom_path, custom_dir=custom_dir)
 
     # fetch info from library.json file
     module_info = get_module_info(
         local_dir_path=dirpath,
@@ -279,38 +292,56 @@
         library_path=library_path,
         disable_library_cache=disable_library_cache,
     )
     module_id = module_info["module_id"]
     extra_files = module_info["extra_files"]
 
     # download the module, install requirements
+    if is_dataset:
+        download_remote_dir_path = llama_datasets_url
+        base_file_name = "rag_dataset.json"
+    else:
+        download_remote_dir_path = llama_hub_url
+
     download_module_and_reqs(
         local_dir_path=dirpath,
-        remote_dir_path=llama_hub_url,
+        remote_dir_path=download_remote_dir_path,
         module_id=module_id,
         extra_files=extra_files,
         refresh_cache=refresh_cache,
         use_gpt_index_import=use_gpt_index_import,
         base_file_name=base_file_name,
         override_path=override_path,
+        is_dataset=is_dataset,
     )
 
-    # loads the module into memory
-    if override_path:
-        spec = util.spec_from_file_location(
-            "custom_module", location=f"{dirpath}/{base_file_name}"
-        )
-        if spec is None:
-            raise ValueError(f"Could not find file: {dirpath}/{base_file_name}.")
+    if is_dataset:
+        # no module to install, instead just store data files in specified path
+        if override_path:
+            module_path = str(dirpath)
+        else:
+            module_path = f"{dirpath}/{module_id}"
+
+        return f"{module_path}/{LLAMA_RAG_DATASET_FILENAME}", [
+            f"{module_path}/{el}" for el in extra_files
+        ]
     else:
-        spec = util.spec_from_file_location(
-            "custom_module", location=f"{dirpath}/{module_id}/{base_file_name}"
-        )
-        if spec is None:
-            raise ValueError(
-                f"Could not find file: {dirpath}/{module_id}/{base_file_name}."
+        # loads the module into memory
+        if override_path:
+            spec = util.spec_from_file_location(
+                "custom_module", location=f"{dirpath}/{base_file_name}"
+            )
+            if spec is None:
+                raise ValueError(f"Could not find file: {dirpath}/{base_file_name}.")
+        else:
+            spec = util.spec_from_file_location(
+                "custom_module", location=f"{dirpath}/{module_id}/{base_file_name}"
             )
+            if spec is None:
+                raise ValueError(
+                    f"Could not find file: {dirpath}/{module_id}/{base_file_name}."
+                )
 
-    module = util.module_from_spec(spec)
-    spec.loader.exec_module(module)  # type: ignore
+        module = util.module_from_spec(spec)
+        spec.loader.exec_module(module)  # type: ignore
 
-    return getattr(module, module_class)
+        return getattr(module, module_class)
```

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/__init__.py` & `llama_index-0.9.9/llama_index/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/adapter.py` & `llama_index-0.9.9/llama_index/embeddings/adapter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/adapter_utils.py` & `llama_index-0.9.9/llama_index/embeddings/adapter_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/azure_openai.py` & `llama_index-0.9.9/llama_index/embeddings/azure_openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/base.py` & `llama_index-0.9.9/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/bedrock.py` & `llama_index-0.9.9/llama_index/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/clarifai.py` & `llama_index-0.9.9/llama_index/embeddings/clarifai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/clip.py` & `llama_index-0.9.9/llama_index/embeddings/clip.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/cohereai.py` & `llama_index-0.9.9/llama_index/embeddings/cohereai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/elasticsearch.py` & `llama_index-0.9.9/llama_index/embeddings/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/fastembed.py` & `llama_index-0.9.9/llama_index/embeddings/fastembed.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/google.py` & `llama_index-0.9.9/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/google_palm.py` & `llama_index-0.9.9/llama_index/embeddings/google_palm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/gradient.py` & `llama_index-0.9.9/llama_index/embeddings/gradient.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/huggingface.py` & `llama_index-0.9.9/llama_index/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/huggingface_optimum.py` & `llama_index-0.9.9/llama_index/embeddings/huggingface_optimum.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/huggingface_utils.py` & `llama_index-0.9.9/llama_index/embeddings/huggingface_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/instructor.py` & `llama_index-0.9.9/llama_index/embeddings/instructor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/jinaai.py` & `llama_index-0.9.9/llama_index/embeddings/jinaai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/langchain.py` & `llama_index-0.9.9/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/llm_rails.py` & `llama_index-0.9.9/llama_index/embeddings/llm_rails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/loading.py` & `llama_index-0.9.9/llama_index/embeddings/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/multi_modal_base.py` & `llama_index-0.9.9/llama_index/embeddings/multi_modal_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/openai.py` & `llama_index-0.9.9/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/pooling.py` & `llama_index-0.9.9/llama_index/embeddings/pooling.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/text_embeddings_inference.py` & `llama_index-0.9.9/llama_index/embeddings/text_embeddings_inference.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/utils.py` & `llama_index-0.9.9/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/embeddings/voyageai.py` & `llama_index-0.9.9/llama_index/embeddings/voyageai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/__init__.py` & `llama_index-0.9.9/llama_index/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/base.py` & `llama_index-0.9.9/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/batch_runner.py` & `llama_index-0.9.9/llama_index/evaluation/batch_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from typing import Any, Dict, List, Optional, Sequence, Tuple, cast
 
+from llama_index.async_utils import asyncio_module
 from llama_index.core import BaseQueryEngine
 from llama_index.evaluation.base import BaseEvaluator, EvaluationResult
-from llama_index.evaluation.eval_utils import asyncio_module
 from llama_index.response.schema import RESPONSE_TYPE, Response
 
 
 async def eval_response_worker(
     semaphore: asyncio.Semaphore,
     evaluator: BaseEvaluator,
     evaluator_name: str,
```

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/benchmarks/beir.py` & `llama_index-0.9.9/llama_index/evaluation/benchmarks/beir.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/benchmarks/hotpotqa.py` & `llama_index-0.9.9/llama_index/evaluation/benchmarks/hotpotqa.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/correctness.py` & `llama_index-0.9.9/llama_index/evaluation/correctness.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/dataset_generation.py` & `llama_index-0.9.9/llama_index/evaluation/dataset_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import asyncio
 import json
 import re
 import uuid
 from typing import Dict, List, Tuple
 
+from deprecated import deprecated
+
 from llama_index import Document, ServiceContext, SummaryIndex
 from llama_index.bridge.pydantic import BaseModel, Field
 from llama_index.ingestion import run_transformations
 from llama_index.llms.openai import OpenAI
 from llama_index.postprocessor.node import KeywordNodePostprocessor
 from llama_index.prompts.base import BasePromptTemplate, PromptTemplate
 from llama_index.prompts.default_prompts import DEFAULT_TEXT_QA_PROMPT
@@ -30,14 +32,18 @@
 
 def _get_default_service_context() -> ServiceContext:
     """Get default service context."""
     llm = OpenAI(temperature=0, model="gpt-3.5-turbo")
     return ServiceContext.from_defaults(llm=llm, chunk_size_limit=3000)
 
 
+@deprecated(
+    "Deprecated in favor of `LabelledRagDataset` which should be used instead.",
+    action="always",
+)
 class QueryResponseDataset(BaseModel):
     """Query Response Dataset.
 
     The response can be empty if the dataset is generated from documents.
 
     Args:
         queries (Dict[str, str]): Query id -> query.
@@ -90,14 +96,18 @@
     def from_json(cls, path: str) -> QueryResponseDataset:
         """Load json."""
         with open(path) as f:
             data = json.load(f)
         return cls(**data)
 
 
+@deprecated(
+    "Deprecated in favor of `RagDatasetGenerator` which should be used instead.",
+    action="always",
+)
 class DatasetGenerator(PromptMixin):
     """Generate dataset (question/ question-answer pairs) \
     based on the given documents.
 
     NOTE: this is a beta feature, subject to change!
 
     Args:
```

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/eval_utils.py` & `llama_index-0.9.9/llama_index/evaluation/eval_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,19 @@
 import asyncio
 from collections import defaultdict
 from typing import Any, List
 
 import numpy as np
 import pandas as pd
 
+from llama_index.async_utils import asyncio_module
 from llama_index.core import BaseQueryEngine
 from llama_index.evaluation.base import EvaluationResult
 
 
-def asyncio_module(show_progress: bool = False) -> Any:
-    if show_progress:
-        from tqdm.asyncio import tqdm_asyncio
-
-        module = tqdm_asyncio
-    else:
-        module = asyncio
-
-    return module
-
-
 async def aget_responses(
     questions: List[str], query_engine: BaseQueryEngine, show_progress: bool = False
 ) -> List[str]:
     """Get responses."""
     tasks = []
     for question in questions:
         tasks.append(query_engine.aquery(question))
```

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/faithfulness.py` & `llama_index-0.9.9/llama_index/evaluation/faithfulness.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/guideline.py` & `llama_index-0.9.9/llama_index/evaluation/guideline.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/multi_modal/faithfulness.py` & `llama_index-0.9.9/llama_index/evaluation/multi_modal/faithfulness.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/multi_modal/relevancy.py` & `llama_index-0.9.9/llama_index/evaluation/multi_modal/relevancy.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/notebook_utils.py` & `llama_index-0.9.9/llama_index/evaluation/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/pairwise.py` & `llama_index-0.9.9/llama_index/evaluation/pairwise.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/relevancy.py` & `llama_index-0.9.9/llama_index/evaluation/relevancy.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/retrieval/base.py` & `llama_index-0.9.9/llama_index/evaluation/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/retrieval/evaluator.py` & `llama_index-0.9.9/llama_index/evaluation/retrieval/evaluator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/retrieval/metrics.py` & `llama_index-0.9.9/llama_index/evaluation/retrieval/metrics.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/retrieval/metrics_base.py` & `llama_index-0.9.9/llama_index/evaluation/retrieval/metrics_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/evaluation/semantic_similarity.py` & `llama_index-0.9.9/llama_index/evaluation/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/exec_utils.py` & `llama_index-0.9.9/llama_index/exec_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/extractors/__init__.py` & `llama_index-0.9.9/llama_index/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/extractors/interface.py` & `llama_index-0.9.9/llama_index/extractors/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/extractors/loading.py` & `llama_index-0.9.9/llama_index/extractors/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/extractors/marvin_metadata_extractor.py` & `llama_index-0.9.9/llama_index/extractors/marvin_metadata_extractor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/extractors/metadata_extractors.py` & `llama_index-0.9.9/llama_index/extractors/metadata_extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             return []
 
         title_jobs = [
             self.llm_predictor.apredict(
                 PromptTemplate(template=self.node_template),
                 context_str=cast(TextNode, node).text,
             )
-            for node in nodes
+            for node in nodes_to_extract_title
         ]
         title_candidates = await run_jobs(
             title_jobs, show_progress=self.show_progress, workers=self.num_workers
         )
 
         if len(nodes_to_extract_title) > 1:
             titles = reduce(
```

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/__init__.py` & `llama_index-0.9.9/llama_index/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/cross_encoders/cross_encoder.py` & `llama_index-0.9.9/llama_index/finetuning/cross_encoders/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/cross_encoders/dataset_gen.py` & `llama_index-0.9.9/llama_index/finetuning/cross_encoders/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/embeddings/adapter.py` & `llama_index-0.9.9/llama_index/finetuning/embeddings/adapter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/embeddings/adapter_utils.py` & `llama_index-0.9.9/llama_index/finetuning/embeddings/adapter_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/embeddings/common.py` & `llama_index-0.9.9/llama_index/finetuning/embeddings/common.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/embeddings/sentence_transformer.py` & `llama_index-0.9.9/llama_index/finetuning/embeddings/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/gradient/base.py` & `llama_index-0.9.9/llama_index/finetuning/gradient/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/openai/base.py` & `llama_index-0.9.9/llama_index/finetuning/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/openai/validate_json.py` & `llama_index-0.9.9/llama_index/finetuning/openai/validate_json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/rerankers/cohere_reranker.py` & `llama_index-0.9.9/llama_index/finetuning/rerankers/cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/rerankers/dataset_gen.py` & `llama_index-0.9.9/llama_index/finetuning/rerankers/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/finetuning/types.py` & `llama_index-0.9.9/llama_index/finetuning/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/graph_stores/falkordb.py` & `llama_index-0.9.9/llama_index/graph_stores/falkordb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/graph_stores/kuzu.py` & `llama_index-0.9.9/llama_index/graph_stores/kuzu.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/graph_stores/nebulagraph.py` & `llama_index-0.9.9/llama_index/graph_stores/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/graph_stores/neo4j.py` & `llama_index-0.9.9/llama_index/graph_stores/neo4j.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/graph_stores/registry.py` & `llama_index-0.9.9/llama_index/graph_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/graph_stores/simple.py` & `llama_index-0.9.9/llama_index/graph_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/graph_stores/types.py` & `llama_index-0.9.9/llama_index/graph_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/img_utils.py` & `llama_index-0.9.9/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/__init__.py` & `llama_index-0.9.9/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/base.py` & `llama_index-0.9.9/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/common/struct_store/base.py` & `llama_index-0.9.9/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.9.9/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.9.9/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/common_tree/base.py` & `llama_index-0.9.9/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/composability/graph.py` & `llama_index-0.9.9/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/document_summary/__init__.py` & `llama_index-0.9.9/llama_index/indices/document_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/document_summary/base.py` & `llama_index-0.9.9/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/document_summary/retrievers.py` & `llama_index-0.9.9/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/empty/base.py` & `llama_index-0.9.9/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/empty/retrievers.py` & `llama_index-0.9.9/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/keyword_table/README.md` & `llama_index-0.9.9/llama_index/indices/keyword_table/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.9.9/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/keyword_table/base.py` & `llama_index-0.9.9/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.9.9/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.9.9/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.9.9/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/keyword_table/utils.py` & `llama_index-0.9.9/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.9.9/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/knowledge_graph/retrievers.py` & `llama_index-0.9.9/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/list/README.md` & `llama_index-0.9.9/llama_index/indices/list/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/list/__init__.py` & `llama_index-0.9.9/llama_index/indices/list/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/list/base.py` & `llama_index-0.9.9/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/list/retrievers.py` & `llama_index-0.9.9/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/loading.py` & `llama_index-0.9.9/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/managed/base.py` & `llama_index-0.9.9/llama_index/indices/managed/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/managed/vectara/base.py` & `llama_index-0.9.9/llama_index/indices/managed/vectara/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/managed/vectara/query.py` & `llama_index-0.9.9/llama_index/indices/managed/vectara/query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/managed/vectara/retriever.py` & `llama_index-0.9.9/llama_index/indices/managed/vectara/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/managed.tar.gz` & `llama_index-0.9.9/llama_index/indices/managed.tar.gz`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/multi_modal/base.py` & `llama_index-0.9.9/llama_index/indices/multi_modal/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/multi_modal/retriever.py` & `llama_index-0.9.9/llama_index/indices/multi_modal/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/postprocessor.py` & `llama_index-0.9.9/llama_index/indices/postprocessor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/prompt_helper.py` & `llama_index-0.9.9/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/query/embedding_utils.py` & `llama_index-0.9.9/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/query/query_transform/base.py` & `llama_index-0.9.9/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/query/query_transform/feedback_transform.py` & `llama_index-0.9.9/llama_index/indices/query/query_transform/feedback_transform.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.9.9/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/registry.py` & `llama_index-0.9.9/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/struct_store/__init__.py` & `llama_index-0.9.9/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/struct_store/base.py` & `llama_index-0.9.9/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.9.9/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/struct_store/json_query.py` & `llama_index-0.9.9/llama_index/indices/struct_store/json_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/struct_store/pandas.py` & `llama_index-0.9.9/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/struct_store/sql.py` & `llama_index-0.9.9/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.9.9/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/struct_store/sql_retriever.py` & `llama_index-0.9.9/llama_index/indices/struct_store/sql_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/README.md` & `llama_index-0.9.9/llama_index/indices/tree/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/__init__.py` & `llama_index-0.9.9/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.9.9/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/base.py` & `llama_index-0.9.9/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/inserter.py` & `llama_index-0.9.9/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.9.9/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.9.9/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.9.9/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/tree/utils.py` & `llama_index-0.9.9/llama_index/indices/tree/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/utils.py` & `llama_index-0.9.9/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/vector_store/base.py` & `llama_index-0.9.9/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `llama_index-0.9.9/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py` & `llama_index-0.9.9/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py` & `llama_index-0.9.9/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/indices/vector_store/retrievers/retriever.py` & `llama_index-0.9.9/llama_index/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/ingestion/cache.py` & `llama_index-0.9.9/llama_index/ingestion/cache.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/ingestion/pipeline.py` & `llama_index-0.9.9/llama_index/ingestion/pipeline.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.9.9/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.9.9/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.9.9/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.9.9/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.9.9/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/langchain_helpers/streaming.py` & `llama_index-0.9.9/llama_index/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llama_pack/download.py` & `llama_index-0.9.9/llama_index/llama_pack/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llm_predictor/base.py` & `llama_index-0.9.9/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llm_predictor/loading.py` & `llama_index-0.9.9/llama_index/llm_predictor/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llm_predictor/mock.py` & `llama_index-0.9.9/llama_index/llm_predictor/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llm_predictor/structured.py` & `llama_index-0.9.9/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llm_predictor/utils.py` & `llama_index-0.9.9/llama_index/llm_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/predictor.py` & `llama_index-0.9.9/llama_index/llm_predictor/vellum/predictor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/prompt_registry.py` & `llama_index-0.9.9/llama_index/llm_predictor/vellum/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llm_predictor/vellum/types.py` & `llama_index-0.9.9/llama_index/llm_predictor/vellum/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/__init__.py` & `llama_index-0.9.9/llama_index/llms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from llama_index.llms.everlyai import EverlyAI
 from llama_index.llms.gradient import GradientBaseModelLLM, GradientModelAdapterLLM
 from llama_index.llms.huggingface import HuggingFaceInferenceAPI, HuggingFaceLLM
 from llama_index.llms.konko import Konko
 from llama_index.llms.langchain import LangChainLLM
 from llama_index.llms.litellm import LiteLLM
 from llama_index.llms.llama_cpp import LlamaCPP
-from llama_index.llms.localai import LocalAI
+from llama_index.llms.localai import LOCALAI_DEFAULTS, LocalAI
 from llama_index.llms.mock import MockLLM
 from llama_index.llms.monsterapi import MonsterLLM
 from llama_index.llms.ollama import Ollama
 from llama_index.llms.openai import OpenAI
 from llama_index.llms.openai_like import OpenAILike
 from llama_index.llms.openllm import OpenLLM, OpenLLMAPI
 from llama_index.llms.palm import PaLM
@@ -65,14 +65,15 @@
     "HuggingFaceLLM",
     "Konko",
     "LLMMetadata",
     "LangChainLLM",
     "LiteLLM",
     "LlamaCPP",
     "LocalAI",
+    "LOCALAI_DEFAULTS",
     "MessageRole",
     "MockLLM",
     "MonsterLLM",
     "Ollama",
     "OpenAI",
     "OpenAILike",
     "OpenLLM",
```

### Comparing `llama_index-0.9.8.post1/llama_index/llms/ai21.py` & `llama_index-0.9.9/llama_index/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/ai21_utils.py` & `llama_index-0.9.9/llama_index/llms/ai21_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/anthropic.py` & `llama_index-0.9.9/llama_index/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/anthropic_utils.py` & `llama_index-0.9.9/llama_index/llms/anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/anyscale.py` & `llama_index-0.9.9/llama_index/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/anyscale_utils.py` & `llama_index-0.9.9/llama_index/llms/anyscale_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/azure_openai.py` & `llama_index-0.9.9/llama_index/llms/azure_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,15 @@
         deployment_id: Optional[str] = None,
         deployment: Optional[str] = None,
         # custom httpx client
         http_client: Optional[httpx.Client] = None,
         **kwargs: Any,
     ) -> None:
         engine = resolve_from_aliases(
-            engine,
-            deployment_name,
-            deployment_id,
-            deployment,
+            engine, deployment_name, deployment_id, deployment, azure_deployment
         )
 
         if engine is None:
             raise ValueError("You must specify an `engine` parameter.")
 
         azure_endpoint = get_from_param_or_env(
             "azure_endpoint", azure_endpoint, "AZURE_OPENAI_ENDPOINT", ""
```

### Comparing `llama_index-0.9.8.post1/llama_index/llms/base.py` & `llama_index-0.9.9/llama_index/llms/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 # ===== Generic Model Input - Chat =====
 class ChatMessage(BaseModel):
     """Chat message."""
 
     role: MessageRole = MessageRole.USER
-    content: Optional[str] = ""
+    content: Optional[Any] = ""
     additional_kwargs: dict = Field(default_factory=dict)
 
     def __str__(self) -> str:
         return f"{self.role.value}: {self.content}"
 
 
 # ===== Generic Model Output - Chat =====
```

### Comparing `llama_index-0.9.8.post1/llama_index/llms/bedrock.py` & `llama_index-0.9.9/llama_index/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/bedrock_utils.py` & `llama_index-0.9.9/llama_index/llms/bedrock_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/clarifai.py` & `llama_index-0.9.9/llama_index/llms/clarifai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/cohere.py` & `llama_index-0.9.9/llama_index/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/cohere_utils.py` & `llama_index-0.9.9/llama_index/llms/cohere_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/custom.py` & `llama_index-0.9.9/llama_index/llms/custom.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/everlyai.py` & `llama_index-0.9.9/llama_index/llms/everlyai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/everlyai_utils.py` & `llama_index-0.9.9/llama_index/llms/everlyai_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/generic_utils.py` & `llama_index-0.9.9/llama_index/llms/generic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/gradient.py` & `llama_index-0.9.9/llama_index/llms/gradient.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/huggingface.py` & `llama_index-0.9.9/llama_index/llms/huggingface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/konko.py` & `llama_index-0.9.9/llama_index/llms/konko.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/konko_utils.py` & `llama_index-0.9.9/llama_index/llms/konko_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/langchain.py` & `llama_index-0.9.9/llama_index/llms/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/langchain_utils.py` & `llama_index-0.9.9/llama_index/llms/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/litellm.py` & `llama_index-0.9.9/llama_index/llms/litellm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/litellm_utils.py` & `llama_index-0.9.9/llama_index/llms/litellm_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/llama_api.py` & `llama_index-0.9.9/llama_index/llms/llama_api.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/llama_cpp.py` & `llama_index-0.9.9/llama_index/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/llama_utils.py` & `llama_index-0.9.9/llama_index/llms/llama_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/loading.py` & `llama_index-0.9.9/llama_index/llms/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/localai.py` & `llama_index-0.9.9/llama_index/llms/localai.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-from typing import Any, Dict, Optional
+"""
+LocalAI is a free, open source, and self-hosted OpenAI alternative.
+
+Docs: https://localai.io/
+Source: https://github.com/go-skynet/LocalAI
+"""
+
+import warnings
+from types import MappingProxyType
+from typing import Any, Dict, Mapping, Optional
 
 from llama_index.bridge.pydantic import Field
 from llama_index.constants import DEFAULT_CONTEXT_WINDOW
 from llama_index.llms.base import LLMMetadata
 from llama_index.llms.openai import OpenAI
+from llama_index.llms.openai_like import OpenAILike
 from llama_index.llms.openai_utils import is_function_calling_model
 
-DEFAULT_API_KEY = "fake"
-DEFAULT_API_HOST = "localhost"
-DEFAULT_API_PORT = 8080
-DEFAULT_API_BASE = f"{DEFAULT_API_HOST}{DEFAULT_API_PORT}"
+# Use these as kwargs for OpenAILike to connect to LocalAIs
+DEFAULT_LOCALAI_PORT = 8080
+LOCALAI_DEFAULTS: Mapping[str, Any] = MappingProxyType(
+    {
+        "api_key": "localai_fake",
+        "api_type": "localai_fake",
+        "api_base": f"http://localhost:{DEFAULT_LOCALAI_PORT}/v1",
+    }
+)
 
 
 class LocalAI(OpenAI):
-    """
-    LocalAI is a free, open source, and self-hosted OpenAI alternative.
-
-    Docs: https://localai.io/
-    Source: https://github.com/go-skynet/LocalAI
-    """
-
     context_window: int = Field(
         default=DEFAULT_CONTEXT_WINDOW,
         description="The maximum number of context tokens for the model.",
         gt=0,
     )
     globally_use_chat_completions: Optional[bool] = Field(
         default=None,
@@ -33,19 +41,28 @@
             " set False to universally use /completions endpoint,"
             " set True to universally use /chat/completions endpoint."
         ),
     )
 
     def __init__(
         self,
-        api_key: Optional[str] = DEFAULT_API_KEY,
-        api_base: Optional[str] = DEFAULT_API_BASE,
+        api_key: Optional[str] = LOCALAI_DEFAULTS["api_key"],
+        api_base: Optional[str] = LOCALAI_DEFAULTS["api_base"],
         **kwargs: Any,
     ) -> None:
         super().__init__(api_key=api_key, api_base=api_base, **kwargs)
+        warnings.warn(
+            (
+                f"{type(self).__name__} subclass is deprecated in favor of"
+                f" {OpenAILike.__name__} composition. The deprecation cycle"
+                " will complete sometime in late December 2023."
+            ),
+            DeprecationWarning,
+            stacklevel=2,
+        )
 
     @classmethod
     def class_name(cls) -> str:
         return "LocalAI"
 
     @property
     def metadata(self) -> LLMMetadata:
```

### Comparing `llama_index-0.9.8.post1/llama_index/llms/mock.py` & `llama_index-0.9.9/llama_index/llms/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/monsterapi.py` & `llama_index-0.9.9/llama_index/llms/monsterapi.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/ollama.py` & `llama_index-0.9.9/llama_index/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/openai.py` & `llama_index-0.9.9/llama_index/llms/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -502,24 +502,35 @@
         message_dicts = to_openai_message_dicts(messages)
 
         async def gen() -> ChatResponseAsyncGen:
             content = ""
             tool_calls: List[ChoiceDeltaToolCall] = []
 
             is_function = False
+            first_chat_chunk = True
             async for response in await self._aclient.chat.completions.create(
                 messages=message_dicts,
                 stream=True,
                 **self._get_model_kwargs(**kwargs),
             ):
                 response = cast(ChatCompletionChunk, response)
                 if len(response.choices) > 0:
+                    # check if the first chunk has neither content nor tool_calls
+                    # this happens when 1106 models end up calling multiple tools
+                    if (
+                        first_chat_chunk
+                        and response.choices[0].delta.content is None
+                        and response.choices[0].delta.tool_calls is None
+                    ):
+                        first_chat_chunk = False
+                        continue
                     delta = response.choices[0].delta
                 else:
                     delta = ChoiceDelta()
+                first_chat_chunk = False
 
                 # check if this chunk is the start of a function call
                 if delta.tool_calls:
                     is_function = True
 
                 # update using deltas
                 role = delta.role or MessageRole.ASSISTANT
```

### Comparing `llama_index-0.9.8.post1/llama_index/llms/openai_like.py` & `llama_index-0.9.9/llama_index/llms/openai_like.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, Union
 
 from llama_index.bridge.pydantic import Field
 from llama_index.constants import DEFAULT_CONTEXT_WINDOW
 from llama_index.llms.base import LLMMetadata
 from llama_index.llms.openai import OpenAI, Tokenizer
 
 
@@ -30,15 +30,15 @@
     )
     is_function_calling_model: bool = Field(
         default=False,
         description=LLMMetadata.__fields__[
             "is_function_calling_model"
         ].field_info.description,
     )
-    tokenizer: Optional[Tokenizer] = Field(
+    tokenizer: Union[Tokenizer, str, None] = Field(
         default=None,
         description=(
             "An instance of a tokenizer object that has an encode method, or the name"
             " of a tokenizer model from Hugging Face. If left as None, then this"
             " disables inference of max_tokens."
         ),
     )
```

### Comparing `llama_index-0.9.8.post1/llama_index/llms/openai_utils.py` & `llama_index-0.9.9/llama_index/llms/openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/openllm.py` & `llama_index-0.9.9/llama_index/llms/openllm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/palm.py` & `llama_index-0.9.9/llama_index/llms/palm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/perplexity.py` & `llama_index-0.9.9/llama_index/llms/perplexity.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/portkey.py` & `llama_index-0.9.9/llama_index/llms/portkey.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/portkey_utils.py` & `llama_index-0.9.9/llama_index/llms/portkey_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/predibase.py` & `llama_index-0.9.9/llama_index/llms/predibase.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/replicate.py` & `llama_index-0.9.9/llama_index/llms/replicate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/rungpt.py` & `llama_index-0.9.9/llama_index/llms/rungpt.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/utils.py` & `llama_index-0.9.9/llama_index/llms/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/vertex.py` & `llama_index-0.9.9/llama_index/llms/vertex.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/vertex_utils.py` & `llama_index-0.9.9/llama_index/llms/vertex_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/watsonx.py` & `llama_index-0.9.9/llama_index/llms/watsonx.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/watsonx_utils.py` & `llama_index-0.9.9/llama_index/llms/watsonx_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/xinference.py` & `llama_index-0.9.9/llama_index/llms/xinference.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/llms/xinference_utils.py` & `llama_index-0.9.9/llama_index/llms/xinference_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/logger/base.py` & `llama_index-0.9.9/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/memory/chat_memory_buffer.py` & `llama_index-0.9.9/llama_index/memory/chat_memory_buffer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/memory/types.py` & `llama_index-0.9.9/llama_index/memory/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/multi_modal_llms/base.py` & `llama_index-0.9.9/llama_index/multi_modal_llms/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,28 @@
 from abc import abstractmethod
-from enum import Enum
-from typing import Any, AsyncGenerator, Generator, Optional, Sequence
+from typing import Any, Sequence
 
 from llama_index.bridge.pydantic import BaseModel, Field
 from llama_index.constants import (
     DEFAULT_CONTEXT_WINDOW,
     DEFAULT_NUM_INPUT_FILES,
     DEFAULT_NUM_OUTPUTS,
 )
+from llama_index.llms.base import (
+    ChatMessage,
+    ChatResponse,
+    ChatResponseAsyncGen,
+    ChatResponseGen,
+    CompletionResponse,
+    CompletionResponseAsyncGen,
+    CompletionResponseGen,
+)
 from llama_index.schema import BaseComponent, ImageDocument
 
 
-class MessageRole(str, Enum):
-    """Message role."""
-
-    SYSTEM = "system"
-    USER = "user"
-    ASSISTANT = "assistant"
-    FUNCTION = "function"
-
-
-# ===== Generic Model Input - Chat =====
-class ChatMessage(BaseModel):
-    """Chat message."""
-
-    role: MessageRole = MessageRole.USER
-    content: Optional[Any] = ""
-    additional_kwargs: dict = Field(default_factory=dict)
-
-    def __str__(self) -> str:
-        return f"{self.role.value}: {self.content}"
-
-
-# ===== Generic Model Output - Completion =====
-class MultiModalCompletionResponse(BaseModel):
-    """
-    Completion response.
-
-    Fields:
-        text: Text content of the response if not streaming, or if streaming,
-            the current extent of streamed text.
-        additional_kwargs: Additional information on the response(i.e. token
-            counts, function calling information).
-        raw: Optional raw JSON that was parsed to populate text, if relevant.
-        delta: New text that just streamed in (only relevant when streaming).
-    """
-
-    text: str
-    additional_kwargs: dict = Field(default_factory=dict)
-    raw: Optional[dict] = None
-    delta: Optional[str] = None
-
-    def __str__(self) -> str:
-        return self.text
-
-
-MultiModalCompletionResponseGen = Generator[MultiModalCompletionResponse, None, None]
-MultiModalCompletionResponseAsyncGen = AsyncGenerator[
-    MultiModalCompletionResponse, None
-]
-
-
 class MultiModalLLMMetadata(BaseModel):
     context_window: int = Field(
         default=DEFAULT_CONTEXT_WINDOW,
         description=(
             "Total number of tokens the model can be input when generating a response."
         ),
     )
@@ -109,27 +67,61 @@
     @abstractmethod
     def metadata(self) -> MultiModalLLMMetadata:
         """Multi-Modal LLM metadata."""
 
     @abstractmethod
     def complete(
         self, prompt: str, image_documents: Sequence[ImageDocument], **kwargs: Any
-    ) -> MultiModalCompletionResponse:
+    ) -> CompletionResponse:
         """Completion endpoint for Multi-Modal LLM."""
 
     @abstractmethod
     def stream_complete(
         self, prompt: str, image_documents: Sequence[ImageDocument], **kwargs: Any
-    ) -> MultiModalCompletionResponseGen:
+    ) -> CompletionResponseGen:
         """Streaming completion endpoint for Multi-Modal LLM."""
 
     @abstractmethod
+    def chat(
+        self,
+        messages: Sequence[ChatMessage],
+        **kwargs: Any,
+    ) -> ChatResponse:
+        """Chat endpoint for Multi-Modal LLM."""
+
+    @abstractmethod
+    def stream_chat(
+        self,
+        messages: Sequence[ChatMessage],
+        **kwargs: Any,
+    ) -> ChatResponseGen:
+        """Stream chat endpoint for Multi-Modal LLM."""
+
+    # ===== Async Endpoints =====
+
+    @abstractmethod
     async def acomplete(
         self, prompt: str, image_documents: Sequence[ImageDocument], **kwargs: Any
-    ) -> MultiModalCompletionResponse:
+    ) -> CompletionResponse:
         """Async completion endpoint for Multi-Modal LLM."""
 
     @abstractmethod
     async def astream_complete(
         self, prompt: str, image_documents: Sequence[ImageDocument], **kwargs: Any
-    ) -> MultiModalCompletionResponseAsyncGen:
+    ) -> CompletionResponseAsyncGen:
         """Async streaming completion endpoint for Multi-Modal LLM."""
+
+    @abstractmethod
+    async def achat(
+        self,
+        messages: Sequence[ChatMessage],
+        **kwargs: Any,
+    ) -> ChatResponse:
+        """Async chat endpoint for Multi-Modal LLM."""
+
+    @abstractmethod
+    async def astream_chat(
+        self,
+        messages: Sequence[ChatMessage],
+        **kwargs: Any,
+    ) -> ChatResponseAsyncGen:
+        """Async streaming chat endpoint for Multi-Modal LLM."""
```

### Comparing `llama_index-0.9.8.post1/llama_index/multi_modal_llms/generic_utils.py` & `llama_index-0.9.9/llama_index/multi_modal_llms/generic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/multi_modal_llms/openai_utils.py` & `llama_index-0.9.9/llama_index/multi_modal_llms/openai_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import logging
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, Optional, Sequence
 
-from openai.types.chat import ChatCompletionMessageParam
-
-from llama_index.llms.openai_utils import to_openai_message_dicts
 from llama_index.multi_modal_llms.base import ChatMessage
 from llama_index.multi_modal_llms.generic_utils import encode_image
 from llama_index.schema import ImageDocument
 
 DEFAULT_OPENAI_API_TYPE = "open_ai"
 DEFAULT_OPENAI_API_BASE = "https://api.openai.com/v1"
 
@@ -23,17 +20,25 @@
 API keys can be found or created at \
 https://platform.openai.com/account/api-keys
 """
 
 logger = logging.getLogger(__name__)
 
 
-def to_openai_multi_modal_payload(
-    prompt: str, image_documents: Sequence[ImageDocument], image_detail: str
-) -> List[ChatCompletionMessageParam]:
+def generate_openai_multi_modal_chat_message(
+    prompt: str,
+    role: str,
+    image_documents: Optional[Sequence[ImageDocument]] = None,
+    image_detail: Optional[str] = "low",
+) -> ChatMessage:
+    # if image_documents is empty, return text only chat message
+    if image_documents is None:
+        return ChatMessage(role=role, content=prompt)
+
+    # if image_documents is not empty, return text with images chat message
     completion_content = [{"type": "text", "text": prompt}]
     for image_document in image_documents:
         image_content: Dict[str, Any] = {}
         if image_document.image_url and image_document.image_url != "":
             image_content = {
                 "type": "image_url",
                 "image_url": image_document.image_url,
@@ -57,10 +62,8 @@
                 "image_url": {
                     "url": f"data:image/jpeg;base64,{base64_image}",
                     "detail": image_detail,
                 },
             }
 
         completion_content.append(image_content)
-    return to_openai_message_dicts(
-        [ChatMessage(role="user", content=completion_content)]
-    )
+    return ChatMessage(role=role, content=completion_content)
```

### Comparing `llama_index-0.9.8.post1/llama_index/multi_modal_llms/replicate_multi_modal.py` & `llama_index-0.9.9/llama_index/multi_modal_llms/replicate_multi_modal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from typing import Any, Callable, Dict, Optional, Sequence
 
 from llama_index.bridge.pydantic import Field, PrivateAttr
 from llama_index.callbacks import CallbackManager
 from llama_index.constants import DEFAULT_CONTEXT_WINDOW, DEFAULT_NUM_OUTPUTS
+from llama_index.llms.base import (
+    ChatMessage,
+    ChatResponse,
+    ChatResponseAsyncGen,
+    ChatResponseGen,
+    CompletionResponse,
+    CompletionResponseAsyncGen,
+    CompletionResponseGen,
+)
 from llama_index.llms.generic_utils import (
     messages_to_prompt as generic_messages_to_prompt,
 )
 from llama_index.multi_modal_llms import (
-    MultiModalCompletionResponse,
-    MultiModalCompletionResponseAsyncGen,
-    MultiModalCompletionResponseGen,
     MultiModalLLM,
     MultiModalLLMMetadata,
 )
 from llama_index.schema import ImageDocument
 
 REPLICATE_MULTI_MODAL_LLM_MODELS = {
     "llava-13b": "yorickvp/llava-13b:2facb4a474a0462c15041b78b1ad70952ea46b5ec6ad29583c0b29dbd4249591",
@@ -108,15 +114,15 @@
             "top_p": self.top_p,
         }
         return {
             **base_kwargs,
             **self.additional_kwargs,
         }
 
-    def _get_multi_modal_input_dict(
+    def _get_multi_modal_chat_messages(
         self, prompt: str, image_document: ImageDocument, **kwargs: Any
     ) -> Dict[str, Any]:
         if image_document.image_path:
             # load local image file and pass file handler to replicate
             try:
                 return {
                     self.prompt_key: prompt,
@@ -139,24 +145,24 @@
         else:
             raise FileNotFoundError(
                 "Could not load image file. Please check whether the file exists"
             )
 
     def complete(
         self, prompt: str, image_documents: Sequence[ImageDocument], **kwargs: Any
-    ) -> MultiModalCompletionResponse:
+    ) -> CompletionResponse:
         response_gen = self.stream_complete(prompt, image_documents, **kwargs)
         response_list = list(response_gen)
         final_response = response_list[-1]
         final_response.delta = None
         return final_response
 
     def stream_complete(
         self, prompt: str, image_documents: Sequence[ImageDocument], **kwargs: Any
-    ) -> MultiModalCompletionResponseGen:
+    ) -> CompletionResponseGen:
         try:
             import replicate
         except ImportError:
             raise ImportError(
                 "Could not import replicate library."
                 "Please install replicate with `pip install replicate`"
             )
@@ -164,41 +170,113 @@
         # TODO: at the current moment, only support uploading one image document
         if len(image_documents) > 1:
             raise NotImplementedError(
                 "ReplicateMultiModal currently only supports uploading one image document"
             )
 
         prompt = self._completion_to_prompt(prompt)
-        input_dict = self._get_multi_modal_input_dict(
+        input_dict = self._get_multi_modal_chat_messages(
             # using the first image for single image completion
             prompt,
             image_documents[0],
             **kwargs,
         )
         if self.model not in REPLICATE_MULTI_MODAL_LLM_MODELS.values():
             raise ValueError(
                 f"Unknown model {self.model!r}. Please provide a valid Replicate Multi-Modal model name in:"
                 f" {', '.join(REPLICATE_MULTI_MODAL_LLM_MODELS.values())}"
             )
 
         response_iter = replicate.run(self.model, input=input_dict)
 
-        def gen() -> MultiModalCompletionResponseGen:
+        def gen() -> CompletionResponseGen:
             text = ""
             for delta in response_iter:
                 text += delta
-                yield MultiModalCompletionResponse(
+                yield CompletionResponse(
                     delta=delta,
                     text=text,
                 )
 
         return gen()
 
+    def chat(
+        self,
+        messages: Sequence[ChatMessage],
+        **kwargs: Any,
+    ) -> ChatResponse:
+        raise NotImplementedError
+
+    def stream_chat(
+        self,
+        messages: Sequence[ChatMessage],
+        **kwargs: Any,
+    ) -> ChatResponseGen:
+        raise NotImplementedError
+
+    # ===== Async Endpoints =====
+
     async def acomplete(
         self, prompt: str, image_documents: Sequence[ImageDocument], **kwargs: Any
-    ) -> MultiModalCompletionResponse:
-        raise NotImplementedError
+    ) -> CompletionResponse:
+        response_gen = self.stream_complete(prompt, image_documents, **kwargs)
+        response_list = list(response_gen)
+        final_response = response_list[-1]
+        final_response.delta = None
+        return final_response
 
     async def astream_complete(
         self, prompt: str, image_documents: Sequence[ImageDocument], **kwargs: Any
-    ) -> MultiModalCompletionResponseAsyncGen:
+    ) -> CompletionResponseAsyncGen:
+        try:
+            import replicate
+        except ImportError:
+            raise ImportError(
+                "Could not import replicate library."
+                "Please install replicate with `pip install replicate`"
+            )
+
+        # TODO: at the current moment, only support uploading one image document
+        if len(image_documents) > 1:
+            raise NotImplementedError(
+                "ReplicateMultiModal currently only supports uploading one image document"
+            )
+
+        prompt = self._completion_to_prompt(prompt)
+        input_dict = self._get_multi_modal_chat_messages(
+            # using the first image for single image completion
+            prompt,
+            image_documents[0],
+            **kwargs,
+        )
+        if self.model not in REPLICATE_MULTI_MODAL_LLM_MODELS.values():
+            raise ValueError(
+                f"Unknown model {self.model!r}. Please provide a valid Replicate Multi-Modal model name in:"
+                f" {', '.join(REPLICATE_MULTI_MODAL_LLM_MODELS.values())}"
+            )
+
+        response_iter = replicate.run(self.model, input=input_dict)
+
+        async def gen() -> CompletionResponseAsyncGen:
+            text = ""
+            for delta in response_iter:
+                text += delta
+                yield CompletionResponse(
+                    delta=delta,
+                    text=text,
+                )
+
+        return gen()
+
+    async def achat(
+        self,
+        messages: Sequence[ChatMessage],
+        **kwargs: Any,
+    ) -> ChatResponse:
+        raise NotImplementedError
+
+    async def astream_chat(
+        self,
+        messages: Sequence[ChatMessage],
+        **kwargs: Any,
+    ) -> ChatResponseAsyncGen:
         raise NotImplementedError
```

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/__init__.py` & `llama_index-0.9.9/llama_index/node_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/file/html.py` & `llama_index-0.9.9/llama_index/node_parser/file/html.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/file/json.py` & `llama_index-0.9.9/llama_index/node_parser/file/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/file/markdown.py` & `llama_index-0.9.9/llama_index/node_parser/file/markdown.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/file/simple_file.py` & `llama_index-0.9.9/llama_index/node_parser/file/simple_file.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/interface.py` & `llama_index-0.9.9/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/loading.py` & `llama_index-0.9.9/llama_index/node_parser/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/node_utils.py` & `llama_index-0.9.9/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/relational/hierarchical.py` & `llama_index-0.9.9/llama_index/node_parser/relational/hierarchical.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,16 @@
             node_parser_ids = [f"chunk_size_{chunk_size}" for chunk_size in chunk_sizes]
             node_parser_map = {}
             for chunk_size, node_parser_id in zip(chunk_sizes, node_parser_ids):
                 node_parser_map[node_parser_id] = SentenceSplitter(
                     chunk_size=chunk_size,
                     callback_manager=callback_manager,
                     chunk_overlap=chunk_overlap,
+                    include_metadata=include_metadata,
+                    include_prev_next_rel=include_prev_next_rel,
                 )
         else:
             if chunk_sizes is not None:
                 raise ValueError("Cannot specify both node_parser_ids and chunk_sizes.")
             if node_parser_map is None:
                 raise ValueError(
                     "Must specify node_parser_map if using node_parser_ids."
```

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/relational/unstructured_element.py` & `llama_index-0.9.9/llama_index/node_parser/relational/unstructured_element.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/text/code.py` & `llama_index-0.9.9/llama_index/node_parser/text/code.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/text/langchain.py` & `llama_index-0.9.9/llama_index/node_parser/text/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/text/sentence.py` & `llama_index-0.9.9/llama_index/node_parser/text/sentence.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/text/sentence_window.py` & `llama_index-0.9.9/llama_index/node_parser/text/sentence_window.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/text/token.py` & `llama_index-0.9.9/llama_index/node_parser/text/token.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/node_parser/text/utils.py` & `llama_index-0.9.9/llama_index/node_parser/text/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/objects/__init__.py` & `llama_index-0.9.9/llama_index/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/objects/base.py` & `llama_index-0.9.9/llama_index/objects/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/objects/base_node_mapping.py` & `llama_index-0.9.9/llama_index/objects/base_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/objects/table_node_mapping.py` & `llama_index-0.9.9/llama_index/objects/table_node_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         )
 
     def _from_node(self, node: BaseNode) -> SQLTableSchema:
         """From node."""
         if node.metadata is None:
             raise ValueError("Metadata must be set")
         return SQLTableSchema(
-            table_name=node.metadata["name"], context_str=node.metadata["context"]
+            table_name=node.metadata["name"], context_str=node.metadata.get("context")
         )
 
     @property
     def obj_node_mapping(self) -> Dict[int, Any]:
         """The mapping data structure between node and object."""
         raise NotImplementedError("Subclasses should implement this!")
```

### Comparing `llama_index-0.9.8.post1/llama_index/objects/tool_node_mapping.py` & `llama_index-0.9.9/llama_index/objects/tool_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/output_parsers/guardrails.py` & `llama_index-0.9.9/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/output_parsers/langchain.py` & `llama_index-0.9.9/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/output_parsers/pydantic.py` & `llama_index-0.9.9/llama_index/output_parsers/pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/output_parsers/selection.py` & `llama_index-0.9.9/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/output_parsers/utils.py` & `llama_index-0.9.9/llama_index/output_parsers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/param_tuner/base.py` & `llama_index-0.9.9/llama_index/param_tuner/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/playground/base.py` & `llama_index-0.9.9/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/__init__.py` & `llama_index-0.9.9/llama_index/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/cohere_rerank.py` & `llama_index-0.9.9/llama_index/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/llm_rerank.py` & `llama_index-0.9.9/llama_index/postprocessor/llm_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/longllmlingua.py` & `llama_index-0.9.9/llama_index/postprocessor/longllmlingua.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/metadata_replacement.py` & `llama_index-0.9.9/llama_index/postprocessor/metadata_replacement.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/node.py` & `llama_index-0.9.9/llama_index/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/node_recency.py` & `llama_index-0.9.9/llama_index/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/optimizer.py` & `llama_index-0.9.9/llama_index/postprocessor/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/pii.py` & `llama_index-0.9.9/llama_index/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/sbert_rerank.py` & `llama_index-0.9.9/llama_index/postprocessor/sbert_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/postprocessor/types.py` & `llama_index-0.9.9/llama_index/postprocessor/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/__init__.py` & `llama_index-0.9.9/llama_index/program/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/guidance_program.py` & `llama_index-0.9.9/llama_index/program/guidance_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/llm_program.py` & `llama_index-0.9.9/llama_index/program/llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/llm_prompt_program.py` & `llama_index-0.9.9/llama_index/program/llm_prompt_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/lmformatenforcer_program.py` & `llama_index-0.9.9/llama_index/program/lmformatenforcer_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/multi_modal_llm_program.py` & `llama_index-0.9.9/llama_index/program/multi_modal_llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/openai_program.py` & `llama_index-0.9.9/llama_index/program/openai_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/predefined/df.py` & `llama_index-0.9.9/llama_index/program/predefined/df.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/predefined/evaporate/base.py` & `llama_index-0.9.9/llama_index/program/predefined/evaporate/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/predefined/evaporate/extractor.py` & `llama_index-0.9.9/llama_index/program/predefined/evaporate/extractor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/predefined/evaporate/prompts.py` & `llama_index-0.9.9/llama_index/program/predefined/evaporate/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/program/utils.py` & `llama_index-0.9.9/llama_index/program/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/base.py` & `llama_index-0.9.9/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/chat_prompts.py` & `llama_index-0.9.9/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.9.9/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/default_prompts.py` & `llama_index-0.9.9/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/guidance_utils.py` & `llama_index-0.9.9/llama_index/prompts/guidance_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/lmformatenforcer_utils.py` & `llama_index-0.9.9/llama_index/prompts/lmformatenforcer_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/mixin.py` & `llama_index-0.9.9/llama_index/prompts/mixin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/prompt_type.py` & `llama_index-0.9.9/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/prompt_utils.py` & `llama_index-0.9.9/llama_index/prompts/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/prompts.py` & `llama_index-0.9.9/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/prompts/system.py` & `llama_index-0.9.9/llama_index/prompts/system.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/__init__.py` & `llama_index-0.9.9/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/citation_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/citation_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/cogniswitch_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/cogniswitch_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/custom.py` & `llama_index-0.9.9/llama_index/query_engine/custom.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/flare/answer_inserter.py` & `llama_index-0.9.9/llama_index/query_engine/flare/answer_inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/flare/base.py` & `llama_index-0.9.9/llama_index/query_engine/flare/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/flare/output_parser.py` & `llama_index-0.9.9/llama_index/query_engine/flare/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/knowledge_graph_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/knowledge_graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/multi_modal.py` & `llama_index-0.9.9/llama_index/query_engine/multi_modal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/pandas_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/pandas_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/retry_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/retry_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/retry_source_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/retry_source_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/router_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/sql_join_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/sql_join_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/sql_vector_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/sql_vector_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/sub_question_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/sub_question_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.9.9/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/question_gen/guidance_generator.py` & `llama_index-0.9.9/llama_index/question_gen/guidance_generator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/question_gen/llm_generators.py` & `llama_index-0.9.9/llama_index/question_gen/llm_generators.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/question_gen/openai_generator.py` & `llama_index-0.9.9/llama_index/question_gen/openai_generator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/question_gen/output_parser.py` & `llama_index-0.9.9/llama_index/question_gen/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/question_gen/prompts.py` & `llama_index-0.9.9/llama_index/question_gen/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/question_gen/types.py` & `llama_index-0.9.9/llama_index/question_gen/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/__init__.py` & `llama_index-0.9.9/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/awadb.py` & `llama_index-0.9.9/llama_index/readers/awadb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/bagel.py` & `llama_index-0.9.9/llama_index/readers/bagel.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/base.py` & `llama_index-0.9.9/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.9.9/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/chroma.py` & `llama_index-0.9.9/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/dashvector.py` & `llama_index-0.9.9/llama_index/readers/dashvector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/database.py` & `llama_index-0.9.9/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/deeplake.py` & `llama_index-0.9.9/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/discord_reader.py` & `llama_index-0.9.9/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/download.py` & `llama_index-0.9.9/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/elasticsearch.py` & `llama_index-0.9.9/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/faiss.py` & `llama_index-0.9.9/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/base.py` & `llama_index-0.9.9/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/docs_reader.py` & `llama_index-0.9.9/llama_index/readers/file/docs_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/epub_reader.py` & `llama_index-0.9.9/llama_index/readers/file/epub_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/flat_reader.py` & `llama_index-0.9.9/llama_index/readers/file/flat_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/html_reader.py` & `llama_index-0.9.9/llama_index/readers/file/html_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/image_caption_reader.py` & `llama_index-0.9.9/llama_index/readers/file/image_caption_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/image_reader.py` & `llama_index-0.9.9/llama_index/readers/file/image_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/image_vision_llm_reader.py` & `llama_index-0.9.9/llama_index/readers/file/image_vision_llm_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/ipynb_reader.py` & `llama_index-0.9.9/llama_index/readers/file/ipynb_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/markdown_reader.py` & `llama_index-0.9.9/llama_index/readers/file/markdown_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/mbox_reader.py` & `llama_index-0.9.9/llama_index/readers/file/mbox_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/slides_reader.py` & `llama_index-0.9.9/llama_index/readers/file/slides_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/tabular_reader.py` & `llama_index-0.9.9/llama_index/readers/file/tabular_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/file/video_audio_reader.py` & `llama_index-0.9.9/llama_index/readers/file/video_audio_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.9.9/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.9.9/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/github_readers/utils.py` & `llama_index-0.9.9/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.9.9/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.9.9/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/json.py` & `llama_index-0.9.9/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/loading.py` & `llama_index-0.9.9/llama_index/readers/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/make_com/wrapper.py` & `llama_index-0.9.9/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/mbox.py` & `llama_index-0.9.9/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/metal.py` & `llama_index-0.9.9/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/milvus.py` & `llama_index-0.9.9/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/mongo.py` & `llama_index-0.9.9/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/myscale.py` & `llama_index-0.9.9/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/notion.py` & `llama_index-0.9.9/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/obsidian.py` & `llama_index-0.9.9/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/pinecone.py` & `llama_index-0.9.9/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/psychic.py` & `llama_index-0.9.9/llama_index/readers/psychic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/qdrant.py` & `llama_index-0.9.9/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/redis/utils.py` & `llama_index-0.9.9/llama_index/readers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/slack.py` & `llama_index-0.9.9/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/steamship/file_reader.py` & `llama_index-0.9.9/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/string_iterable.py` & `llama_index-0.9.9/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/twitter.py` & `llama_index-0.9.9/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/weaviate/reader.py` & `llama_index-0.9.9/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/web.py` & `llama_index-0.9.9/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/wikipedia.py` & `llama_index-0.9.9/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/readers/youtube_transcript.py` & `llama_index-0.9.9/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response/notebook_utils.py` & `llama_index-0.9.9/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response/pprint_utils.py` & `llama_index-0.9.9/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response/schema.py` & `llama_index-0.9.9/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/__init__.py` & `llama_index-0.9.9/llama_index/response_synthesizers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/accumulate.py` & `llama_index-0.9.9/llama_index/response_synthesizers/accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/base.py` & `llama_index-0.9.9/llama_index/response_synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/compact_and_accumulate.py` & `llama_index-0.9.9/llama_index/response_synthesizers/compact_and_accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/compact_and_refine.py` & `llama_index-0.9.9/llama_index/response_synthesizers/compact_and_refine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/factory.py` & `llama_index-0.9.9/llama_index/response_synthesizers/factory.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/generation.py` & `llama_index-0.9.9/llama_index/response_synthesizers/generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/no_text.py` & `llama_index-0.9.9/llama_index/response_synthesizers/no_text.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/refine.py` & `llama_index-0.9.9/llama_index/response_synthesizers/refine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/simple_summarize.py` & `llama_index-0.9.9/llama_index/response_synthesizers/simple_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/tree_summarize.py` & `llama_index-0.9.9/llama_index/response_synthesizers/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/response_synthesizers/type.py` & `llama_index-0.9.9/llama_index/response_synthesizers/type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/retrievers/__init__.py` & `llama_index-0.9.9/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/retrievers/auto_merging_retriever.py` & `llama_index-0.9.9/llama_index/retrievers/auto_merging_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/retrievers/bm25_retriever.py` & `llama_index-0.9.9/llama_index/retrievers/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/retrievers/fusion_retriever.py` & `llama_index-0.9.9/llama_index/retrievers/fusion_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/retrievers/recursive_retriever.py` & `llama_index-0.9.9/llama_index/retrievers/recursive_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/retrievers/router_retriever.py` & `llama_index-0.9.9/llama_index/retrievers/router_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/retrievers/transform_retriever.py` & `llama_index-0.9.9/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/retrievers/you_retriever.py` & `llama_index-0.9.9/llama_index/retrievers/you_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/schema.py` & `llama_index-0.9.9/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/selectors/__init__.py` & `llama_index-0.9.9/llama_index/selectors/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/selectors/embedding_selectors.py` & `llama_index-0.9.9/llama_index/selectors/embedding_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/selectors/llm_selectors.py` & `llama_index-0.9.9/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/selectors/prompts.py` & `llama_index-0.9.9/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/selectors/pydantic_selectors.py` & `llama_index-0.9.9/llama_index/selectors/pydantic_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/selectors/types.py` & `llama_index-0.9.9/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/selectors/utils.py` & `llama_index-0.9.9/llama_index/selectors/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/service_context.py` & `llama_index-0.9.9/llama_index/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/__init__.py` & `llama_index-0.9.9/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/dynamodb_docstore.py` & `llama_index-0.9.9/llama_index/storage/docstore/dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/firestore_docstore.py` & `llama_index-0.9.9/llama_index/storage/docstore/firestore_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.9.9/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.9.9/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/redis_docstore.py` & `llama_index-0.9.9/llama_index/storage/docstore/redis_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/registry.py` & `llama_index-0.9.9/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.9.9/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/types.py` & `llama_index-0.9.9/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/docstore/utils.py` & `llama_index-0.9.9/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/__init__.py` & `llama_index-0.9.9/llama_index/storage/index_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/dynamodb_index_store.py` & `llama_index-0.9.9/llama_index/storage/index_store/dynamodb_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/firestore_indexstore.py` & `llama_index-0.9.9/llama_index/storage/index_store/firestore_indexstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.9.9/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.9.9/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/redis_index_store.py` & `llama_index-0.9.9/llama_index/storage/index_store/redis_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.9.9/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/types.py` & `llama_index-0.9.9/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/index_store/utils.py` & `llama_index-0.9.9/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/kvstore/dynamodb_kvstore.py` & `llama_index-0.9.9/llama_index/storage/kvstore/dynamodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/kvstore/firestore_kvstore.py` & `llama_index-0.9.9/llama_index/storage/kvstore/firestore_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.9.9/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/kvstore/redis_kvstore.py` & `llama_index-0.9.9/llama_index/storage/kvstore/redis_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/kvstore/s3_kvstore.py` & `llama_index-0.9.9/llama_index/storage/kvstore/s3_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.9.9/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/kvstore/types.py` & `llama_index-0.9.9/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/storage/storage_context.py` & `llama_index-0.9.9/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.9.9/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/token_counter/utils.py` & `llama_index-0.9.9/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/__init__.py` & `llama_index-0.9.9/llama_index/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/download.py` & `llama_index-0.9.9/llama_index/tools/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/function_tool.py` & `llama_index-0.9.9/llama_index/tools/function_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/ondemand_loader_tool.py` & `llama_index-0.9.9/llama_index/tools/ondemand_loader_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/query_engine.py` & `llama_index-0.9.9/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/query_plan.py` & `llama_index-0.9.9/llama_index/tools/query_plan.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/retriever_tool.py` & `llama_index-0.9.9/llama_index/tools/retriever_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/tool_spec/base.py` & `llama_index-0.9.9/llama_index/tools/tool_spec/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/tool_spec/load_and_search/README.md` & `llama_index-0.9.9/llama_index/tools/tool_spec/load_and_search/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/tool_spec/load_and_search/base.py` & `llama_index-0.9.9/llama_index/tools/tool_spec/load_and_search/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/tool_spec/notion/base.py` & `llama_index-0.9.9/llama_index/tools/tool_spec/notion/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/tool_spec/slack/base.py` & `llama_index-0.9.9/llama_index/tools/tool_spec/slack/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/types.py` & `llama_index-0.9.9/llama_index/tools/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tools/utils.py` & `llama_index-0.9.9/llama_index/tools/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tts/bark.py` & `llama_index-0.9.9/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tts/base.py` & `llama_index-0.9.9/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/tts/elevenlabs.py` & `llama_index-0.9.9/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/types.py` & `llama_index-0.9.9/llama_index/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/utilities/sql_wrapper.py` & `llama_index-0.9.9/llama_index/utilities/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/utilities/token_counting.py` & `llama_index-0.9.9/llama_index/utilities/token_counting.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/utils.py` & `llama_index-0.9.9/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/__init__.py` & `llama_index-0.9.9/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/awadb.py` & `llama_index-0.9.9/llama_index/vector_stores/awadb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/azurecosmosmongo.py` & `llama_index-0.9.9/llama_index/vector_stores/azurecosmosmongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/bagel.py` & `llama_index-0.9.9/llama_index/vector_stores/bagel.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/cassandra.py` & `llama_index-0.9.9/llama_index/vector_stores/cassandra.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.9.9/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/chroma.py` & `llama_index-0.9.9/llama_index/vector_stores/chroma.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,26 @@
     metadata_dict_to_node,
     node_to_metadata_dict,
 )
 
 logger = logging.getLogger(__name__)
 
 
-def _to_chroma_filter(standard_filters: MetadataFilters) -> dict:
+def _to_chroma_filter(
+    standard_filters: MetadataFilters, condition: Optional[str] = None
+) -> dict:
     """Translate standard metadata filters to Chroma specific spec."""
     filters = {}
-    for filter in standard_filters.filters:
-        filters[filter.key] = filter.value
+    if len(standard_filters.filters) == 1:
+        filters[standard_filters.filters[0].key] = standard_filters.filters[0].value
+    else:
+        condition = condition or "$and"
+        filters[condition] = [
+            {filter.key: filter.value} for filter in standard_filters.filters
+        ]
     return filters
 
 
 import_err_msg = "`chromadb` package not found, please run `pip install chromadb`"
 
 MAX_CHUNK_SIZE = 41665  # One less than the max chunk size for ChromaDB
```

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/cogsearch.py` & `llama_index-0.9.9/llama_index/vector_stores/cogsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/dashvector.py` & `llama_index-0.9.9/llama_index/vector_stores/dashvector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/deeplake.py` & `llama_index-0.9.9/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/docarray/base.py` & `llama_index-0.9.9/llama_index/vector_stores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/docarray/hnsw.py` & `llama_index-0.9.9/llama_index/vector_stores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/docarray/in_memory.py` & `llama_index-0.9.9/llama_index/vector_stores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/dynamodb.py` & `llama_index-0.9.9/llama_index/vector_stores/dynamodb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/elasticsearch.py` & `llama_index-0.9.9/llama_index/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/epsilla.py` & `llama_index-0.9.9/llama_index/vector_stores/epsilla.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/faiss.py` & `llama_index-0.9.9/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/lancedb.py` & `llama_index-0.9.9/llama_index/vector_stores/lancedb.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         if self.refine_factor is not None:
             lance_query.refine_factor(self.refine_factor)
 
         results = lance_query.to_df()
         nodes = []
         for _, item in results.iterrows():
             node = TextNode(
-                text=item.text,
+                text=item.text or "",  # ensure text is a string
                 id_=item.id,
                 relationships={
                     NodeRelationship.SOURCE: RelatedNodeInfo(node_id=item.doc_id),
                 },
             )
             nodes.append(node)
```

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/lantern.py` & `llama_index-0.9.9/llama_index/vector_stores/lantern.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/loading.py` & `llama_index-0.9.9/llama_index/vector_stores/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/metal.py` & `llama_index-0.9.9/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/milvus.py` & `llama_index-0.9.9/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/mongodb.py` & `llama_index-0.9.9/llama_index/vector_stores/mongodb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/myscale.py` & `llama_index-0.9.9/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/neo4jvector.py` & `llama_index-0.9.9/llama_index/vector_stores/neo4jvector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/opensearch.py` & `llama_index-0.9.9/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/pgvecto_rs.py` & `llama_index-0.9.9/llama_index/vector_stores/pgvecto_rs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/pinecone.py` & `llama_index-0.9.9/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/postgres.py` & `llama_index-0.9.9/llama_index/vector_stores/postgres.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/qdrant.py` & `llama_index-0.9.9/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/redis.py` & `llama_index-0.9.9/llama_index/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/registry.py` & `llama_index-0.9.9/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/rocksetdb.py` & `llama_index-0.9.9/llama_index/vector_stores/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/simple.py` & `llama_index-0.9.9/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/singlestoredb.py` & `llama_index-0.9.9/llama_index/vector_stores/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/supabase.py` & `llama_index-0.9.9/llama_index/vector_stores/supabase.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/tair.py` & `llama_index-0.9.9/llama_index/vector_stores/tair.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/tencentvectordb.py` & `llama_index-0.9.9/llama_index/vector_stores/tencentvectordb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/timescalevector.py` & `llama_index-0.9.9/llama_index/vector_stores/timescalevector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/types.py` & `llama_index-0.9.9/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/typesense.py` & `llama_index-0.9.9/llama_index/vector_stores/typesense.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/utils.py` & `llama_index-0.9.9/llama_index/vector_stores/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/weaviate.py` & `llama_index-0.9.9/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/weaviate_utils.py` & `llama_index-0.9.9/llama_index/vector_stores/weaviate_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/llama_index/vector_stores/zep.py` & `llama_index-0.9.9/llama_index/vector_stores/zep.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.9.8.post1/pyproject.toml` & `llama_index-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Simon Suo <simon@llamaindex.ai>",
     "Sourabh Desai <sourabh@llamaindex.ai>",
 ]
 name = "llama-index"
 packages = [{include = "llama_index"}]
 readme = "README.md"
 repository = "https://github.com/run-llama/llama_index"
-version = "0.9.8.post1"
+version = "0.9.9"
 
 [tool.poetry.dependencies]
 SQLAlchemy = {extras = ["asyncio"], version = ">=1.4.49"}
 beautifulsoup4 = "^4.12.2"
 dataclasses-json = "*"
 deprecated = ">=1.2.9.3"
 fsspec = ">=2023.5.0"
@@ -66,15 +66,15 @@
 optimum = {extras = ["onnxruntime"], optional = true, version = "^1.13.2"}
 sentencepiece = {optional = true, version = "^0.1.99"}
 transformers = {extras = ["torch"], optional = true, version = "^4.34.0"}
 guidance = {optional = true, version = "^0.0.64"}
 lm-format-enforcer = {optional = true, version = "^0.4.3"}
 jsonpath-ng = {optional = true, version = "^1.6.0"}
 rank-bm25 = {optional = true, version = "^0.2.2"}
-scikit-learn = {optional = true, version = "<1.3.0"}
+scikit-learn = {optional = true, version = "*"}
 spacy = {optional = true, version = "^3.7.1"}
 aiostream = "^0.5.2"
 aiohttp = "^3.8.6"
 
 [tool.poetry.extras]
 langchain = [
     "langchain",
@@ -133,14 +133,15 @@
 myst-nb = "0.17.2"
 myst-parser = "0.18.1"
 pydantic = "<2.0.0"
 sphinx = ">=4.3.0"
 sphinx-autobuild = "^2021.3.14"
 sphinx-reredirects = "^0.1.3"
 sphinx-rtd-theme = "^1.3.0"
+sphinxcontrib-gtagjs = "^0.2.1"
 
 [tool.poetry.scripts]
 llamaindex-cli = 'llama_index.command_line.command_line:main'
 
 [tool.ruff]
 exclude = [
     "examples",
```

### Comparing `llama_index-0.9.8.post1/PKG-INFO` & `llama_index-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index
-Version: 0.9.8.post1
+Version: 0.9.9
 Summary: Interface between LLMs and your data
 Home-page: https://llamaindex.ai
 License: MIT
 Keywords: LLM,NLP,RAG,data,devtools,index,retrieval
 Author: Jerry Liu
 Author-email: jerry@llamaindex.ai
 Maintainer: Jerry Liu
@@ -41,15 +41,15 @@
 Requires-Dist: openai (>=1.1.0)
 Requires-Dist: optimum[onnxruntime] (>=1.13.2,<2.0.0) ; extra == "local-models"
 Requires-Dist: pandas
 Requires-Dist: pgvector (>=0.1.0,<0.2.0) ; extra == "postgres"
 Requires-Dist: psycopg-binary (>=3.1.12,<4.0.0) ; extra == "postgres"
 Requires-Dist: rank-bm25 (>=0.2.2,<0.3.0) ; extra == "query-tools"
 Requires-Dist: requests (>=2.31.0)
-Requires-Dist: scikit-learn (<1.3.0) ; extra == "query-tools"
+Requires-Dist: scikit-learn ; extra == "query-tools"
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0) ; extra == "local-models"
 Requires-Dist: spacy (>=3.7.1,<4.0.0) ; extra == "query-tools"
 Requires-Dist: tenacity (>=8.2.0,<9.0.0)
 Requires-Dist: tiktoken (>=0.3.3)
 Requires-Dist: transformers[torch] (>=4.34.0,<5.0.0) ; extra == "local-models"
 Requires-Dist: typing-extensions (>=4.5.0)
 Requires-Dist: typing-inspect (>=0.8.0)
```

