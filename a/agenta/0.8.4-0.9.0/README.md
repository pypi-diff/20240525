# Comparing `tmp/agenta-0.8.4.tar.gz` & `tmp/agenta-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenta-0.8.4.tar", max compression
+gzip compressed data, was "agenta-0.9.0.tar", max compression
```

## Comparing `agenta-0.8.4.tar` & `agenta-0.9.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    26017 2024-01-27 12:45:44.608032 agenta-0.8.4/README.md
--rw-r--r--   0        0        0      493 2024-01-27 12:45:44.608032 agenta-0.8.4/agenta/__init__.py
--rw-r--r--   0        0        0      474 2024-01-27 12:45:44.608032 agenta-0.8.4/agenta/cli/evaluation_commands.py
--rw-r--r--   0        0        0     6199 2024-01-27 12:45:44.608032 agenta-0.8.4/agenta/cli/helper.py
--rw-r--r--   0        0        0     7599 2024-01-27 12:45:44.608032 agenta-0.8.4/agenta/cli/main.py
--rw-r--r--   0        0        0     1317 2024-01-27 12:45:44.608032 agenta-0.8.4/agenta/cli/telemetry.py
--rw-r--r--   0        0        0    16858 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/cli/variant_commands.py
--rw-r--r--   0        0        0     1293 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/cli/variant_configs.py
--rw-r--r--   0        0        0     2756 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/__init__.py
--rw-r--r--   0        0        0     2429 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/api.py
--rw-r--r--   0        0        0      623 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/api_models.py
--rw-r--r--   0        0        0     2246 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/__init__.py
--rw-r--r--   0        0        0   223416 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/client.py
--rw-r--r--   0        0        0      519 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/core/__init__.py
--rw-r--r--   0        0        0      440 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/core/api_error.py
--rw-r--r--   0        0        0      972 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/core/datetime_utils.py
--rw-r--r--   0        0        0     3825 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      170 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     3345 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/__init__.py
--rw-r--r--   0        0        0      211 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/add_variant_from_base_and_config_response.py
--rw-r--r--   0        0        0      974 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/app.py
--rw-r--r--   0        0        0     1287 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/app_variant_output.py
--rw-r--r--   0        0        0      983 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/base_output.py
--rw-r--r--   0        0        0     1061 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/body_import_testset.py
--rw-r--r--   0        0        0      182 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/container_templates_response.py
--rw-r--r--   0        0        0      986 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/create_app_output.py
--rw-r--r--   0        0        0     1021 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/create_custom_evaluation.py
--rw-r--r--   0        0        0     1089 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/custom_evaluation_detail.py
--rw-r--r--   0        0        0      995 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/custom_evaluation_names.py
--rw-r--r--   0        0        0     1040 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/custom_evaluation_output.py
--rw-r--r--   0        0        0      986 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/docker_env_vars.py
--rw-r--r--   0        0        0     1082 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/environment_output.py
--rw-r--r--   0        0        0     1410 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation.py
--rw-r--r--   0        0        0     1527 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_scenario.py
--rw-r--r--   0        0        0     1001 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_scenario_input.py
--rw-r--r--   0        0        0     1005 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_scenario_output.py
--rw-r--r--   0        0        0      129 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_scenario_score.py
--rw-r--r--   0        0        0      135 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_scenario_update_score.py
--rw-r--r--   0        0        0     1127 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_status_enum.py
--rw-r--r--   0        0        0     1972 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_type.py
--rw-r--r--   0        0        0     1287 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_type_settings.py
--rw-r--r--   0        0        0      971 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/evaluation_webhook.py
--rw-r--r--   0        0        0     1136 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/feedback.py
--rw-r--r--   0        0        0     1063 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/get_config_reponse.py
--rw-r--r--   0        0        0     1060 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/http_validation_error.py
--rw-r--r--   0        0        0     1048 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/image.py
--rw-r--r--   0        0        0      965 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/invite_request.py
--rw-r--r--   0        0        0     1095 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/list_api_keys_output.py
--rw-r--r--   0        0        0     1009 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/new_testset.py
--rw-r--r--   0        0        0     1181 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/organization.py
--rw-r--r--   0        0        0      981 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/organization_output.py
--rw-r--r--   0        0        0     1117 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/simple_evaluation_output.py
--rw-r--r--   0        0        0     1546 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/span.py
--rw-r--r--   0        0        0     1037 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/template.py
--rw-r--r--   0        0        0     1189 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/template_image_info.py
--rw-r--r--   0        0        0     1088 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/test_set_output_response.py
--rw-r--r--   0        0        0     1004 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/test_set_simple_response.py
--rw-r--r--   0        0        0     1353 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/trace.py
--rw-r--r--   0        0        0      953 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/uri.py
--rw-r--r--   0        0        0     1086 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1031 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/variant_action.py
--rw-r--r--   0        0        0      511 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/backend/types/variant_action_enum.py
--rw-r--r--   0        0        0    19648 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/client.py
--rw-r--r--   0        0        0       94 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/client/exceptions.py
--rw-r--r--   0        0        0      732 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/config.py
--rw-r--r--   0        0        0      223 2024-01-27 12:45:44.612032 agenta-0.8.4/agenta/config.toml
--rw-r--r--   0        0        0      317 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/docker/docker-assets/Dockerfile.cloud.template
--rw-r--r--   0        0        0      285 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/docker/docker-assets/README.md
--rwxr-xr-x   0        0        0       74 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/docker/docker-assets/entrypoint.sh
--rw-r--r--   0        0        0       83 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/docker/docker-assets/lambda_function.py
--rw-r--r--   0        0        0      327 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     3542 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      565 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/__init__.py
--rw-r--r--   0        0        0    15429 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/agenta_decorator.py
--rw-r--r--   0        0        0     7792 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/agenta_init.py
--rw-r--r--   0        0        0      901 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/context.py
--rw-r--r--   0        0        0      269 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/router.py
--rw-r--r--   0        0        0     4658 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/types.py
--rw-r--r--   0        0        0      360 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/utils/globals.py
--rw-r--r--   0        0        0     5877 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/utils/helper/openai_cost.py
--rw-r--r--   0        0        0     1278 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/sdk/utils/preinit.py
--rw-r--r--   0        0        0      308 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/compose_email/README.md
--rw-r--r--   0        0        0     2384 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/compose_email/app.py
--rw-r--r--   0        0        0       70 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/compose_email/env.example
--rw-r--r--   0        0        0       23 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/compose_email/requirements.txt
--rw-r--r--   0        0        0       47 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/compose_email/template.toml
--rw-r--r--   0        0        0      308 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/extract_data_to_json/README.md
--rw-r--r--   0        0        0     1320 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/extract_data_to_json/app.py
--rw-r--r--   0        0        0       70 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/extract_data_to_json/env.example
--rw-r--r--   0        0        0       23 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/extract_data_to_json/requirements.txt
--rw-r--r--   0        0        0       60 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/extract_data_to_json/template.toml
--rw-r--r--   0        0        0      308 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      646 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       70 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/simple_prompt/env.example
--rw-r--r--   0        0        0       23 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2024-01-27 12:45:44.616032 agenta-0.8.4/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0     1041 2024-01-27 12:45:44.616032 agenta-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    27295 1970-01-01 00:00:00.000000 agenta-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0    26017 2024-01-29 22:04:11.437783 agenta-0.9.0/README.md
+-rw-r--r--   0        0        0      493 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/__init__.py
+-rw-r--r--   0        0        0      474 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/cli/evaluation_commands.py
+-rw-r--r--   0        0        0     6199 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/cli/helper.py
+-rw-r--r--   0        0        0     7599 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/cli/main.py
+-rw-r--r--   0        0        0     1317 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/cli/telemetry.py
+-rw-r--r--   0        0        0    16858 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/cli/variant_commands.py
+-rw-r--r--   0        0        0     1293 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/cli/variant_configs.py
+-rw-r--r--   0        0        0     2756 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/__init__.py
+-rw-r--r--   0        0        0     2429 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/api.py
+-rw-r--r--   0        0        0      623 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/api_models.py
+-rw-r--r--   0        0        0     2246 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/__init__.py
+-rw-r--r--   0        0        0   223416 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/client.py
+-rw-r--r--   0        0        0      519 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/core/datetime_utils.py
+-rw-r--r--   0        0        0     3825 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      170 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     3345 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/__init__.py
+-rw-r--r--   0        0        0      211 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/add_variant_from_base_and_config_response.py
+-rw-r--r--   0        0        0      974 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/app.py
+-rw-r--r--   0        0        0     1287 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/app_variant_output.py
+-rw-r--r--   0        0        0      983 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/base_output.py
+-rw-r--r--   0        0        0     1061 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/body_import_testset.py
+-rw-r--r--   0        0        0      182 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/container_templates_response.py
+-rw-r--r--   0        0        0      986 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/create_app_output.py
+-rw-r--r--   0        0        0     1021 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/create_custom_evaluation.py
+-rw-r--r--   0        0        0     1089 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/custom_evaluation_detail.py
+-rw-r--r--   0        0        0      995 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/custom_evaluation_names.py
+-rw-r--r--   0        0        0     1040 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/custom_evaluation_output.py
+-rw-r--r--   0        0        0      986 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/docker_env_vars.py
+-rw-r--r--   0        0        0     1082 2024-01-29 22:04:11.437783 agenta-0.9.0/agenta/client/backend/types/environment_output.py
+-rw-r--r--   0        0        0     1410 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation.py
+-rw-r--r--   0        0        0     1527 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_scenario.py
+-rw-r--r--   0        0        0     1001 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_scenario_input.py
+-rw-r--r--   0        0        0     1005 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_scenario_output.py
+-rw-r--r--   0        0        0      129 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_scenario_score.py
+-rw-r--r--   0        0        0      135 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_scenario_update_score.py
+-rw-r--r--   0        0        0     1127 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_status_enum.py
+-rw-r--r--   0        0        0     1972 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_type.py
+-rw-r--r--   0        0        0     1287 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_type_settings.py
+-rw-r--r--   0        0        0      971 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/evaluation_webhook.py
+-rw-r--r--   0        0        0     1136 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/feedback.py
+-rw-r--r--   0        0        0     1063 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/get_config_reponse.py
+-rw-r--r--   0        0        0     1060 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/http_validation_error.py
+-rw-r--r--   0        0        0     1048 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/image.py
+-rw-r--r--   0        0        0      965 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/invite_request.py
+-rw-r--r--   0        0        0     1095 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/list_api_keys_output.py
+-rw-r--r--   0        0        0     1009 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/new_testset.py
+-rw-r--r--   0        0        0     1181 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/organization.py
+-rw-r--r--   0        0        0      981 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/organization_output.py
+-rw-r--r--   0        0        0     1117 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/simple_evaluation_output.py
+-rw-r--r--   0        0        0     1546 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/span.py
+-rw-r--r--   0        0        0     1037 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/template.py
+-rw-r--r--   0        0        0     1189 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/template_image_info.py
+-rw-r--r--   0        0        0     1088 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/test_set_output_response.py
+-rw-r--r--   0        0        0     1004 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/test_set_simple_response.py
+-rw-r--r--   0        0        0     1353 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/trace.py
+-rw-r--r--   0        0        0      953 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/uri.py
+-rw-r--r--   0        0        0     1086 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1031 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/variant_action.py
+-rw-r--r--   0        0        0      511 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/backend/types/variant_action_enum.py
+-rw-r--r--   0        0        0    19648 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/client.py
+-rw-r--r--   0        0        0       94 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/client/exceptions.py
+-rw-r--r--   0        0        0      732 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/config.py
+-rw-r--r--   0        0        0      223 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/config.toml
+-rw-r--r--   0        0        0      317 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/docker/docker-assets/Dockerfile.cloud.template
+-rw-r--r--   0        0        0      285 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/docker/docker-assets/README.md
+-rwxr-xr-x   0        0        0       74 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/docker/docker-assets/entrypoint.sh
+-rw-r--r--   0        0        0       83 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/docker/docker-assets/lambda_function.py
+-rw-r--r--   0        0        0      327 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     3542 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      565 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/__init__.py
+-rw-r--r--   0        0        0    15429 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/agenta_decorator.py
+-rw-r--r--   0        0        0     7792 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/agenta_init.py
+-rw-r--r--   0        0        0      901 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/context.py
+-rw-r--r--   0        0        0      269 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/router.py
+-rw-r--r--   0        0        0     4658 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/types.py
+-rw-r--r--   0        0        0      360 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/utils/globals.py
+-rw-r--r--   0        0        0     5877 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/utils/helper/openai_cost.py
+-rw-r--r--   0        0        0     1278 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/sdk/utils/preinit.py
+-rw-r--r--   0        0        0      308 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/compose_email/README.md
+-rw-r--r--   0        0        0     2384 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/compose_email/app.py
+-rw-r--r--   0        0        0       70 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/compose_email/env.example
+-rw-r--r--   0        0        0       23 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/compose_email/requirements.txt
+-rw-r--r--   0        0        0       47 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/compose_email/template.toml
+-rw-r--r--   0        0        0      308 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/extract_data_to_json/README.md
+-rw-r--r--   0        0        0     1320 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/extract_data_to_json/app.py
+-rw-r--r--   0        0        0       70 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/extract_data_to_json/env.example
+-rw-r--r--   0        0        0       23 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/extract_data_to_json/requirements.txt
+-rw-r--r--   0        0        0       60 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/extract_data_to_json/template.toml
+-rw-r--r--   0        0        0      308 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      646 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       70 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/simple_prompt/env.example
+-rw-r--r--   0        0        0       23 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2024-01-29 22:04:11.441783 agenta-0.9.0/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0     1041 2024-01-29 22:04:11.445783 agenta-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    27295 1970-01-01 00:00:00.000000 agenta-0.9.0/PKG-INFO
```

### Comparing `agenta-0.8.4/README.md` & `agenta-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/cli/helper.py` & `agenta-0.9.0/agenta/cli/helper.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/cli/main.py` & `agenta-0.9.0/agenta/cli/main.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/cli/telemetry.py` & `agenta-0.9.0/agenta/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/cli/variant_commands.py` & `agenta-0.9.0/agenta/cli/variant_commands.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/cli/variant_configs.py` & `agenta-0.9.0/agenta/cli/variant_configs.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/Readme.md` & `agenta-0.9.0/agenta/client/Readme.md`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/api.py` & `agenta-0.9.0/agenta/client/api.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/api_models.py` & `agenta-0.9.0/agenta/client/api_models.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/__init__.py` & `agenta-0.9.0/agenta/client/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/client.py` & `agenta-0.9.0/agenta/client/backend/client.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/core/__init__.py` & `agenta-0.9.0/agenta/client/backend/core/__init__.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/core/client_wrapper.py` & `agenta-0.9.0/agenta/client/backend/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/core/datetime_utils.py` & `agenta-0.9.0/agenta/client/backend/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/core/jsonable_encoder.py` & `agenta-0.9.0/agenta/client/backend/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/__init__.py` & `agenta-0.9.0/agenta/client/backend/types/__init__.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/app.py` & `agenta-0.9.0/agenta/client/backend/types/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/app_variant_output.py` & `agenta-0.9.0/agenta/client/backend/types/app_variant_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/base_output.py` & `agenta-0.9.0/agenta/client/backend/types/base_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/body_import_testset.py` & `agenta-0.9.0/agenta/client/backend/types/body_import_testset.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/create_app_output.py` & `agenta-0.9.0/agenta/client/backend/types/create_app_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/create_custom_evaluation.py` & `agenta-0.9.0/agenta/client/backend/types/create_custom_evaluation.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/custom_evaluation_detail.py` & `agenta-0.9.0/agenta/client/backend/types/custom_evaluation_detail.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/custom_evaluation_names.py` & `agenta-0.9.0/agenta/client/backend/types/custom_evaluation_names.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/custom_evaluation_output.py` & `agenta-0.9.0/agenta/client/backend/types/custom_evaluation_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/docker_env_vars.py` & `agenta-0.9.0/agenta/client/backend/types/docker_env_vars.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/environment_output.py` & `agenta-0.9.0/agenta/client/backend/types/environment_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/evaluation.py` & `agenta-0.9.0/agenta/client/backend/types/evaluation.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/evaluation_scenario.py` & `agenta-0.9.0/agenta/client/backend/types/evaluation_scenario.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/evaluation_scenario_input.py` & `agenta-0.9.0/agenta/client/backend/types/evaluation_scenario_input.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/evaluation_scenario_output.py` & `agenta-0.9.0/agenta/client/backend/types/evaluation_scenario_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/evaluation_status_enum.py` & `agenta-0.9.0/agenta/client/backend/types/evaluation_status_enum.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/evaluation_type.py` & `agenta-0.9.0/agenta/client/backend/types/evaluation_type.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/evaluation_type_settings.py` & `agenta-0.9.0/agenta/client/backend/types/evaluation_type_settings.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/evaluation_webhook.py` & `agenta-0.9.0/agenta/client/backend/types/evaluation_webhook.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/feedback.py` & `agenta-0.9.0/agenta/client/backend/types/feedback.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/get_config_reponse.py` & `agenta-0.9.0/agenta/client/backend/types/get_config_reponse.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/http_validation_error.py` & `agenta-0.9.0/agenta/client/backend/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/image.py` & `agenta-0.9.0/agenta/client/backend/types/image.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/invite_request.py` & `agenta-0.9.0/agenta/client/backend/types/invite_request.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/list_api_keys_output.py` & `agenta-0.9.0/agenta/client/backend/types/list_api_keys_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/new_testset.py` & `agenta-0.9.0/agenta/client/backend/types/new_testset.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/organization.py` & `agenta-0.9.0/agenta/client/backend/types/organization.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/organization_output.py` & `agenta-0.9.0/agenta/client/backend/types/organization_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/simple_evaluation_output.py` & `agenta-0.9.0/agenta/client/backend/types/simple_evaluation_output.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/span.py` & `agenta-0.9.0/agenta/client/backend/types/span.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/template.py` & `agenta-0.9.0/agenta/client/backend/types/template.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/template_image_info.py` & `agenta-0.9.0/agenta/client/backend/types/template_image_info.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/test_set_output_response.py` & `agenta-0.9.0/agenta/client/backend/types/test_set_output_response.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/test_set_simple_response.py` & `agenta-0.9.0/agenta/client/backend/types/test_set_simple_response.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/trace.py` & `agenta-0.9.0/agenta/client/backend/types/trace.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/uri.py` & `agenta-0.9.0/agenta/client/backend/types/uri.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/validation_error.py` & `agenta-0.9.0/agenta/client/backend/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/backend/types/variant_action.py` & `agenta-0.9.0/agenta/client/backend/types/variant_action.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/client/client.py` & `agenta-0.9.0/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/config.py` & `agenta-0.9.0/agenta/config.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/docker/docker_utils.py` & `agenta-0.9.0/agenta/docker/docker_utils.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/sdk/__init__.py` & `agenta-0.9.0/agenta/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/sdk/agenta_decorator.py` & `agenta-0.9.0/agenta/sdk/agenta_decorator.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/sdk/agenta_init.py` & `agenta-0.9.0/agenta/sdk/agenta_init.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/sdk/context.py` & `agenta-0.9.0/agenta/sdk/context.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/sdk/types.py` & `agenta-0.9.0/agenta/sdk/types.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/sdk/utils/helper/openai_cost.py` & `agenta-0.9.0/agenta/sdk/utils/helper/openai_cost.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/sdk/utils/preinit.py` & `agenta-0.9.0/agenta/sdk/utils/preinit.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/templates/compose_email/app.py` & `agenta-0.9.0/agenta/templates/compose_email/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/templates/extract_data_to_json/app.py` & `agenta-0.9.0/agenta/templates/extract_data_to_json/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/agenta/templates/simple_prompt/app.py` & `agenta-0.9.0/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.8.4/pyproject.toml` & `agenta-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agenta"
-version = "0.8.4"
+version = "0.9.0"
 description = "The SDK for agenta is an open-source LLMOps platform."
 readme = "README.md"
 authors = ["Mahmoud Mabrouk <mahmoud@agenta.ai>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9",
```

### Comparing `agenta-0.8.4/PKG-INFO` & `agenta-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agenta
-Version: 0.8.4
+Version: 0.9.0
 Summary: The SDK for agenta is an open-source LLMOps platform.
 Home-page: https://agenta.ai
 Keywords: LLMOps,LLM,evaluation,prompt engineering
 Author: Mahmoud Mabrouk
 Author-email: mahmoud@agenta.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: agenta Version: 0.8.4 Summary: The SDK for agenta
+Metadata-Version: 2.1 Name: agenta Version: 0.9.0 Summary: The SDK for agenta
 is an open-source LLMOps platform. Home-page: https://agenta.ai Keywords:
 LLMOps,LLM,evaluation,prompt engineering Author: Mahmoud Mabrouk Author-email:
 mahmoud@agenta.ai Requires-Python: >=3.9,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

