# Comparing `tmp/litellm-1.9.5.tar.gz` & `tmp/litellm-1.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-1.9.5.tar", max compression
+gzip compressed data, was "litellm-1.9.dev0.tar", max compression
```

## Comparing `litellm-1.9.5.tar` & `litellm-1.9.dev0.tar`

### file list

```diff
@@ -1,154 +1,153 @@
--rw-r--r--   0        0        0     1065 2023-12-02 01:28:12.722783 litellm-1.9.5/LICENSE
--rw-r--r--   0        0        0    10280 2023-12-02 01:28:12.722783 litellm-1.9.5/README.md
--rw-r--r--   0        0        0    13838 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/__init__.py
--rw-r--r--   0        0        0      101 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/_version.py
--rw-r--r--   0        0        0     7264 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/budget_manager.py
--rw-r--r--   0        0        0    10882 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/caching.py
--rw-r--r--   0        0        0      108 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/cost.json
--rw-r--r--   0        0        0      941 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/deprecated_litellm_server/.env.template
--rw-r--r--   0        0        0      224 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/deprecated_litellm_server/Dockerfile
--rw-r--r--   0        0        0       62 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/deprecated_litellm_server/README.md
--rw-r--r--   0        0        0       51 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/deprecated_litellm_server/__init__.py
--rw-r--r--   0        0        0     8376 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/deprecated_litellm_server/main.py
--rw-r--r--   0        0        0       70 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/deprecated_litellm_server/requirements.txt
--rw-r--r--   0        0        0     3245 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/deprecated_litellm_server/server_utils.py
--rw-r--r--   0        0        0     6318 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/exceptions.py
--rw-r--r--   0        0        0       16 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/__init__.py
--rw-r--r--   0        0        0     6535 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     6656 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     1913 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/custom_logger.py
--rw-r--r--   0        0        0     4184 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     3081 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/langfuse.py
--rw-r--r--   0        0        0     3269 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/langsmith.py
--rw-r--r--   0        0        0    10553 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/litedebugger.py
--rw-r--r--   0        0        0     3663 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/llmonitor.py
--rw-r--r--   0        0        0     2945 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/prompt_layer.py
--rw-r--r--   0        0        0     4121 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/supabase.py
--rw-r--r--   0        0        0     3321 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/traceloop.py
--rw-r--r--   0        0        0     7802 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/integrations/weights_biases.py
--rw-r--r--   0        0        0       16 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/llms/__init__.py
--rw-r--r--   0        0        0     7732 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/llms/ai21.py
--rw-r--r--   0        0        0    12561 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/llms/aleph_alpha.py
--rw-r--r--   0        0        0     6522 2023-12-02 01:28:13.162797 litellm-1.9.5/litellm/llms/anthropic.py
--rw-r--r--   0        0        0    17951 2023-12-02 01:28:13.166797 litellm-1.9.5/litellm/llms/azure.py
--rw-r--r--   0        0        0     1384 2023-12-02 01:28:13.166797 litellm-1.9.5/litellm/llms/base.py
--rw-r--r--   0        0        0     5753 2023-12-02 01:28:13.166797 litellm-1.9.5/litellm/llms/baseten.py
--rw-r--r--   0        0        0    23751 2023-12-02 01:28:13.166797 litellm-1.9.5/litellm/llms/bedrock.py
--rw-r--r--   0        0        0    10085 2023-12-02 01:28:13.166797 litellm-1.9.5/litellm/llms/cohere.py
--rw-r--r--   0        0        0    76183 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/huggingface_llms_metadata/hf_conversational_models.txt
--rw-r--r--   0        0        0  1288358 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/huggingface_llms_metadata/hf_text_generation_models.txt
--rw-r--r--   0        0        0    27299 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/huggingface_restapi.py
--rw-r--r--   0        0        0     5762 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/maritalk.py
--rw-r--r--   0        0        0     7692 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/nlp_cloud.py
--rw-r--r--   0        0        0    10894 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/ollama.py
--rw-r--r--   0        0        0     4133 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/oobabooga.py
--rw-r--r--   0        0        0    27717 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/openai.py
--rw-r--r--   0        0        0     6787 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/palm.py
--rw-r--r--   0        0        0     6939 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/petals.py
--rw-r--r--   0        0        0    15012 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/prompt_templates/factory.py
--rw-r--r--   0        0        0    12557 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/replicate.py
--rw-r--r--   0        0        0     6709 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/sagemaker.py
--rw-r--r--   0        0        0     8273 2023-12-02 01:28:13.170797 litellm-1.9.5/litellm/llms/together_ai.py
--rw-r--r--   0        0        0  1774213 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/llms/tokenizers/anthropic_tokenizer.json
--rw-r--r--   0        0        0     7010 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/llms/vertex_ai.py
--rw-r--r--   0        0        0     6041 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/llms/vllm.py
--rw-r--r--   0        0        0    99504 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/main.py
--rw-r--r--   0        0        0    19706 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/model_prices_and_context_window_backup.json
--rw-r--r--   0        0        0       17 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/.gitignore
--rw-r--r--   0        0        0      787 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/README.md
--rw-r--r--   0        0        0       15 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/__init__.py
--rw-r--r--   0        0        0     1103 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/config.yaml
--rw-r--r--   0        0        0     1225 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/example_config_yaml/aliases_config.yaml
--rw-r--r--   0        0        0      476 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/example_config_yaml/azure_config.yaml
--rw-r--r--   0        0        0      382 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/example_config_yaml/azure_config_with_tpm.yaml
--rw-r--r--   0        0        0      174 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/example_config_yaml/hosted_litellm.yaml
--rw-r--r--   0        0        0      181 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/example_config_yaml/langfuse_config.yaml
--rw-r--r--   0        0        0      886 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/example_config_yaml/load_balancer.yaml
--rw-r--r--   0        0        0      326 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/example_config_yaml/queue.yaml
--rw-r--r--   0        0        0      107 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/lambda.py
--rw-r--r--   0        0        0     7163 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/openapi.json
--rw-r--r--   0        0        0    10897 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/proxy_cli.py
--rw-r--r--   0        0        0    42572 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/proxy_server.py
--rw-r--r--   0        0        0     2536 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/queue/celery_app.py
--rw-r--r--   0        0        0      312 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/queue/celery_worker.py
--rw-r--r--   0        0        0      874 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/queue/rq_worker.py
--rw-r--r--   0        0        0      387 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/schema.prisma
--rwxr-xr-x   0        0        0       32 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/start.sh
--rw-r--r--   0        0        0     1512 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/bursty_load_test_completion.py
--rw-r--r--   0        0        0        0 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/error_log.txt
--rw-r--r--   0        0        0     1436 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/load_test_completion.py
--rw-r--r--   0        0        0     2947 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/load_test_embedding.py
--rw-r--r--   0        0        0     1592 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/load_test_embedding_100.py
--rw-r--r--   0        0        0     2989 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/load_test_embedding_proxy.py
--rw-r--r--   0        0        0     3867 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/load_test_q.py
--rw-r--r--   0        0        0        0 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/request_log.txt
--rw-r--r--   0        0        0      743 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/test_async.py
--rw-r--r--   0        0        0      388 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/test_openai_request.py
--rw-r--r--   0        0        0      730 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/test_proxy_exception_mapping.py
--rw-r--r--   0        0        0     2487 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/tests/test_q.py
--rw-r--r--   0        0        0     2866 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/proxy/utils.py
--rw-r--r--   0        0        0    50131 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/router.py
--rw-r--r--   0        0        0     1455 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/api_log.json
--rw-r--r--   0        0        0     3939 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/data_map.txt
--rw-r--r--   0        0        0       36 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0       37 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/model_cost.json
--rw-r--r--   0        0        0     5914 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/test_acooldowns_router.py
--rw-r--r--   0        0        0     2537 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/test_add_function_to_prompt.py
--rw-r--r--   0        0        0     5882 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     4380 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0     1999 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/test_batch_completions.py
--rw-r--r--   0        0        0     5098 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/test_budget_manager.py
--rw-r--r--   0        0        0    12101 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/test_caching.py
--rw-r--r--   0        0        0     2194 2023-12-02 01:28:13.182798 litellm-1.9.5/litellm/tests/test_class.py
--rw-r--r--   0        0        0    54467 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     1898 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_completion_with_retries.py
--rw-r--r--   0        0        0     3056 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_config.py
--rw-r--r--   0        0        0     4508 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_custom_logger.py
--rw-r--r--   0        0        0     7217 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_embedding.py
--rw-r--r--   0        0        0    11601 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0     8324 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_function_calling.py
--rw-r--r--   0        0        0     3991 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_get_model_cost_map.py
--rw-r--r--   0        0        0      284 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_get_model_file.py
--rw-r--r--   0        0        0      253 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_get_model_list.py
--rw-r--r--   0        0        0      769 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1920 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_hf_prompt_templates.py
--rw-r--r--   0        0        0     2797 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_langchain_ChatLiteLLM.py
--rw-r--r--   0        0        0     4430 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_langfuse.py
--rw-r--r--   0        0        0     1444 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_langsmith.py
--rw-r--r--   0        0        0     1119 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_litellm_max_budget.py
--rw-r--r--   0        0        0     2247 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_llmonitor_integration.py
--rw-r--r--   0        0        0     2440 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_loadtest_router.py
--rw-r--r--   0        0        0    13738 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      322 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_longer_context_fallback.py
--rw-r--r--   0        0        0     1114 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_mock_request.py
--rw-r--r--   0        0        0      950 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_model_alias_map.py
--rw-r--r--   0        0        0      626 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_model_response_typing/server.py
--rw-r--r--   0        0        0      495 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_model_response_typing/test.py
--rw-r--r--   0        0        0     1755 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_multiple_deployments.py
--rw-r--r--   0        0        0     3660 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_ollama.py
--rw-r--r--   0        0        0     4671 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_ollama_local.py
--rw-r--r--   0        0        0     5356 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_profiling_router.py
--rw-r--r--   0        0        0      698 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_prompt_factory.py
--rw-r--r--   0        0        0     2402 2023-12-02 01:28:13.186798 litellm-1.9.5/litellm/tests/test_promptlayer_integration.py
--rw-r--r--   0        0        0    20205 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_provider_specific_config.py
--rw-r--r--   0        0        0     2810 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_proxy_server.py
--rw-r--r--   0        0        0     1765 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_register_model.py
--rw-r--r--   0        0        0     9399 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_router.py
--rw-r--r--   0        0        0     4991 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_router_fallbacks.py
--rw-r--r--   0        0        0     9283 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_router_get_deployments.py
--rw-r--r--   0        0        0     2749 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_rules.py
--rw-r--r--   0        0        0     3148 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_stream_chunk_builder.py
--rw-r--r--   0        0        0    47035 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_streaming.py
--rw-r--r--   0        0        0     2075 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0    19400 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_text_completion.py
--rw-r--r--   0        0        0     1758 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0     3544 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_token_counter.py
--rw-r--r--   0        0        0     9244 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_utils.py
--rw-r--r--   0        0        0      296 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_validate_environment.py
--rw-r--r--   0        0        0     1832 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/test_wandb.py
--rw-r--r--   0        0        0      208 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/tests/user_cost.json
--rw-r--r--   0        0        0     4315 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/timeout.py
--rw-r--r--   0        0        0   272304 2023-12-02 01:28:13.190798 litellm-1.9.5/litellm/utils.py
--rw-r--r--   0        0        0      953 2023-12-02 01:28:13.194798 litellm-1.9.5/pyproject.toml
--rw-r--r--   0        0        0      137 2023-12-02 01:28:13.194798 litellm-1.9.5/requirements.txt
--rw-r--r--   0        0        0    11418 1970-01-01 00:00:00.000000 litellm-1.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-27 00:10:35.076914 litellm-1.9.dev0/LICENSE
+-rw-r--r--   0        0        0    10280 2023-11-30 00:44:40.403748 litellm-1.9.dev0/README.md
+-rw-r--r--   0        0        0    13838 2023-11-29 01:49:53.315605 litellm-1.9.dev0/litellm/__init__.py
+-rw-r--r--   0        0        0      101 2023-08-28 16:20:23.192479 litellm-1.9.dev0/litellm/_version.py
+-rw-r--r--   0        0        0     7264 2023-11-04 20:23:02.408280 litellm-1.9.dev0/litellm/budget_manager.py
+-rw-r--r--   0        0        0    10882 2023-11-24 22:01:21.870623 litellm-1.9.dev0/litellm/caching.py
+-rw-r--r--   0        0        0      108 2023-09-10 02:11:35.203870 litellm-1.9.dev0/litellm/cost.json
+-rw-r--r--   0        0        0      941 2023-11-20 23:43:32.986397 litellm-1.9.dev0/litellm/deprecated_litellm_server/.env.template
+-rw-r--r--   0        0        0      224 2023-11-20 23:43:32.986595 litellm-1.9.dev0/litellm/deprecated_litellm_server/Dockerfile
+-rw-r--r--   0        0        0       62 2023-11-20 23:43:32.986782 litellm-1.9.dev0/litellm/deprecated_litellm_server/README.md
+-rw-r--r--   0        0        0       51 2023-11-20 23:43:32.987455 litellm-1.9.dev0/litellm/deprecated_litellm_server/__init__.py
+-rw-r--r--   0        0        0     8376 2023-11-20 23:43:32.987967 litellm-1.9.dev0/litellm/deprecated_litellm_server/main.py
+-rw-r--r--   0        0        0       70 2023-11-20 23:43:32.988152 litellm-1.9.dev0/litellm/deprecated_litellm_server/requirements.txt
+-rw-r--r--   0        0        0     3245 2023-11-20 23:43:32.988914 litellm-1.9.dev0/litellm/deprecated_litellm_server/server_utils.py
+-rw-r--r--   0        0        0     6318 2023-11-21 21:31:18.858343 litellm-1.9.dev0/litellm/exceptions.py
+-rw-r--r--   0        0        0       16 2023-08-18 18:04:08.284134 litellm-1.9.dev0/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0     6535 2023-08-18 18:04:08.335799 litellm-1.9.dev0/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     6656 2023-08-18 18:04:08.323912 litellm-1.9.dev0/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     1913 2023-11-25 00:52:54.013934 litellm-1.9.dev0/litellm/integrations/custom_logger.py
+-rw-r--r--   0        0        0     4184 2023-08-18 18:04:08.313780 litellm-1.9.dev0/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     3081 2023-11-30 22:08:49.535350 litellm-1.9.dev0/litellm/integrations/langfuse.py
+-rw-r--r--   0        0        0     3269 2023-10-18 19:00:07.520393 litellm-1.9.dev0/litellm/integrations/langsmith.py
+-rw-r--r--   0        0        0    10553 2023-09-08 19:36:33.876423 litellm-1.9.dev0/litellm/integrations/litedebugger.py
+-rw-r--r--   0        0        0     3663 2023-10-20 16:05:14.765281 litellm-1.9.dev0/litellm/integrations/llmonitor.py
+-rw-r--r--   0        0        0     2945 2023-11-02 15:18:00.621732 litellm-1.9.dev0/litellm/integrations/prompt_layer.py
+-rw-r--r--   0        0        0     4121 2023-10-11 19:19:43.658350 litellm-1.9.dev0/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0     3321 2023-10-25 00:40:59.602578 litellm-1.9.dev0/litellm/integrations/traceloop.py
+-rw-r--r--   0        0        0     7802 2023-11-21 02:52:02.562879 litellm-1.9.dev0/litellm/integrations/weights_biases.py
+-rw-r--r--   0        0        0       16 2023-08-18 18:04:08.288983 litellm-1.9.dev0/litellm/llms/__init__.py
+-rw-r--r--   0        0        0     7732 2023-11-21 02:28:19.472920 litellm-1.9.dev0/litellm/llms/ai21.py
+-rw-r--r--   0        0        0    12561 2023-11-21 02:28:19.473092 litellm-1.9.dev0/litellm/llms/aleph_alpha.py
+-rw-r--r--   0        0        0     6522 2023-11-21 17:58:02.447563 litellm-1.9.dev0/litellm/llms/anthropic.py
+-rw-r--r--   0        0        0    17859 2023-11-30 21:33:17.047507 litellm-1.9.dev0/litellm/llms/azure.py
+-rw-r--r--   0        0        0     1384 2023-11-16 01:45:52.037747 litellm-1.9.dev0/litellm/llms/base.py
+-rw-r--r--   0        0        0     5753 2023-11-21 02:28:19.473441 litellm-1.9.dev0/litellm/llms/baseten.py
+-rw-r--r--   0        0        0    23751 2023-11-30 00:36:07.551803 litellm-1.9.dev0/litellm/llms/bedrock.py
+-rw-r--r--   0        0        0    10085 2023-11-21 02:28:19.473797 litellm-1.9.dev0/litellm/llms/cohere.py
+-rw-r--r--   0        0        0    76183 2023-09-27 22:56:45.021072 litellm-1.9.dev0/litellm/llms/huggingface_llms_metadata/hf_conversational_models.txt
+-rw-r--r--   0        0        0  1288358 2023-09-27 22:56:45.026183 litellm-1.9.dev0/litellm/llms/huggingface_llms_metadata/hf_text_generation_models.txt
+-rw-r--r--   0        0        0    27299 2023-11-23 15:55:12.819071 litellm-1.9.dev0/litellm/llms/huggingface_restapi.py
+-rw-r--r--   0        0        0     5762 2023-11-21 02:28:19.474311 litellm-1.9.dev0/litellm/llms/maritalk.py
+-rw-r--r--   0        0        0     7692 2023-11-25 21:50:16.412899 litellm-1.9.dev0/litellm/llms/nlp_cloud.py
+-rw-r--r--   0        0        0    10894 2023-11-15 01:50:44.014411 litellm-1.9.dev0/litellm/llms/ollama.py
+-rw-r--r--   0        0        0     4133 2023-11-21 02:28:19.474637 litellm-1.9.dev0/litellm/llms/oobabooga.py
+-rw-r--r--   0        0        0    27862 2023-11-30 03:58:12.064978 litellm-1.9.dev0/litellm/llms/openai.py
+-rw-r--r--   0        0        0     6787 2023-11-21 02:28:19.474804 litellm-1.9.dev0/litellm/llms/palm.py
+-rw-r--r--   0        0        0     6939 2023-11-21 02:28:19.475057 litellm-1.9.dev0/litellm/llms/petals.py
+-rw-r--r--   0        0        0    15012 2023-11-21 17:58:02.447930 litellm-1.9.dev0/litellm/llms/prompt_templates/factory.py
+-rw-r--r--   0        0        0    12557 2023-11-30 03:45:08.127220 litellm-1.9.dev0/litellm/llms/replicate.py
+-rw-r--r--   0        0        0     6709 2023-11-27 18:27:40.239543 litellm-1.9.dev0/litellm/llms/sagemaker.py
+-rw-r--r--   0        0        0     8273 2023-11-21 02:28:19.475610 litellm-1.9.dev0/litellm/llms/together_ai.py
+-rw-r--r--   0        0        0  1774213 2023-09-23 03:34:59.167844 litellm-1.9.dev0/litellm/llms/tokenizers/anthropic_tokenizer.json
+-rw-r--r--   0        0        0     7010 2023-11-30 02:28:45.154079 litellm-1.9.dev0/litellm/llms/vertex_ai.py
+-rw-r--r--   0        0        0     6041 2023-11-23 15:55:12.819717 litellm-1.9.dev0/litellm/llms/vllm.py
+-rw-r--r--   0        0        0    99504 2023-11-30 21:33:17.048524 litellm-1.9.dev0/litellm/main.py
+-rw-r--r--   0        0        0    19706 2023-11-16 17:51:17.134491 litellm-1.9.dev0/litellm/model_prices_and_context_window_backup.json
+-rw-r--r--   0        0        0       17 2023-10-13 04:25:18.062435 litellm-1.9.dev0/litellm/proxy/.gitignore
+-rw-r--r--   0        0        0      787 2023-11-18 01:40:28.713919 litellm-1.9.dev0/litellm/proxy/README.md
+-rw-r--r--   0        0        0       15 2023-09-29 00:00:44.125765 litellm-1.9.dev0/litellm/proxy/__init__.py
+-rw-r--r--   0        0        0     1103 2023-11-30 21:16:46.322845 litellm-1.9.dev0/litellm/proxy/config.yaml
+-rw-r--r--   0        0        0     1225 2023-11-29 21:25:40.785995 litellm-1.9.dev0/litellm/proxy/example_config_yaml/aliases_config.yaml
+-rw-r--r--   0        0        0      476 2023-11-27 15:35:22.346175 litellm-1.9.dev0/litellm/proxy/example_config_yaml/azure_config.yaml
+-rw-r--r--   0        0        0      382 2023-11-30 21:16:30.341744 litellm-1.9.dev0/litellm/proxy/example_config_yaml/azure_config_with_tpm.yaml
+-rw-r--r--   0        0        0      174 2023-11-22 16:10:26.844631 litellm-1.9.dev0/litellm/proxy/example_config_yaml/hosted_litellm.yaml
+-rw-r--r--   0        0        0      181 2023-11-16 00:41:06.743941 litellm-1.9.dev0/litellm/proxy/example_config_yaml/langfuse_config.yaml
+-rw-r--r--   0        0        0      886 2023-11-22 00:22:30.494291 litellm-1.9.dev0/litellm/proxy/example_config_yaml/load_balancer.yaml
+-rw-r--r--   0        0        0      326 2023-11-22 00:21:41.574403 litellm-1.9.dev0/litellm/proxy/example_config_yaml/queue.yaml
+-rw-r--r--   0        0        0      107 2023-11-23 18:40:32.163589 litellm-1.9.dev0/litellm/proxy/lambda.py
+-rw-r--r--   0        0        0     7163 2023-10-14 04:48:28.451373 litellm-1.9.dev0/litellm/proxy/openapi.json
+-rw-r--r--   0        0        0    10897 2023-11-29 01:38:09.870081 litellm-1.9.dev0/litellm/proxy/proxy_cli.py
+-rw-r--r--   0        0        0    40103 2023-11-30 18:03:40.991872 litellm-1.9.dev0/litellm/proxy/proxy_server.py
+-rw-r--r--   0        0        0     2521 2023-11-22 04:48:56.273157 litellm-1.9.dev0/litellm/proxy/queue/celery_app.py
+-rw-r--r--   0        0        0      312 2023-11-22 02:02:49.971540 litellm-1.9.dev0/litellm/proxy/queue/celery_worker.py
+-rw-r--r--   0        0        0      874 2023-11-22 00:59:33.726869 litellm-1.9.dev0/litellm/proxy/queue/rq_worker.py
+-rw-r--r--   0        0        0      387 2023-11-24 04:11:23.522406 litellm-1.9.dev0/litellm/proxy/schema.prisma
+-rwxr-xr-x   0        0        0       32 2023-11-18 01:37:48.436307 litellm-1.9.dev0/litellm/proxy/start.sh
+-rw-r--r--   0        0        0     1512 2023-11-30 21:15:02.613241 litellm-1.9.dev0/litellm/proxy/tests/bursty_load_test_completion.py
+-rw-r--r--   0        0        0        0 2023-11-30 21:15:24.084102 litellm-1.9.dev0/litellm/proxy/tests/error_log.txt
+-rw-r--r--   0        0        0     1436 2023-11-30 21:17:14.546705 litellm-1.9.dev0/litellm/proxy/tests/load_test_completion.py
+-rw-r--r--   0        0        0     2947 2023-11-25 01:14:17.278099 litellm-1.9.dev0/litellm/proxy/tests/load_test_embedding.py
+-rw-r--r--   0        0        0     2989 2023-11-25 01:06:18.452735 litellm-1.9.dev0/litellm/proxy/tests/load_test_embedding_proxy.py
+-rw-r--r--   0        0        0     3867 2023-11-22 05:07:13.692517 litellm-1.9.dev0/litellm/proxy/tests/load_test_q.py
+-rw-r--r--   0        0        0        0 2023-11-25 01:14:33.607516 litellm-1.9.dev0/litellm/proxy/tests/request_log.txt
+-rw-r--r--   0        0        0      743 2023-11-24 22:01:21.872176 litellm-1.9.dev0/litellm/proxy/tests/test_async.py
+-rw-r--r--   0        0        0      388 2023-11-30 04:05:12.292551 litellm-1.9.dev0/litellm/proxy/tests/test_openai_request.py
+-rw-r--r--   0        0        0      730 2023-11-23 04:33:24.710675 litellm-1.9.dev0/litellm/proxy/tests/test_proxy_exception_mapping.py
+-rw-r--r--   0        0        0     2487 2023-11-22 17:13:11.181659 litellm-1.9.dev0/litellm/proxy/tests/test_q.py
+-rw-r--r--   0        0        0     2866 2023-11-25 01:02:11.378301 litellm-1.9.dev0/litellm/proxy/utils.py
+-rw-r--r--   0        0        0    48957 2023-11-30 18:56:34.174344 litellm-1.9.dev0/litellm/router.py
+-rw-r--r--   0        0        0     1455 2023-11-06 15:17:35.848528 litellm-1.9.dev0/litellm/tests/api_log.json
+-rw-r--r--   0        0        0     3939 2023-11-11 00:11:33.982672 litellm-1.9.dev0/litellm/tests/data_map.txt
+-rw-r--r--   0        0        0       36 2023-08-03 04:02:44.603873 litellm-1.9.dev0/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0       37 2023-09-10 23:04:25.835866 litellm-1.9.dev0/litellm/tests/model_cost.json
+-rw-r--r--   0        0        0     5914 2023-11-29 01:07:48.245727 litellm-1.9.dev0/litellm/tests/test_acooldowns_router.py
+-rw-r--r--   0        0        0     2537 2023-11-17 22:31:02.833824 litellm-1.9.dev0/litellm/tests/test_add_function_to_prompt.py
+-rw-r--r--   0        0        0     5802 2023-11-29 01:49:53.317451 litellm-1.9.dev0/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     4380 2023-11-27 21:26:10.127474 litellm-1.9.dev0/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0     1999 2023-11-25 01:02:11.378998 litellm-1.9.dev0/litellm/tests/test_batch_completions.py
+-rw-r--r--   0        0        0     5098 2023-09-30 22:45:00.803571 litellm-1.9.dev0/litellm/tests/test_budget_manager.py
+-rw-r--r--   0        0        0    12101 2023-11-25 23:33:46.417480 litellm-1.9.dev0/litellm/tests/test_caching.py
+-rw-r--r--   0        0        0     2194 2023-11-15 20:39:51.716563 litellm-1.9.dev0/litellm/tests/test_class.py
+-rw-r--r--   0        0        0    54382 2023-11-30 21:33:17.048993 litellm-1.9.dev0/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     1898 2023-11-21 00:57:37.449984 litellm-1.9.dev0/litellm/tests/test_completion_with_retries.py
+-rw-r--r--   0        0        0     3056 2023-10-12 22:07:51.536575 litellm-1.9.dev0/litellm/tests/test_config.py
+-rw-r--r--   0        0        0     4508 2023-11-30 00:09:31.297599 litellm-1.9.dev0/litellm/tests/test_custom_logger.py
+-rw-r--r--   0        0        0     7217 2023-11-30 03:43:44.695312 litellm-1.9.dev0/litellm/tests/test_embedding.py
+-rw-r--r--   0        0        0    11601 2023-11-29 05:22:01.558771 litellm-1.9.dev0/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0     8324 2023-11-30 00:09:31.297813 litellm-1.9.dev0/litellm/tests/test_function_calling.py
+-rw-r--r--   0        0        0     3991 2023-11-24 05:41:38.651973 litellm-1.9.dev0/litellm/tests/test_get_model_cost_map.py
+-rw-r--r--   0        0        0      284 2023-10-19 00:35:38.822650 litellm-1.9.dev0/litellm/tests/test_get_model_file.py
+-rw-r--r--   0        0        0      253 2023-08-22 22:17:15.768398 litellm-1.9.dev0/litellm/tests/test_get_model_list.py
+-rw-r--r--   0        0        0      769 2023-10-31 21:29:43.647142 litellm-1.9.dev0/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1920 2023-09-30 22:45:00.804738 litellm-1.9.dev0/litellm/tests/test_hf_prompt_templates.py
+-rw-r--r--   0        0        0     2797 2023-11-14 04:21:45.814351 litellm-1.9.dev0/litellm/tests/test_langchain_ChatLiteLLM.py
+-rw-r--r--   0        0        0     4430 2023-11-30 21:55:47.940997 litellm-1.9.dev0/litellm/tests/test_langfuse.py
+-rw-r--r--   0        0        0     1444 2023-10-18 19:00:19.826316 litellm-1.9.dev0/litellm/tests/test_langsmith.py
+-rw-r--r--   0        0        0     1119 2023-09-14 23:24:03.911168 litellm-1.9.dev0/litellm/tests/test_litellm_max_budget.py
+-rw-r--r--   0        0        0     2247 2023-11-27 21:25:53.794653 litellm-1.9.dev0/litellm/tests/test_llmonitor_integration.py
+-rw-r--r--   0        0        0     2440 2023-11-20 17:44:57.789006 litellm-1.9.dev0/litellm/tests/test_loadtest_router.py
+-rw-r--r--   0        0        0    13738 2023-10-09 15:13:12.187156 litellm-1.9.dev0/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      322 2023-09-26 04:42:46.696676 litellm-1.9.dev0/litellm/tests/test_longer_context_fallback.py
+-rw-r--r--   0        0        0     1114 2023-09-28 00:49:31.904105 litellm-1.9.dev0/litellm/tests/test_mock_request.py
+-rw-r--r--   0        0        0      950 2023-11-16 02:07:04.156187 litellm-1.9.dev0/litellm/tests/test_model_alias_map.py
+-rw-r--r--   0        0        0      626 2023-08-18 18:04:08.682322 litellm-1.9.dev0/litellm/tests/test_model_response_typing/server.py
+-rw-r--r--   0        0        0      495 2023-08-18 18:04:08.682784 litellm-1.9.dev0/litellm/tests/test_model_response_typing/test.py
+-rw-r--r--   0        0        0     1755 2023-11-21 05:23:18.689343 litellm-1.9.dev0/litellm/tests/test_multiple_deployments.py
+-rw-r--r--   0        0        0     3660 2023-10-11 23:49:07.689805 litellm-1.9.dev0/litellm/tests/test_ollama.py
+-rw-r--r--   0        0        0     4671 2023-11-10 16:54:02.268382 litellm-1.9.dev0/litellm/tests/test_ollama_local.py
+-rw-r--r--   0        0        0     3965 2023-11-30 04:05:13.732795 litellm-1.9.dev0/litellm/tests/test_profiling_router.py
+-rw-r--r--   0        0        0      698 2023-10-12 04:32:00.858917 litellm-1.9.dev0/litellm/tests/test_prompt_factory.py
+-rw-r--r--   0        0        0     2402 2023-11-02 15:18:00.628536 litellm-1.9.dev0/litellm/tests/test_promptlayer_integration.py
+-rw-r--r--   0        0        0    20205 2023-10-12 23:02:09.506177 litellm-1.9.dev0/litellm/tests/test_provider_specific_config.py
+-rw-r--r--   0        0        0     2812 2023-11-24 05:16:51.696988 litellm-1.9.dev0/litellm/tests/test_proxy_server.py
+-rw-r--r--   0        0        0     1765 2023-11-30 04:15:52.168304 litellm-1.9.dev0/litellm/tests/test_register_model.py
+-rw-r--r--   0        0        0     9399 2023-11-30 03:45:06.359056 litellm-1.9.dev0/litellm/tests/test_router.py
+-rw-r--r--   0        0        0     4991 2023-11-27 15:18:35.215142 litellm-1.9.dev0/litellm/tests/test_router_fallbacks.py
+-rw-r--r--   0        0        0     9283 2023-11-30 01:54:34.430215 litellm-1.9.dev0/litellm/tests/test_router_get_deployments.py
+-rw-r--r--   0        0        0     2749 2023-11-21 19:08:46.388212 litellm-1.9.dev0/litellm/tests/test_rules.py
+-rw-r--r--   0        0        0     3148 2023-11-30 16:52:06.592685 litellm-1.9.dev0/litellm/tests/test_stream_chunk_builder.py
+-rw-r--r--   0        0        0    47035 2023-11-30 03:58:12.053267 litellm-1.9.dev0/litellm/tests/test_streaming.py
+-rw-r--r--   0        0        0     2075 2023-11-18 01:46:31.923500 litellm-1.9.dev0/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0    19400 2023-11-21 16:22:19.466245 litellm-1.9.dev0/litellm/tests/test_text_completion.py
+-rw-r--r--   0        0        0     1758 2023-11-21 21:48:29.067833 litellm-1.9.dev0/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0     2589 2023-11-11 20:13:36.148586 litellm-1.9.dev0/litellm/tests/test_token_counter.py
+-rw-r--r--   0        0        0     9294 2023-11-13 16:02:29.770766 litellm-1.9.dev0/litellm/tests/test_utils.py
+-rw-r--r--   0        0        0      296 2023-09-25 14:33:24.288928 litellm-1.9.dev0/litellm/tests/test_validate_environment.py
+-rw-r--r--   0        0        0     1832 2023-11-21 03:08:53.292279 litellm-1.9.dev0/litellm/tests/test_wandb.py
+-rw-r--r--   0        0        0      208 2023-09-11 18:57:49.439877 litellm-1.9.dev0/litellm/tests/user_cost.json
+-rw-r--r--   0        0        0     4315 2023-11-16 22:30:31.556562 litellm-1.9.dev0/litellm/timeout.py
+-rw-r--r--   0        0        0   271994 2023-11-30 21:50:47.775692 litellm-1.9.dev0/litellm/utils.py
+-rw-r--r--   0        0        0      669 2023-11-30 22:17:08.788822 litellm-1.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0      137 2023-11-29 01:49:53.320534 litellm-1.9.dev0/requirements.txt
+-rw-r--r--   0        0        0    11190 1970-01-01 00:00:00.000000 litellm-1.9.dev0/PKG-INFO
```

### Comparing `litellm-1.9.5/LICENSE` & `litellm-1.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/README.md` & `litellm-1.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/__init__.py` & `litellm-1.9.dev0/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/budget_manager.py` & `litellm-1.9.dev0/litellm/budget_manager.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/caching.py` & `litellm-1.9.dev0/litellm/caching.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/deprecated_litellm_server/.env.template` & `litellm-1.9.dev0/litellm/deprecated_litellm_server/.env.template`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/deprecated_litellm_server/main.py` & `litellm-1.9.dev0/litellm/deprecated_litellm_server/main.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/deprecated_litellm_server/server_utils.py` & `litellm-1.9.dev0/litellm/deprecated_litellm_server/server_utils.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/exceptions.py` & `litellm-1.9.dev0/litellm/exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/aispend.py` & `litellm-1.9.dev0/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/berrispend.py` & `litellm-1.9.dev0/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/custom_logger.py` & `litellm-1.9.dev0/litellm/integrations/custom_logger.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/helicone.py` & `litellm-1.9.dev0/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/langfuse.py` & `litellm-1.9.dev0/litellm/integrations/langfuse.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/langsmith.py` & `litellm-1.9.dev0/litellm/integrations/langsmith.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/litedebugger.py` & `litellm-1.9.dev0/litellm/integrations/litedebugger.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/llmonitor.py` & `litellm-1.9.dev0/litellm/integrations/llmonitor.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/prompt_layer.py` & `litellm-1.9.dev0/litellm/integrations/prompt_layer.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/supabase.py` & `litellm-1.9.dev0/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/traceloop.py` & `litellm-1.9.dev0/litellm/integrations/traceloop.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/integrations/weights_biases.py` & `litellm-1.9.dev0/litellm/integrations/weights_biases.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/ai21.py` & `litellm-1.9.dev0/litellm/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/aleph_alpha.py` & `litellm-1.9.dev0/litellm/llms/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/anthropic.py` & `litellm-1.9.dev0/litellm/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/azure.py` & `litellm-1.9.dev0/litellm/llms/azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,37 +114,36 @@
             if model is None or messages is None:
                 raise AzureOpenAIError(status_code=422, message=f"Missing model or messages")
             
             max_retries = optional_params.pop("max_retries", 2)
 
             ### CHECK IF CLOUDFLARE AI GATEWAY ###
             ### if so - set the model as part of the base url 
-            if "gateway.ai.cloudflare.com" in api_base: 
+            if "gateway.ai.cloudflare.com" in api_base and client is None: 
                 ## build base url - assume api base includes resource name
-                if client is None:
-                    if not api_base.endswith("/"): 
-                        api_base += "/"
-                    api_base += f"{model}"
-                    
-                    azure_client_params = {
-                        "api_version": api_version,
-                        "base_url": f"{api_base}",
-                        "http_client": litellm.client_session,
-                        "max_retries": max_retries,
-                        "timeout": timeout
-                    }
-                    if api_key is not None:
-                        azure_client_params["api_key"] = api_key
-                    elif azure_ad_token is not None:
-                        azure_client_params["azure_ad_token"] = azure_ad_token
+                if not api_base.endswith("/"): 
+                    api_base += "/"
+                api_base += f"{model}"
+                
+                azure_client_params = {
+                    "api_version": api_version,
+                    "base_url": f"{api_base}",
+                    "http_client": litellm.client_session,
+                    "max_retries": max_retries,
+                    "timeout": timeout
+                }
+                if api_key is not None:
+                    azure_client_params["api_key"] = api_key
+                elif azure_ad_token is not None:
+                    azure_client_params["azure_ad_token"] = azure_ad_token
 
-                    if acompletion is True:
-                        client = AsyncAzureOpenAI(**azure_client_params)
-                    else:
-                        client = AzureOpenAI(**azure_client_params)
+                if acompletion is True:
+                    client = AsyncAzureOpenAI(**azure_client_params)
+                else:
+                    client = AzureOpenAI(**azure_client_params)
                 
                 data = {
                     "model": None,
                     "messages": messages, 
                     **optional_params
                 }
             else:
```

### Comparing `litellm-1.9.5/litellm/llms/base.py` & `litellm-1.9.dev0/litellm/llms/base.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/baseten.py` & `litellm-1.9.dev0/litellm/llms/baseten.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/bedrock.py` & `litellm-1.9.dev0/litellm/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/cohere.py` & `litellm-1.9.dev0/litellm/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/huggingface_llms_metadata/hf_conversational_models.txt` & `litellm-1.9.dev0/litellm/llms/huggingface_llms_metadata/hf_conversational_models.txt`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/huggingface_llms_metadata/hf_text_generation_models.txt` & `litellm-1.9.dev0/litellm/llms/huggingface_llms_metadata/hf_text_generation_models.txt`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/huggingface_restapi.py` & `litellm-1.9.dev0/litellm/llms/huggingface_restapi.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/maritalk.py` & `litellm-1.9.dev0/litellm/llms/maritalk.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/nlp_cloud.py` & `litellm-1.9.dev0/litellm/llms/nlp_cloud.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/ollama.py` & `litellm-1.9.dev0/litellm/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/oobabooga.py` & `litellm-1.9.dev0/litellm/llms/oobabooga.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/openai.py` & `litellm-1.9.dev0/litellm/llms/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
         response = None
         try: 
             if client is None:
                 openai_aclient = AsyncOpenAI(api_key=api_key, base_url=api_base, http_client=litellm.aclient_session, timeout=timeout, max_retries=max_retries)
             else:
                 openai_aclient = client
             response = await openai_aclient.embeddings.create(**data) # type: ignore
-            return response
+            return convert_to_model_response_object(response_object=json.loads(response.model_dump_json()), model_response_object=model_response, response_type="embedding")
         except Exception as e:
             raise e
     def embedding(self,
                 model: str,
                 input: list,
                 timeout: float, 
                 api_key: Optional[str] = None,
```

### Comparing `litellm-1.9.5/litellm/llms/palm.py` & `litellm-1.9.dev0/litellm/llms/palm.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/petals.py` & `litellm-1.9.dev0/litellm/llms/petals.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/prompt_templates/factory.py` & `litellm-1.9.dev0/litellm/llms/prompt_templates/factory.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/replicate.py` & `litellm-1.9.dev0/litellm/llms/replicate.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/sagemaker.py` & `litellm-1.9.dev0/litellm/llms/sagemaker.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/together_ai.py` & `litellm-1.9.dev0/litellm/llms/together_ai.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/tokenizers/anthropic_tokenizer.json` & `litellm-1.9.dev0/litellm/llms/tokenizers/anthropic_tokenizer.json`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/vertex_ai.py` & `litellm-1.9.dev0/litellm/llms/vertex_ai.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/llms/vllm.py` & `litellm-1.9.dev0/litellm/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/main.py` & `litellm-1.9.dev0/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/model_prices_and_context_window_backup.json` & `litellm-1.9.dev0/litellm/model_prices_and_context_window_backup.json`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/README.md` & `litellm-1.9.dev0/litellm/proxy/README.md`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/config.yaml` & `litellm-1.9.dev0/litellm/proxy/config.yaml`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/example_config_yaml/aliases_config.yaml` & `litellm-1.9.dev0/litellm/proxy/example_config_yaml/aliases_config.yaml`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/example_config_yaml/load_balancer.yaml` & `litellm-1.9.dev0/litellm/proxy/example_config_yaml/load_balancer.yaml`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/openapi.json` & `litellm-1.9.dev0/litellm/proxy/openapi.json`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/proxy_cli.py` & `litellm-1.9.dev0/litellm/proxy/proxy_cli.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/proxy_server.py` & `litellm-1.9.dev0/litellm/proxy/proxy_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 import sys, os, platform, time, copy, re, asyncio
 import threading, ast
 import shutil, random, traceback, requests
 from datetime import datetime, timedelta
 from typing import Optional, List
 import secrets, subprocess
-import warnings
 messages: list = []
 sys.path.insert(
     0, os.path.abspath("../..")
 )  # Adds the parent directory to the system path - for litellm local dev
 
 try:
     import uvicorn
     import fastapi
     import appdirs
     import backoff
     import yaml
     import rq
-    import orjson
 except ImportError:
     import sys
 
     subprocess.check_call(
         [
             sys.executable,
             "-m",
             "pip",
             "install",
             "uvicorn",
             "fastapi",
             "appdirs",
             "backoff",
             "pyyaml", 
-            "rq",
-            "orjson"
+            "rq"
         ]
     )
     import uvicorn
     import fastapi
     import appdirs
     import backoff
     import yaml
-    import orjson
-
-    warnings.warn(
-        "Installed runtime dependencies for proxy server. Specify these dependencies explicitly with `pip install litellm[proxy]`"
-    )
 
 import random
 
 list_of_messages = [
     "'The thing I wish you improved is...'",
     "'A feature I really want is...'",
     "'The worst thing about this product is...'",
@@ -90,73 +82,33 @@
 
 import litellm
 from litellm.caching import DualCache
 litellm.suppress_debug_info = True
 from fastapi import FastAPI, Request, HTTPException, status, Depends
 from fastapi.routing import APIRouter
 from fastapi.encoders import jsonable_encoder
-from fastapi.responses import StreamingResponse, FileResponse, ORJSONResponse
+from fastapi.responses import StreamingResponse, FileResponse
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.security.api_key import APIKeyHeader
 import json
 import logging
-from typing import Union
 # from litellm.proxy.queue import start_rq_worker_in_background
 
 app = FastAPI(docs_url="/", title="LiteLLM API")
 router = APIRouter()
 origins = ["*"]
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
-
-from typing import Dict
-from pydantic import BaseModel         
-######### Request Class Definition ######
-class ProxyChatCompletionRequest(BaseModel):
-    model: str
-    messages: List[Dict[str, str]]
-    temperature: Optional[float] = None
-    top_p: Optional[float] = None
-    n: Optional[int] = None
-    stream: Optional[bool] = None
-    stop: Optional[List[str]] = None
-    max_tokens: Optional[int] = None
-    presence_penalty: Optional[float] = None
-    frequency_penalty: Optional[float] = None
-    logit_bias: Optional[Dict[str, float]] = None
-    user: Optional[str] = None
-    response_format: Optional[Dict[str, str]] = None
-    seed: Optional[int] = None
-    tools: Optional[List[str]] = None
-    tool_choice: Optional[str] = None
-    functions: Optional[List[str]] = None  # soon to be deprecated
-    function_call: Optional[str] = None # soon to be deprecated
-
-    # Optional LiteLLM params
-    caching: Optional[bool] = None
-    api_base: Optional[str] = None
-    api_version: Optional[str] = None
-    api_key: Optional[str] = None
-    num_retries: Optional[int] = None
-    context_window_fallback_dict: Optional[Dict[str, str]] = None
-    fallbacks: Optional[List[str]] = None
-    metadata: Optional[Dict[str, str]] = {}
-    deployment_id: Optional[str] = None
-    request_timeout: Optional[int] = None
-
-    class Config:
-        extra='allow' # allow params not defined here, these fall in litellm.completion(**kwargs)
-
 user_api_base = None
 user_model = None
 user_debug = False
 user_max_tokens = None
 user_request_timeout = None
 user_temperature = None
 user_telemetry = True
@@ -212,26 +164,27 @@
         
         if (route == "/key/generate" or route == "/key/delete" or route == "/key/info") and not is_master_key_valid:
             raise Exception(f"If master key is set, only master key can be used to generate, delete or get info for new keys")
 
         if prisma_client: 
             ## check for cache hit (In-Memory Cache)
             valid_token = user_api_key_cache.get_cache(key=api_key)
-            if valid_token is None and "Bearer " in api_key: 
+            if valid_token is None: 
                 ## check db 
-                cleaned_api_key = api_key[len("Bearer "):]
+                if "Bearer " in api_key:
+                    cleaned_api_key = api_key[len("Bearer "):]
                 valid_token = await prisma_client.litellm_verificationtoken.find_first(
                     where={
                         "token": cleaned_api_key,
                         "expires": {"gte": datetime.utcnow()}  # Check if the token is not expired
                     }
                 )
                 ## save to cache for 60s
                 user_api_key_cache.set_cache(key=api_key, value=valid_token, ttl=60)
-            elif valid_token is not None: 
+            else: 
                 print(f"API Key Cache Hit!")
             if valid_token:
                 litellm.model_alias_map = valid_token.aliases
                 config = valid_token.config
                 if config != {}:
                     model_list = config.get("model_list", [])
                     llm_model_list =  model_list
@@ -722,19 +675,15 @@
             or user_model # model name passed via cli args
             or model # for azure deployments
             or data["model"] # default passed in http request
         )
         if user_model:
             data["model"] = user_model
         data["call_type"] = "text_completion"
-        if "metadata" in data:
-            data["metadata"]["user_api_key"] = user_api_key_dict["api_key"]
-        else:
-            data["metadata"] = {"user_api_key": user_api_key_dict["api_key"]}
-
+        data["metadata"] = {"user_api_key": user_api_key_dict["api_key"]}
         return litellm_completion(
             **data
         )
     except Exception as e: 
         print(f"\033[1;31mAn error occurred: {e}\n\n Debug this by setting `--debug`, e.g. `litellm --model gpt-3.5-turbo --debug`")
         error_traceback = traceback.format_exc()
         error_msg = f"{str(e)}\n\n{error_traceback}"
@@ -742,38 +691,36 @@
             status = e.status_code  # type: ignore
         except:
             status = 500
         raise HTTPException(
             status_code=status,
             detail=error_msg
         )
+                              
 
-
-@router.post("/v1/chat/completions", dependencies=[Depends(user_api_key_auth)], tags=["chat/completions"])
-@router.post("/chat/completions", dependencies=[Depends(user_api_key_auth)], tags=["chat/completions"])
-@router.post("/openai/deployments/{model:path}/chat/completions", dependencies=[Depends(user_api_key_auth)], tags=["chat/completions"]) # azure compatible endpoint
-async def chat_completion(request: ProxyChatCompletionRequest, model: Optional[str] = None, user_api_key_dict: dict = Depends(user_api_key_auth)):
+@router.post("/v1/chat/completions", dependencies=[Depends(user_api_key_auth)])
+@router.post("/chat/completions", dependencies=[Depends(user_api_key_auth)])
+@router.post("/openai/deployments/{model:path}/chat/completions", dependencies=[Depends(user_api_key_auth)]) # azure compatible endpoint
+async def chat_completion(request: Request, model: Optional[str] = None, user_api_key_dict: dict = Depends(user_api_key_auth)):
     global general_settings, user_debug
     try: 
-        data = {}
-        request_items = request.dict() # type: ignore 
-        data = {key: value for key, value in request_items.items() if value is not None} # pydantic sets all values to None, filter out None values here
-        
+        body = await request.body()
+        body_str = body.decode()
+        try:
+            data = ast.literal_eval(body_str)
+        except: 
+            data = json.loads(body_str)
         print_verbose(f"receiving data: {data}")
         data["model"] = (
             general_settings.get("completion_model", None) # server default
             or user_model # model name passed via cli args
             or model # for azure deployments
             or data["model"] # default passed in http request
         )
-
-        if "metadata" in data:
-            data["metadata"]["user_api_key"] = user_api_key_dict["api_key"]
-        else:
-            data["metadata"] = {"user_api_key": user_api_key_dict["api_key"]}
+        data["metadata"] = {"user_api_key": user_api_key_dict["api_key"]}
 
         global user_temperature, user_request_timeout, user_max_tokens, user_api_base
         # override with user settings, these are params passed via cli
         if user_temperature: 
             data["temperature"] = user_temperature
         if user_request_timeout:
             data["request_timeout"] = user_request_timeout
@@ -787,16 +734,15 @@
         else: 
             response = await litellm.acompletion(**data)
         if 'stream' in data and data['stream'] == True: # use generate_responses to stream responses
             return StreamingResponse(async_data_generator(response), media_type='text/event-stream')
         return response
     except Exception as e: 
         print(f"\033[1;31mAn error occurred: {e}\n\n Debug this by setting `--debug`, e.g. `litellm --model gpt-3.5-turbo --debug`")
-        router_model_names = [m["model_name"] for m in llm_model_list] if llm_model_list is not None else []
-        if llm_router is not None and data.get("model", "") in router_model_names: 
+        if llm_router is not None and data["model"] in router_model_names: 
             print("Results from router")
             print("\nRouter stats")
             print("\nTotal Calls made")
             for key, value in llm_router.total_calls.items():
                 print(f"{key}: {value}")
             print("\nSuccess Calls made")
             for key, value in llm_router.success_calls.items():
@@ -813,35 +759,28 @@
         except:
             status = 500
         raise HTTPException(
             status_code=status,
             detail=error_msg
         )
 
-@router.post("/v1/embeddings", dependencies=[Depends(user_api_key_auth)], response_class=ORJSONResponse)
-@router.post("/embeddings", dependencies=[Depends(user_api_key_auth)], response_class=ORJSONResponse)
+@router.post("/v1/embeddings", dependencies=[Depends(user_api_key_auth)])
+@router.post("/embeddings", dependencies=[Depends(user_api_key_auth)])
 async def embeddings(request: Request, user_api_key_dict: dict = Depends(user_api_key_auth)): 
     try: 
-
-        # Use orjson to parse JSON data, orjson speeds up requests significantly
-        body = await request.body()
-        data = orjson.loads(body)
-
+        data = await request.json()
+        print_verbose(f"data: {data}")
         data["model"] = (
             general_settings.get("embedding_model", None) # server default
             or user_model # model name passed via cli args
             or data["model"] # default passed in http request
         )
         if user_model:
             data["model"] = user_model
-        if "metadata" in data:
-            data["metadata"]["user_api_key"] = user_api_key_dict["api_key"]
-        else:
-            data["metadata"] = {"user_api_key": user_api_key_dict["api_key"]}
-
+        data["metadata"] = {"user_api_key": user_api_key_dict["api_key"]}
         ## ROUTE TO CORRECT ENDPOINT ##
         router_model_names = [m["model_name"] for m in llm_model_list] if llm_model_list is not None else []
         if llm_router is not None and data["model"] in router_model_names: # model in router model list 
             response = await llm_router.aembedding(**data)
         else:
             response = await litellm.aembedding(**data)
         return response
```

### Comparing `litellm-1.9.5/litellm/proxy/queue/celery_app.py` & `litellm-1.9.dev0/litellm/proxy/queue/celery_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 # Celery task
 @celery_app.task(name='process_job', max_retries=3)
 def process_job(*args, **kwargs):
     try: 
         llm_router: litellm.Router = litellm.Router(model_list=kwargs.pop("llm_model_list"))
-        response = llm_router.completion(*args, **kwargs) # type: ignore
+        response = llm_router.completion(*args, **kwargs)
         if isinstance(response, litellm.ModelResponse): 
             response = response.model_dump_json()
             return json.loads(response)
         return str(response)
     except Exception as e: 
         raise e
```

### Comparing `litellm-1.9.5/litellm/proxy/queue/rq_worker.py` & `litellm-1.9.dev0/litellm/proxy/queue/rq_worker.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/tests/bursty_load_test_completion.py` & `litellm-1.9.dev0/litellm/proxy/tests/bursty_load_test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/tests/load_test_completion.py` & `litellm-1.9.dev0/litellm/proxy/tests/load_test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/tests/load_test_embedding.py` & `litellm-1.9.dev0/litellm/proxy/tests/load_test_embedding.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/tests/load_test_embedding_proxy.py` & `litellm-1.9.dev0/litellm/proxy/tests/load_test_embedding_proxy.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/tests/load_test_q.py` & `litellm-1.9.dev0/litellm/proxy/tests/load_test_q.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/tests/test_async.py` & `litellm-1.9.dev0/litellm/proxy/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/tests/test_proxy_exception_mapping.py` & `litellm-1.9.dev0/litellm/proxy/tests/test_proxy_exception_mapping.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/tests/test_q.py` & `litellm-1.9.dev0/litellm/proxy/tests/test_q.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/proxy/utils.py` & `litellm-1.9.dev0/litellm/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/router.py` & `litellm-1.9.dev0/litellm/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,18 +407,15 @@
             original_exception = e
             ### CHECK IF RATE LIMIT / CONTEXT WINDOW ERROR w/ fallbacks available
             if ((isinstance(original_exception, litellm.ContextWindowExceededError) and context_window_fallbacks is None) 
                 or (isinstance(original_exception, openai.RateLimitError) and fallbacks is not None)): 
                 raise original_exception
             ### RETRY
             #### check if it should retry + back-off if required
-            if "No models available" in str(e): 
-                timeout = litellm._calculate_retry_after(remaining_retries=num_retries, max_retries=num_retries)
-                await asyncio.sleep(timeout)
-            elif hasattr(original_exception, "status_code") and hasattr(original_exception, "response") and litellm._should_retry(status_code=original_exception.status_code):
+            if hasattr(original_exception, "status_code") and hasattr(original_exception, "response") and litellm._should_retry(status_code=original_exception.status_code):
                 if hasattr(original_exception.response, "headers"):
                     timeout = litellm._calculate_retry_after(remaining_retries=num_retries, max_retries=num_retries, response_headers=original_exception.response.headers)
                 else:
                     timeout = litellm._calculate_retry_after(remaining_retries=num_retries, max_retries=num_retries)
                 await asyncio.sleep(timeout)
             else: 
                 raise original_exception
@@ -429,23 +426,21 @@
                     # if the function call is successful, no exception will be raised and we'll break out of the loop
                     response = await original_function(*args, **kwargs)
                     if inspect.iscoroutinefunction(response): # async errors are often returned as coroutines 
                         response = await response
                     return response
                 
                 except Exception as e: 
-                    remaining_retries = num_retries - current_attempt
-                    if "No models available" in str(e): 
-                        timeout = litellm._calculate_retry_after(remaining_retries=remaining_retries, max_retries=num_retries, min_timeout=1)
-                        await asyncio.sleep(timeout)
-                    elif hasattr(e, "status_code") and hasattr(e, "response") and litellm._should_retry(status_code=e.status_code):
+                    if hasattr(e, "status_code") and hasattr(e, "response") and litellm._should_retry(status_code=e.status_code):
+                        remaining_retries = num_retries - current_attempt
                         if hasattr(e.response, "headers"):
-                            timeout = litellm._calculate_retry_after(remaining_retries=remaining_retries, max_retries=num_retries, response_headers=e.response.headers)
+                            timeout = litellm._calculate_retry_after(remaining_retries=num_retries, max_retries=num_retries, response_headers=e.response.headers)
                         else:
-                            timeout = litellm._calculate_retry_after(remaining_retries=remaining_retries, max_retries=num_retries)
+                            timeout = litellm._calculate_retry_after(remaining_retries=num_retries, max_retries=num_retries)
+                        timeout = litellm._calculate_retry_after(remaining_retries=remaining_retries, max_retries=num_retries)
                         await asyncio.sleep(timeout)
                     else: 
                         raise e
             raise original_exception
     
     def function_with_fallbacks(self, *args, **kwargs): 
         """
@@ -857,40 +852,24 @@
                 if api_version and api_version.startswith("os.environ/"):
                     api_version_env_name = api_version.replace("os.environ/", "")
                     api_version = os.getenv(api_version_env_name)
                 self.print_verbose(f"Initializing OpenAI Client for {model_name}, {str(api_base)}")
                 if "azure" in model_name:
                     if api_version is None:
                         api_version = "2023-07-01-preview"
-                    if "gateway.ai.cloudflare.com" in api_base: 
-                        if not api_base.endswith("/"): 
-                            api_base += "/"
-                        azure_model = model_name.replace("azure/", "")
-                        api_base += f"{azure_model}"
-                        model["async_client"] = openai.AsyncAzureOpenAI(
-                            api_key=api_key,
-                            base_url=api_base,
-                            api_version=api_version
-                        )
-                        model["client"] = openai.AzureOpenAI(
-                            api_key=api_key,
-                            base_url=api_base,
-                            api_version=api_version
-                        )
-                    else:
-                        model["async_client"] = openai.AsyncAzureOpenAI(
-                            api_key=api_key,
-                            azure_endpoint=api_base,
-                            api_version=api_version
-                        )
-                        model["client"] = openai.AzureOpenAI(
-                            api_key=api_key,
-                            azure_endpoint=api_base,
-                            api_version=api_version
-                        )
+                    model["async_client"] = openai.AsyncAzureOpenAI(
+                        api_key=api_key,
+                        azure_endpoint=api_base,
+                        api_version=api_version
+                    )
+                    model["client"] = openai.AzureOpenAI(
+                        api_key=api_key,
+                        azure_endpoint=api_base,
+                        api_version=api_version
+                    )
                 else:
                     model["async_client"] = openai.AsyncOpenAI(
                         api_key=api_key,
                         base_url=api_base,
                     )
                     model["client"] = openai.OpenAI(
                         api_key=api_key,
```

### Comparing `litellm-1.9.5/litellm/tests/api_log.json` & `litellm-1.9.dev0/litellm/tests/api_log.json`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/data_map.txt` & `litellm-1.9.dev0/litellm/tests/data_map.txt`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_acooldowns_router.py` & `litellm-1.9.dev0/litellm/tests/test_acooldowns_router.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_add_function_to_prompt.py` & `litellm-1.9.dev0/litellm/tests/test_add_function_to_prompt.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_async_fn.py` & `litellm-1.9.dev0/litellm/tests/test_async_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,26 +61,25 @@
 def test_async_response_azure():
     import asyncio
     litellm.set_verbose = True
     async def test_get_response():
         user_message = "What do you know?"
         messages = [{"content": user_message, "role": "user"}]
         try:
-            response = await acompletion(model="azure/gpt-turbo", messages=messages, base_url=os.getenv("CLOUDFLARE_AZURE_BASE_URL"), api_key=os.getenv("AZURE_FRANCE_API_KEY"))
+            response = await acompletion(model="azure/chatgpt-v-2", messages=messages, timeout=5)
             print(f"response: {response}")
         except litellm.Timeout as e: 
             pass
         except Exception as e:
             pytest.fail(f"An exception occurred: {e}")
 
     asyncio.run(test_get_response())
 
 # test_async_response_azure()
 
-
 def test_async_anyscale_response():
     import asyncio
     litellm.set_verbose = True
     async def test_get_response():
         user_message = "Hello, how are you?"
         messages = [{"content": user_message, "role": "user"}]
         try:
```

### Comparing `litellm-1.9.5/litellm/tests/test_bad_params.py` & `litellm-1.9.dev0/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_batch_completions.py` & `litellm-1.9.dev0/litellm/tests/test_batch_completions.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_budget_manager.py` & `litellm-1.9.dev0/litellm/tests/test_budget_manager.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_caching.py` & `litellm-1.9.dev0/litellm/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_class.py` & `litellm-1.9.dev0/litellm/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_completion.py` & `litellm-1.9.dev0/litellm/tests/test_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -863,43 +863,43 @@
         response_str = response["choices"][0]["message"]["content"]
         print("RESPONSE STRING\n", response_str)
         if type(response_str) != str:
             pytest.fail(f"Error occurred: {e}")
     except Exception as e:
         pytest.fail(f"Error occurred: {e}")
 # test_completion_replicate_vicuna()
-# commenting out - flaky test
-# def test_completion_replicate_llama2_stream():
-#     litellm.set_verbose=False
-#     model_name = "replicate/meta/llama-2-7b-chat:13c3cdee13ee059ab779f0291d29054dab00a47dad8261375654de5540165fb0"
-#     try:
-#         response = completion(
-#             model=model_name, 
-#             messages=[
-#                 {
-#                     "role": "user",
-#                     "content": "what is yc write 1 paragraph",
-#                 }
-#             ], 
-#             stream=True,
-#             max_tokens=20,
-#             num_retries=3
-#         )
-#         print(f"response: {response}")
-#         # Add any assertions here to check the response
-#         complete_response = "" 
-#         for i, chunk in enumerate(response):
-#             complete_response += chunk.choices[0].delta["content"]
-#             # if i == 0:
-#             #     assert len(chunk.choices[0].delta["content"]) > 2
-#             # print(chunk)
-#         assert len(complete_response) > 5
-#         print(f"complete_response: {complete_response}")
-#     except Exception as e:
-#         pytest.fail(f"Error occurred: {e}")
+
+def test_completion_replicate_llama2_stream():
+    litellm.set_verbose=False
+    model_name = "replicate/meta/llama-2-7b-chat:13c3cdee13ee059ab779f0291d29054dab00a47dad8261375654de5540165fb0"
+    try:
+        response = completion(
+            model=model_name, 
+            messages=[
+                {
+                    "role": "user",
+                    "content": "what is yc write 1 paragraph",
+                }
+            ], 
+            stream=True,
+            max_tokens=20,
+            num_retries=3
+        )
+        print(f"response: {response}")
+        # Add any assertions here to check the response
+        complete_response = "" 
+        for i, chunk in enumerate(response):
+            complete_response += chunk.choices[0].delta["content"]
+            # if i == 0:
+            #     assert len(chunk.choices[0].delta["content"]) > 2
+            # print(chunk)
+        assert len(complete_response) > 5
+        print(f"complete_response: {complete_response}")
+    except Exception as e:
+        pytest.fail(f"Error occurred: {e}")
 # test_completion_replicate_llama2_stream()
 
 def test_replicate_custom_prompt_dict(): 
     litellm.set_verbose = True
     model_name = "replicate/meta/llama-2-7b-chat:13c3cdee13ee059ab779f0291d29054dab00a47dad8261375654de5540165fb0"
     litellm.register_prompt_template(
         model="replicate/meta/llama-2-7b-chat:13c3cdee13ee059ab779f0291d29054dab00a47dad8261375654de5540165fb0",
```

### Comparing `litellm-1.9.5/litellm/tests/test_completion_with_retries.py` & `litellm-1.9.dev0/litellm/tests/test_completion_with_retries.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_config.py` & `litellm-1.9.dev0/litellm/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_custom_logger.py` & `litellm-1.9.dev0/litellm/tests/test_custom_logger.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_embedding.py` & `litellm-1.9.dev0/litellm/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_exceptions.py` & `litellm-1.9.dev0/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_function_calling.py` & `litellm-1.9.dev0/litellm/tests/test_function_calling.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_get_model_cost_map.py` & `litellm-1.9.dev0/litellm/tests/test_get_model_cost_map.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_helicone_integration.py` & `litellm-1.9.dev0/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_hf_prompt_templates.py` & `litellm-1.9.dev0/litellm/tests/test_hf_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_langchain_ChatLiteLLM.py` & `litellm-1.9.dev0/litellm/tests/test_langchain_ChatLiteLLM.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_langfuse.py` & `litellm-1.9.dev0/litellm/tests/test_langfuse.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_langsmith.py` & `litellm-1.9.dev0/litellm/tests/test_langsmith.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_litellm_max_budget.py` & `litellm-1.9.dev0/litellm/tests/test_litellm_max_budget.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_llmonitor_integration.py` & `litellm-1.9.dev0/litellm/tests/test_llmonitor_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_loadtest_router.py` & `litellm-1.9.dev0/litellm/tests/test_loadtest_router.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_logging.py` & `litellm-1.9.dev0/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_mock_request.py` & `litellm-1.9.dev0/litellm/tests/test_mock_request.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_model_alias_map.py` & `litellm-1.9.dev0/litellm/tests/test_model_alias_map.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_model_response_typing/server.py` & `litellm-1.9.dev0/litellm/tests/test_model_response_typing/server.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_multiple_deployments.py` & `litellm-1.9.dev0/litellm/tests/test_multiple_deployments.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_ollama.py` & `litellm-1.9.dev0/litellm/tests/test_ollama.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_ollama_local.py` & `litellm-1.9.dev0/litellm/tests/test_ollama_local.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_prompt_factory.py` & `litellm-1.9.dev0/litellm/tests/test_prompt_factory.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_promptlayer_integration.py` & `litellm-1.9.dev0/litellm/tests/test_promptlayer_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_provider_specific_config.py` & `litellm-1.9.dev0/litellm/tests/test_provider_specific_config.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_proxy_server.py` & `litellm-1.9.dev0/litellm/tests/test_proxy_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         assert response.status_code == 200
         result = response.json()
         print(f"Received response: {result}")
     except Exception as e:
         pytest.fail("LiteLLM Proxy test failed. Exception", e)
 
 # Run the test
-test_chat_completion()
+# test_chat_completion()
 
 
 def test_chat_completion_azure():
     try:
         # Your test data
         test_data = {
             "model": "azure/chatgpt-v-2",
```

### Comparing `litellm-1.9.5/litellm/tests/test_register_model.py` & `litellm-1.9.dev0/litellm/tests/test_register_model.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_router.py` & `litellm-1.9.dev0/litellm/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_router_fallbacks.py` & `litellm-1.9.dev0/litellm/tests/test_router_fallbacks.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_router_get_deployments.py` & `litellm-1.9.dev0/litellm/tests/test_router_get_deployments.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_rules.py` & `litellm-1.9.dev0/litellm/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_stream_chunk_builder.py` & `litellm-1.9.dev0/litellm/tests/test_stream_chunk_builder.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_streaming.py` & `litellm-1.9.dev0/litellm/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_supabase_integration.py` & `litellm-1.9.dev0/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_text_completion.py` & `litellm-1.9.dev0/litellm/tests/test_text_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_timeout.py` & `litellm-1.9.dev0/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/tests/test_utils.py` & `litellm-1.9.dev0/litellm/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 
 def test_trimming_with_system_message_exceeding_max_tokens():
     # This message is 33 tokens long. The system message is 13 tokens long.
     messages = [{"role": "system", "content": "This is a short system message"}, {"role": "user", "content": "This is a medium normal message, let's say litellm is awesome."}]
     trimmed_messages = trim_messages(messages, max_tokens=12, model="gpt-4-0613")
     assert len(trimmed_messages) == 1
+    assert '..' in trimmed_messages[0]["content"]
 
 def test_trimming_should_not_change_original_messages():
     messages = [{"role": "system", "content": "This is a short system message"}, {"role": "user", "content": "This is a medium normal message, let's say litellm is awesome."}]
     messages_copy = copy.deepcopy(messages)
     trimmed_messages = trim_messages(messages, max_tokens=12, model="gpt-4-0613")
     assert(messages==messages_copy)
```

### Comparing `litellm-1.9.5/litellm/tests/test_wandb.py` & `litellm-1.9.dev0/litellm/tests/test_wandb.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/timeout.py` & `litellm-1.9.dev0/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-1.9.5/litellm/utils.py` & `litellm-1.9.dev0/litellm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,21 +51,16 @@
     Timeout,
     APIConnectionError,
     APIError,
     BudgetExceededError
 )
 from typing import cast, List, Dict, Union, Optional, Literal
 from .caching import Cache
-from concurrent.futures import ThreadPoolExecutor
-####### ENVIRONMENT VARIABLES ####################
-# Adjust to your specific application needs / system capabilities.
-MAX_THREADS = 100 
 
-# Create a ThreadPoolExecutor 
-executor = ThreadPoolExecutor(max_workers=MAX_THREADS)
+####### ENVIRONMENT VARIABLES ####################
 dotenv.load_dotenv()  # Loading env variables using dotenv
 sentry_sdk_instance = None
 capture_exception = None
 add_breadcrumb = None
 posthog = None
 slack_app = None
 alerts_channel = None
@@ -1557,46 +1552,55 @@
     return enc
 
 def decode(model: str, tokens: List[int]): 
     tokenizer_json = _select_tokenizer(model=model)
     dec = tokenizer_json["tokenizer"].decode(tokens)
     return dec
 
-def openai_token_counter(messages: Optional[list]=None, model="gpt-3.5-turbo-0613", text: Optional[str]= None):
+def openai_token_counter(messages, model="gpt-3.5-turbo-0613"):
     """
     Return the number of tokens used by a list of messages.
 
     Borrowed from https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb.
     """
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         print_verbose("Warning: model not found. Using cl100k_base encoding.")
         encoding = tiktoken.get_encoding("cl100k_base")
-    if model == "gpt-3.5-turbo-0301":
-        tokens_per_message = 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
-        tokens_per_name = -1  # if there's a name, the role is omitted
-    elif model in litellm.open_ai_chat_completion_models:
+    if model in {
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-16k-0613",
+        "gpt-4-0314",
+        "gpt-4-32k-0314",
+        "gpt-4-0613",
+        "gpt-4-32k-0613",
+        }:
         tokens_per_message = 3
         tokens_per_name = 1
+    elif model == "gpt-3.5-turbo-0301":
+        tokens_per_message = 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
+        tokens_per_name = -1  # if there's a name, the role is omitted
+    elif "gpt-3.5-turbo" in model:
+        print_verbose("Warning: gpt-3.5-turbo may update over time. Returning num tokens assuming gpt-3.5-turbo-0613.")
+        return openai_token_counter(messages, model="gpt-3.5-turbo-0613")
+    elif "gpt-4" in model:
+        print_verbose("Warning: gpt-4 may update over time. Returning num tokens assuming gpt-4-0613.")
+        return openai_token_counter(messages, model="gpt-4-0613")
     else:
         raise NotImplementedError(
             f"""num_tokens_from_messages() is not implemented for model {model}. See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens."""
         )
     num_tokens = 0
-
-    if text: 
-        num_tokens = len(encoding.encode(text, disallowed_special=()))
-    elif messages: 
-        for message in messages:
-            num_tokens += tokens_per_message
-            for key, value in message.items():
-                num_tokens += len(encoding.encode(value, disallowed_special=()))
-                if key == "name":
-                    num_tokens += tokens_per_name
+    for message in messages:
+        num_tokens += tokens_per_message
+        for key, value in message.items():
+            num_tokens += len(encoding.encode(value))
+            if key == "name":
+                num_tokens += tokens_per_name
     num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
     return num_tokens
 
 def token_counter(model="", text=None,  messages: Optional[List] = None):
     """
     Count the number of tokens in a given text using a specified model.
 
@@ -1608,34 +1612,27 @@
     Returns:
     int: The number of tokens in the text.
     """
     # use tiktoken, anthropic, cohere or llama2's tokenizer depending on the model
     if text == None:
         if messages is not None:
             print_verbose(f"token_counter messages received: {messages}")
-            text = "" 
-            for message in messages: 
-                if message.get("content", None):
-                    text += message["content"]
-                if 'tool_calls' in message:
-                    for tool_call in message['tool_calls']:
-                        if 'function' in tool_call:
-                            function_arguments = tool_call['function']['arguments']
-                            text += function_arguments
+            text = "".join([message["content"] for message in messages])
         else:
             raise ValueError("text and messages cannot both be None")
     num_tokens = 0
+
     if model is not None:
         tokenizer_json = _select_tokenizer(model=model)
         if tokenizer_json["type"] == "huggingface_tokenizer": 
             enc = tokenizer_json["tokenizer"].encode(text)
             num_tokens = len(enc.ids)
         elif tokenizer_json["type"] == "openai_tokenizer": 
-            if model in litellm.open_ai_chat_completion_models:
-                num_tokens = openai_token_counter(text=text, model=model)
+            if model in litellm.open_ai_chat_completion_models and messages != None:
+                num_tokens = openai_token_counter(messages, model=model)
             else:
                 enc = tokenizer_json["tokenizer"].encode(text)
                 num_tokens = len(enc)
     else:
         num_tokens = len(encoding.encode(text))
     return num_tokens
 
@@ -3494,15 +3491,15 @@
 
     # Retry internal errors.
     if status_code >= 500:
         return True
 
     return False
 
-def _calculate_retry_after(remaining_retries: int, max_retries: int, response_headers: Optional[httpx.Headers]=None, min_timeout: int = 0):
+def _calculate_retry_after(remaining_retries: int, max_retries: int, response_headers: Optional[httpx.Headers]=None):
     """
     Reimplementation of openai's calculate retry after, since that one can't be imported.
     https://github.com/openai/openai-python/blob/af67cfab4210d8e497c05390ce14f39105c77519/src/openai/_base_client.py#L631
     """
     try:
         import email # openai import
         # About the Retry-After header: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After
@@ -3536,15 +3533,15 @@
 
     # Apply exponential backoff, but not more than the max.
     sleep_seconds = min(initial_retry_delay * pow(2.0, nb_retries), max_retry_delay)
 
     # Apply some jitter, plus-or-minus half a second.
     jitter = 1 - 0.25 * random.random()
     timeout = sleep_seconds * jitter
-    return timeout if timeout >= min_timeout else min_timeout
+    return timeout if timeout >= 0 else 0
 
 # integration helper function
 def modify_integration(integration_name, integration_params):
     global supabaseClient
     if integration_name == "supabase":
         if "table_name" in integration_params:
             Supabase.supabase_table_name = integration_params["table_name"]
@@ -4639,16 +4636,15 @@
 ####### CRASH REPORTING ################
 def safe_crash_reporting(model=None, exception=None, custom_llm_provider=None):
     data = {
         "model": model,
         "exception": str(exception),
         "custom_llm_provider": custom_llm_provider,
     }
-    executor.submit(litellm_telemetry, data)
-    # threading.Thread(target=litellm_telemetry, args=(data,), daemon=True).start()
+    threading.Thread(target=litellm_telemetry, args=(data,), daemon=True).start()
 
 def get_or_generate_uuid():
     temp_dir = os.path.join(os.path.abspath(os.sep), "tmp")
     uuid_file =  os.path.join(temp_dir, "litellm_uuid.txt")
     try:
         # Try to open the file and load the UUID
         with open(uuid_file, "r") as file:
@@ -4707,14 +4703,15 @@
             json=payload,
         )
         response.raise_for_status()  # Raise an exception for HTTP errors
     except:
         # [Non-Blocking Error]
         return
 
+
 ######### Secret Manager ############################
 # checks if user has passed in a secret manager client
 # if passed in then checks the secret there
 def get_secret(secret_name):
     if litellm.secret_manager_client != None:
         # TODO: check which secret manager is being used
         # currently only supports Infisical
```

### Comparing `litellm-1.9.5/pyproject.toml` & `litellm-1.9.dev0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litellm"
-version = "1.9.5"
+version = "1.9.dev0"
 description = "Library to easily interface with LLM API providers"
 authors = ["BerriAI"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -15,34 +15,20 @@
 tokenizers = "*"
 click = "*"
 jinja2 = "^3.1.2"
 certifi = "^2023.7.22"
 appdirs = "^1.4.4"
 aiohttp = "*"
 
-uvicorn = {version = "^0.24.0.post1", optional = true}
-fastapi = {version = "^0.104.1", optional = true}
-backoff = {version = "*", optional = true}
-rq = {version = "*", optional = true}
-
-[tool.poetry.extras]
-proxy = [
-    "uvicorn",
-    "fastapi",
-    "backoff",
-    "rq",
-    "orjson",
-]
-
 [tool.poetry.scripts]
 litellm = 'litellm:run_server'
 
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.commitizen]
-version = "1.9.5"
+version = "1.9.dev0"
 version_files = [
     "pyproject.toml:^version"
 ]
```

### Comparing `litellm-1.9.5/PKG-INFO` & `litellm-1.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 1.9.5
+Version: 1.9.dev0
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: proxy
 Requires-Dist: aiohttp
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: backoff ; extra == "proxy"
 Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
 Requires-Dist: click
-Requires-Dist: fastapi (>=0.104.1,<0.105.0) ; extra == "proxy"
 Requires-Dist: importlib-metadata (>=6.8.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: openai (>=1.0.0)
 Requires-Dist: python-dotenv (>=0.2.0)
-Requires-Dist: rq ; extra == "proxy"
 Requires-Dist: tiktoken (>=0.4.0)
 Requires-Dist: tokenizers
-Requires-Dist: uvicorn (>=0.24.0.post1,<0.25.0) ; extra == "proxy"
 Description-Content-Type: text/markdown
 
 <h1 align="center">
         🚅 LiteLLM
     </h1>
     <p align="center">
         <p align="center">Call all LLM APIs using the OpenAI format [Bedrock, Huggingface, Cohere, TogetherAI, Azure, OpenAI, etc.]
```

#### html2text {}

```diff
@@ -1,23 +1,19 @@
-Metadata-Version: 2.1 Name: litellm Version: 1.9.5 Summary: Library to easily
-interface with LLM API providers License: MIT Author: BerriAI Requires-Python:
->=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
-Extra: proxy Requires-Dist: aiohttp Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: backoff ; extra == "proxy" Requires-Dist: certifi
-(>=2023.7.22,<2024.0.0) Requires-Dist: click Requires-Dist: fastapi
-(>=0.104.1,<0.105.0) ; extra == "proxy" Requires-Dist: importlib-metadata
-(>=6.8.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0) Requires-Dist: openai
-(>=1.0.0) Requires-Dist: python-dotenv (>=0.2.0) Requires-Dist: rq ; extra ==
-"proxy" Requires-Dist: tiktoken (>=0.4.0) Requires-Dist: tokenizers Requires-
-Dist: uvicorn (>=0.24.0.post1,<0.25.0) ; extra == "proxy" Description-Content-
-Type: text/markdown
+Metadata-Version: 2.1 Name: litellm Version: 1.9.dev0 Summary: Library to
+easily interface with LLM API providers License: MIT Author: BerriAI Requires-
+Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist:
+certifi (>=2023.7.22,<2024.0.0) Requires-Dist: click Requires-Dist: importlib-
+metadata (>=6.8.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0) Requires-Dist: openai
+(>=1.0.0) Requires-Dist: python-dotenv (>=0.2.0) Requires-Dist: tiktoken
+(>=0.4.0) Requires-Dist: tokenizers Description-Content-Type: text/markdown
                           ************ ?ð??? LLiitteeLLLLMM ************
    Call all LLM APIs using the OpenAI format [Bedrock, Huggingface, Cohere,
                        TogetherAI, Azure, OpenAI, etc.]
                        ****** _OO_pp_ee_nn_AA_II_--_CC_oo_mm_pp_aa_tt_ii_bb_ll_ee_ _SS_ee_rr_vv_ee_rr ******
      ****** _[[_PP_yy_PP_II_ _VV_ee_rr_ss_ii_oo_nn_]]_[[_CC_ii_rr_cc_ll_ee_CC_II_]]_[[_YY_ _CC_oo_mm_bb_ii_nn_aa_tt_oo_rr_ _WW_22_33_]]_[[_WW_hh_aa_tt_ss_aa_pp_pp_]]_[[_DD_ii_ss_cc_oo_rr_dd_]] ******
 LiteLLM manages - Translating inputs to the provider's `completion` and
 `embedding` endpoints - Guarantees [consistent output](https://docs.litellm.ai/
```

