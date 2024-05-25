# Comparing `tmp/fusio_sdk-5.0.7.tar.gz` & `tmp/fusio_sdk-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusio_sdk-5.0.7.tar", last modified: Sun Apr 14 18:03:38 2024, max compression
+gzip compressed data, was "fusio_sdk-5.0.8.tar", last modified: Sat May 25 16:20:14 2024, max compression
```

## Comparing `fusio_sdk-5.0.7.tar` & `fusio_sdk-5.0.8.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:03:38.663508 fusio_sdk-5.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/authorization_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_account_change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_response_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_response_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_audit_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_audit_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_audit_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_backup_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_backup_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_backup_import_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_backup_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_config_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_config_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_config_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_introspection_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_introspection_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_introspection_entity_row.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_index_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_index_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_provider_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_provider_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log_error_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_collection_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_local_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_remote_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_throws.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_preview_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_category_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_sdk_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_sdk_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_sdk_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_sdk_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_statistic_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_statistic_chart_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_statistic_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    18687 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_statistic_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_tenant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_data_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_select.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_text_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_message_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_authorize_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_authorize_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_authorize_response_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_grant_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_grant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_checkout_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_checkout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_portal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_portal_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_password_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/passthru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_about.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_about_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_about_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_meta_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_o_auth_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_route.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_route_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_route_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_schema_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:20:14.252063 fusio_sdk-5.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-25 16:20:14.248063 fusio_sdk-5.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 16:20:14.252063 fusio_sdk-5.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:20:14.204063 fusio_sdk-5.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:20:14.248063 fusio_sdk-5.0.8/src/fusio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-25 16:20:14.000000 fusio_sdk-5.0.8/src/fusio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-25 16:20:14.000000 fusio_sdk-5.0.8/src/fusio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:20:14.000000 fusio_sdk-5.0.8/src/fusio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 16:20:14.000000 fusio_sdk-5.0.8/src/fusio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-25 16:20:14.000000 fusio_sdk-5.0.8/src/fusio_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:20:14.248063 fusio_sdk-5.0.8/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/authorization_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_account_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_execute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_execute_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_execute_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_execute_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_execute_response_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_action_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_audit_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_audit_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_audit_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_backup_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_backup_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_backup_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_backup_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_category_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_category_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_category_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_category_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_config_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_config_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_config_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_introspection_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_introspection_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_introspection_entity_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_connection_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_cronjob_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_cronjob_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_cronjob_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_cronjob_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_cronjob_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_dashboard_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_event_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_event_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_generator_index_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_generator_index_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_generator_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_generator_provider_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_generator_provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_generator_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_identity_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_identity_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_identity_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_identity_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_identity_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_log_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_log_error_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_marketplace_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_marketplace_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_marketplace_collection_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_marketplace_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_marketplace_local_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_marketplace_remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_marketplace_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_operation_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_operation_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_operation_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_operation_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_operation_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_operation_throws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_operation_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_page_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_page_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_rate_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_rate_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_rate_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_rate_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_rate_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_role_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_role_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_schema_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_schema_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_schema_preview_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_schema_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_schema_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope_category_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_scope_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_sdk_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_sdk_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_sdk_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_sdk_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_statistic_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_statistic_chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_statistic_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18687 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_statistic_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_tenant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_trash_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_trash_data_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_trash_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_trash_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_trash_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_user_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/backend_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_form_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_form_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_form_element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_form_element_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_form_element_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_form_element_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_form_element_text_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_message_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_authorize_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_authorize_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_authorize_response_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_grant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_grant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_payment_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_payment_checkout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_payment_portal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_payment_portal_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_token_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_token_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_token_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_password_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_user_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/consumer_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/passthru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_about_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_about_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_meta_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_o_auth_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_route_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_route_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_schema_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-25 16:20:10.000000 fusio_sdk-5.0.8/src/sdk/system_tag.py
```

### Comparing `fusio_sdk-5.0.7/LICENSE` & `fusio_sdk-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/PKG-INFO` & `fusio_sdk-5.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusio-sdk
-Version: 5.0.7
+Version: 5.0.8
 Summary: SDK to talk to the Fusio REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-sdk-python
 Project-URL: Issues, https://github.com/apioo/fusio-sdk-sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusio_sdk-5.0.7/README.md` & `fusio_sdk-5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/pyproject.toml` & `fusio_sdk-5.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fusio-sdk"
-version = "5.0.7"
+version = "5.0.8"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "SDK to talk to the Fusio REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `fusio_sdk-5.0.7/src/fusio_sdk.egg-info/PKG-INFO` & `fusio_sdk-5.0.8/src/fusio_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusio-sdk
-Version: 5.0.7
+Version: 5.0.8
 Summary: SDK to talk to the Fusio REST API
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/apioo/fusio-sdk-python
 Project-URL: Issues, https://github.com/apioo/fusio-sdk-sdkgen-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusio_sdk-5.0.7/src/fusio_sdk.egg-info/SOURCES.txt` & `fusio_sdk-5.0.8/src/fusio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/authorization_tag.py` & `fusio_sdk-5.0.8/src/sdk/authorization_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_account_change_password.py` & `fusio_sdk-5.0.8/src/sdk/backend_account_change_password.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_account_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_account_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_action.py` & `fusio_sdk-5.0.8/src/sdk/backend_action.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_action_config.py` & `fusio_sdk-5.0.8/src/sdk/backend_action_config.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_action_execute_request.py` & `fusio_sdk-5.0.8/src/sdk/backend_action_execute_request.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_action_execute_request_body.py` & `fusio_sdk-5.0.8/src/sdk/backend_action_execute_request_body.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_action_execute_response.py` & `fusio_sdk-5.0.8/src/sdk/backend_action_execute_response.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_action_execute_response_body.py` & `fusio_sdk-5.0.8/src/sdk/backend_action_execute_response_body.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_action_execute_response_headers.py` & `fusio_sdk-5.0.8/src/sdk/backend_action_execute_response_headers.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_action_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_action_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_app.py` & `fusio_sdk-5.0.8/src/sdk/backend_app.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_app_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_app_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_audit.py` & `fusio_sdk-5.0.8/src/sdk/backend_audit.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_audit_object.py` & `fusio_sdk-5.0.8/src/sdk/backend_audit_object.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_audit_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_audit_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_backup_import_result.py` & `fusio_sdk-5.0.8/src/sdk/backend_backup_import_result.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_backup_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_backup_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_category_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_category_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_config.py` & `fusio_sdk-5.0.8/src/sdk/backend_config.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_config_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_config_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_connection.py` & `fusio_sdk-5.0.8/src/sdk/backend_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 from .backend_connection_config import BackendConnectionConfig
 from .common_metadata import CommonMetadata
 class BackendConnection(BaseModel):
     id: Optional[int] = Field(default=None, alias="id")
     name: Optional[str] = Field(default=None, alias="name")
     class_: Optional[str] = Field(default=None, alias="class")
+    oauth_: Optional[bool] = Field(default=None, alias="oauth2")
     config: Optional[BackendConnectionConfig] = Field(default=None, alias="config")
     metadata: Optional[CommonMetadata] = Field(default=None, alias="metadata")
     pass
```

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_connection_config.py` & `fusio_sdk-5.0.8/src/sdk/backend_connection_config.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_connection_index.py` & `fusio_sdk-5.0.8/src/sdk/backend_connection_index.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_connection_introspection_entity.py` & `fusio_sdk-5.0.8/src/sdk/backend_connection_introspection_entity.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_connection_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_connection_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_cronjob.py` & `fusio_sdk-5.0.8/src/sdk/backend_cronjob.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_cronjob_error.py` & `fusio_sdk-5.0.8/src/sdk/backend_cronjob_error.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_cronjob_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_cronjob_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_dashboard.py` & `fusio_sdk-5.0.8/src/sdk/backend_dashboard.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_dashboard_app.py` & `fusio_sdk-5.0.8/src/sdk/backend_dashboard_app.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_dashboard_request.py` & `fusio_sdk-5.0.8/src/sdk/backend_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_dashboard_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_dashboard_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_dashboard_transaction.py` & `fusio_sdk-5.0.8/src/sdk/backend_dashboard_transaction.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_dashboard_transactions.py` & `fusio_sdk-5.0.8/src/sdk/backend_dashboard_transactions.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_dashboard_user.py` & `fusio_sdk-5.0.8/src/sdk/backend_dashboard_user.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_event.py` & `fusio_sdk-5.0.8/src/sdk/backend_event.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_event_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_event_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_generator_index_providers.py` & `fusio_sdk-5.0.8/src/sdk/backend_generator_index_providers.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_generator_provider.py` & `fusio_sdk-5.0.8/src/sdk/backend_generator_provider.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_generator_provider_changelog.py` & `fusio_sdk-5.0.8/src/sdk/backend_generator_provider_changelog.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_generator_provider_config.py` & `fusio_sdk-5.0.8/src/sdk/backend_generator_provider_config.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_generator_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_generator_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_identity.py` & `fusio_sdk-5.0.8/src/sdk/backend_identity.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_identity_config.py` & `fusio_sdk-5.0.8/src/sdk/backend_identity_config.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_identity_index.py` & `fusio_sdk-5.0.8/src/sdk/backend_identity_index.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_identity_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_identity_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_log.py` & `fusio_sdk-5.0.8/src/sdk/backend_log.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_log_error.py` & `fusio_sdk-5.0.8/src/sdk/backend_log_error.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_log_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_log_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_marketplace_app.py` & `fusio_sdk-5.0.8/src/sdk/backend_marketplace_app.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_marketplace_collection.py` & `fusio_sdk-5.0.8/src/sdk/backend_marketplace_collection.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_marketplace_collection_apps.py` & `fusio_sdk-5.0.8/src/sdk/backend_marketplace_collection_apps.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_marketplace_local_app.py` & `fusio_sdk-5.0.8/src/sdk/backend_marketplace_local_app.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_marketplace_remote_app.py` & `fusio_sdk-5.0.8/src/sdk/backend_marketplace_remote_app.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_marketplace_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_marketplace_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_operation.py` & `fusio_sdk-5.0.8/src/sdk/backend_operation.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_operation_parameters.py` & `fusio_sdk-5.0.8/src/sdk/backend_operation_parameters.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_operation_schema.py` & `fusio_sdk-5.0.8/src/sdk/backend_operation_schema.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_operation_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_operation_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_operation_throws.py` & `fusio_sdk-5.0.8/src/sdk/backend_operation_throws.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_page.py` & `fusio_sdk-5.0.8/src/sdk/backend_page.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_page_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_page_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_plan.py` & `fusio_sdk-5.0.8/src/sdk/backend_plan.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_plan_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_plan_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_rate.py` & `fusio_sdk-5.0.8/src/sdk/backend_rate.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_rate_allocation.py` & `fusio_sdk-5.0.8/src/sdk/backend_rate_allocation.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_rate_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_rate_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_role.py` & `fusio_sdk-5.0.8/src/sdk/backend_role.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_role_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_role_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_schema.py` & `fusio_sdk-5.0.8/src/sdk/backend_schema.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_schema_form.py` & `fusio_sdk-5.0.8/src/sdk/backend_schema_form.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_schema_source.py` & `fusio_sdk-5.0.8/src/sdk/backend_schema_source.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_schema_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_schema_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_scope.py` & `fusio_sdk-5.0.8/src/sdk/backend_scope.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_scope_category.py` & `fusio_sdk-5.0.8/src/sdk/backend_scope_category.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_scope_category_scope.py` & `fusio_sdk-5.0.8/src/sdk/backend_scope_category_scope.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_scope_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_scope_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_sdk_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_sdk_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_sdk_types.py` & `fusio_sdk-5.0.8/src/sdk/backend_sdk_types.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_statistic_chart.py` & `fusio_sdk-5.0.8/src/sdk/backend_statistic_chart.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_statistic_chart_data.py` & `fusio_sdk-5.0.8/src/sdk/backend_statistic_chart_data.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_statistic_count.py` & `fusio_sdk-5.0.8/src/sdk/backend_statistic_count.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_statistic_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_statistic_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_tenant_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_tenant_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_token.py` & `fusio_sdk-5.0.8/src/sdk/backend_token.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_token_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_token_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_transaction.py` & `fusio_sdk-5.0.8/src/sdk/backend_transaction.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_transaction_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_transaction_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_trash_data.py` & `fusio_sdk-5.0.8/src/sdk/backend_trash_data.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_trash_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_trash_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_user.py` & `fusio_sdk-5.0.8/src/sdk/backend_user.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_user_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_user_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_webhook.py` & `fusio_sdk-5.0.8/src/sdk/backend_webhook.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_webhook_response.py` & `fusio_sdk-5.0.8/src/sdk/backend_webhook_response.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/backend_webhook_tag.py` & `fusio_sdk-5.0.8/src/sdk/backend_webhook_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/client.py` & `fusio_sdk-5.0.8/src/sdk/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,10 +40,10 @@
             self.http_client,
             self.parser
         )
 
 
 
     @staticmethod
-    def build(clientId: str, clientSecret: str, tokenStore: sdkgen.TokenStoreInterface, scopes: List[str]):
-        return Client("https://api.typehub.cloud/", sdkgen.OAuth2(clientId, clientSecret, "https://api.typehub.cloud/authorization/token", "", tokenStore, scopes))
+    def build():
+        return Client("https://api.sdkgen.app/", sdkgen.Anonymous())
```

### Comparing `fusio_sdk-5.0.7/src/sdk/common_collection.py` & `fusio_sdk-5.0.8/src/sdk/common_collection.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/common_form_container.py` & `fusio_sdk-5.0.8/src/sdk/common_form_container.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/common_form_element.py` & `fusio_sdk-5.0.8/src/sdk/common_form_element.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/common_form_element_select.py` & `fusio_sdk-5.0.8/src/sdk/common_form_element_select.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/common_message.py` & `fusio_sdk-5.0.8/src/sdk/common_message.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/common_metadata.py` & `fusio_sdk-5.0.8/src/sdk/common_metadata.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_account_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_account_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_app.py` & `fusio_sdk-5.0.8/src/sdk/consumer_app.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_app_create.py` & `fusio_sdk-5.0.8/src/sdk/consumer_app_create.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_app_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_app_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_app_update.py` & `fusio_sdk-5.0.8/src/sdk/consumer_app_update.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_authorize_meta.py` & `fusio_sdk-5.0.8/src/sdk/consumer_authorize_meta.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_authorize_request.py` & `fusio_sdk-5.0.8/src/sdk/consumer_authorize_request.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_authorize_response.py` & `fusio_sdk-5.0.8/src/sdk/consumer_authorize_response.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_authorize_response_token.py` & `fusio_sdk-5.0.8/src/sdk/consumer_authorize_response_token.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_event.py` & `fusio_sdk-5.0.8/src/sdk/consumer_event.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_event_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_event_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_grant.py` & `fusio_sdk-5.0.8/src/sdk/consumer_grant.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_grant_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_grant_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_identity.py` & `fusio_sdk-5.0.8/src/sdk/consumer_identity.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_identity_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_identity_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_log.py` & `fusio_sdk-5.0.8/src/sdk/consumer_log.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_log_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_log_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_page.py` & `fusio_sdk-5.0.8/src/sdk/consumer_page.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_page_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_page_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_payment_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_payment_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_plan.py` & `fusio_sdk-5.0.8/src/sdk/consumer_plan.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_plan_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_plan_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_scope.py` & `fusio_sdk-5.0.8/src/sdk/consumer_scope.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_scope_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_scope_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_token.py` & `fusio_sdk-5.0.8/src/sdk/consumer_token.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_token_access_token.py` & `fusio_sdk-5.0.8/src/sdk/consumer_token_access_token.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_token_create.py` & `fusio_sdk-5.0.8/src/sdk/consumer_token_create.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_token_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_token_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_transaction.py` & `fusio_sdk-5.0.8/src/sdk/consumer_transaction.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_transaction_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_transaction_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_user_account.py` & `fusio_sdk-5.0.8/src/sdk/consumer_user_account.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_user_jwt.py` & `fusio_sdk-5.0.8/src/sdk/consumer_user_jwt.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_user_login.py` & `fusio_sdk-5.0.8/src/sdk/consumer_user_login.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_user_plan.py` & `fusio_sdk-5.0.8/src/sdk/consumer_user_plan.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_user_register.py` & `fusio_sdk-5.0.8/src/sdk/consumer_user_register.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_webhook.py` & `fusio_sdk-5.0.8/src/sdk/consumer_webhook.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_webhook_create.py` & `fusio_sdk-5.0.8/src/sdk/consumer_webhook_create.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_webhook_response.py` & `fusio_sdk-5.0.8/src/sdk/consumer_webhook_response.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_webhook_tag.py` & `fusio_sdk-5.0.8/src/sdk/consumer_webhook_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/consumer_webhook_update.py` & `fusio_sdk-5.0.8/src/sdk/consumer_webhook_update.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/passthru.py` & `fusio_sdk-5.0.8/src/sdk/passthru.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_about.py` & `fusio_sdk-5.0.8/src/sdk/system_about.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_about_apps.py` & `fusio_sdk-5.0.8/src/sdk/system_about_apps.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_connection_tag.py` & `fusio_sdk-5.0.8/src/sdk/system_connection_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_meta_tag.py` & `fusio_sdk-5.0.8/src/sdk/system_meta_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_o_auth_configuration.py` & `fusio_sdk-5.0.8/src/sdk/system_o_auth_configuration.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_payment_tag.py` & `fusio_sdk-5.0.8/src/sdk/system_payment_tag.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_route_method.py` & `fusio_sdk-5.0.8/src/sdk/system_route_method.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_route_path.py` & `fusio_sdk-5.0.8/src/sdk/system_route_path.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_schema.py` & `fusio_sdk-5.0.8/src/sdk/system_schema.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_schema_form.py` & `fusio_sdk-5.0.8/src/sdk/system_schema_form.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_schema_type_schema.py` & `fusio_sdk-5.0.8/src/sdk/system_schema_type_schema.py`

 * *Files identical despite different names*

### Comparing `fusio_sdk-5.0.7/src/sdk/system_tag.py` & `fusio_sdk-5.0.8/src/sdk/system_tag.py`

 * *Files identical despite different names*

