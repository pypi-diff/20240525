# Comparing `tmp/athena_intelligence-0.1.62.tar.gz` & `tmp/athena_intelligence-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.62.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.63.tar", max compression
```

## Comparing `athena_intelligence-0.1.62.tar` & `athena_intelligence-0.1.63.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0     4235 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/README.md
--rw-r--r--   0        0        0      603 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/pyproject.toml
--rw-r--r--   0        0        0     1697 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/__init__.py
--rw-r--r--   0        0        0     6867 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/base_client.py
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/chain/__init__.py
--rw-r--r--   0        0        0    16177 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/chain/client.py
--rw-r--r--   0        0        0     3576 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/client.py
--rw-r--r--   0        0        0      853 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1495 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6182 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12498 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6338 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6623 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/search/__init__.py
--rw-r--r--   0        0        0     7640 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.504528 athena_intelligence-0.1.62/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0    11323 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/snippet/client.py
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/tools/__init__.py
--rw-r--r--   0        0        0    26539 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/tools/client.py
--rw-r--r--   0        0        0     1957 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/__init__.py
--rw-r--r--   0        0        0      994 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/dataset.py
--rw-r--r--   0        0        0     1061 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/document.py
--rw-r--r--   0        0        0      875 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/excecute_tool_first_workflow_out.py
--rw-r--r--   0        0        0     1171 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/file_data_response.py
--rw-r--r--   0        0        0     1001 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
--rw-r--r--   0        0        0     1143 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/firecrawl_scrape_url_metadata.py
--rw-r--r--   0        0        0      969 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      879 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/get_snippet_out.py
--rw-r--r--   0        0        0      969 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      953 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      892 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/langchain_documents_request_out.py
--rw-r--r--   0        0        0     4238 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/llm_model.py
--rw-r--r--   0        0        0      950 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/map_reduce_chain_out.py
--rw-r--r--   0        0        0      845 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1031 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     3125 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/model.py
--rw-r--r--   0        0        0      926 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/report.py
--rw-r--r--   0        0        0      879 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/researcher_out.py
--rw-r--r--   0        0        0     1106 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/snippet.py
--rw-r--r--   0        0        0      880 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/status_enum.py
--rw-r--r--   0        0        0      885 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/structured_parse_result.py
--rw-r--r--   0        0        0     1577 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/tools.py
--rw-r--r--   0        0        0      986 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/upload_documents_out.py
--rw-r--r--   0        0        0      873 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/url_result.py
--rw-r--r--   0        0        0      972 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       65 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/upload/__init__.py
--rw-r--r--   0        0        0     6385 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/upload/client.py
--rw-r--r--   0        0        0       87 2024-05-25 00:48:46.508528 athena_intelligence-0.1.62/src/athena/version.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.62/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/README.md
+-rw-r--r--   0        0        0      603 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/pyproject.toml
+-rw-r--r--   0        0        0     1739 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/__init__.py
+-rw-r--r--   0        0        0     6867 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/base_client.py
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/chain/__init__.py
+-rw-r--r--   0        0        0    16177 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/chain/client.py
+-rw-r--r--   0        0        0     3576 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/client.py
+-rw-r--r--   0        0        0      853 2024-05-25 18:00:14.018452 athena_intelligence-0.1.63/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1495 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6182 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12498 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6338 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6623 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/search/__init__.py
+-rw-r--r--   0        0        0     7640 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0    11323 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/snippet/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/tools/__init__.py
+-rw-r--r--   0        0        0    27502 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/tools/client.py
+-rw-r--r--   0        0        0     2023 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/__init__.py
+-rw-r--r--   0        0        0      994 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/dataset.py
+-rw-r--r--   0        0        0     1061 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/document.py
+-rw-r--r--   0        0        0      875 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/excecute_tool_first_workflow_out.py
+-rw-r--r--   0        0        0     1171 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/file_data_response.py
+-rw-r--r--   0        0        0     1001 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py
+-rw-r--r--   0        0        0     1143 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/firecrawl_scrape_url_metadata.py
+-rw-r--r--   0        0        0      969 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      879 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/get_snippet_out.py
+-rw-r--r--   0        0        0      969 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      953 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      892 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/langchain_documents_request_out.py
+-rw-r--r--   0        0        0     4238 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/llm_model.py
+-rw-r--r--   0        0        0      950 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/map_reduce_chain_out.py
+-rw-r--r--   0        0        0      845 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1031 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     3125 2024-05-25 18:00:14.022451 athena_intelligence-0.1.63/src/athena/types/model.py
+-rw-r--r--   0        0        0      885 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/publish_formats.py
+-rw-r--r--   0        0        0      926 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/report.py
+-rw-r--r--   0        0        0      879 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/researcher_out.py
+-rw-r--r--   0        0        0     1106 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      880 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0      885 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/structured_parse_result.py
+-rw-r--r--   0        0        0     1577 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/tools.py
+-rw-r--r--   0        0        0      986 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/upload_documents_out.py
+-rw-r--r--   0        0        0      873 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      972 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       65 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/upload/__init__.py
+-rw-r--r--   0        0        0     6385 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/upload/client.py
+-rw-r--r--   0        0        0       87 2024-05-25 18:00:14.026451 athena_intelligence-0.1.63/src/athena/version.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.63/PKG-INFO
```

### Comparing `athena_intelligence-0.1.62/README.md` & `athena_intelligence-0.1.63/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/pyproject.toml` & `athena_intelligence-0.1.63/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athena-intelligence"
-version = "0.1.62"
+version = "0.1.63"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "athena", from = "src"}
 ]
```

### Comparing `athena_intelligence-0.1.62/src/athena/__init__.py` & `athena_intelligence-0.1.63/src/athena/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     HttpValidationError,
     LangchainDocumentsRequestOut,
     LlmModel,
     MapReduceChainOut,
     MessageOut,
     MessageOutDto,
     Model,
+    PublishFormats,
     Report,
     ResearcherOut,
     Snippet,
     SqlResults,
     StatusEnum,
     StructuredParseResult,
     Tools,
@@ -48,14 +49,15 @@
     "HttpValidationError",
     "LangchainDocumentsRequestOut",
     "LlmModel",
     "MapReduceChainOut",
     "MessageOut",
     "MessageOutDto",
     "Model",
+    "PublishFormats",
     "Report",
     "ResearcherOut",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "StructuredParseResult",
     "Tools",
```

### Comparing `athena_intelligence-0.1.62/src/athena/base_client.py` & `athena_intelligence-0.1.63/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/chain/client.py` & `athena_intelligence-0.1.63/src/athena/chain/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/client.py` & `athena_intelligence-0.1.63/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/core/__init__.py` & `athena_intelligence-0.1.63/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.63/src/athena/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.62",
+            "X-Fern-SDK-Version": "0.1.63",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.62/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.63/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/core/file.py` & `athena_intelligence-0.1.63/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/core/http_client.py` & `athena_intelligence-0.1.63/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.63/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/core/request_options.py` & `athena_intelligence-0.1.63/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/dataset/client.py` & `athena_intelligence-0.1.63/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/message/client.py` & `athena_intelligence-0.1.63/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/polling_message_client.py` & `athena_intelligence-0.1.63/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/query/client.py` & `athena_intelligence-0.1.63/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/report/client.py` & `athena_intelligence-0.1.63/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/search/client.py` & `athena_intelligence-0.1.63/src/athena/search/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/snippet/client.py` & `athena_intelligence-0.1.63/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/tools/client.py` & `athena_intelligence-0.1.63/src/athena/tools/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.excecute_tool_first_workflow_out import ExcecuteToolFirstWorkflowOut
 from ..types.firecrawl_scrape_url_data_reponse_dto import FirecrawlScrapeUrlDataReponseDto
 from ..types.http_validation_error import HttpValidationError
 from ..types.langchain_documents_request_out import LangchainDocumentsRequestOut
 from ..types.llm_model import LlmModel
+from ..types.publish_formats import PublishFormats
 from ..types.researcher_out import ResearcherOut
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ToolsClient:
@@ -244,51 +245,67 @@
 
     def researcher(
         self,
         *,
         query: str,
         max_sections: int,
         guidelines: typing.Sequence[str],
+        publish_formats: typing.Optional[PublishFormats] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ResearcherOut:
         """
         Parameters:
             - query: str.
 
             - max_sections: int.
 
             - guidelines: typing.Sequence[str].
 
+            - publish_formats: typing.Optional[PublishFormats].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from athena import PublishFormats
         from athena.client import Athena
 
         client = Athena(
             api_key="YOUR_API_KEY",
         )
         client.tools.researcher(
             query="Write a report about the company Athena Intelligence.",
             max_sections=10,
             guidelines=[
                 "The report MUST be written in APA format",
                 "Each sub section MUST include supporting sources using hyperlinks. If none exist, erase the sub section or rewrite it to be a part of the previous section",
                 "The report MUST be written in english",
             ],
+            publish_formats=PublishFormats(
+                markdown=False,
+                pdf=True,
+                docx=False,
+            ),
         )
         """
+        _request: typing.Dict[str, typing.Any] = {
+            "query": query,
+            "max_sections": max_sections,
+            "guidelines": guidelines,
+        }
+        if publish_formats is not OMIT:
+            _request["publish_formats"] = publish_formats
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/researcher"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"query": query, "max_sections": max_sections, "guidelines": guidelines})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"query": query, "max_sections": max_sections, "guidelines": guidelines}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -536,51 +553,67 @@
 
     async def researcher(
         self,
         *,
         query: str,
         max_sections: int,
         guidelines: typing.Sequence[str],
+        publish_formats: typing.Optional[PublishFormats] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ResearcherOut:
         """
         Parameters:
             - query: str.
 
             - max_sections: int.
 
             - guidelines: typing.Sequence[str].
 
+            - publish_formats: typing.Optional[PublishFormats].
+
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from athena import PublishFormats
         from athena.client import AsyncAthena
 
         client = AsyncAthena(
             api_key="YOUR_API_KEY",
         )
         await client.tools.researcher(
             query="Write a report about the company Athena Intelligence.",
             max_sections=10,
             guidelines=[
                 "The report MUST be written in APA format",
                 "Each sub section MUST include supporting sources using hyperlinks. If none exist, erase the sub section or rewrite it to be a part of the previous section",
                 "The report MUST be written in english",
             ],
+            publish_formats=PublishFormats(
+                markdown=False,
+                pdf=True,
+                docx=False,
+            ),
         )
         """
+        _request: typing.Dict[str, typing.Any] = {
+            "query": query,
+            "max_sections": max_sections,
+            "guidelines": guidelines,
+        }
+        if publish_formats is not OMIT:
+            _request["publish_formats"] = publish_formats
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/v0/tools/researcher"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder({"query": query, "max_sections": max_sections, "guidelines": guidelines})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"query": query, "max_sections": max_sections, "guidelines": guidelines}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
```

### Comparing `athena_intelligence-0.1.62/src/athena/types/__init__.py` & `athena_intelligence-0.1.63/src/athena/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .http_validation_error import HttpValidationError
 from .langchain_documents_request_out import LangchainDocumentsRequestOut
 from .llm_model import LlmModel
 from .map_reduce_chain_out import MapReduceChainOut
 from .message_out import MessageOut
 from .message_out_dto import MessageOutDto
 from .model import Model
+from .publish_formats import PublishFormats
 from .report import Report
 from .researcher_out import ResearcherOut
 from .snippet import Snippet
 from .sql_results import SqlResults
 from .status_enum import StatusEnum
 from .structured_parse_result import StructuredParseResult
 from .tools import Tools
@@ -41,14 +42,15 @@
     "HttpValidationError",
     "LangchainDocumentsRequestOut",
     "LlmModel",
     "MapReduceChainOut",
     "MessageOut",
     "MessageOutDto",
     "Model",
+    "PublishFormats",
     "Report",
     "ResearcherOut",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "StructuredParseResult",
     "Tools",
```

### Comparing `athena_intelligence-0.1.62/src/athena/types/dataset.py` & `athena_intelligence-0.1.63/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/document.py` & `athena_intelligence-0.1.63/src/athena/types/document.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/excecute_tool_first_workflow_out.py` & `athena_intelligence-0.1.63/src/athena/types/excecute_tool_first_workflow_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/file_data_response.py` & `athena_intelligence-0.1.63/src/athena/types/file_data_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py` & `athena_intelligence-0.1.63/src/athena/types/firecrawl_scrape_url_data_reponse_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/firecrawl_scrape_url_metadata.py` & `athena_intelligence-0.1.63/src/athena/types/firecrawl_scrape_url_metadata.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.63/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/get_snippet_out.py` & `athena_intelligence-0.1.63/src/athena/types/get_snippet_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.63/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.63/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/langchain_documents_request_out.py` & `athena_intelligence-0.1.63/src/athena/types/langchain_documents_request_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/llm_model.py` & `athena_intelligence-0.1.63/src/athena/types/llm_model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/map_reduce_chain_out.py` & `athena_intelligence-0.1.63/src/athena/types/map_reduce_chain_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/message_out.py` & `athena_intelligence-0.1.63/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.63/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/model.py` & `athena_intelligence-0.1.63/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/report.py` & `athena_intelligence-0.1.63/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/researcher_out.py` & `athena_intelligence-0.1.63/src/athena/types/researcher_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/snippet.py` & `athena_intelligence-0.1.63/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/sql_results.py` & `athena_intelligence-0.1.63/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/status_enum.py` & `athena_intelligence-0.1.63/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/structured_parse_result.py` & `athena_intelligence-0.1.63/src/athena/types/structured_parse_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/tools.py` & `athena_intelligence-0.1.63/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/upload_documents_out.py` & `athena_intelligence-0.1.63/src/athena/types/upload_documents_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/url_result.py` & `athena_intelligence-0.1.63/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/types/validation_error.py` & `athena_intelligence-0.1.63/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/src/athena/upload/client.py` & `athena_intelligence-0.1.63/src/athena/upload/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.62/PKG-INFO` & `athena_intelligence-0.1.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.62
+Version: 0.1.63
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

