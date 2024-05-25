# Comparing `tmp/athena_intelligence-0.1.63.tar.gz` & `tmp/athena_intelligence-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.63.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.64.tar", max compression
```

## Comparing `athena_intelligence-0.1.63.tar` & `athena_intelligence-0.1.64.tar`

### file list

```diff
@@ -1,69 +1,72 @@
--rw-r--r--   0        0        0     4235 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/README.md
--rw-r--r--   0        0        0      603 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/pyproject.toml
--rw-r--r--   0        0        0     1739 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/__init__.py
--rw-r--r--   0        0        0     6867 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/base_client.py
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/chain/__init__.py
--rw-r--r--   0        0        0    16177 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/chain/client.py
--rw-r--r--   0        0        0     3576 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/client.py
--rw-r--r--   0        0        0      853 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1495 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6182 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12498 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6338 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6623 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/search/__init__.py
--rw-r--r--   0        0        0     7640 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0    11323 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/tools/__init__.py
--rw-r--r--   0        0        0    27502 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/tools/client.py
--rw-r--r--   0        0        0     2023 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/__init__.py
--rw-r--r--   0        0        0      994 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/dataset.py
--rw-r--r--   0        0        0     1061 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/document.py
--rw-r--r--   0        0        0      875 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/excecute_tool_first_workflow_out.py
--rw-r--r--   0        0        0     1171 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/file_data_response.py
--rw-r--r--   0        0        0     1001 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1143 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      969 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      879 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/get_snippet_out.py
--rw-r--r--   0        0        0      969 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      953 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      892 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/langchain_documents_request_out.py
--rw-r--r--   0        0        0     4238 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/llm_model.py
--rw-r--r--   0        0        0      950 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/map_reduce_chain_out.py
--rw-r--r--   0        0        0      845 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1031 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     3125 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/model.py
--rw-r--r--   0        0        0      885 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/publish_formats.py
--rw-r--r--   0        0        0      926 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/report.py
--rw-r--r--   0        0        0      879 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/researcher_out.py
--rw-r--r--   0        0        0     1106 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/snippet.py
--rw-r--r--   0        0        0      880 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      885 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1577 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/tools.py
--rw-r--r--   0        0        0      986 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/upload_documents_out.py
--rw-r--r--   0        0        0      873 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/url_result.py
--rw-r--r--   0        0        0      972 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       65 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/upload/__init__.py
--rw-r--r--   0        0        0     6385 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/upload/client.py
--rw-r--r--   0        0        0       87 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/version.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.63/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/README.md
+-rw-r--r--   0        0        0      603 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/pyproject.toml
+-rw-r--r--   0        0        0     1813 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/__init__.py
+-rw-r--r--   0        0        0     7089 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/base_client.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0    16177 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/chain/client.py
+-rw-r--r--   0        0        0     3576 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/client.py
+-rw-r--r--   0        0        0      853 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1495 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6182 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12498 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6338 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6623 2024-05-25 19:36:43.289585 athena_intelligence-0.1.64/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7640 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0    11323 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    27502 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/tools/client.py
+-rw-r--r--   0        0        0     2099 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/__init__.py
+-rw-r--r--   0        0        0      994 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1061 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/document.py
+-rw-r--r--   0        0        0      875 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1171 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/file_data_response.py
+-rw-r--r--   0        0        0     1001 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1143 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      969 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      879 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/get_snippet_out.py
+-rw-r--r--   0        0        0      969 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      953 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      892 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/langchain_documents_request_out.py
+-rw-r--r--   0        0        0     4238 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/llm_model.py
+-rw-r--r--   0        0        0      950 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/map_reduce_chain_out.py
+-rw-r--r--   0        0        0      845 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1031 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     3125 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/model.py
+-rw-r--r--   0        0        0      885 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/publish_formats.py
+-rw-r--r--   0        0        0      926 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/report.py
+-rw-r--r--   0        0        0      879 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/researcher_out.py
+-rw-r--r--   0        0        0     1106 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      880 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      885 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1577 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/tools.py
+-rw-r--r--   0        0        0      986 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/upload_documents_out.py
+-rw-r--r--   0        0        0      873 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      972 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      905 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/types/workflow_status_out.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/upload/__init__.py
+-rw-r--r--   0        0        0     6385 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/upload/client.py
+-rw-r--r--   0        0        0       87 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/version.py
+-rw-r--r--   0        0        0       65 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/workflow/__init__.py
+-rw-r--r--   0        0        0     6249 2024-05-25 19:36:43.293585 athena_intelligence-0.1.64/src/athena/workflow/client.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.64/PKG-INFO
```

### Comparing `athena_intelligence-0.1.63/README.md` & `athena_intelligence-0.1.64/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/pyproject.toml` & `athena_intelligence-0.1.64/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athena-intelligence"
-version = "0.1.63"
+version = "0.1.64"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "athena", from = "src"}
 ]
```

### Comparing `athena_intelligence-0.1.63/src/athena/__init__.py` & `athena_intelligence-0.1.64/src/athena/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,18 @@
     StatusEnum,
     StructuredParseResult,
     Tools,
     UploadDocumentsOut,
     UrlResult,
     ValidationError,
     ValidationErrorLocItem,
+    WorkflowStatusOut,
 )
 from .errors import UnprocessableEntityError
-from . import chain, dataset, message, query, report, search, snippet, tools, upload
+from . import chain, dataset, message, query, report, search, snippet, tools, upload, workflow
 from .environment import AthenaEnvironment
 from .version import __version__
 
 __all__ = [
     "AthenaEnvironment",
     "Dataset",
     "Document",
@@ -62,18 +63,20 @@
     "StructuredParseResult",
     "Tools",
     "UnprocessableEntityError",
     "UploadDocumentsOut",
     "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
+    "WorkflowStatusOut",
     "__version__",
     "chain",
     "dataset",
     "message",
     "query",
     "report",
     "search",
     "snippet",
     "tools",
     "upload",
+    "workflow",
 ]
```

### Comparing `athena_intelligence-0.1.63/src/athena/base_client.py` & `athena_intelligence-0.1.64/src/athena/base_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .message.client import AsyncMessageClient, MessageClient
 from .query.client import AsyncQueryClient, QueryClient
 from .report.client import AsyncReportClient, ReportClient
 from .search.client import AsyncSearchClient, SearchClient
 from .snippet.client import AsyncSnippetClient, SnippetClient
 from .tools.client import AsyncToolsClient, ToolsClient
 from .upload.client import AsyncUploadClient, UploadClient
+from .workflow.client import AsyncWorkflowClient, WorkflowClient
 
 
 class BaseAthena:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
@@ -69,14 +70,15 @@
         self.snippet = SnippetClient(client_wrapper=self._client_wrapper)
         self.report = ReportClient(client_wrapper=self._client_wrapper)
         self.query = QueryClient(client_wrapper=self._client_wrapper)
         self.search = SearchClient(client_wrapper=self._client_wrapper)
         self.chain = ChainClient(client_wrapper=self._client_wrapper)
         self.tools = ToolsClient(client_wrapper=self._client_wrapper)
         self.upload = UploadClient(client_wrapper=self._client_wrapper)
+        self.workflow = WorkflowClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseAthena:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
@@ -127,14 +129,15 @@
         self.snippet = AsyncSnippetClient(client_wrapper=self._client_wrapper)
         self.report = AsyncReportClient(client_wrapper=self._client_wrapper)
         self.query = AsyncQueryClient(client_wrapper=self._client_wrapper)
         self.search = AsyncSearchClient(client_wrapper=self._client_wrapper)
         self.chain = AsyncChainClient(client_wrapper=self._client_wrapper)
         self.tools = AsyncToolsClient(client_wrapper=self._client_wrapper)
         self.upload = AsyncUploadClient(client_wrapper=self._client_wrapper)
+        self.workflow = AsyncWorkflowClient(client_wrapper=self._client_wrapper)
 
 
 def _get_base_url(*, base_url: typing.Optional[str] = None, environment: AthenaEnvironment) -> str:
     if base_url is not None:
         return base_url
     elif environment is not None:
         return environment.value
```

### Comparing `athena_intelligence-0.1.63/src/athena/chain/client.py` & `athena_intelligence-0.1.64/src/athena/chain/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/client.py` & `athena_intelligence-0.1.64/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/core/__init__.py` & `athena_intelligence-0.1.64/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.64/src/athena/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.63",
+            "X-Fern-SDK-Version": "0.1.64",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.63/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.64/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/core/file.py` & `athena_intelligence-0.1.64/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/core/http_client.py` & `athena_intelligence-0.1.64/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.64/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/core/request_options.py` & `athena_intelligence-0.1.64/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/dataset/client.py` & `athena_intelligence-0.1.64/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/message/client.py` & `athena_intelligence-0.1.64/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/polling_message_client.py` & `athena_intelligence-0.1.64/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/query/client.py` & `athena_intelligence-0.1.64/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/report/client.py` & `athena_intelligence-0.1.64/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/search/client.py` & `athena_intelligence-0.1.64/src/athena/search/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/snippet/client.py` & `athena_intelligence-0.1.64/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/tools/client.py` & `athena_intelligence-0.1.64/src/athena/tools/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/__init__.py` & `athena_intelligence-0.1.64/src/athena/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .status_enum import StatusEnum
 from .structured_parse_result import StructuredParseResult
 from .tools import Tools
 from .upload_documents_out import UploadDocumentsOut
 from .url_result import UrlResult
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
+from .workflow_status_out import WorkflowStatusOut
 
 __all__ = [
     "Dataset",
     "Document",
     "ExcecuteToolFirstWorkflowOut",
     "FileDataResponse",
     "FirecrawlScrapeUrlDataReponseDto",
@@ -54,8 +55,9 @@
     "StatusEnum",
     "StructuredParseResult",
     "Tools",
     "UploadDocumentsOut",
     "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
+    "WorkflowStatusOut",
 ]
```

### Comparing `athena_intelligence-0.1.63/src/athena/types/dataset.py` & `athena_intelligence-0.1.64/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/document.py` & `athena_intelligence-0.1.64/src/athena/types/document.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/excecute_tool_first_workflow_out.py` & `athena_intelligence-0.1.64/src/athena/types/excecute_tool_first_workflow_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/file_data_response.py` & `athena_intelligence-0.1.64/src/athena/types/file_data_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.64/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.64/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.64/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/get_snippet_out.py` & `athena_intelligence-0.1.64/src/athena/types/get_snippet_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.64/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.64/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/langchain_documents_request_out.py` & `athena_intelligence-0.1.64/src/athena/types/langchain_documents_request_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/llm_model.py` & `athena_intelligence-0.1.64/src/athena/types/llm_model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/map_reduce_chain_out.py` & `athena_intelligence-0.1.64/src/athena/types/map_reduce_chain_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/message_out.py` & `athena_intelligence-0.1.64/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.64/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/model.py` & `athena_intelligence-0.1.64/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/publish_formats.py` & `athena_intelligence-0.1.64/src/athena/types/publish_formats.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/report.py` & `athena_intelligence-0.1.64/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/researcher_out.py` & `athena_intelligence-0.1.64/src/athena/types/researcher_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/snippet.py` & `athena_intelligence-0.1.64/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/sql_results.py` & `athena_intelligence-0.1.64/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/status_enum.py` & `athena_intelligence-0.1.64/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.64/src/athena/types/structured_parse_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/tools.py` & `athena_intelligence-0.1.64/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/upload_documents_out.py` & `athena_intelligence-0.1.64/src/athena/types/upload_documents_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/url_result.py` & `athena_intelligence-0.1.64/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/types/validation_error.py` & `athena_intelligence-0.1.64/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/src/athena/upload/client.py` & `athena_intelligence-0.1.64/src/athena/upload/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.63/PKG-INFO` & `athena_intelligence-0.1.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.63
+Version: 0.1.64
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

