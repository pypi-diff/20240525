# Comparing `tmp/scorecard_ai-1.0.0b2.tar.gz` & `tmp/scorecard_ai-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecard_ai-1.0.0b2.tar", max compression
+gzip compressed data, was "scorecard_ai-1.0.0b3.tar", max compression
```

## Comparing `scorecard_ai-1.0.0b2.tar` & `scorecard_ai-1.0.0b3.tar`

### file list

```diff
@@ -1,94 +1,96 @@
--rw-r--r--   0        0        0    11355 2024-05-15 03:56:18.822297 scorecard_ai-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     3605 2024-05-15 03:56:18.822297 scorecard_ai-1.0.0b2/README.md
--rw-r--r--   0        0        0     1113 2024-05-15 03:56:18.822297 scorecard_ai-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     3177 2024-05-15 03:56:18.822297 scorecard_ai-1.0.0b2/src/scorecard/__init__.py
--rw-r--r--   0        0        0     7323 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/base_client.py
--rw-r--r--   0        0        0     4257 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/client.py
--rw-r--r--   0        0        0     1006 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/api_error.py
--rw-r--r--   0        0        0     1494 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/request_options.py
--rw-r--r--   0        0        0     7165 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/core/unchecked_base_model.py
--rw-r--r--   0        0        0      162 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/environment.py
--rw-r--r--   0        0        0      363 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/errors/__init__.py
--rw-r--r--   0        0        0      309 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/errors/forbidden_error.py
--rw-r--r--   0        0        0      297 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/errors/not_found_error.py
--rw-r--r--   0        0        0      308 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/errors/unauthorized_error.py
--rw-r--r--   0        0        0      313 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      169 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/prompt/__init__.py
--rw-r--r--   0        0        0    48381 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/prompt/client.py
--rw-r--r--   0        0        0      203 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/prompt/types/__init__.py
--rw-r--r--   0        0        0      153 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/prompt/types/prompt_create_params_model_params_value.py
--rw-r--r--   0        0        0        0 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/py.typed
--rw-r--r--   0        0        0       65 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/run/__init__.py
--rw-r--r--   0        0        0    24494 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/run/client.py
--rw-r--r--   0        0        0       65 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/run_metric/__init__.py
--rw-r--r--   0        0        0     7629 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/run_metric/client.py
--rw-r--r--   0        0        0       65 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/score/__init__.py
--rw-r--r--   0        0        0    18323 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/score/client.py
--rw-r--r--   0        0        0     2481 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/telemetry.py
--rw-r--r--   0        0        0      255 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testcase/__init__.py
--rw-r--r--   0        0        0    23624 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testcase/client.py
--rw-r--r--   0        0        0      347 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testcase/types/__init__.py
--rw-r--r--   0        0        0      242 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testcase/types/testcase_create_params_custom_inputs_value.py
--rw-r--r--   0        0        0      242 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testcase/types/testcase_create_params_custom_labels_value.py
--rw-r--r--   0        0        0      567 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testrecord/__init__.py
--rw-r--r--   0        0        0    21204 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testrecord/client.py
--rw-r--r--   0        0        0      812 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testrecord/types/__init__.py
--rw-r--r--   0        0        0      244 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testrecord/types/testrecord_create_params_custom_inputs_value.py
--rw-r--r--   0        0        0      244 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testrecord/types/testrecord_create_params_custom_labels_value.py
--rw-r--r--   0        0        0      245 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testrecord/types/testrecord_create_params_custom_outputs_value.py
--rw-r--r--   0        0        0      154 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testrecord/types/testrecord_create_params_model_debug_info_value.py
--rw-r--r--   0        0        0      151 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testrecord/types/testrecord_create_params_model_params_value.py
--rw-r--r--   0        0        0       65 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testset/__init__.py
--rw-r--r--   0        0        0    35470 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/testset/client.py
--rw-r--r--   0        0        0       65 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/traces/__init__.py
--rw-r--r--   0        0        0     7578 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/traces/client.py
--rw-r--r--   0        0        0     2885 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/__init__.py
--rw-r--r--   0        0        0      120 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/create_github_workflow_params.py
--rw-r--r--   0        0        0      109 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/create_run_params.py
--rw-r--r--   0        0        0     1165 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/custom_schema.py
--rw-r--r--   0        0        0     1159 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/custom_variable.py
--rw-r--r--   0        0        0      171 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/data_type_enum.py
--rw-r--r--   0        0        0      988 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/file_url.py
--rw-r--r--   0        0        0     1551 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/grade.py
--rw-r--r--   0        0        0     1009 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/http_validation_error.py
--rw-r--r--   0        0        0     1244 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/json_object.py
--rw-r--r--   0        0        0      231 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/json_object_input_value.py
--rw-r--r--   0        0        0      232 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/json_object_output_value.py
--rw-r--r--   0        0        0     1031 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/not_found_error_body.py
--rw-r--r--   0        0        0     1066 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/paginated_testcase_response.py
--rw-r--r--   0        0        0     1527 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/prompt.py
--rw-r--r--   0        0        0      135 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/prompt_model_params_value.py
--rw-r--r--   0        0        0      172 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/role_enum.py
--rw-r--r--   0        0        0     1645 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/run.py
--rw-r--r--   0        0        0     1059 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/run_metric.py
--rw-r--r--   0        0        0      339 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/run_status.py
--rw-r--r--   0        0        0      168 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/score_status.py
--rw-r--r--   0        0        0     2684 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/span.py
--rw-r--r--   0        0        0     1441 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/test_case.py
--rw-r--r--   0        0        0     1055 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/test_case_create.py
--rw-r--r--   0        0        0      214 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/test_case_custom_inputs_value.py
--rw-r--r--   0        0        0      214 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/test_case_custom_labels_value.py
--rw-r--r--   0        0        0      110 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/test_record_create.py
--rw-r--r--   0        0        0      107 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/test_set_create.py
--rw-r--r--   0        0        0     2303 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/testrecord.py
--rw-r--r--   0        0        0      216 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/testrecord_custom_inputs_value.py
--rw-r--r--   0        0        0      216 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/testrecord_custom_labels_value.py
--rw-r--r--   0        0        0      217 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/testrecord_custom_outputs_value.py
--rw-r--r--   0        0        0      142 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/testrecord_model_debug_info_value.py
--rw-r--r--   0        0        0      139 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/testrecord_model_params_value.py
--rw-r--r--   0        0        0     1486 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/testset.py
--rw-r--r--   0        0        0     1129 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/trace.py
--rw-r--r--   0        0        0     1034 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/unauthenticated_error.py
--rw-r--r--   0        0        0     1035 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/unauthorized_error_body.py
--rw-r--r--   0        0        0     1028 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       80 2024-05-15 03:56:18.826297 scorecard_ai-1.0.0b2/src/scorecard/version.py
--rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 scorecard_ai-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0     3605 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/README.md
+-rw-r--r--   0        0        0     1862 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     3239 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/__init__.py
+-rw-r--r--   0        0        0     7323 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/base_client.py
+-rw-r--r--   0        0        0     4257 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/client.py
+-rw-r--r--   0        0        0     1126 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/api_error.py
+-rw-r--r--   0        0        0     1494 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1266 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/request_options.py
+-rw-r--r--   0        0        0     8148 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      162 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/environment.py
+-rw-r--r--   0        0        0      363 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/errors/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/errors/forbidden_error.py
+-rw-r--r--   0        0        0      297 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/errors/not_found_error.py
+-rw-r--r--   0        0        0      308 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      313 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      169 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/prompt/__init__.py
+-rw-r--r--   0        0        0    39019 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/prompt/client.py
+-rw-r--r--   0        0        0      203 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/prompt/types/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/prompt/types/prompt_create_params_model_params_value.py
+-rw-r--r--   0        0        0        0 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/py.typed
+-rw-r--r--   0        0        0       65 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/run/__init__.py
+-rw-r--r--   0        0        0    24806 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/run/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/run_metric/__init__.py
+-rw-r--r--   0        0        0     7779 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/run_metric/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/score/__init__.py
+-rw-r--r--   0        0        0    19247 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/score/client.py
+-rw-r--r--   0        0        0     2481 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/telemetry.py
+-rw-r--r--   0        0        0      255 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testcase/__init__.py
+-rw-r--r--   0        0        0    25300 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testcase/client.py
+-rw-r--r--   0        0        0      347 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testcase/types/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testcase/types/testcase_create_params_custom_inputs_value.py
+-rw-r--r--   0        0        0      260 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testcase/types/testcase_create_params_custom_labels_value.py
+-rw-r--r--   0        0        0      567 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testrecord/__init__.py
+-rw-r--r--   0        0        0    21576 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testrecord/client.py
+-rw-r--r--   0        0        0      812 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testrecord/types/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testrecord/types/testrecord_create_params_custom_inputs_value.py
+-rw-r--r--   0        0        0      244 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testrecord/types/testrecord_create_params_custom_labels_value.py
+-rw-r--r--   0        0        0      245 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testrecord/types/testrecord_create_params_custom_outputs_value.py
+-rw-r--r--   0        0        0      154 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testrecord/types/testrecord_create_params_model_debug_info_value.py
+-rw-r--r--   0        0        0      151 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testrecord/types/testrecord_create_params_model_params_value.py
+-rw-r--r--   0        0        0       65 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testset/__init__.py
+-rw-r--r--   0        0        0    37062 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/testset/client.py
+-rw-r--r--   0        0        0       65 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/traces/__init__.py
+-rw-r--r--   0        0        0     7728 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/traces/client.py
+-rw-r--r--   0        0        0     2982 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/create_github_workflow_params.py
+-rw-r--r--   0        0        0      109 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/create_run_params.py
+-rw-r--r--   0        0        0     1428 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/custom_schema.py
+-rw-r--r--   0        0        0     1422 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/custom_variable.py
+-rw-r--r--   0        0        0      171 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/data_type_enum.py
+-rw-r--r--   0        0        0     1251 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/file_url.py
+-rw-r--r--   0        0        0     1979 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/grade.py
+-rw-r--r--   0        0        0     1272 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/http_validation_error.py
+-rw-r--r--   0        0        0     1507 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/json_object.py
+-rw-r--r--   0        0        0      231 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/json_object_input_value.py
+-rw-r--r--   0        0        0      232 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/json_object_output_value.py
+-rw-r--r--   0        0        0     1294 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/not_found_error_body.py
+-rw-r--r--   0        0        0     1417 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/paginated_testcase_response.py
+-rw-r--r--   0        0        0     1790 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/prompt.py
+-rw-r--r--   0        0        0      135 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/prompt_model_params_value.py
+-rw-r--r--   0        0        0      172 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/role_enum.py
+-rw-r--r--   0        0        0     1908 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/run.py
+-rw-r--r--   0        0        0     1322 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/run_metric.py
+-rw-r--r--   0        0        0      339 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/run_status.py
+-rw-r--r--   0        0        0      168 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/score_status.py
+-rw-r--r--   0        0        0     2947 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/span.py
+-rw-r--r--   0        0        0     1870 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/test_case.py
+-rw-r--r--   0        0        0     1318 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/test_case_create.py
+-rw-r--r--   0        0        0      232 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/test_case_custom_inputs_value.py
+-rw-r--r--   0        0        0      232 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/test_case_custom_labels_value.py
+-rw-r--r--   0        0        0      110 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/test_record_create.py
+-rw-r--r--   0        0        0      107 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/test_set_create.py
+-rw-r--r--   0        0        0     1369 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/testcase_deletion_response.py
+-rw-r--r--   0        0        0     2521 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/testrecord.py
+-rw-r--r--   0        0        0      216 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/testrecord_custom_inputs_value.py
+-rw-r--r--   0        0        0      216 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/testrecord_custom_labels_value.py
+-rw-r--r--   0        0        0      217 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/testrecord_custom_outputs_value.py
+-rw-r--r--   0        0        0      142 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/testrecord_model_debug_info_value.py
+-rw-r--r--   0        0        0      139 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/testrecord_model_params_value.py
+-rw-r--r--   0        0        0     1749 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/testset.py
+-rw-r--r--   0        0        0     1392 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/trace.py
+-rw-r--r--   0        0        0     1297 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/unauthenticated_error.py
+-rw-r--r--   0        0        0     1298 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     1291 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       80 2024-05-25 05:21:58.149531 scorecard_ai-1.0.0b3/src/scorecard/version.py
+-rw-r--r--   0        0        0     5248 1970-01-01 00:00:00.000000 scorecard_ai-1.0.0b3/PKG-INFO
```

### Comparing `scorecard_ai-1.0.0b2/LICENSE` & `scorecard_ai-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/README.md` & `scorecard_ai-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/__init__.py` & `scorecard_ai-1.0.0b3/src/scorecard/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     Span,
     TestCase,
     TestCaseCreate,
     TestCaseCustomInputsValue,
     TestCaseCustomLabelsValue,
     TestRecordCreate,
     TestSetCreate,
+    TestcaseDeletionResponse,
     Testrecord,
     TestrecordCustomInputsValue,
     TestrecordCustomLabelsValue,
     TestrecordCustomOutputsValue,
     TestrecordModelDebugInfoValue,
     TestrecordModelParamsValue,
     Testset,
@@ -85,14 +86,15 @@
     "TestCaseCreate",
     "TestCaseCustomInputsValue",
     "TestCaseCustomLabelsValue",
     "TestRecordCreate",
     "TestSetCreate",
     "TestcaseCreateParamsCustomInputsValue",
     "TestcaseCreateParamsCustomLabelsValue",
+    "TestcaseDeletionResponse",
     "Testrecord",
     "TestrecordCreateParamsCustomInputsValue",
     "TestrecordCreateParamsCustomLabelsValue",
     "TestrecordCreateParamsCustomOutputsValue",
     "TestrecordCreateParamsModelDebugInfoValue",
     "TestrecordCreateParamsModelParamsValue",
     "TestrecordCustomInputsValue",
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/base_client.py` & `scorecard_ai-1.0.0b3/src/scorecard/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .testrecord.client import AsyncTestrecordClient, TestrecordClient
 from .testset.client import AsyncTestsetClient, TestsetClient
 from .traces.client import AsyncTracesClient, TracesClient
 
 
 class BaseScorecard:
     """
-    Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
+    Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propagate to these functions.
 
     Parameters
     ----------
     base_url : typing.Optional[str]
         The base url to use for requests from the client.
 
     environment : ScorecardEnvironment
@@ -88,15 +88,15 @@
         self.run_metric = RunMetricClient(client_wrapper=self._client_wrapper)
         self.traces = TracesClient(client_wrapper=self._client_wrapper)
         self.prompt = PromptClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseScorecard:
     """
-    Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
+    Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propagate to these functions.
 
     Parameters
     ----------
     base_url : typing.Optional[str]
         The base url to use for requests from the client.
 
     environment : ScorecardEnvironment
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/core/__init__.py` & `scorecard_ai-1.0.0b3/src/scorecard/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from .api_error import ApiError
 from .client_wrapper import AsyncClientWrapper, BaseClientWrapper, SyncClientWrapper
 from .datetime_utils import serialize_datetime
 from .file import File, convert_file_dict_to_httpx_tuples
 from .http_client import AsyncHttpClient, HttpClient
 from .jsonable_encoder import jsonable_encoder
-from .pydantic_utilities import pydantic_v1
+from .pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .query_encoder import encode_query
 from .remove_none_from_dict import remove_none_from_dict
 from .request_options import RequestOptions
 from .unchecked_base_model import UncheckedBaseModel, UnionMetadata, construct_type
 
 __all__ = [
     "ApiError",
     "AsyncClientWrapper",
@@ -20,12 +21,14 @@
     "HttpClient",
     "RequestOptions",
     "SyncClientWrapper",
     "UncheckedBaseModel",
     "UnionMetadata",
     "construct_type",
     "convert_file_dict_to_httpx_tuples",
+    "deep_union_pydantic_dicts",
+    "encode_query",
     "jsonable_encoder",
     "pydantic_v1",
     "remove_none_from_dict",
     "serialize_datetime",
 ]
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/core/client_wrapper.py` & `scorecard_ai-1.0.0b3/src/scorecard/core/client_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "scorecard-ai",
-            "X-Fern-SDK-Version": "v1.0.0-beta2",
+            "X-Fern-SDK-Version": "v1.0.0-beta3",
         }
         headers["X-API-Key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/core/datetime_utils.py` & `scorecard_ai-1.0.0b3/src/scorecard/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/core/file.py` & `scorecard_ai-1.0.0b3/src/scorecard/core/file.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/core/http_client.py` & `scorecard_ai-1.0.0b3/src/scorecard/core/http_client.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/core/jsonable_encoder.py` & `scorecard_ai-1.0.0b3/src/scorecard/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/core/request_options.py` & `scorecard_ai-1.0.0b3/src/scorecard/core/request_options.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/core/unchecked_base_model.py` & `scorecard_ai-1.0.0b3/src/scorecard/core/unchecked_base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import inspect
 import typing
 import uuid
 
 import typing_extensions
 
 from .datetime_utils import serialize_datetime
-from .pydantic_utilities import pydantic_v1
+from .pydantic_utilities import IS_PYDANTIC_V2, pydantic_v1
 
 
 class UnionMetadata:
     discriminant: str
 
     def __init__(self, *, discriminant: str) -> None:
         self.discriminant = discriminant
@@ -56,29 +56,39 @@
                 if (
                     values[key] is None and not field.required
                 ):  # Moved this check since None value can be passed for Optional nested field
                     fields_values[name] = field.get_default()
                 else:
                     type_ = typing.cast(typing.Type, field.outer_type_)  # type: ignore
                     fields_values[name] = construct_type(object_=values[key], type_=type_)
+                _fields_set.add(name)
             elif not field.required:
                 default = field.get_default()
                 fields_values[name] = default
 
                 # If the default values are non-null act like they've been set
                 # This effectively allows exclude_unset to work like exclude_none where
                 # the latter passes through intentionally set none values.
                 if default != None:
                     _fields_set.add(key)
 
         # Add extras back in
+        _extra = {}
         for key, value in values.items():
-            if key not in cls.__fields__:
-                _fields_set.add(key)
-                fields_values[key] = value
+            if key not in _fields_set:
+                _extra[key] = value
+                # In v2 we'll need to exclude extra fields from fields_values
+                if not IS_PYDANTIC_V2:
+                    _fields_set.add(key)
+                    fields_values[key] = value
+
+        if IS_PYDANTIC_V2:
+            object.__setattr__(m, "__pydantic_private__", None)
+            object.__setattr__(m, "__pydantic_extra__", _extra)
+            object.__setattr__(m, "__pydantic_fields_set__", _fields_set)
 
         object.__setattr__(m, "__dict__", fields_values)
         object.__setattr__(m, "__fields_set__", _fields_set)
         m._init_private_attributes()
         return m
 
 
@@ -140,16 +150,20 @@
     if base_type == typing.Any:
         return object_
 
     if base_type == dict:
         if not isinstance(object_, typing.Mapping):
             return object_
 
-        _, items_type = pydantic_v1.typing.get_args(type_)
-        return {key: construct_type(object_=item, type_=items_type) for key, item in object_.items()}
+        key_type, items_type = pydantic_v1.typing.get_args(type_)
+        d = {
+            construct_type(object_=key, type_=key_type): construct_type(object_=item, type_=items_type)
+            for key, item in object_.items()
+        }
+        return d
 
     if base_type == list:
         if not isinstance(object_, list):
             return object_
 
         inner_type = pydantic_v1.typing.get_args(type_)[0]
         return [construct_type(object_=entry, type_=inner_type) for entry in object_]
@@ -186,8 +200,24 @@
 
     if base_type == uuid.UUID:
         try:
             return uuid.UUID(object_)
         except Exception:
             return object_
 
+    if base_type == int:
+        try:
+            return int(object_)
+        except Exception:
+            return object_
+
+    if base_type == bool:
+        try:
+            if isinstance(object_, str):
+                stringified_object = object_.lower()
+                return stringified_object == "true" or stringified_object == "1"
+
+            return bool(object_)
+        except Exception:
+            return object_
+
     return object_
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/prompt/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/testset/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,114 +3,76 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.not_found_error import NotFoundError
 from ..errors.unauthorized_error import UnauthorizedError
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
+from ..types.custom_schema import CustomSchema
 from ..types.http_validation_error import HttpValidationError
 from ..types.not_found_error_body import NotFoundErrorBody
-from ..types.prompt import Prompt
+from ..types.paginated_testcase_response import PaginatedTestcaseResponse
+from ..types.testset import Testset
 from ..types.unauthenticated_error import UnauthenticatedError
 from ..types.unauthorized_error_body import UnauthorizedErrorBody
-from .types.prompt_create_params_model_params_value import PromptCreateParamsModelParamsValue
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class PromptClient:
+class TestsetClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def create(
-        self,
-        *,
-        prompt_template: str,
-        name: typing.Optional[str] = OMIT,
-        parent_id: typing.Optional[str] = OMIT,
-        description: typing.Optional[str] = OMIT,
-        model_params: typing.Optional[typing.Dict[str, typing.Optional[PromptCreateParamsModelParamsValue]]] = OMIT,
-        is_prod: typing.Optional[bool] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> Prompt:
+    def get(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> Testset:
         """
-        Create a new prompt
+        Retrieve Testset metadata without Testcase data
 
         Parameters
         ----------
-        prompt_template : str
-
-        name : typing.Optional[str]
-
-        parent_id : typing.Optional[str]
-
-        description : typing.Optional[str]
-
-        model_params : typing.Optional[typing.Dict[str, typing.Optional[PromptCreateParamsModelParamsValue]]]
-
-        is_prod : typing.Optional[bool]
+        testset_id : int
+            The ID of the Testset to retrieve.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Prompt
+        Testset
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.prompt.create(
-            prompt_template="You are a virtual assistant",
-            name="Prompt Name",
-            description="Description of the prompt",
-            model_params={
-                "param1": "value1",
-                "param2": 0.1,
-                "param3": 100,
-                "param4": True,
-            },
+        client.testset.get(
+            testset_id=1,
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"prompt_template": prompt_template}
-        if name is not OMIT:
-            _request["name"] = name
-        if parent_id is not OMIT:
-            _request["parent_id"] = parent_id
-        if description is not OMIT:
-            _request["description"] = description
-        if model_params is not OMIT:
-            _request["model_params"] = model_params
-        if is_prod is not OMIT:
-            _request["is_prod"] = is_prod
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/prompt"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -118,15 +80,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
+            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -141,174 +103,55 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_roots(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.List[Prompt]:
+    def delete(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> Testset:
         """
-        Retrieve active root prompts for the org
+        Delete a Testset
 
         Parameters
         ----------
-        request_options : typing.Optional[RequestOptions]
-            Request-specific configuration.
-
-        Returns
-        -------
-        typing.List[Prompt]
-            Successful Response
-
-        Examples
-        --------
-        from scorecard.client import Scorecard
-
-        client = Scorecard(
-            api_key="YOUR_API_KEY",
-        )
-        client.prompt.get_roots()
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/prompt/roots"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return typing.cast(typing.List[Prompt], construct_type(type_=typing.List[Prompt], object_=_response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(
-                typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
-            )
-        if _response.status_code == 403:
-            raise ForbiddenError(
-                typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
-            )
-        if _response.status_code == 404:
-            raise NotFoundError(
-                typing.cast(NotFoundErrorBody, construct_type(type_=NotFoundErrorBody, object_=_response.json()))  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_prods(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.List[Prompt]:
-        """
-        Retrieve prod prompts for the org
+        testset_id : int
+            The ID of the Testset to delete.
 
-        Parameters
-        ----------
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        typing.List[Prompt]
+        Testset
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.prompt.get_prods()
+        client.testset.delete(
+            testset_id=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/prompt/prods"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}"
             ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return typing.cast(typing.List[Prompt], construct_type(type_=typing.List[Prompt], object_=_response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(
-                typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
-            )
-        if _response.status_code == 403:
-            raise ForbiddenError(
-                typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
-            )
-        if _response.status_code == 404:
-            raise NotFoundError(
-                typing.cast(NotFoundErrorBody, construct_type(type_=NotFoundErrorBody, object_=_response.json()))  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Prompt:
-        """
-        Retrieve a prompt by id
-
-        Parameters
-        ----------
-        id : str
-            The id of the prompt to get.
-
-        request_options : typing.Optional[RequestOptions]
-            Request-specific configuration.
-
-        Returns
-        -------
-        Prompt
-            Successful Response
-
-        Examples
-        --------
-        from scorecard.client import Scorecard
-
-        client = Scorecard(
-            api_key="YOUR_API_KEY",
-        )
-        client.prompt.get(
-            id="id",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -316,15 +159,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
+            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -339,64 +182,69 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(
+    def create(
         self,
-        id: str,
         *,
-        is_archived: typing.Optional[bool] = OMIT,
-        is_prod: typing.Optional[bool] = OMIT,
+        name: str,
+        description: typing.Optional[str] = OMIT,
+        using_retrieval: typing.Optional[bool] = OMIT,
+        custom_schema: typing.Optional[CustomSchema] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Prompt:
+    ) -> Testset:
         """
-        Update a prompt
+        Create a new Testset
 
         Parameters
         ----------
-        id : str
-            The id of the prompt to update.
+        name : str
+
+        description : typing.Optional[str]
 
-        is_archived : typing.Optional[bool]
+        using_retrieval : typing.Optional[bool]
 
-        is_prod : typing.Optional[bool]
+        custom_schema : typing.Optional[CustomSchema]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Prompt
+        Testset
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.prompt.update(
-            id="id",
-            is_archived=True,
+        client.testset.create(
+            name="name",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if is_archived is not OMIT:
-            _request["is_archived"] = is_archived
-        if is_prod is not OMIT:
-            _request["is_prod"] = is_prod
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if description is not OMIT:
+            _request["description"] = description
+        if using_retrieval is not OMIT:
+            _request["using_retrieval"] = using_retrieval
+        if custom_schema is not OMIT:
+            _request["custom_schema"] = custom_schema
         _response = self._client_wrapper.httpx_client.request(
-            method="PATCH",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/testset"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -411,15 +259,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
+            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -434,49 +282,51 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_by_name(self, name: str, *, request_options: typing.Optional[RequestOptions] = None) -> Prompt:
+    def read_schema(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> CustomSchema:
         """
-        Retrieve a prod prompt by name
+        Read the schema of a Testset
 
         Parameters
         ----------
-        name : str
-            Name of the prompt.
+        testset_id : int
+            The ID of the Testset to retrieve the schema from.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Prompt
+        CustomSchema
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.prompt.get_by_name(
-            name="name",
+        client.testset.read_schema(
+            testset_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/name/{jsonable_encoder(name)}"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/schema"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -485,15 +335,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
+            return typing.cast(CustomSchema, construct_type(type_=CustomSchema, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -508,49 +358,74 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_graph(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.List[Prompt]:
+    def get_testcases(
+        self,
+        testset_id: int,
+        *,
+        offset: typing.Optional[int] = None,
+        limit: typing.Optional[int] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> PaginatedTestcaseResponse:
         """
-        Retrieve all nodes within the same graph as the prompt, sorted by created_at desc
+        Retrieve all Testcases from a Testset
 
         Parameters
         ----------
-        id : str
-            The id of the prompt.
+        testset_id : int
+            The Testset ID to retrieve testcases from.
+
+        offset : typing.Optional[int]
+            The offset to start from.
+
+        limit : typing.Optional[int]
+            The number of testcases to return.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        typing.List[Prompt]
+        PaginatedTestcaseResponse
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.prompt.get_graph(
-            id="id",
+        client.testset.get_testcases(
+            testset_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}/graph"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/testcase"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "offset": offset,
+                            "limit": limit,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -559,15 +434,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(typing.List[Prompt], construct_type(type_=typing.List[Prompt], object_=_response.json()))  # type: ignore
+            return typing.cast(PaginatedTestcaseResponse, construct_type(type_=PaginatedTestcaseResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -583,96 +458,56 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncPromptClient:
+class AsyncTestsetClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def create(
-        self,
-        *,
-        prompt_template: str,
-        name: typing.Optional[str] = OMIT,
-        parent_id: typing.Optional[str] = OMIT,
-        description: typing.Optional[str] = OMIT,
-        model_params: typing.Optional[typing.Dict[str, typing.Optional[PromptCreateParamsModelParamsValue]]] = OMIT,
-        is_prod: typing.Optional[bool] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> Prompt:
+    async def get(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> Testset:
         """
-        Create a new prompt
+        Retrieve Testset metadata without Testcase data
 
         Parameters
         ----------
-        prompt_template : str
-
-        name : typing.Optional[str]
-
-        parent_id : typing.Optional[str]
-
-        description : typing.Optional[str]
-
-        model_params : typing.Optional[typing.Dict[str, typing.Optional[PromptCreateParamsModelParamsValue]]]
-
-        is_prod : typing.Optional[bool]
+        testset_id : int
+            The ID of the Testset to retrieve.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Prompt
+        Testset
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.prompt.create(
-            prompt_template="You are a virtual assistant",
-            name="Prompt Name",
-            description="Description of the prompt",
-            model_params={
-                "param1": "value1",
-                "param2": 0.1,
-                "param3": 100,
-                "param4": True,
-            },
+        await client.testset.get(
+            testset_id=1,
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"prompt_template": prompt_template}
-        if name is not OMIT:
-            _request["name"] = name
-        if parent_id is not OMIT:
-            _request["parent_id"] = parent_id
-        if description is not OMIT:
-            _request["description"] = description
-        if model_params is not OMIT:
-            _request["model_params"] = model_params
-        if is_prod is not OMIT:
-            _request["is_prod"] = is_prod
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/prompt"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}"
+            ),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -680,15 +515,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
+            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -703,174 +538,55 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_roots(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.List[Prompt]:
+    async def delete(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> Testset:
         """
-        Retrieve active root prompts for the org
+        Delete a Testset
 
         Parameters
         ----------
-        request_options : typing.Optional[RequestOptions]
-            Request-specific configuration.
-
-        Returns
-        -------
-        typing.List[Prompt]
-            Successful Response
-
-        Examples
-        --------
-        from scorecard.client import AsyncScorecard
-
-        client = AsyncScorecard(
-            api_key="YOUR_API_KEY",
-        )
-        await client.prompt.get_roots()
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/prompt/roots"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return typing.cast(typing.List[Prompt], construct_type(type_=typing.List[Prompt], object_=_response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(
-                typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
-            )
-        if _response.status_code == 403:
-            raise ForbiddenError(
-                typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
-            )
-        if _response.status_code == 404:
-            raise NotFoundError(
-                typing.cast(NotFoundErrorBody, construct_type(type_=NotFoundErrorBody, object_=_response.json()))  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_prods(self, *, request_options: typing.Optional[RequestOptions] = None) -> typing.List[Prompt]:
-        """
-        Retrieve prod prompts for the org
+        testset_id : int
+            The ID of the Testset to delete.
 
-        Parameters
-        ----------
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        typing.List[Prompt]
+        Testset
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.prompt.get_prods()
+        await client.testset.delete(
+            testset_id=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/prompt/prods"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}"
             ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else self._client_wrapper.get_timeout(),
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return typing.cast(typing.List[Prompt], construct_type(type_=typing.List[Prompt], object_=_response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(
-                typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
-            )
-        if _response.status_code == 403:
-            raise ForbiddenError(
-                typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
-            )
-        if _response.status_code == 404:
-            raise NotFoundError(
-                typing.cast(NotFoundErrorBody, construct_type(type_=NotFoundErrorBody, object_=_response.json()))  # type: ignore
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Prompt:
-        """
-        Retrieve a prompt by id
-
-        Parameters
-        ----------
-        id : str
-            The id of the prompt to get.
-
-        request_options : typing.Optional[RequestOptions]
-            Request-specific configuration.
-
-        Returns
-        -------
-        Prompt
-            Successful Response
-
-        Examples
-        --------
-        from scorecard.client import AsyncScorecard
-
-        client = AsyncScorecard(
-            api_key="YOUR_API_KEY",
-        )
-        await client.prompt.get(
-            id="id",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -878,15 +594,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
+            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -901,64 +617,69 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
+    async def create(
         self,
-        id: str,
         *,
-        is_archived: typing.Optional[bool] = OMIT,
-        is_prod: typing.Optional[bool] = OMIT,
+        name: str,
+        description: typing.Optional[str] = OMIT,
+        using_retrieval: typing.Optional[bool] = OMIT,
+        custom_schema: typing.Optional[CustomSchema] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> Prompt:
+    ) -> Testset:
         """
-        Update a prompt
+        Create a new Testset
 
         Parameters
         ----------
-        id : str
-            The id of the prompt to update.
+        name : str
+
+        description : typing.Optional[str]
 
-        is_archived : typing.Optional[bool]
+        using_retrieval : typing.Optional[bool]
 
-        is_prod : typing.Optional[bool]
+        custom_schema : typing.Optional[CustomSchema]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Prompt
+        Testset
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.prompt.update(
-            id="id",
-            is_archived=True,
+        await client.testset.create(
+            name="name",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if is_archived is not OMIT:
-            _request["is_archived"] = is_archived
-        if is_prod is not OMIT:
-            _request["is_prod"] = is_prod
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if description is not OMIT:
+            _request["description"] = description
+        if using_retrieval is not OMIT:
+            _request["using_retrieval"] = using_retrieval
+        if custom_schema is not OMIT:
+            _request["custom_schema"] = custom_schema
         _response = await self._client_wrapper.httpx_client.request(
-            method="PATCH",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/testset"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -973,15 +694,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
+            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -996,49 +717,53 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_by_name(self, name: str, *, request_options: typing.Optional[RequestOptions] = None) -> Prompt:
+    async def read_schema(
+        self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> CustomSchema:
         """
-        Retrieve a prod prompt by name
+        Read the schema of a Testset
 
         Parameters
         ----------
-        name : str
-            Name of the prompt.
+        testset_id : int
+            The ID of the Testset to retrieve the schema from.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Prompt
+        CustomSchema
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.prompt.get_by_name(
-            name="name",
+        await client.testset.read_schema(
+            testset_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/name/{jsonable_encoder(name)}"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/schema"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -1047,15 +772,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
+            return typing.cast(CustomSchema, construct_type(type_=CustomSchema, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -1070,51 +795,74 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_graph(
-        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.List[Prompt]:
+    async def get_testcases(
+        self,
+        testset_id: int,
+        *,
+        offset: typing.Optional[int] = None,
+        limit: typing.Optional[int] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> PaginatedTestcaseResponse:
         """
-        Retrieve all nodes within the same graph as the prompt, sorted by created_at desc
+        Retrieve all Testcases from a Testset
 
         Parameters
         ----------
-        id : str
-            The id of the prompt.
+        testset_id : int
+            The Testset ID to retrieve testcases from.
+
+        offset : typing.Optional[int]
+            The offset to start from.
+
+        limit : typing.Optional[int]
+            The number of testcases to return.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        typing.List[Prompt]
+        PaginatedTestcaseResponse
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.prompt.get_graph(
-            id="id",
+        await client.testset.get_testcases(
+            testset_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}/graph"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/testcase"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "offset": offset,
+                            "limit": limit,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -1123,15 +871,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(typing.List[Prompt], construct_type(type_=typing.List[Prompt], object_=_response.json()))  # type: ignore
+            return typing.cast(PaginatedTestcaseResponse, construct_type(type_=PaginatedTestcaseResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/run/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/run/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.not_found_error import NotFoundError
 from ..errors.unauthorized_error import UnauthorizedError
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
@@ -74,20 +75,15 @@
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.run.create(
-            testset_id=1,
-            status="RUNNING_EXECUTION",
-            model_params={"param1": "value1", "param2": "value2"},
-            metrics=[1, 2],
-        )
+        client.run.create()
         """
         _request: typing.Dict[str, typing.Any] = {}
         if testset_id is not OMIT:
             _request["testset_id"] = testset_id
         if scoring_config_id is not OMIT:
             _request["scoring_config_id"] = scoring_config_id
         if status is not OMIT:
@@ -101,16 +97,18 @@
         if prompt_template is not OMIT:
             _request["prompt_template"] = prompt_template
         if metrics is not OMIT:
             _request["metrics"] = metrics
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/run"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -179,16 +177,18 @@
         client.run.get(
             run_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{jsonable_encoder(run_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -221,25 +221,29 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_status(
-        self, run_id: int, *, status: RunStatus, request_options: typing.Optional[RequestOptions] = None
+        self,
+        run_id: int,
+        *,
+        status: typing.Optional[RunStatus] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> Run:
         """
         Update the status of a run.
 
         Parameters
         ----------
         run_id : int
             The id of the run to update.
 
-        status : RunStatus
+        status : typing.Optional[RunStatus]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         Run
@@ -250,29 +254,33 @@
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
         client.run.update_status(
             run_id=1,
-            status="pending",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if status is not OMIT:
+            _request["status"] = status
         _response = self._client_wrapper.httpx_client.request(
             method="PATCH",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/run/{jsonable_encoder(run_id)}/status"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder({"status": status})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"status": status}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -359,20 +367,15 @@
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.run.create(
-            testset_id=1,
-            status="RUNNING_EXECUTION",
-            model_params={"param1": "value1", "param2": "value2"},
-            metrics=[1, 2],
-        )
+        await client.run.create()
         """
         _request: typing.Dict[str, typing.Any] = {}
         if testset_id is not OMIT:
             _request["testset_id"] = testset_id
         if scoring_config_id is not OMIT:
             _request["scoring_config_id"] = scoring_config_id
         if status is not OMIT:
@@ -386,16 +389,18 @@
         if prompt_template is not OMIT:
             _request["prompt_template"] = prompt_template
         if metrics is not OMIT:
             _request["metrics"] = metrics
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/run"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -464,16 +469,18 @@
         await client.run.get(
             run_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{jsonable_encoder(run_id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -506,25 +513,29 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_status(
-        self, run_id: int, *, status: RunStatus, request_options: typing.Optional[RequestOptions] = None
+        self,
+        run_id: int,
+        *,
+        status: typing.Optional[RunStatus] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> Run:
         """
         Update the status of a run.
 
         Parameters
         ----------
         run_id : int
             The id of the run to update.
 
-        status : RunStatus
+        status : typing.Optional[RunStatus]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         Run
@@ -535,29 +546,33 @@
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
         await client.run.update_status(
             run_id=1,
-            status="pending",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if status is not OMIT:
+            _request["status"] = status
         _response = await self._client_wrapper.httpx_client.request(
             method="PATCH",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/run/{jsonable_encoder(run_id)}/status"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder({"status": status})
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder({"status": status}),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/run_metric/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/run_metric/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.not_found_error import NotFoundError
 from ..errors.unauthorized_error import UnauthorizedError
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
@@ -54,16 +55,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/run_metric/{jsonable_encoder(run_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -135,16 +138,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/run_metric/{jsonable_encoder(run_id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/score/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/score/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.not_found_error import NotFoundError
 from ..errors.unauthorized_error import UnauthorizedError
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
@@ -41,18 +42,21 @@
     ) -> Grade:
         """
         Create a score
 
         Parameters
         ----------
         run_id : int
+            The ID of the run that created the testrecord to be scored.
 
         testrecord_id : int
+            The ID of the testrecord to be scored.
 
         metric_id : int
+            The ID of the metric
 
         int_score : typing.Optional[int]
 
         binary_score : typing.Optional[bool]
 
         reasoning : typing.Optional[str]
 
@@ -86,16 +90,18 @@
             _request["reasoning"] = reasoning
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/run/{jsonable_encoder(run_id)}/testrecord/{jsonable_encoder(testrecord_id)}/score",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -150,18 +156,21 @@
     ) -> Grade:
         """
         Update a score
 
         Parameters
         ----------
         run_id : int
+            The run ID that created the test record to be scored.
 
         testrecord_id : int
+            The ID of the testrecord whose score will be updated.
 
         score_id : int
+            The ID of the score to be updated.
 
         int_score : typing.Optional[int]
 
         binary_score : typing.Optional[bool]
 
         reasoning : typing.Optional[str]
 
@@ -195,16 +204,18 @@
             _request["reasoning"] = reasoning
         _response = self._client_wrapper.httpx_client.request(
             method="PATCH",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/run/{jsonable_encoder(run_id)}/testrecord/{jsonable_encoder(testrecord_id)}/score/{jsonable_encoder(score_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -264,18 +275,21 @@
     ) -> Grade:
         """
         Create a score
 
         Parameters
         ----------
         run_id : int
+            The ID of the run that created the testrecord to be scored.
 
         testrecord_id : int
+            The ID of the testrecord to be scored.
 
         metric_id : int
+            The ID of the metric
 
         int_score : typing.Optional[int]
 
         binary_score : typing.Optional[bool]
 
         reasoning : typing.Optional[str]
 
@@ -309,16 +323,18 @@
             _request["reasoning"] = reasoning
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/run/{jsonable_encoder(run_id)}/testrecord/{jsonable_encoder(testrecord_id)}/score",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -373,18 +389,21 @@
     ) -> Grade:
         """
         Update a score
 
         Parameters
         ----------
         run_id : int
+            The run ID that created the test record to be scored.
 
         testrecord_id : int
+            The ID of the testrecord whose score will be updated.
 
         score_id : int
+            The ID of the score to be updated.
 
         int_score : typing.Optional[int]
 
         binary_score : typing.Optional[bool]
 
         reasoning : typing.Optional[str]
 
@@ -418,16 +437,18 @@
             _request["reasoning"] = reasoning
         _response = await self._client_wrapper.httpx_client.request(
             method="PATCH",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/run/{jsonable_encoder(run_id)}/testrecord/{jsonable_encoder(testrecord_id)}/score/{jsonable_encoder(score_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/telemetry.py` & `scorecard_ai-1.0.0b3/src/scorecard/telemetry.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/testcase/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/testcase/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.not_found_error import NotFoundError
 from ..errors.unauthorized_error import UnauthorizedError
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
 from ..types.not_found_error_body import NotFoundErrorBody
 from ..types.test_case import TestCase
+from ..types.testcase_deletion_response import TestcaseDeletionResponse
 from ..types.unauthenticated_error import UnauthenticatedError
 from ..types.unauthorized_error_body import UnauthorizedErrorBody
 from .types.testcase_create_params_custom_inputs_value import TestcaseCreateParamsCustomInputsValue
 from .types.testcase_create_params_custom_labels_value import TestcaseCreateParamsCustomLabelsValue
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
@@ -30,29 +32,31 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
         self,
         testset_id: int,
         *,
-        user_query: str,
+        user_query: typing.Optional[str] = OMIT,
         context: typing.Optional[str] = OMIT,
         ideal: typing.Optional[str] = OMIT,
         custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]] = OMIT,
         custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> TestCase:
         """
         Create a new Testcase
 
         Parameters
         ----------
         testset_id : int
+            The ID of the Testset to create the Testcase in.
 
-        user_query : str
+        user_query : typing.Optional[str]
+            The user query to be executed.
 
         context : typing.Optional[str]
 
         ideal : typing.Optional[str]
 
         custom_inputs : typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]]
 
@@ -71,33 +75,36 @@
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
         client.testcase.create(
             testset_id=1,
-            user_query="user_query",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"user_query": user_query}
+        _request: typing.Dict[str, typing.Any] = {}
+        if user_query is not OMIT:
+            _request["user_query"] = user_query
         if context is not OMIT:
             _request["context"] = context
         if ideal is not OMIT:
             _request["ideal"] = ideal
         if custom_inputs is not OMIT:
             _request["custom_inputs"] = custom_inputs
         if custom_labels is not OMIT:
             _request["custom_labels"] = custom_labels
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/testcase"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -144,16 +151,18 @@
     ) -> TestCase:
         """
         Retrieve Testcase data
 
         Parameters
         ----------
         testcase_id : int
+            The ID of the Testcase to retrieve.
 
         testset_id : int
+            The ID of the Testset to retrieve the Testcase from.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         TestCase
@@ -173,16 +182,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/testset/{jsonable_encoder(testset_id)}/testcase/{jsonable_encoder(testcase_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -216,30 +227,32 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(
         self, testcase_id: int, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
+    ) -> TestcaseDeletionResponse:
         """
         Delete a Testcase
 
         Parameters
         ----------
         testcase_id : int
+            The ID of the Testcase to delete.
 
         testset_id : int
+            The ID of the Testset to delete the Testcase from.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        typing.Any
+        TestcaseDeletionResponse
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
@@ -252,17 +265,22 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/testset/{jsonable_encoder(testset_id)}/testcase/{jsonable_encoder(testcase_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -270,15 +288,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            return typing.cast(TestcaseDeletionResponse, construct_type(type_=TestcaseDeletionResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -302,29 +320,31 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create(
         self,
         testset_id: int,
         *,
-        user_query: str,
+        user_query: typing.Optional[str] = OMIT,
         context: typing.Optional[str] = OMIT,
         ideal: typing.Optional[str] = OMIT,
         custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]] = OMIT,
         custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomLabelsValue]]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> TestCase:
         """
         Create a new Testcase
 
         Parameters
         ----------
         testset_id : int
+            The ID of the Testset to create the Testcase in.
 
-        user_query : str
+        user_query : typing.Optional[str]
+            The user query to be executed.
 
         context : typing.Optional[str]
 
         ideal : typing.Optional[str]
 
         custom_inputs : typing.Optional[typing.Dict[str, typing.Optional[TestcaseCreateParamsCustomInputsValue]]]
 
@@ -343,33 +363,36 @@
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
         await client.testcase.create(
             testset_id=1,
-            user_query="user_query",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"user_query": user_query}
+        _request: typing.Dict[str, typing.Any] = {}
+        if user_query is not OMIT:
+            _request["user_query"] = user_query
         if context is not OMIT:
             _request["context"] = context
         if ideal is not OMIT:
             _request["ideal"] = ideal
         if custom_inputs is not OMIT:
             _request["custom_inputs"] = custom_inputs
         if custom_labels is not OMIT:
             _request["custom_labels"] = custom_labels
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/testcase"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -416,16 +439,18 @@
     ) -> TestCase:
         """
         Retrieve Testcase data
 
         Parameters
         ----------
         testcase_id : int
+            The ID of the Testcase to retrieve.
 
         testset_id : int
+            The ID of the Testset to retrieve the Testcase from.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
         TestCase
@@ -445,16 +470,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/testset/{jsonable_encoder(testset_id)}/testcase/{jsonable_encoder(testcase_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -488,30 +515,32 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(
         self, testcase_id: int, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> typing.Any:
+    ) -> TestcaseDeletionResponse:
         """
         Delete a Testcase
 
         Parameters
         ----------
         testcase_id : int
+            The ID of the Testcase to delete.
 
         testset_id : int
+            The ID of the Testset to delete the Testcase from.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        typing.Any
+        TestcaseDeletionResponse
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
@@ -524,17 +553,22 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="DELETE",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/testset/{jsonable_encoder(testset_id)}/testcase/{jsonable_encoder(testcase_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -542,15 +576,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
+            return typing.cast(TestcaseDeletionResponse, construct_type(type_=TestcaseDeletionResponse, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/testrecord/__init__.py` & `scorecard_ai-1.0.0b3/src/scorecard/testrecord/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/testrecord/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/testrecord/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.not_found_error import NotFoundError
 from ..errors.unauthorized_error import UnauthorizedError
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
@@ -67,16 +68,18 @@
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/run/{jsonable_encoder(run_id)}/testrecord/{jsonable_encoder(testrecord_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -140,14 +143,15 @@
     ) -> Testrecord:
         """
         Create a new Testrecord
 
         Parameters
         ----------
         run_id : int
+            The ID of the Run to create the Testrecord in.
 
         testset_id : typing.Optional[int]
 
         testcase_id : typing.Optional[int]
 
         user_query : typing.Optional[str]
 
@@ -214,16 +218,18 @@
         if model_debug_info is not OMIT:
             _request["model_debug_info"] = model_debug_info
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/run/{jsonable_encoder(run_id)}/testrecord"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -304,16 +310,18 @@
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"v1/run/{jsonable_encoder(run_id)}/testrecord/{jsonable_encoder(testrecord_id)}",
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -377,14 +385,15 @@
     ) -> Testrecord:
         """
         Create a new Testrecord
 
         Parameters
         ----------
         run_id : int
+            The ID of the Run to create the Testrecord in.
 
         testset_id : typing.Optional[int]
 
         testcase_id : typing.Optional[int]
 
         user_query : typing.Optional[str]
 
@@ -451,16 +460,18 @@
         if model_debug_info is not OMIT:
             _request["model_debug_info"] = model_debug_info
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/run/{jsonable_encoder(run_id)}/testrecord"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/testrecord/types/__init__.py` & `scorecard_ai-1.0.0b3/src/scorecard/testrecord/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/testset/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/prompt/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,72 +3,121 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.not_found_error import NotFoundError
 from ..errors.unauthorized_error import UnauthorizedError
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
-from ..types.custom_schema import CustomSchema
 from ..types.http_validation_error import HttpValidationError
 from ..types.not_found_error_body import NotFoundErrorBody
-from ..types.paginated_testcase_response import PaginatedTestcaseResponse
-from ..types.testset import Testset
+from ..types.prompt import Prompt
 from ..types.unauthenticated_error import UnauthenticatedError
 from ..types.unauthorized_error_body import UnauthorizedErrorBody
+from .types.prompt_create_params_model_params_value import PromptCreateParamsModelParamsValue
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class TestsetClient:
+class PromptClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> Testset:
+    def create(
+        self,
+        *,
+        prompt_template: str,
+        name: typing.Optional[str] = OMIT,
+        parent_id: typing.Optional[str] = OMIT,
+        description: typing.Optional[str] = OMIT,
+        model_params: typing.Optional[typing.Dict[str, typing.Optional[PromptCreateParamsModelParamsValue]]] = OMIT,
+        is_prod: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> Prompt:
         """
-        Retrieve Testset metadata without Testcase data
+        Two types of prompts can be created - a root prompt or a child prompt (aka Prompt Version in app).
+
+                A root prompt can be created by providing the `name` param, and it will always be tagged as prod.
+
+                A child prompt can be created by providing the `parent_id` param. Note that the `name` param in this case will be ignored as all descendents from a root prompt would share the root's name. `is_prod` can also be provided to configure whether a child should be tagged as prod.
 
         Parameters
         ----------
-        testset_id : int
+        prompt_template : str
+
+        name : typing.Optional[str]
+
+        parent_id : typing.Optional[str]
+
+        description : typing.Optional[str]
+
+        model_params : typing.Optional[typing.Dict[str, typing.Optional[PromptCreateParamsModelParamsValue]]]
+
+        is_prod : typing.Optional[bool]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Testset
+        Prompt
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.testset.get(
-            testset_id=1,
+        client.prompt.create(
+            prompt_template="<system>\nYou are a helpful assistant. Use the provided context to answer the user's query.\n\nContext: {context}\n</system>\n\n<user>\n{user_query}\n</user>",
+            name="Prompt Name",
+            description="Description of the prompt",
+            model_params={
+                "param1": "value1",
+                "param2": 0.1,
+                "param3": 100,
+                "param4": True,
+            },
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"prompt_template": prompt_template}
+        if name is not OMIT:
+            _request["name"] = name
+        if parent_id is not OMIT:
+            _request["parent_id"] = parent_id
+        if description is not OMIT:
+            _request["description"] = description
+        if model_params is not OMIT:
+            _request["model_params"] = model_params
+        if is_prod is not OMIT:
+            _request["is_prod"] = is_prod
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/prompt"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -76,15 +125,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
+            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -99,48 +148,49 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> Testset:
+    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Prompt:
         """
-        Delete a Testset
+        Retrieve a prompt by id
 
         Parameters
         ----------
-        testset_id : int
+        id : str
+            The id of the prompt to get.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Testset
+        Prompt
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.testset.delete(
-            testset_id=1,
+        client.prompt.get(
+            id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            method="DELETE",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -149,15 +199,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
+            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -172,74 +222,53 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(
-        self,
-        *,
-        name: str,
-        description: typing.Optional[str] = OMIT,
-        using_retrieval: typing.Optional[bool] = OMIT,
-        custom_schema: typing.Optional[CustomSchema] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> Testset:
+    def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
-        Create a new Testset
+        Delete a root prompt and all of its children.
 
         Parameters
         ----------
-        name : str
-
-        description : typing.Optional[str]
-
-        using_retrieval : typing.Optional[bool]
-
-        custom_schema : typing.Optional[CustomSchema]
+        id : str
+            The id of the root prompt to delete.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Testset
+        typing.Any
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.testset.create(
-            name="name",
+        client.prompt.delete(
+            id="id",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if description is not OMIT:
-            _request["description"] = description
-        if using_retrieval is not OMIT:
-            _request["using_retrieval"] = using_retrieval
-        if custom_schema is not OMIT:
-            _request["custom_schema"] = custom_schema
         _response = self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/testset"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -247,15 +276,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -270,49 +299,66 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def read_schema(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> CustomSchema:
+    def update(
+        self, id: str, *, is_prod: typing.Optional[bool] = OMIT, request_options: typing.Optional[RequestOptions] = None
+    ) -> Prompt:
         """
-        Read the schema of a Testset
+        Update a prompt.
+
+                `is_prod` tags the provided prompt as the production prompt within the prompt graph.
 
         Parameters
         ----------
-        testset_id : int
+        id : str
+            The id of the prompt to update.
+
+        is_prod : typing.Optional[bool]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        CustomSchema
+        Prompt
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.testset.read_schema(
-            testset_id=1,
+        client.prompt.update(
+            id="id",
+            is_prod=True,
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if is_prod is not OMIT:
+            _request["is_prod"] = is_prod
         _response = self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/schema"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PATCH",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -320,15 +366,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(CustomSchema, construct_type(type_=CustomSchema, object_=_response.json()))  # type: ignore
+            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -343,68 +389,50 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_testcases(
-        self,
-        testset_id: int,
-        *,
-        offset: typing.Optional[int] = None,
-        limit: typing.Optional[int] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> PaginatedTestcaseResponse:
+    def get_by_name(self, name: str, *, request_options: typing.Optional[RequestOptions] = None) -> Prompt:
         """
-        Retrieve all Testcases from a Testset
+        Retrieve a prod prompt by name
 
         Parameters
         ----------
-        testset_id : int
-
-        offset : typing.Optional[int]
-
-        limit : typing.Optional[int]
+        name : str
+            Name of the prompt.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        PaginatedTestcaseResponse
+        Prompt
             Successful Response
 
         Examples
         --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
-        client.testset.get_testcases(
-            testset_id=1,
+        client.prompt.get_by_name(
+            name="name",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/testcase"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/name/{jsonable_encoder(name)}"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "offset": offset,
-                        "limit": limit,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -414,15 +442,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(PaginatedTestcaseResponse, construct_type(type_=PaginatedTestcaseResponse, object_=_response.json()))  # type: ignore
+            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -438,53 +466,102 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTestsetClient:
+class AsyncPromptClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> Testset:
+    async def create(
+        self,
+        *,
+        prompt_template: str,
+        name: typing.Optional[str] = OMIT,
+        parent_id: typing.Optional[str] = OMIT,
+        description: typing.Optional[str] = OMIT,
+        model_params: typing.Optional[typing.Dict[str, typing.Optional[PromptCreateParamsModelParamsValue]]] = OMIT,
+        is_prod: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> Prompt:
         """
-        Retrieve Testset metadata without Testcase data
+        Two types of prompts can be created - a root prompt or a child prompt (aka Prompt Version in app).
+
+                A root prompt can be created by providing the `name` param, and it will always be tagged as prod.
+
+                A child prompt can be created by providing the `parent_id` param. Note that the `name` param in this case will be ignored as all descendents from a root prompt would share the root's name. `is_prod` can also be provided to configure whether a child should be tagged as prod.
 
         Parameters
         ----------
-        testset_id : int
+        prompt_template : str
+
+        name : typing.Optional[str]
+
+        parent_id : typing.Optional[str]
+
+        description : typing.Optional[str]
+
+        model_params : typing.Optional[typing.Dict[str, typing.Optional[PromptCreateParamsModelParamsValue]]]
+
+        is_prod : typing.Optional[bool]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Testset
+        Prompt
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.testset.get(
-            testset_id=1,
+        await client.prompt.create(
+            prompt_template="<system>\nYou are a helpful assistant. Use the provided context to answer the user's query.\n\nContext: {context}\n</system>\n\n<user>\n{user_query}\n</user>",
+            name="Prompt Name",
+            description="Description of the prompt",
+            model_params={
+                "param1": "value1",
+                "param2": 0.1,
+                "param3": 100,
+                "param4": True,
+            },
         )
         """
+        _request: typing.Dict[str, typing.Any] = {"prompt_template": prompt_template}
+        if name is not OMIT:
+            _request["name"] = name
+        if parent_id is not OMIT:
+            _request["parent_id"] = parent_id
+        if description is not OMIT:
+            _request["description"] = description
+        if model_params is not OMIT:
+            _request["model_params"] = model_params
+        if is_prod is not OMIT:
+            _request["is_prod"] = is_prod
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/prompt"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -492,15 +569,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
+            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -515,48 +592,49 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None) -> Testset:
+    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Prompt:
         """
-        Delete a Testset
+        Retrieve a prompt by id
 
         Parameters
         ----------
-        testset_id : int
+        id : str
+            The id of the prompt to get.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Testset
+        Prompt
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.testset.delete(
-            testset_id=1,
+        await client.prompt.get(
+            id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            method="DELETE",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -565,15 +643,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
+            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -588,74 +666,53 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(
-        self,
-        *,
-        name: str,
-        description: typing.Optional[str] = OMIT,
-        using_retrieval: typing.Optional[bool] = OMIT,
-        custom_schema: typing.Optional[CustomSchema] = OMIT,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> Testset:
+    async def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> typing.Any:
         """
-        Create a new Testset
+        Delete a root prompt and all of its children.
 
         Parameters
         ----------
-        name : str
-
-        description : typing.Optional[str]
-
-        using_retrieval : typing.Optional[bool]
-
-        custom_schema : typing.Optional[CustomSchema]
+        id : str
+            The id of the root prompt to delete.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        Testset
+        typing.Any
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.testset.create(
-            name="name",
+        await client.prompt.delete(
+            id="id",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if description is not OMIT:
-            _request["description"] = description
-        if using_retrieval is not OMIT:
-            _request["using_retrieval"] = using_retrieval
-        if custom_schema is not OMIT:
-            _request["custom_schema"] = custom_schema
         _response = await self._client_wrapper.httpx_client.request(
-            method="POST",
-            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/testset"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
-            json=jsonable_encoder(_request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(_request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -663,15 +720,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(Testset, construct_type(type_=Testset, object_=_response.json()))  # type: ignore
+            return typing.cast(typing.Any, construct_type(type_=typing.Any, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -686,51 +743,66 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def read_schema(
-        self, testset_id: int, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> CustomSchema:
+    async def update(
+        self, id: str, *, is_prod: typing.Optional[bool] = OMIT, request_options: typing.Optional[RequestOptions] = None
+    ) -> Prompt:
         """
-        Read the schema of a Testset
+        Update a prompt.
+
+                `is_prod` tags the provided prompt as the production prompt within the prompt graph.
 
         Parameters
         ----------
-        testset_id : int
+        id : str
+            The id of the prompt to update.
+
+        is_prod : typing.Optional[bool]
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        CustomSchema
+        Prompt
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.testset.read_schema(
-            testset_id=1,
+        await client.prompt.update(
+            id="id",
+            is_prod=True,
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if is_prod is not OMIT:
+            _request["is_prod"] = is_prod
         _response = await self._client_wrapper.httpx_client.request(
-            method="GET",
-            url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/schema"
-            ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PATCH",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
@@ -738,15 +810,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(CustomSchema, construct_type(type_=CustomSchema, object_=_response.json()))  # type: ignore
+            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
@@ -761,68 +833,50 @@
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_testcases(
-        self,
-        testset_id: int,
-        *,
-        offset: typing.Optional[int] = None,
-        limit: typing.Optional[int] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> PaginatedTestcaseResponse:
+    async def get_by_name(self, name: str, *, request_options: typing.Optional[RequestOptions] = None) -> Prompt:
         """
-        Retrieve all Testcases from a Testset
+        Retrieve a prod prompt by name
 
         Parameters
         ----------
-        testset_id : int
-
-        offset : typing.Optional[int]
-
-        limit : typing.Optional[int]
+        name : str
+            Name of the prompt.
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        PaginatedTestcaseResponse
+        Prompt
             Successful Response
 
         Examples
         --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
-        await client.testset.get_testcases(
-            testset_id=1,
+        await client.prompt.get_by_name(
+            name="name",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/testset/{jsonable_encoder(testset_id)}/testcase"
+                f"{self._client_wrapper.get_base_url()}/", f"v1/prompt/name/{jsonable_encoder(name)}"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "offset": offset,
-                        "limit": limit,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -832,15 +886,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return typing.cast(PaginatedTestcaseResponse, construct_type(type_=PaginatedTestcaseResponse, object_=_response.json()))  # type: ignore
+            return typing.cast(Prompt, construct_type(type_=Prompt, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
             )
         if _response.status_code == 403:
             raise ForbiddenError(
                 typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/traces/client.py` & `scorecard_ai-1.0.0b3/src/scorecard/traces/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.not_found_error import NotFoundError
 from ..errors.unauthorized_error import UnauthorizedError
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
@@ -54,16 +55,18 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/traces/{jsonable_encoder(trace_id)}/spans"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -133,16 +136,18 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/traces/{jsonable_encoder(trace_id)}/spans"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/__init__.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .span import Span
 from .test_case import TestCase
 from .test_case_create import TestCaseCreate
 from .test_case_custom_inputs_value import TestCaseCustomInputsValue
 from .test_case_custom_labels_value import TestCaseCustomLabelsValue
 from .test_record_create import TestRecordCreate
 from .test_set_create import TestSetCreate
+from .testcase_deletion_response import TestcaseDeletionResponse
 from .testrecord import Testrecord
 from .testrecord_custom_inputs_value import TestrecordCustomInputsValue
 from .testrecord_custom_labels_value import TestrecordCustomLabelsValue
 from .testrecord_custom_outputs_value import TestrecordCustomOutputsValue
 from .testrecord_model_debug_info_value import TestrecordModelDebugInfoValue
 from .testrecord_model_params_value import TestrecordModelParamsValue
 from .testset import Testset
@@ -64,14 +65,15 @@
     "Span",
     "TestCase",
     "TestCaseCreate",
     "TestCaseCustomInputsValue",
     "TestCaseCustomLabelsValue",
     "TestRecordCreate",
     "TestSetCreate",
+    "TestcaseDeletionResponse",
     "Testrecord",
     "TestrecordCustomInputsValue",
     "TestrecordCustomLabelsValue",
     "TestrecordCustomOutputsValue",
     "TestrecordModelDebugInfoValue",
     "TestrecordModelParamsValue",
     "Testset",
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/custom_schema.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/custom_variable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .custom_variable import CustomVariable
+from .data_type_enum import DataTypeEnum
+from .role_enum import RoleEnum
 
 
-class CustomSchema(UncheckedBaseModel):
+class CustomVariable(UncheckedBaseModel):
     """
-    Custom schema model with an ordered list of custom variables.
+    Custom variable model with name, description, role and data type.
     """
 
-    variables: typing.Optional[typing.List[CustomVariable]] = pydantic_v1.Field(default=None)
-    """
-    Ordered list of custom variables
-    """
+    name: str
+    description: typing.Optional[str] = None
+    role: RoleEnum
+    data_type: DataTypeEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/custom_variable.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/file_url.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .data_type_enum import DataTypeEnum
-from .role_enum import RoleEnum
 
 
-class CustomVariable(UncheckedBaseModel):
+class FileUrl(UncheckedBaseModel):
     """
-    Custom variable model with name, description, role and data type.
+    File model with url and name.
     """
 
-    name: str
-    description: typing.Optional[str] = None
-    role: RoleEnum
-    data_type: DataTypeEnum
+    url: str
+    name: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/file_url.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/testcase_deletion_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class FileUrl(UncheckedBaseModel):
+class TestcaseDeletionResponse(UncheckedBaseModel):
+    id: int = pydantic_v1.Field()
     """
-    File model with url and name.
+    The ID of the testcase that was deleted.
     """
 
-    url: str
-    name: typing.Optional[str] = None
+    detail: str = pydantic_v1.Field()
+    """
+    The message indicating the testcase was deleted.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/grade.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .score_status import ScoreStatus
 
 
-class Grade(UncheckedBaseModel):
-    user_id: typing.Optional[str] = None
+class Run(UncheckedBaseModel):
     id: typing.Optional[int] = None
-    run_id: typing.Optional[int] = None
-    testcase_id: typing.Optional[int] = None
-    testrecord_id: typing.Optional[int] = None
-    metric_id: typing.Optional[int] = None
-    binary_score: typing.Optional[bool] = None
-    int_score: typing.Optional[int] = None
-    reasoning: typing.Optional[str] = None
-    human_eval: typing.Optional[bool] = None
-    status: typing.Optional[ScoreStatus] = None
-    error_message: typing.Optional[str] = None
     created_at: typing.Optional[dt.datetime] = None
     updated_at: typing.Optional[dt.datetime] = None
+    execution_start_time: typing.Optional[dt.datetime] = None
+    execution_end_time: typing.Optional[dt.datetime] = None
+    testset_id: typing.Optional[int] = None
+    status: typing.Optional[str] = None
+    limit_testcases: typing.Optional[int] = None
+    source: typing.Optional[str] = None
+    model_params: typing.Optional[typing.Dict[str, typing.Any]] = None
+    notes: typing.Optional[str] = None
+    scoring_config_id: typing.Optional[int] = None
+    prompt_template: typing.Optional[str] = None
+    scoring_start_time: typing.Optional[dt.datetime] = None
+    scoring_end_time: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/http_validation_error.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/test_case_create.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .validation_error import ValidationError
 
 
-class HttpValidationError(UncheckedBaseModel):
-    detail: typing.Optional[typing.List[ValidationError]] = None
+class TestCaseCreate(UncheckedBaseModel):
+    testset_id: int
+    user_query: str
+    context: typing.Optional[str] = None
+    response: typing.Optional[str] = None
+    ideal: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/json_object.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/paginated_testcase_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .test_case import TestCase
 
 
-class JsonObject(UncheckedBaseModel):
-    value: typing.Optional[JsonObjectOutputValue] = pydantic_v1.Field(default=None)
+class PaginatedTestcaseResponse(UncheckedBaseModel):
+    count: int
+    next: typing.Optional[str] = None
+    previous: typing.Optional[str] = None
+    results: typing.List[TestCase] = pydantic_v1.Field()
     """
-    The value of the JSON object, which can be a dictionary, list, string, integer, float, boolean, or None.
+    The list of Testcases retrieved in this page.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .json_object_output_value import JsonObjectOutputValue  # noqa: E402
-
-JsonObject.update_forward_refs()
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/not_found_error_body.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/run_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class NotFoundErrorBody(UncheckedBaseModel):
-    error: typing.Optional[str] = None
-    error_description: typing.Optional[str] = None
-    status_code: typing.Optional[int] = None
+class RunMetric(UncheckedBaseModel):
+    id: typing.Optional[int] = None
+    run_id: typing.Optional[int] = None
+    metric_id: typing.Optional[int] = None
+    created_at: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/paginated_testcase_response.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/unauthorized_error_body.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .test_case import TestCase
 
 
-class PaginatedTestcaseResponse(UncheckedBaseModel):
-    count: int
-    next: typing.Optional[str] = None
-    previous: typing.Optional[str] = None
-    results: typing.List[TestCase]
+class UnauthorizedErrorBody(UncheckedBaseModel):
+    error: typing.Optional[str] = None
+    error_description: typing.Optional[str] = None
+    status_code: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/prompt.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .prompt_model_params_value import PromptModelParamsValue
 
 
 class Prompt(UncheckedBaseModel):
     org_id: typing.Optional[str] = None
     user_id: typing.Optional[str] = None
@@ -24,15 +24,19 @@
     created_at: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/run.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/grade.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,52 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .score_status import ScoreStatus
 
 
-class Run(UncheckedBaseModel):
+class Grade(UncheckedBaseModel):
+    user_id: typing.Optional[str] = None
     id: typing.Optional[int] = None
+    run_id: typing.Optional[int] = None
+    testcase_id: typing.Optional[int] = None
+    testrecord_id: typing.Optional[int] = None
+    metric_id: typing.Optional[int] = None
+    binary_score: typing.Optional[bool] = None
+    int_score: typing.Optional[int] = None
+    reasoning: typing.Optional[str] = None
+    human_eval: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    Indicates if a human should assign a grade.
+    """
+
+    status: typing.Optional[ScoreStatus] = pydantic_v1.Field(default=None)
+    """
+    The status of the grade.
+    """
+
+    error_message: typing.Optional[str] = None
     created_at: typing.Optional[dt.datetime] = None
     updated_at: typing.Optional[dt.datetime] = None
-    execution_start_time: typing.Optional[dt.datetime] = None
-    execution_end_time: typing.Optional[dt.datetime] = None
-    testset_id: typing.Optional[int] = None
-    status: typing.Optional[str] = None
-    limit_testcases: typing.Optional[int] = None
-    source: typing.Optional[str] = None
-    model_params: typing.Optional[typing.Dict[str, typing.Any]] = None
-    notes: typing.Optional[str] = None
-    scoring_config_id: typing.Optional[int] = None
-    prompt_template: typing.Optional[str] = None
-    scoring_start_time: typing.Optional[dt.datetime] = None
-    scoring_end_time: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/run_metric.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/not_found_error_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class RunMetric(UncheckedBaseModel):
-    id: typing.Optional[int] = None
-    run_id: typing.Optional[int] = None
-    metric_id: typing.Optional[int] = None
-    created_at: typing.Optional[dt.datetime] = None
+class NotFoundErrorBody(UncheckedBaseModel):
+    error: typing.Optional[str] = None
+    error_description: typing.Optional[str] = None
+    status_code: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/span.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/span.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class Span(UncheckedBaseModel):
     children: typing.List[Span] = pydantic_v1.Field(alias="Children")
     timestamp: dt.datetime = pydantic_v1.Field(alias="Timestamp")
     trace_id: str = pydantic_v1.Field(alias="TraceId")
@@ -36,16 +36,20 @@
     links_attributes: typing.List[typing.Dict[str, str]] = pydantic_v1.Field(alias="Links.Attributes")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/test_case.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/test_case.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .test_case_custom_inputs_value import TestCaseCustomInputsValue
 from .test_case_custom_labels_value import TestCaseCustomLabelsValue
 
 
 class TestCase(UncheckedBaseModel):
     id: typing.Optional[int] = None
     created_at: typing.Optional[dt.datetime] = None
-    testset_id: int
-    user_query: str
+    testset_id: int = pydantic_v1.Field()
+    """
+    The ID of the testset the testcase belongs to.
+    """
+
+    user_query: str = pydantic_v1.Field()
+    """
+    The user query for the testcase.
+    """
+
     context: typing.Optional[str] = None
     ideal: typing.Optional[str] = None
     custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestCaseCustomInputsValue]]] = None
     custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestCaseCustomLabelsValue]]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/test_case_create.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/unauthenticated_error.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class TestCaseCreate(UncheckedBaseModel):
-    testset_id: int
-    user_query: str
-    context: typing.Optional[str] = None
-    response: typing.Optional[str] = None
-    ideal: typing.Optional[str] = None
+class UnauthenticatedError(UncheckedBaseModel):
+    error: typing.Optional[str] = None
+    error_description: typing.Optional[str] = None
+    status_code: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/testrecord.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/testrecord.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .testrecord_custom_inputs_value import TestrecordCustomInputsValue
 from .testrecord_custom_labels_value import TestrecordCustomLabelsValue
 from .testrecord_custom_outputs_value import TestrecordCustomOutputsValue
 from .testrecord_model_debug_info_value import TestrecordModelDebugInfoValue
 from .testrecord_model_params_value import TestrecordModelParamsValue
 
@@ -19,29 +19,32 @@
     run_id: typing.Optional[int] = None
     testset_id: typing.Optional[int] = None
     testcase_id: typing.Optional[int] = None
     user_query: typing.Optional[str] = None
     context: typing.Optional[str] = None
     model_response: typing.Optional[str] = None
     ideal: typing.Optional[str] = None
-    full_prompt: typing.Optional[str] = None
     custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomInputsValue]]] = None
     custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomLabelsValue]]] = None
     custom_outputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomOutputsValue]]] = None
     status: typing.Optional[str] = None
     prompt: typing.Optional[str] = None
     model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordModelParamsValue]]] = None
     model_debug_info: typing.Optional[typing.Dict[str, typing.Optional[TestrecordModelDebugInfoValue]]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/testset.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/testset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .custom_schema import CustomSchema
 
 
 class Testset(UncheckedBaseModel):
     id: typing.Optional[int] = None
     created_at: typing.Optional[dt.datetime] = None
@@ -24,15 +24,19 @@
     custom_schema: typing.Optional[CustomSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/trace.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/trace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class Trace(UncheckedBaseModel):
     trace_id: str = pydantic_v1.Field(alias="TraceId")
     start: dt.datetime = pydantic_v1.Field(alias="Start")
     end: dt.datetime = pydantic_v1.Field(alias="End")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/unauthenticated_error.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/custom_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .custom_variable import CustomVariable
 
 
-class UnauthenticatedError(UncheckedBaseModel):
-    error: typing.Optional[str] = None
-    error_description: typing.Optional[str] = None
-    status_code: typing.Optional[int] = None
+class CustomSchema(UncheckedBaseModel):
+    """
+    Custom schema model with an ordered list of custom variables.
+    """
+
+    variables: typing.Optional[typing.List[CustomVariable]] = pydantic_v1.Field(default=None)
+    """
+    Ordered list of custom variables
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/unauthorized_error_body.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/validation_error.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class UnauthorizedErrorBody(UncheckedBaseModel):
-    error: typing.Optional[str] = None
-    error_description: typing.Optional[str] = None
-    status_code: typing.Optional[int] = None
+class ValidationError(UncheckedBaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/src/scorecard/types/validation_error.py` & `scorecard_ai-1.0.0b3/src/scorecard/types/http_validation_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .validation_error_loc_item import ValidationErrorLocItem
+from .validation_error import ValidationError
 
 
-class ValidationError(UncheckedBaseModel):
-    loc: typing.List[ValidationErrorLocItem]
-    msg: str
-    type: str
+class HttpValidationError(UncheckedBaseModel):
+    detail: typing.Optional[typing.List[ValidationError]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-1.0.0b2/PKG-INFO` & `scorecard_ai-1.0.0b3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 Metadata-Version: 2.1
 Name: scorecard-ai
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: 
 License: Apache-2.0
 Requires-Python: >=3.9,<3.13
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Dist: boto3 (>=1.34.100,<2.0.0)
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: openai (>=1.21.2,<2.0.0)
 Requires-Dist: openinference-instrumentation-bedrock (>=0.1.3,<0.2.0)
 Requires-Dist: openinference-instrumentation-dspy (>=0.1.7,<0.2.0)
 Requires-Dist: openinference-instrumentation-langchain (>=0.1.14,<0.2.0)
 Requires-Dist: openinference-instrumentation-llama-index (>=1.3.0,<2.0.0)
```

