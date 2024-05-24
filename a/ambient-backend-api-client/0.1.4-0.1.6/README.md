# Comparing `tmp/ambient_backend_api_client-0.1.4.tar.gz` & `tmp/ambient_backend_api_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_backend_api_client-0.1.4.tar", last modified: Sat May 11 03:38:24 2024, max compression
+gzip compressed data, was "ambient_backend_api_client-0.1.6.tar", last modified: Fri May 24 19:01:02 2024, max compression
```

## Comparing `ambient_backend_api_client-0.1.4.tar` & `ambient_backend_api_client-0.1.6.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:24.834988 ambient_backend_api_client-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-11 03:38:24.834988 ambient_backend_api_client-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:24.814988 ambient_backend_api_client-0.1.4/ambient_backend_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:24.818988 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71865 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/clusters_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    82469 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53254 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/requests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    42278 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/services_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/unimplemented_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    62218 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:24.826988 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/ambient_action_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/ambient_event_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/auth0_device_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/cluster_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/create_service_acct_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/creation_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/event_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/event_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/interface_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/list_results_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/models_cluster_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/models_node_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/network_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/node_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/node_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/node_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/notification_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/notification_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/notification_severity_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/organization_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/owner_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/post_clusters_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/post_service_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/request_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/status_enum_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/subscription_model_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/user_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/user_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/validation_error_loc_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:24.814988 ambient_backend_api_client-0.1.4/ambient_backend_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-11 03:38:24.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-11 03:38:24.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:38:24.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-11 03:38:24.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-11 03:38:24.000000 ambient_backend_api_client-0.1.4/ambient_backend_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-11 03:38:24.834988 ambient_backend_api_client-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:38:24.834988 ambient_backend_api_client-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_ambient_action_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_ambient_event_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_auth0_device_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_cluster_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_clusters_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_create_service_acct_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_creation_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_event_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_event_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_health_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_interface_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_list_results_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_models_cluster_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_models_node_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_network_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_node_architecture_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_node_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_node_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_nodes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_notification_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_notification_severity_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_organization_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_owner_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_ping_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_post_clusters_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_post_service_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_request_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_requests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_service_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_service_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_service_status_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_services_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_status_enum_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_subscription_model_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_unimplemented_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_user_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_user_role_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-11 03:38:15.000000 ambient_backend_api_client-0.1.4/test/test_validation_error_loc_inner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:01:02.974156 ambient_backend_api_client-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 19:01:02.974156 ambient_backend_api_client-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:01:02.958156 ambient_backend_api_client-0.1.6/ambient_backend_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:01:02.958156 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71865 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82480 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53254 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42278 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31740 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/unimplemented_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62218 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:01:02.966156 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/ambient_action_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/ambient_event_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/auth0_device_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/cluster_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/create_service_acct_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/creation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/event_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/interface_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/list_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/models_cluster_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/models_node_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/node_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/node_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/node_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/notification_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/notification_severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/owner_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/post_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/post_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/request_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/status_enum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/subscription_model_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/user_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/validation_error_loc_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:01:02.958156 ambient_backend_api_client-0.1.6/ambient_backend_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 19:01:02.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-24 19:01:02.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:01:02.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 19:01:02.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 19:01:02.000000 ambient_backend_api_client-0.1.6/ambient_backend_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 19:01:02.974156 ambient_backend_api_client-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:01:02.974156 ambient_backend_api_client-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_ambient_action_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_ambient_event_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_auth0_device_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_cluster_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_create_service_acct_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_creation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_event_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_event_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_interface_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_list_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_models_cluster_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_models_node_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_node_architecture_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_node_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_node_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_nodes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_notification_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_notification_severity_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_owner_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_post_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_post_service_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_request_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_service_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_service_status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_services_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_status_enum_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_subscription_model_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_unimplemented_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_user_role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-24 19:00:56.000000 ambient_backend_api_client-0.1.6/test/test_validation_error_loc_inner.py
```

### Comparing `ambient_backend_api_client-0.1.4/README.md` & `ambient_backend_api_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/__init__.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 from ambient_backend_api_client.models.node_create import NodeCreate
 from ambient_backend_api_client.models.node_role_enum import NodeRoleEnum
 from ambient_backend_api_client.models.notification import Notification
 from ambient_backend_api_client.models.notification_list import NotificationList
 from ambient_backend_api_client.models.notification_request import NotificationRequest
 from ambient_backend_api_client.models.notification_severity_enum import NotificationSeverityEnum
 from ambient_backend_api_client.models.organization_create import OrganizationCreate
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.post_clusters_response import PostClustersResponse
 from ambient_backend_api_client.models.post_service_response import PostServiceResponse
 from ambient_backend_api_client.models.request import Request
 from ambient_backend_api_client.models.request_status_enum import RequestStatusEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
 from ambient_backend_api_client.models.role_enum import RoleEnum
 from ambient_backend_api_client.models.service import Service
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/__init__.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/clusters_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/health_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/nodes_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/nodes_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import StrictStr
+from pydantic import StrictInt, StrictStr
 from typing import Any, Dict, Optional
 from ambient_backend_api_client.models.list_results_response import ListResultsResponse
 from ambient_backend_api_client.models.node import Node
 from ambient_backend_api_client.models.node_create import NodeCreate
 from ambient_backend_api_client.models.token_response import TokenResponse
 
 from ambient_backend_api_client.api_client import ApiClient, RequestSerialized
@@ -40,15 +40,15 @@
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
     async def authorize_node_nodes_node_id_authorize_post(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         device_code: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -59,15 +59,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> TokenResponse:
         """Authorize Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param device_code: (required)
         :type device_code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -111,15 +111,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def authorize_node_nodes_node_id_authorize_post_with_http_info(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         device_code: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -130,15 +130,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[TokenResponse]:
         """Authorize Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param device_code: (required)
         :type device_code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -182,15 +182,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def authorize_node_nodes_node_id_authorize_post_without_preload_content(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         device_code: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -201,15 +201,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Authorize Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param device_code: (required)
         :type device_code: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -588,15 +588,15 @@
 
 
 
 
     @validate_call
     async def delete_node_nodes_node_id_delete(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -606,15 +606,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """Delete Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -655,15 +655,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def delete_node_nodes_node_id_delete_with_http_info(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -673,15 +673,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """Delete Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -722,15 +722,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def delete_node_nodes_node_id_delete_without_preload_content(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -740,15 +740,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Delete Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -846,15 +846,15 @@
 
 
 
 
     @validate_call
     async def get_node_nodes_node_id_get(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -864,15 +864,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Node:
         """Get Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -913,15 +913,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def get_node_nodes_node_id_get_with_http_info(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -931,15 +931,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Node]:
         """Get Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -980,15 +980,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def get_node_nodes_node_id_get_without_preload_content(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -998,15 +998,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1380,15 +1380,15 @@
 
 
 
 
     @validate_call
     async def refresh_node_token_nodes_node_id_refresh_token_post(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         refresh_token: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1399,15 +1399,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> TokenResponse:
         """Refresh Node Token
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param refresh_token: (required)
         :type refresh_token: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -1451,15 +1451,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def refresh_node_token_nodes_node_id_refresh_token_post_with_http_info(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         refresh_token: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1470,15 +1470,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[TokenResponse]:
         """Refresh Node Token
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param refresh_token: (required)
         :type refresh_token: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -1522,15 +1522,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def refresh_node_token_nodes_node_id_refresh_token_post_without_preload_content(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         refresh_token: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1541,15 +1541,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Refresh Node Token
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param refresh_token: (required)
         :type refresh_token: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -1655,15 +1655,15 @@
 
 
 
 
     @validate_call
     async def request_new_auth_nodes_node_id_auth_post(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1673,15 +1673,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Node:
         """Request New Auth
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1722,15 +1722,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def request_new_auth_nodes_node_id_auth_post_with_http_info(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1740,15 +1740,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Node]:
         """Request New Auth
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1789,15 +1789,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def request_new_auth_nodes_node_id_auth_post_without_preload_content(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1807,15 +1807,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Request New Auth
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1913,15 +1913,15 @@
 
 
 
 
     @validate_call
     async def update_node_nodes_node_id_patch(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         body: Dict[str, Any],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -1932,15 +1932,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Node:
         """Update Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param body: (required)
         :type body: object
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -1984,15 +1984,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     async def update_node_nodes_node_id_patch_with_http_info(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         body: Dict[str, Any],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -2003,15 +2003,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Node]:
         """Update Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param body: (required)
         :type body: object
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -2055,15 +2055,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     async def update_node_nodes_node_id_patch_without_preload_content(
         self,
-        node_id: StrictStr,
+        node_id: StrictInt,
         body: Dict[str, Any],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
@@ -2074,15 +2074,15 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Update Node
 
 
         :param node_id: (required)
-        :type node_id: str
+        :type node_id: int
         :param body: (required)
         :type body: object
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/notifications_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/ping_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/requests_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/services_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/services_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/unimplemented_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/unimplemented_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api/users_api.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api_client.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/api_response.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/api_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/configuration.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/exceptions.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/__init__.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 from ambient_backend_api_client.models.node_create import NodeCreate
 from ambient_backend_api_client.models.node_role_enum import NodeRoleEnum
 from ambient_backend_api_client.models.notification import Notification
 from ambient_backend_api_client.models.notification_list import NotificationList
 from ambient_backend_api_client.models.notification_request import NotificationRequest
 from ambient_backend_api_client.models.notification_severity_enum import NotificationSeverityEnum
 from ambient_backend_api_client.models.organization_create import OrganizationCreate
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.post_clusters_response import PostClustersResponse
 from ambient_backend_api_client.models.post_service_response import PostServiceResponse
 from ambient_backend_api_client.models.request import Request
 from ambient_backend_api_client.models.request_status_enum import RequestStatusEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
 from ambient_backend_api_client.models.role_enum import RoleEnum
 from ambient_backend_api_client.models.service import Service
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/account_type.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/ambient_action_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/ambient_action_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/ambient_event_type_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/ambient_event_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/architecture_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/auth0_device_code_response.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/cluster.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,46 +13,44 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from ambient_backend_api_client.models.architecture_enum import ArchitectureEnum
 from ambient_backend_api_client.models.models_cluster_status_enum import ModelsClusterStatusEnum
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
 from ambient_backend_api_client.models.role_enum import RoleEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Cluster(BaseModel):
     """
     Cluster
     """ # noqa: E501
+    id: Optional[StrictInt] = None
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = 'c7e806f5-f7ef-4afa-8223-8c3cc12298c9'
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
+    org_id: Optional[StrictInt] = None
+    user_id: Optional[StrictInt] = None
     role: RoleEnum
     architecture: ArchitectureEnum
     nodes: List[StrictStr]
     docker_swarm_attrs: Optional[Dict[str, Any]] = None
     site: Optional[StrictStr] = ''
     manager_node: Optional[StrictStr] = None
     cluster_group: Optional[StrictStr] = 'default'
     tags: Optional[List[StrictStr]] = None
+    identifier: Optional[StrictStr] = '29c0a882-515b-46b0-9ce5-6fcbe160981c'
     status: ModelsClusterStatusEnum
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "role", "architecture", "nodes", "docker_swarm_attrs", "site", "manager_node", "cluster_group", "tags", "status"]
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "role", "architecture", "nodes", "docker_swarm_attrs", "site", "manager_node", "cluster_group", "tags", "identifier", "status"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -85,29 +83,34 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if owner_id (nullable) is None
+        # set to None if id (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
-
-        # set to None if owner_type (nullable) is None
-        # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
+        if self.id is None and "id" in self.model_fields_set:
+            _dict['id'] = None
 
         # set to None if description (nullable) is None
         # and model_fields_set contains the field
         if self.description is None and "description" in self.model_fields_set:
             _dict['description'] = None
 
+        # set to None if org_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.org_id is None and "org_id" in self.model_fields_set:
+            _dict['org_id'] = None
+
+        # set to None if user_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.user_id is None and "user_id" in self.model_fields_set:
+            _dict['user_id'] = None
+
         # set to None if docker_swarm_attrs (nullable) is None
         # and model_fields_set contains the field
         if self.docker_swarm_attrs is None and "docker_swarm_attrs" in self.model_fields_set:
             _dict['docker_swarm_attrs'] = None
 
         # set to None if manager_node (nullable) is None
         # and model_fields_set contains the field
@@ -122,28 +125,27 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else 'c7e806f5-f7ef-4afa-8223-8c3cc12298c9',
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
             "role": obj.get("role"),
             "architecture": obj.get("architecture"),
             "nodes": obj.get("nodes"),
             "docker_swarm_attrs": obj.get("docker_swarm_attrs"),
             "site": obj.get("site") if obj.get("site") is not None else '',
             "manager_node": obj.get("manager_node"),
             "cluster_group": obj.get("cluster_group") if obj.get("cluster_group") is not None else 'default',
             "tags": obj.get("tags"),
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '29c0a882-515b-46b0-9ce5-6fcbe160981c',
             "status": obj.get("status")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/cluster_create.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/cluster_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,44 +13,42 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from ambient_backend_api_client.models.architecture_enum import ArchitectureEnum
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
 from ambient_backend_api_client.models.role_enum import RoleEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ClusterCreate(BaseModel):
     """
     ClusterCreate
     """ # noqa: E501
+    id: Optional[StrictInt] = None
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = 'c7e806f5-f7ef-4afa-8223-8c3cc12298c9'
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
+    org_id: Optional[StrictInt] = None
+    user_id: Optional[StrictInt] = None
     role: RoleEnum
     architecture: ArchitectureEnum
     nodes: List[StrictStr]
     docker_swarm_attrs: Optional[Dict[str, Any]] = None
     site: Optional[StrictStr] = ''
     manager_node: Optional[StrictStr] = None
     cluster_group: Optional[StrictStr] = 'default'
     tags: Optional[List[StrictStr]] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "role", "architecture", "nodes", "docker_swarm_attrs", "site", "manager_node", "cluster_group", "tags"]
+    identifier: Optional[StrictStr] = '29c0a882-515b-46b0-9ce5-6fcbe160981c'
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "role", "architecture", "nodes", "docker_swarm_attrs", "site", "manager_node", "cluster_group", "tags", "identifier"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -83,29 +81,34 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if owner_id (nullable) is None
+        # set to None if id (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
-
-        # set to None if owner_type (nullable) is None
-        # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
+        if self.id is None and "id" in self.model_fields_set:
+            _dict['id'] = None
 
         # set to None if description (nullable) is None
         # and model_fields_set contains the field
         if self.description is None and "description" in self.model_fields_set:
             _dict['description'] = None
 
+        # set to None if org_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.org_id is None and "org_id" in self.model_fields_set:
+            _dict['org_id'] = None
+
+        # set to None if user_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.user_id is None and "user_id" in self.model_fields_set:
+            _dict['user_id'] = None
+
         # set to None if docker_swarm_attrs (nullable) is None
         # and model_fields_set contains the field
         if self.docker_swarm_attrs is None and "docker_swarm_attrs" in self.model_fields_set:
             _dict['docker_swarm_attrs'] = None
 
         # set to None if manager_node (nullable) is None
         # and model_fields_set contains the field
@@ -120,27 +123,26 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else 'c7e806f5-f7ef-4afa-8223-8c3cc12298c9',
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
             "role": obj.get("role"),
             "architecture": obj.get("architecture"),
             "nodes": obj.get("nodes"),
             "docker_swarm_attrs": obj.get("docker_swarm_attrs"),
             "site": obj.get("site") if obj.get("site") is not None else '',
             "manager_node": obj.get("manager_node"),
             "cluster_group": obj.get("cluster_group") if obj.get("cluster_group") is not None else 'default',
-            "tags": obj.get("tags")
+            "tags": obj.get("tags"),
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '29c0a882-515b-46b0-9ce5-6fcbe160981c'
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/create_service_acct_request.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/creation_method.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/event.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/event.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/event_label.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/event_label.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/event_template.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/event_template.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/http_validation_error.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/interface_type_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/list_results_response.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/list_results_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing_extensions import Self
 
 class ListResultsResponse(BaseModel):
     """
     ListResultsResponse
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Fri May 10 21:28:39 2024'
+    timestamp: Optional[StrictStr] = '2024-05-24T12:36:49.790989'
     results: List[Any]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -79,13 +79,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Fri May 10 21:28:39 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-24T12:36:49.790989',
             "results": obj.get("results")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/models_node_status_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/network_interface.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/node.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,46 +13,44 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from ambient_backend_api_client.models.auth0_device_code_response import Auth0DeviceCodeResponse
 from ambient_backend_api_client.models.models_node_status_enum import ModelsNodeStatusEnum
 from ambient_backend_api_client.models.network_interface import NetworkInterface
 from ambient_backend_api_client.models.node_architecture_enum import NodeArchitectureEnum
 from ambient_backend_api_client.models.node_role_enum import NodeRoleEnum
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Node(BaseModel):
     """
     Node
     """ # noqa: E501
+    id: Optional[StrictInt] = None
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: StrictStr
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
+    org_id: StrictInt
+    user_id: StrictInt
     role: NodeRoleEnum
     architecture: NodeArchitectureEnum
     interfaces: Optional[List[NetworkInterface]] = None
     last_seen: Optional[StrictStr] = None
     status: ModelsNodeStatusEnum
+    identifier: Optional[StrictStr] = None
     cluster: Optional[StrictStr] = None
     authorization: Optional[Auth0DeviceCodeResponse] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "role", "architecture", "interfaces", "last_seen", "status", "cluster", "authorization"]
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "role", "architecture", "interfaces", "last_seen", "status", "identifier", "cluster", "authorization"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -95,23 +93,18 @@
             for _item in self.interfaces:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['interfaces'] = _items
         # override the default output from pydantic by calling `to_dict()` of authorization
         if self.authorization:
             _dict['authorization'] = self.authorization.to_dict()
-        # set to None if owner_id (nullable) is None
+        # set to None if id (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
-
-        # set to None if owner_type (nullable) is None
-        # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
+        if self.id is None and "id" in self.model_fields_set:
+            _dict['id'] = None
 
         # set to None if description (nullable) is None
         # and model_fields_set contains the field
         if self.description is None and "description" in self.model_fields_set:
             _dict['description'] = None
 
         # set to None if interfaces (nullable) is None
@@ -120,14 +113,19 @@
             _dict['interfaces'] = None
 
         # set to None if last_seen (nullable) is None
         # and model_fields_set contains the field
         if self.last_seen is None and "last_seen" in self.model_fields_set:
             _dict['last_seen'] = None
 
+        # set to None if identifier (nullable) is None
+        # and model_fields_set contains the field
+        if self.identifier is None and "identifier" in self.model_fields_set:
+            _dict['identifier'] = None
+
         # set to None if cluster (nullable) is None
         # and model_fields_set contains the field
         if self.cluster is None and "cluster" in self.model_fields_set:
             _dict['cluster'] = None
 
         # set to None if authorization (nullable) is None
         # and model_fields_set contains the field
@@ -142,26 +140,25 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier"),
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
             "role": obj.get("role"),
             "architecture": obj.get("architecture"),
             "interfaces": [NetworkInterface.from_dict(_item) for _item in obj["interfaces"]] if obj.get("interfaces") is not None else None,
             "last_seen": obj.get("last_seen"),
             "status": obj.get("status"),
+            "identifier": obj.get("identifier"),
             "cluster": obj.get("cluster"),
             "authorization": Auth0DeviceCodeResponse.from_dict(obj["authorization"]) if obj.get("authorization") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/node_architecture_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/node_create.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/request.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,46 +13,40 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from ambient_backend_api_client.models.auth0_device_code_response import Auth0DeviceCodeResponse
-from ambient_backend_api_client.models.network_interface import NetworkInterface
-from ambient_backend_api_client.models.node_architecture_enum import NodeArchitectureEnum
-from ambient_backend_api_client.models.node_role_enum import NodeRoleEnum
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
+from pydantic import BaseModel, ConfigDict, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
+from ambient_backend_api_client.models.request_status_enum import RequestStatusEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
-from ambient_backend_api_client.models.status_enum_input import StatusEnumInput
 from typing import Optional, Set
 from typing_extensions import Self
 
-class NodeCreate(BaseModel):
+class Request(BaseModel):
     """
-    NodeCreate
+    Request
     """ # noqa: E501
+    id: StrictInt
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = None
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
-    role: NodeRoleEnum
-    architecture: NodeArchitectureEnum
-    interfaces: Optional[List[NetworkInterface]] = None
-    last_seen: Optional[StrictStr] = None
-    status: Optional[StatusEnumInput] = None
-    cluster: Optional[StrictStr] = None
-    authorization: Optional[Auth0DeviceCodeResponse] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "role", "architecture", "interfaces", "last_seen", "status", "cluster", "authorization"]
+    org_id: Optional[StrictInt] = None
+    user_id: Optional[StrictInt] = None
+    status: Optional[RequestStatusEnum] = None
+    error: Optional[StrictStr] = None
+    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.716575809788515E9
+    started_ts: Optional[Union[StrictFloat, StrictInt]] = None
+    failed_ts: Optional[Union[StrictFloat, StrictInt]] = None
+    completed_ts: Optional[Union[StrictFloat, StrictInt]] = None
+    notes: Optional[List[StrictStr]] = None
+    data: Optional[Dict[str, Any]] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "status", "error", "requested_ts", "started_ts", "failed_ts", "completed_ts", "notes", "data"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -64,15 +58,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of NodeCreate from a JSON string"""
+        """Create an instance of Request from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -85,88 +79,72 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in interfaces (list)
-        _items = []
-        if self.interfaces:
-            for _item in self.interfaces:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['interfaces'] = _items
-        # override the default output from pydantic by calling `to_dict()` of authorization
-        if self.authorization:
-            _dict['authorization'] = self.authorization.to_dict()
-        # set to None if identifier (nullable) is None
-        # and model_fields_set contains the field
-        if self.identifier is None and "identifier" in self.model_fields_set:
-            _dict['identifier'] = None
-
-        # set to None if owner_id (nullable) is None
+        # set to None if description (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
+        if self.description is None and "description" in self.model_fields_set:
+            _dict['description'] = None
 
-        # set to None if owner_type (nullable) is None
+        # set to None if org_id (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
+        if self.org_id is None and "org_id" in self.model_fields_set:
+            _dict['org_id'] = None
 
-        # set to None if description (nullable) is None
+        # set to None if user_id (nullable) is None
         # and model_fields_set contains the field
-        if self.description is None and "description" in self.model_fields_set:
-            _dict['description'] = None
+        if self.user_id is None and "user_id" in self.model_fields_set:
+            _dict['user_id'] = None
 
-        # set to None if interfaces (nullable) is None
+        # set to None if error (nullable) is None
         # and model_fields_set contains the field
-        if self.interfaces is None and "interfaces" in self.model_fields_set:
-            _dict['interfaces'] = None
+        if self.error is None and "error" in self.model_fields_set:
+            _dict['error'] = None
 
-        # set to None if last_seen (nullable) is None
+        # set to None if started_ts (nullable) is None
         # and model_fields_set contains the field
-        if self.last_seen is None and "last_seen" in self.model_fields_set:
-            _dict['last_seen'] = None
+        if self.started_ts is None and "started_ts" in self.model_fields_set:
+            _dict['started_ts'] = None
 
-        # set to None if cluster (nullable) is None
+        # set to None if failed_ts (nullable) is None
         # and model_fields_set contains the field
-        if self.cluster is None and "cluster" in self.model_fields_set:
-            _dict['cluster'] = None
+        if self.failed_ts is None and "failed_ts" in self.model_fields_set:
+            _dict['failed_ts'] = None
 
-        # set to None if authorization (nullable) is None
+        # set to None if completed_ts (nullable) is None
         # and model_fields_set contains the field
-        if self.authorization is None and "authorization" in self.model_fields_set:
-            _dict['authorization'] = None
+        if self.completed_ts is None and "completed_ts" in self.model_fields_set:
+            _dict['completed_ts'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of NodeCreate from a dict"""
+        """Create an instance of Request from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier"),
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
-            "role": obj.get("role"),
-            "architecture": obj.get("architecture"),
-            "interfaces": [NetworkInterface.from_dict(_item) for _item in obj["interfaces"]] if obj.get("interfaces") is not None else None,
-            "last_seen": obj.get("last_seen"),
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
             "status": obj.get("status"),
-            "cluster": obj.get("cluster"),
-            "authorization": Auth0DeviceCodeResponse.from_dict(obj["authorization"]) if obj.get("authorization") is not None else None
+            "error": obj.get("error"),
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.716575809788515E9,
+            "started_ts": obj.get("started_ts"),
+            "failed_ts": obj.get("failed_ts"),
+            "completed_ts": obj.get("completed_ts"),
+            "notes": obj.get("notes"),
+            "data": obj.get("data")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/node_role_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/notification.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/notification.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,38 +16,35 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from ambient_backend_api_client.models.notification_severity_enum import NotificationSeverityEnum
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
 class Notification(BaseModel):
     """
     Notification
     """ # noqa: E501
+    id: Optional[StrictInt] = None
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = None
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
+    org_id: Optional[StrictInt] = None
+    user_id: Optional[StrictInt] = None
     message: StrictStr
     severity: NotificationSeverityEnum
     target_resource_id: StrictStr
     target_resource_type: ResourceTypeEnum
     timestamp: StrictInt
     read: Optional[StrictBool] = False
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "message", "severity", "target_resource_id", "target_resource_type", "timestamp", "read"]
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "message", "severity", "target_resource_id", "target_resource_type", "timestamp", "read"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -80,54 +77,52 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if identifier (nullable) is None
+        # set to None if id (nullable) is None
         # and model_fields_set contains the field
-        if self.identifier is None and "identifier" in self.model_fields_set:
-            _dict['identifier'] = None
+        if self.id is None and "id" in self.model_fields_set:
+            _dict['id'] = None
 
-        # set to None if owner_id (nullable) is None
+        # set to None if description (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
+        if self.description is None and "description" in self.model_fields_set:
+            _dict['description'] = None
 
-        # set to None if owner_type (nullable) is None
+        # set to None if org_id (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
+        if self.org_id is None and "org_id" in self.model_fields_set:
+            _dict['org_id'] = None
 
-        # set to None if description (nullable) is None
+        # set to None if user_id (nullable) is None
         # and model_fields_set contains the field
-        if self.description is None and "description" in self.model_fields_set:
-            _dict['description'] = None
+        if self.user_id is None and "user_id" in self.model_fields_set:
+            _dict['user_id'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of Notification from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier"),
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
             "message": obj.get("message"),
             "severity": obj.get("severity"),
             "target_resource_id": obj.get("target_resource_id"),
             "target_resource_type": obj.get("target_resource_type"),
             "timestamp": obj.get("timestamp"),
             "read": obj.get("read") if obj.get("read") is not None else False
         })
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/notification_list.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/notification_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class NotificationList(BaseModel):
     """
     NotificationList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Fri May 10 21:28:39 2024'
+    timestamp: Optional[StrictStr] = '2024-05-24T12:36:49.790989'
     results: List[Notification]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -87,13 +87,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Fri May 10 21:28:39 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-24T12:36:49.790989',
             "results": [Notification.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/notification_request.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/notification_severity_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/organization_create.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,39 +13,38 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
-from ambient_backend_api_client.models.subscription_model_enum import SubscriptionModelEnum
+from ambient_backend_api_client.models.service_state import ServiceState
+from ambient_backend_api_client.models.service_status_enum import ServiceStatusEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OrganizationCreate(BaseModel):
+class Service(BaseModel):
     """
-    OrganizationCreate
+    Service
     """ # noqa: E501
+    id: Optional[StrictInt] = None
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = None
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
-    subscription: SubscriptionModelEnum
-    root_email: StrictStr
-    okta_group_id: Optional[StrictStr] = None
-    auth0_org_id: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "subscription", "root_email", "okta_group_id", "auth0_org_id"]
+    org_id: Optional[StrictInt] = None
+    user_id: Optional[StrictInt] = None
+    image: StrictStr
+    tags: Optional[List[StrictStr]] = None
+    ports: Optional[List[StrictStr]] = None
+    state: Optional[ServiceState] = None
+    status: ServiceStatusEnum
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "image", "tags", "ports", "state", "status"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -57,15 +56,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OrganizationCreate from a JSON string"""
+        """Create an instance of Service from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,65 +77,59 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if identifier (nullable) is None
+        # set to None if id (nullable) is None
         # and model_fields_set contains the field
-        if self.identifier is None and "identifier" in self.model_fields_set:
-            _dict['identifier'] = None
-
-        # set to None if owner_id (nullable) is None
-        # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
-
-        # set to None if owner_type (nullable) is None
-        # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
+        if self.id is None and "id" in self.model_fields_set:
+            _dict['id'] = None
 
         # set to None if description (nullable) is None
         # and model_fields_set contains the field
         if self.description is None and "description" in self.model_fields_set:
             _dict['description'] = None
 
-        # set to None if okta_group_id (nullable) is None
+        # set to None if org_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.org_id is None and "org_id" in self.model_fields_set:
+            _dict['org_id'] = None
+
+        # set to None if user_id (nullable) is None
         # and model_fields_set contains the field
-        if self.okta_group_id is None and "okta_group_id" in self.model_fields_set:
-            _dict['okta_group_id'] = None
+        if self.user_id is None and "user_id" in self.model_fields_set:
+            _dict['user_id'] = None
 
-        # set to None if auth0_org_id (nullable) is None
+        # set to None if ports (nullable) is None
         # and model_fields_set contains the field
-        if self.auth0_org_id is None and "auth0_org_id" in self.model_fields_set:
-            _dict['auth0_org_id'] = None
+        if self.ports is None and "ports" in self.model_fields_set:
+            _dict['ports'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OrganizationCreate from a dict"""
+        """Create an instance of Service from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier"),
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
-            "subscription": obj.get("subscription"),
-            "root_email": obj.get("root_email"),
-            "okta_group_id": obj.get("okta_group_id"),
-            "auth0_org_id": obj.get("auth0_org_id")
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
+            "image": obj.get("image"),
+            "tags": obj.get("tags"),
+            "ports": obj.get("ports"),
+            "state": obj.get("state"),
+            "status": obj.get("status")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/owner_type_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/post_clusters_response.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/post_service_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from ambient_backend_api_client.models.cluster import Cluster
+from ambient_backend_api_client.models.service import Service
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PostClustersResponse(BaseModel):
+class PostServiceResponse(BaseModel):
     """
-    PostClustersResponse
+    PostServiceResponse
     """ # noqa: E501
     request_id: StrictStr
-    requested_ts: Optional[StrictStr] = 'Fri May 10 21:28:39 2024'
+    requested_ts: Optional[StrictStr] = '2024-05-24T12:36:49.791531'
     location_root: Optional[StrictStr] = 'http://localhost:8001/requests/'
     refresh_interval: Optional[StrictInt] = 10
-    cluster: Cluster
-    __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "cluster"]
+    service: Service
+    __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "service"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PostClustersResponse from a JSON string"""
+        """Create an instance of PostServiceResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,31 +69,31 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of cluster
-        if self.cluster:
-            _dict['cluster'] = self.cluster.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of service
+        if self.service:
+            _dict['service'] = self.service.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PostClustersResponse from a dict"""
+        """Create an instance of PostServiceResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "request_id": obj.get("request_id"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Fri May 10 21:28:39 2024',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else '2024-05-24T12:36:49.791531',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
-            "cluster": Cluster.from_dict(obj["cluster"]) if obj.get("cluster") is not None else None
+            "service": Service.from_dict(obj["service"]) if obj.get("service") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/post_service_response.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/user_preferences.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,30 +13,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
-from ambient_backend_api_client.models.service import Service
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PostServiceResponse(BaseModel):
+class UserPreferences(BaseModel):
     """
-    PostServiceResponse
+    UserPreferences
     """ # noqa: E501
-    request_id: StrictStr
-    requested_ts: Optional[StrictStr] = 'Fri May 10 21:28:39 2024'
-    location_root: Optional[StrictStr] = 'http://localhost:8001/requests/'
-    refresh_interval: Optional[StrictInt] = 10
-    service: Service
-    __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "service"]
+    dark_mode: Optional[StrictBool] = False
+    __properties: ClassVar[List[str]] = ["dark_mode"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,15 +43,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PostServiceResponse from a JSON string"""
+        """Create an instance of UserPreferences from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,31 +64,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of service
-        if self.service:
-            _dict['service'] = self.service.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PostServiceResponse from a dict"""
+        """Create an instance of UserPreferences from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "request_id": obj.get("request_id"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Fri May 10 21:28:39 2024',
-            "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
-            "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
-            "service": Service.from_dict(obj["service"]) if obj.get("service") is not None else None
+            "dark_mode": obj.get("dark_mode") if obj.get("dark_mode") is not None else False
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/request.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,43 +13,38 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
-from ambient_backend_api_client.models.request_status_enum import RequestStatusEnum
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
+from ambient_backend_api_client.models.service_state import ServiceState
+from ambient_backend_api_client.models.service_status_enum import ServiceStatusEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Request(BaseModel):
+class ServiceCreate(BaseModel):
     """
-    Request
+    ServiceCreate
     """ # noqa: E501
+    id: Optional[StrictInt] = None
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: StrictStr
-    owner_id: StrictStr
-    owner_type: OwnerTypeEnum
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
-    status: Optional[RequestStatusEnum] = None
-    error: Optional[StrictStr] = None
-    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.715398119204992E9
-    started_ts: Optional[Union[StrictFloat, StrictInt]] = None
-    failed_ts: Optional[Union[StrictFloat, StrictInt]] = None
-    completed_ts: Optional[Union[StrictFloat, StrictInt]] = None
-    notes: Optional[List[StrictStr]] = None
-    data: Optional[Dict[str, Any]] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "status", "error", "requested_ts", "started_ts", "failed_ts", "completed_ts", "notes", "data"]
+    org_id: Optional[StrictInt] = None
+    user_id: Optional[StrictInt] = None
+    image: StrictStr
+    tags: Optional[List[StrictStr]] = None
+    ports: Optional[List[StrictStr]] = None
+    state: Optional[ServiceState] = None
+    status: Optional[ServiceStatusEnum] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "image", "tags", "ports", "state", "status"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -61,15 +56,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Request from a JSON string"""
+        """Create an instance of ServiceCreate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,64 +77,64 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if id (nullable) is None
+        # and model_fields_set contains the field
+        if self.id is None and "id" in self.model_fields_set:
+            _dict['id'] = None
+
         # set to None if description (nullable) is None
         # and model_fields_set contains the field
         if self.description is None and "description" in self.model_fields_set:
             _dict['description'] = None
 
-        # set to None if error (nullable) is None
+        # set to None if org_id (nullable) is None
         # and model_fields_set contains the field
-        if self.error is None and "error" in self.model_fields_set:
-            _dict['error'] = None
+        if self.org_id is None and "org_id" in self.model_fields_set:
+            _dict['org_id'] = None
 
-        # set to None if started_ts (nullable) is None
+        # set to None if user_id (nullable) is None
         # and model_fields_set contains the field
-        if self.started_ts is None and "started_ts" in self.model_fields_set:
-            _dict['started_ts'] = None
+        if self.user_id is None and "user_id" in self.model_fields_set:
+            _dict['user_id'] = None
 
-        # set to None if failed_ts (nullable) is None
+        # set to None if ports (nullable) is None
         # and model_fields_set contains the field
-        if self.failed_ts is None and "failed_ts" in self.model_fields_set:
-            _dict['failed_ts'] = None
+        if self.ports is None and "ports" in self.model_fields_set:
+            _dict['ports'] = None
 
-        # set to None if completed_ts (nullable) is None
+        # set to None if status (nullable) is None
         # and model_fields_set contains the field
-        if self.completed_ts is None and "completed_ts" in self.model_fields_set:
-            _dict['completed_ts'] = None
+        if self.status is None and "status" in self.model_fields_set:
+            _dict['status'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Request from a dict"""
+        """Create an instance of ServiceCreate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier"),
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
-            "status": obj.get("status"),
-            "error": obj.get("error"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.715398119204992E9,
-            "started_ts": obj.get("started_ts"),
-            "failed_ts": obj.get("failed_ts"),
-            "completed_ts": obj.get("completed_ts"),
-            "notes": obj.get("notes"),
-            "data": obj.get("data")
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
+            "image": obj.get("image"),
+            "tags": obj.get("tags"),
+            "ports": obj.get("ports"),
+            "state": obj.get("state"),
+            "status": obj.get("status")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/request_status_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/resource_type_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/role_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/organization_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,39 +15,31 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
-from ambient_backend_api_client.models.service_state import ServiceState
-from ambient_backend_api_client.models.service_status_enum import ServiceStatusEnum
+from ambient_backend_api_client.models.subscription_model_enum import SubscriptionModelEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Service(BaseModel):
+class OrganizationCreate(BaseModel):
     """
-    Service
+    OrganizationCreate
     """ # noqa: E501
     name: StrictStr
-    resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = None
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
-    image: StrictStr
-    tags: Optional[List[StrictStr]] = None
-    ports: Optional[List[StrictStr]] = None
-    state: Optional[ServiceState] = None
-    status: ServiceStatusEnum
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "image", "tags", "ports", "state", "status"]
+    resource_type: Optional[ResourceTypeEnum] = None
+    subscription: SubscriptionModelEnum
+    root_email: StrictStr
+    okta_group_id: Optional[StrictStr] = None
+    auth0_org_id: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["name", "description", "resource_type", "subscription", "root_email", "okta_group_id", "auth0_org_id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -59,15 +51,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Service from a JSON string"""
+        """Create an instance of OrganizationCreate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,61 +72,45 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if identifier (nullable) is None
-        # and model_fields_set contains the field
-        if self.identifier is None and "identifier" in self.model_fields_set:
-            _dict['identifier'] = None
-
-        # set to None if owner_id (nullable) is None
-        # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
-
-        # set to None if owner_type (nullable) is None
-        # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
-
         # set to None if description (nullable) is None
         # and model_fields_set contains the field
         if self.description is None and "description" in self.model_fields_set:
             _dict['description'] = None
 
-        # set to None if ports (nullable) is None
+        # set to None if okta_group_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.okta_group_id is None and "okta_group_id" in self.model_fields_set:
+            _dict['okta_group_id'] = None
+
+        # set to None if auth0_org_id (nullable) is None
         # and model_fields_set contains the field
-        if self.ports is None and "ports" in self.model_fields_set:
-            _dict['ports'] = None
+        if self.auth0_org_id is None and "auth0_org_id" in self.model_fields_set:
+            _dict['auth0_org_id'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Service from a dict"""
+        """Create an instance of OrganizationCreate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
-            "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier"),
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
-            "image": obj.get("image"),
-            "tags": obj.get("tags"),
-            "ports": obj.get("ports"),
-            "state": obj.get("state"),
-            "status": obj.get("status")
+            "resource_type": obj.get("resource_type"),
+            "subscription": obj.get("subscription"),
+            "root_email": obj.get("root_email"),
+            "okta_group_id": obj.get("okta_group_id"),
+            "auth0_org_id": obj.get("auth0_org_id")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service_create.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,41 +13,46 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
+from ambient_backend_api_client.models.account_type import AccountType
+from ambient_backend_api_client.models.creation_method import CreationMethod
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
-from ambient_backend_api_client.models.service_state import ServiceState
-from ambient_backend_api_client.models.service_status_enum import ServiceStatusEnum
+from ambient_backend_api_client.models.user_preferences import UserPreferences
+from ambient_backend_api_client.models.user_role_enum import UserRoleEnum
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ServiceCreate(BaseModel):
+class User(BaseModel):
     """
-    ServiceCreate
+    User
     """ # noqa: E501
+    id: StrictInt
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = None
-    owner_id: Optional[StrictStr] = None
-    owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
-    image: StrictStr
-    tags: Optional[List[StrictStr]] = None
-    ports: Optional[List[StrictStr]] = None
-    state: Optional[ServiceState] = None
-    status: Optional[ServiceStatusEnum] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "image", "tags", "ports", "state", "status"]
+    org_id: StrictInt
+    user_id: Optional[StrictInt] = None
+    account_type: Optional[AccountType] = None
+    creation_method: Optional[CreationMethod] = None
+    email: StrictStr
+    first_name: StrictStr
+    last_name: StrictStr
+    role: Optional[UserRoleEnum] = None
+    preferences: Optional[UserPreferences] = None
+    auth_provider_uid: Optional[StrictStr] = None
+    phone_number: Optional[StrictStr] = None
+    username: Optional[StrictStr] = None
+    is_super_admin: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "account_type", "creation_method", "email", "first_name", "last_name", "role", "preferences", "auth_provider_uid", "phone_number", "username", "is_super_admin"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -59,15 +64,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ServiceCreate from a JSON string"""
+        """Create an instance of User from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,66 +85,78 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # set to None if identifier (nullable) is None
+        # override the default output from pydantic by calling `to_dict()` of preferences
+        if self.preferences:
+            _dict['preferences'] = self.preferences.to_dict()
+        # set to None if description (nullable) is None
         # and model_fields_set contains the field
-        if self.identifier is None and "identifier" in self.model_fields_set:
-            _dict['identifier'] = None
+        if self.description is None and "description" in self.model_fields_set:
+            _dict['description'] = None
 
-        # set to None if owner_id (nullable) is None
+        # set to None if user_id (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_id is None and "owner_id" in self.model_fields_set:
-            _dict['owner_id'] = None
+        if self.user_id is None and "user_id" in self.model_fields_set:
+            _dict['user_id'] = None
 
-        # set to None if owner_type (nullable) is None
+        # set to None if preferences (nullable) is None
         # and model_fields_set contains the field
-        if self.owner_type is None and "owner_type" in self.model_fields_set:
-            _dict['owner_type'] = None
+        if self.preferences is None and "preferences" in self.model_fields_set:
+            _dict['preferences'] = None
 
-        # set to None if description (nullable) is None
+        # set to None if auth_provider_uid (nullable) is None
         # and model_fields_set contains the field
-        if self.description is None and "description" in self.model_fields_set:
-            _dict['description'] = None
+        if self.auth_provider_uid is None and "auth_provider_uid" in self.model_fields_set:
+            _dict['auth_provider_uid'] = None
+
+        # set to None if phone_number (nullable) is None
+        # and model_fields_set contains the field
+        if self.phone_number is None and "phone_number" in self.model_fields_set:
+            _dict['phone_number'] = None
 
-        # set to None if ports (nullable) is None
+        # set to None if username (nullable) is None
         # and model_fields_set contains the field
-        if self.ports is None and "ports" in self.model_fields_set:
-            _dict['ports'] = None
+        if self.username is None and "username" in self.model_fields_set:
+            _dict['username'] = None
 
-        # set to None if status (nullable) is None
+        # set to None if is_super_admin (nullable) is None
         # and model_fields_set contains the field
-        if self.status is None and "status" in self.model_fields_set:
-            _dict['status'] = None
+        if self.is_super_admin is None and "is_super_admin" in self.model_fields_set:
+            _dict['is_super_admin'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ServiceCreate from a dict"""
+        """Create an instance of User from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier"),
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
-            "image": obj.get("image"),
-            "tags": obj.get("tags"),
-            "ports": obj.get("ports"),
-            "state": obj.get("state"),
-            "status": obj.get("status")
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
+            "account_type": obj.get("account_type"),
+            "creation_method": obj.get("creation_method"),
+            "email": obj.get("email"),
+            "first_name": obj.get("first_name"),
+            "last_name": obj.get("last_name"),
+            "role": obj.get("role"),
+            "preferences": UserPreferences.from_dict(obj["preferences"]) if obj.get("preferences") is not None else None,
+            "auth_provider_uid": obj.get("auth_provider_uid"),
+            "phone_number": obj.get("phone_number"),
+            "username": obj.get("username"),
+            "is_super_admin": obj.get("is_super_admin")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service_list.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class ServiceList(BaseModel):
     """
     ServiceList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Fri May 10 21:28:39 2024'
+    timestamp: Optional[StrictStr] = '2024-05-24T12:36:49.790989'
     results: List[Service]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -87,13 +87,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Fri May 10 21:28:39 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else '2024-05-24T12:36:49.790989',
             "results": [Service.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service_state.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/service_status_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/status_enum_input.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/subscription_model_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/token_response.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/user.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/node_create.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,49 +13,44 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from ambient_backend_api_client.models.account_type import AccountType
-from ambient_backend_api_client.models.creation_method import CreationMethod
-from ambient_backend_api_client.models.owner_type_enum import OwnerTypeEnum
+from ambient_backend_api_client.models.auth0_device_code_response import Auth0DeviceCodeResponse
+from ambient_backend_api_client.models.network_interface import NetworkInterface
+from ambient_backend_api_client.models.node_architecture_enum import NodeArchitectureEnum
+from ambient_backend_api_client.models.node_role_enum import NodeRoleEnum
 from ambient_backend_api_client.models.resource_type_enum import ResourceTypeEnum
-from ambient_backend_api_client.models.user_preferences import UserPreferences
-from ambient_backend_api_client.models.user_role_enum import UserRoleEnum
+from ambient_backend_api_client.models.status_enum_input import StatusEnumInput
 from typing import Optional, Set
 from typing_extensions import Self
 
-class User(BaseModel):
+class NodeCreate(BaseModel):
     """
-    User
+    NodeCreate
     """ # noqa: E501
+    id: Optional[StrictInt] = None
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: StrictStr
-    owner_id: StrictStr
-    owner_type: OwnerTypeEnum
     description: Optional[StrictStr] = None
-    requests: Optional[List[StrictStr]] = None
-    notifications: Optional[List[StrictStr]] = None
-    account_type: Optional[AccountType] = None
-    creation_method: Optional[CreationMethod] = None
-    email: StrictStr
-    first_name: StrictStr
-    last_name: StrictStr
-    role: Optional[UserRoleEnum] = None
-    preferences: Optional[UserPreferences] = None
-    auth_provider_uid: Optional[StrictStr] = None
-    phone_number: Optional[StrictStr] = None
-    username: Optional[StrictStr] = None
-    is_super_admin: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "account_type", "creation_method", "email", "first_name", "last_name", "role", "preferences", "auth_provider_uid", "phone_number", "username", "is_super_admin"]
+    org_id: Optional[StrictInt] = None
+    user_id: Optional[StrictInt] = None
+    role: NodeRoleEnum
+    architecture: NodeArchitectureEnum
+    interfaces: Optional[List[NetworkInterface]] = None
+    last_seen: Optional[StrictStr] = None
+    status: Optional[StatusEnumInput] = None
+    identifier: Optional[StrictStr] = None
+    cluster: Optional[StrictStr] = None
+    authorization: Optional[Auth0DeviceCodeResponse] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "resource_type", "description", "org_id", "user_id", "role", "architecture", "interfaces", "last_seen", "status", "identifier", "cluster", "authorization"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -67,15 +62,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of User from a JSON string"""
+        """Create an instance of NodeCreate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -88,75 +83,92 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of preferences
-        if self.preferences:
-            _dict['preferences'] = self.preferences.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in interfaces (list)
+        _items = []
+        if self.interfaces:
+            for _item in self.interfaces:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['interfaces'] = _items
+        # override the default output from pydantic by calling `to_dict()` of authorization
+        if self.authorization:
+            _dict['authorization'] = self.authorization.to_dict()
+        # set to None if id (nullable) is None
+        # and model_fields_set contains the field
+        if self.id is None and "id" in self.model_fields_set:
+            _dict['id'] = None
+
         # set to None if description (nullable) is None
         # and model_fields_set contains the field
         if self.description is None and "description" in self.model_fields_set:
             _dict['description'] = None
 
-        # set to None if preferences (nullable) is None
+        # set to None if org_id (nullable) is None
+        # and model_fields_set contains the field
+        if self.org_id is None and "org_id" in self.model_fields_set:
+            _dict['org_id'] = None
+
+        # set to None if user_id (nullable) is None
         # and model_fields_set contains the field
-        if self.preferences is None and "preferences" in self.model_fields_set:
-            _dict['preferences'] = None
+        if self.user_id is None and "user_id" in self.model_fields_set:
+            _dict['user_id'] = None
 
-        # set to None if auth_provider_uid (nullable) is None
+        # set to None if interfaces (nullable) is None
         # and model_fields_set contains the field
-        if self.auth_provider_uid is None and "auth_provider_uid" in self.model_fields_set:
-            _dict['auth_provider_uid'] = None
+        if self.interfaces is None and "interfaces" in self.model_fields_set:
+            _dict['interfaces'] = None
 
-        # set to None if phone_number (nullable) is None
+        # set to None if last_seen (nullable) is None
         # and model_fields_set contains the field
-        if self.phone_number is None and "phone_number" in self.model_fields_set:
-            _dict['phone_number'] = None
+        if self.last_seen is None and "last_seen" in self.model_fields_set:
+            _dict['last_seen'] = None
 
-        # set to None if username (nullable) is None
+        # set to None if identifier (nullable) is None
         # and model_fields_set contains the field
-        if self.username is None and "username" in self.model_fields_set:
-            _dict['username'] = None
+        if self.identifier is None and "identifier" in self.model_fields_set:
+            _dict['identifier'] = None
 
-        # set to None if is_super_admin (nullable) is None
+        # set to None if cluster (nullable) is None
         # and model_fields_set contains the field
-        if self.is_super_admin is None and "is_super_admin" in self.model_fields_set:
-            _dict['is_super_admin'] = None
+        if self.cluster is None and "cluster" in self.model_fields_set:
+            _dict['cluster'] = None
+
+        # set to None if authorization (nullable) is None
+        # and model_fields_set contains the field
+        if self.authorization is None and "authorization" in self.model_fields_set:
+            _dict['authorization'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of User from a dict"""
+        """Create an instance of NodeCreate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier"),
-            "owner_id": obj.get("owner_id"),
-            "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
-            "requests": obj.get("requests"),
-            "notifications": obj.get("notifications"),
-            "account_type": obj.get("account_type"),
-            "creation_method": obj.get("creation_method"),
-            "email": obj.get("email"),
-            "first_name": obj.get("first_name"),
-            "last_name": obj.get("last_name"),
+            "org_id": obj.get("org_id"),
+            "user_id": obj.get("user_id"),
             "role": obj.get("role"),
-            "preferences": UserPreferences.from_dict(obj["preferences"]) if obj.get("preferences") is not None else None,
-            "auth_provider_uid": obj.get("auth_provider_uid"),
-            "phone_number": obj.get("phone_number"),
-            "username": obj.get("username"),
-            "is_super_admin": obj.get("is_super_admin")
+            "architecture": obj.get("architecture"),
+            "interfaces": [NetworkInterface.from_dict(_item) for _item in obj["interfaces"]] if obj.get("interfaces") is not None else None,
+            "last_seen": obj.get("last_seen"),
+            "status": obj.get("status"),
+            "identifier": obj.get("identifier"),
+            "cluster": obj.get("cluster"),
+            "authorization": Auth0DeviceCodeResponse.from_dict(obj["authorization"]) if obj.get("authorization") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/user_preferences.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/validation_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List
+from ambient_backend_api_client.models.validation_error_loc_inner import ValidationErrorLocInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserPreferences(BaseModel):
+class ValidationError(BaseModel):
     """
-    UserPreferences
+    ValidationError
     """ # noqa: E501
-    dark_mode: Optional[StrictBool] = False
-    __properties: ClassVar[List[str]] = ["dark_mode"]
+    loc: List[ValidationErrorLocInner]
+    msg: StrictStr
+    type: StrictStr
+    __properties: ClassVar[List[str]] = ["loc", "msg", "type"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -43,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserPreferences from a JSON string"""
+        """Create an instance of ValidationError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -64,24 +67,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in loc (list)
+        _items = []
+        if self.loc:
+            for _item in self.loc:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['loc'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserPreferences from a dict"""
+        """Create an instance of ValidationError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "dark_mode": obj.get("dark_mode") if obj.get("dark_mode") is not None else False
+            "loc": [ValidationErrorLocInner.from_dict(_item) for _item in obj["loc"]] if obj.get("loc") is not None else None,
+            "msg": obj.get("msg"),
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/user_role_enum.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/models/validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client/rest.py` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/ambient_backend_api_client.egg-info/SOURCES.txt` & `ambient_backend_api_client-0.1.6/ambient_backend_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/pyproject.toml` & `ambient_backend_api_client-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/setup.py` & `ambient_backend_api_client-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "ambient_backend_api_client"
-VERSION = "0.1.4"
+VERSION = "0.1.6"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "aiohttp >= 3.0.0",
     "aiohttp-retry >= 2.8.3",
     "pydantic >= 2",
```

### Comparing `ambient_backend_api_client-0.1.4/test/test_account_type.py` & `ambient_backend_api_client-0.1.6/test/test_account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_ambient_action_enum.py` & `ambient_backend_api_client-0.1.6/test/test_ambient_action_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_ambient_event_type_enum.py` & `ambient_backend_api_client-0.1.6/test/test_ambient_event_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_architecture_enum.py` & `ambient_backend_api_client-0.1.6/test/test_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_auth0_device_code_response.py` & `ambient_backend_api_client-0.1.6/test/test_auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_cluster.py` & `ambient_backend_api_client-0.1.6/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_cluster_create.py` & `ambient_backend_api_client-0.1.6/test/test_cluster_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_clusters_api.py` & `ambient_backend_api_client-0.1.6/test/test_clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_create_service_acct_request.py` & `ambient_backend_api_client-0.1.6/test/test_create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_creation_method.py` & `ambient_backend_api_client-0.1.6/test/test_creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_event.py` & `ambient_backend_api_client-0.1.6/test/test_event.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_event_label.py` & `ambient_backend_api_client-0.1.6/test/test_event_label.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_event_template.py` & `ambient_backend_api_client-0.1.6/test/test_event_template.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_health_api.py` & `ambient_backend_api_client-0.1.6/test/test_health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_http_validation_error.py` & `ambient_backend_api_client-0.1.6/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_interface_type_enum.py` & `ambient_backend_api_client-0.1.6/test/test_interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_list_results_response.py` & `ambient_backend_api_client-0.1.6/test/test_list_results_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.6/test/test_models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_models_node_status_enum.py` & `ambient_backend_api_client-0.1.6/test/test_models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_network_interface.py` & `ambient_backend_api_client-0.1.6/test/test_network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_node.py` & `ambient_backend_api_client-0.1.6/test/test_node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_node_architecture_enum.py` & `ambient_backend_api_client-0.1.6/test/test_node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_node_create.py` & `ambient_backend_api_client-0.1.6/test/test_node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_node_role_enum.py` & `ambient_backend_api_client-0.1.6/test/test_node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_nodes_api.py` & `ambient_backend_api_client-0.1.6/test/test_nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_notification.py` & `ambient_backend_api_client-0.1.6/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_notification_list.py` & `ambient_backend_api_client-0.1.6/test/test_notification_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_notification_request.py` & `ambient_backend_api_client-0.1.6/test/test_notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_notification_severity_enum.py` & `ambient_backend_api_client-0.1.6/test/test_notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_notifications_api.py` & `ambient_backend_api_client-0.1.6/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_organization_create.py` & `ambient_backend_api_client-0.1.6/test/test_organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_owner_type_enum.py` & `ambient_backend_api_client-0.1.6/test/test_owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_ping_api.py` & `ambient_backend_api_client-0.1.6/test/test_ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_post_clusters_response.py` & `ambient_backend_api_client-0.1.6/test/test_post_clusters_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_post_service_response.py` & `ambient_backend_api_client-0.1.6/test/test_post_service_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_request.py` & `ambient_backend_api_client-0.1.6/test/test_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_request_status_enum.py` & `ambient_backend_api_client-0.1.6/test/test_request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_requests_api.py` & `ambient_backend_api_client-0.1.6/test/test_requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_resource_type_enum.py` & `ambient_backend_api_client-0.1.6/test/test_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_role_enum.py` & `ambient_backend_api_client-0.1.6/test/test_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_service.py` & `ambient_backend_api_client-0.1.6/test/test_service.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_service_create.py` & `ambient_backend_api_client-0.1.6/test/test_service_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_service_list.py` & `ambient_backend_api_client-0.1.6/test/test_service_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_service_state.py` & `ambient_backend_api_client-0.1.6/test/test_service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_service_status_enum.py` & `ambient_backend_api_client-0.1.6/test/test_service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_services_api.py` & `ambient_backend_api_client-0.1.6/test/test_services_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_status_enum_input.py` & `ambient_backend_api_client-0.1.6/test/test_status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_subscription_model_enum.py` & `ambient_backend_api_client-0.1.6/test/test_subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_token_response.py` & `ambient_backend_api_client-0.1.6/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_unimplemented_api.py` & `ambient_backend_api_client-0.1.6/test/test_unimplemented_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_user.py` & `ambient_backend_api_client-0.1.6/test/test_user.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_user_preferences.py` & `ambient_backend_api_client-0.1.6/test/test_user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_user_role_enum.py` & `ambient_backend_api_client-0.1.6/test/test_user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_users_api.py` & `ambient_backend_api_client-0.1.6/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_validation_error.py` & `ambient_backend_api_client-0.1.6/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.4/test/test_validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.6/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

